# Comparing `tmp/better_rtplot-0.1.4.tar.gz` & `tmp/better_rtplot-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_rtplot-0.1.4.tar", max compression
+gzip compressed data, was "better_rtplot-0.1.5.tar", max compression
```

## Comparing `better_rtplot-0.1.4.tar` & `better_rtplot-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0    35149 2023-06-28 20:16:53.824192 better_rtplot-0.1.4/LICENSE
--rwxr-xr-x   0        0        0     7489 2023-07-19 02:18:57.469955 better_rtplot-0.1.4/README.md
--rwxr-xr-x   0        0        0      631 2023-07-25 16:06:34.096792 better_rtplot-0.1.4/pyproject.toml
--rwxr-xr-x   0        0        0     7588 2023-07-17 19:06:32.364262 better_rtplot-0.1.4/rtplot/client.py
--rwxr-xr-x   0        0        0     6240 2023-03-09 21:43:09.016987 better_rtplot-0.1.4/rtplot/example_code.py
--rwxr-xr-x   0        0        0     1062 2023-07-13 18:31:13.985659 better_rtplot-0.1.4/rtplot/plot_log.py
--rwxr-xr-x   0        0        0       71 2023-03-09 21:43:09.016987 better_rtplot-0.1.4/rtplot/saved_plots/.gitignore
--rwxr-xr-x   0        0        0    22802 2023-07-17 19:02:58.496380 better_rtplot-0.1.4/rtplot/server.py
--rw-r--r--   0        0        0     8241 1970-01-01 00:00:00.000000 better_rtplot-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-11 01:15:37.992109 better_rtplot-0.1.5/LICENSE
+-rwxr-xr-x   0        0        0    12535 2023-08-17 22:19:46.960932 better_rtplot-0.1.5/README.md
+-rwxr-xr-x   0        0        0      646 2024-04-11 01:24:27.850580 better_rtplot-0.1.5/pyproject.toml
+-rwxr-xr-x   0        0        0     9251 2024-04-11 01:16:00.456553 better_rtplot-0.1.5/rtplot/client.py
+-rwxr-xr-x   0        0        0     6252 2023-08-17 22:15:47.496837 better_rtplot-0.1.5/rtplot/example_code.py
+-rwxr-xr-x   0        0        0     1564 2023-08-16 23:13:59.843588 better_rtplot-0.1.5/rtplot/plot_log.py
+-rw-r--r--   0        0        0       71 2024-04-11 01:15:37.992109 better_rtplot-0.1.5/rtplot/saved_plots/.gitignore
+-rwxr-xr-x   0        0        0    26529 2023-08-17 22:17:18.462393 better_rtplot-0.1.5/rtplot/server.py
+-rw-r--r--   0        0        0    13287 1970-01-01 00:00:00.000000 better_rtplot-0.1.5/PKG-INFO
```

### Comparing `better_rtplot-0.1.4/LICENSE` & `better_rtplot-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `better_rtplot-0.1.4/pyproject.toml` & `better_rtplot-0.1.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "better-rtplot"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["jmontp <jmontp@umich.edu>"]
 license = "GPL V3.0"
 readme = "README.md"
 packages = [{include = "rtplot"}]
 
 [tool.poetry.dependencies]
-python = ">= 3.8, <3.11"
-numpy = "1.23.5"
-pyzmq = "25.0.0"
+python = ">= 3.9, < 3.12"
+numpy = ">= 1.23.5"
+pyzmq = ">= 25.0.0"
 
-pandas = {version = "1.5.3", optional = true}
-pyarrow = {version="11.0.0", optional = true}
-pyqtgraph = {version = "0.13.0", optional = true}
-pyside6 = {version = "<= 6.4.0", optional = true}
+pandas = {version = ">= 1.5.3", optional = true}
+pyarrow = {version=">= 11.0.0", optional = true}
+pyqtgraph = {version = ">= 0.13.0", optional = true}
+pyside6 = {version = "> 6.4.0", optional = true}
 
 [tool.poetry.extras]
 server = ["pyqtgraph", "pyside6", "pandas", "pyarrow"]
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `better_rtplot-0.1.4/rtplot/client.py` & `better_rtplot-0.1.5/rtplot/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import zmq
 import numpy as np
 import time
 from collections import OrderedDict
-
+import csv
+from typing import List
 
 ###################
 # ZMQ Networking #
 ##################
 
 #Get the context for networking setup
 context = zmq.Context()
@@ -26,16 +27,14 @@
 
 # The subscriber or the publisher must be fixed
 # set which is which here
 known_pi_address_prev = True
 # Add flag to indicate if we ever failed to bind
 failed_bind = False
 
-
-
 ## Define the default behaviour of the pi
 
 # Assume that you know the ip address of the pi
 if known_pi_address_prev:
     
     try:
         #Attempt to bind to incoming addresses on the port
@@ -54,14 +53,21 @@
    
 # Secondary default behavior is that you know the ip address 
 # of the computer that will plot
 else:
     #Connect to the computer that will plot information
     socket.connect(prev_address)
 
+
+############################
+# Local plot save config #
+###########################
+local_log_file = None
+csv_writer = None
+
 ############################
 # PyQTgraph Configuration #
 ###########################
 
 #Create definitions for categories
 SENDING_PLOT_UPDATE = "0"
 SENDING_DATA = "1"
@@ -151,54 +157,81 @@
 
     #Remember the last configuration you had
     known_pi_address_prev = known_pi_address
 
     #Sleep so that the connection can be established
     time.sleep(1)
 
+def create_local_log(plot_desc_dict:List[dict], log_name:str=None):
+    """Create a current log file based on the data that is sent"""
+    global local_log_file
+    global csv_writer
+    
+    #If we have a local log file, then delete it
+    if local_log_file is not None:
+        local_log_file.close()
+        local_log_file = None
+
+    # Create a new log file with a csv writter object which uses the log_name
+    # argument in conjunction with the timestamp to create a unique log file
+    local_log_file = open(f"{log_name}_{time.time()}.csv", 'w', newline='')
+    csv_writer = csv.writer(local_log_file, delimiter=',',
+                             quotechar='"', quoting=csv.QUOTE_MINIMAL)
+
+    # Add the header to the csv file based on the plot description
+    csv_writer.writerow(["Time"] + [name for plot in plot_desc_dict.values() for name in plot["names"]])
+    
+
 
 def send_array(A, flags=0, copy=True, track=False):
     """send a numpy array with metadata
     Inputs
     ------
     A: (subplots,dim) np array to transmit
         subplots - the amount of subplots that are 
                    defined in the current plot
         dim - the amount of data that you want to plot.
               This is not fixed 
     """
     #If you get a float value, convert it to a numpy array
     if(isinstance(A,float) or isinstance(A,list)):
         A = np.array(A).reshape(-1,1)
-
     #If array is one dimensional, reshape to two dimensions
     if(len(A.shape) ==1):
         A = A.reshape(-1,1)
-
     #Create dict to reconstruct array
     md = dict(
         dtype = str(A.dtype),
         shape = A.shape,
     )
-
+    
     #Send category
     socket.send_string(SENDING_DATA)
-    
     #Send json description
     socket.send_json(md, flags | zmq.SNDMORE)
     #Send array
-    return socket.send(A, flags, copy=copy, track=track)
+    socket.send(A, flags, copy=copy, track=track)
+    
+    #If we have a local log file, then save the data
+    if local_log_file is not None:
+        csv_writer.writerow([time.time()] + A.flatten().tolist())
 
 
-def initialize_plots(plot_descriptions=1):
+def initialize_plots(plot_descriptions=1, log_name=None):
     """Send a json description of desired plot
     Inputs
     ------
     plot_description: list of names or list of plot descriptions dictionaries
+        list of names - the names of the plots that you want to create
+        list of plot descriptions - the dictionary of the plot descriptions
+    log_name: string, name of the file that will be stored locally
     """
+    
+    global local_log_file
+    global plot_desc_dict
 
     #Process int inputs
     if isinstance(plot_descriptions,int):
         plot_desc_dict = OrderedDict()
         plot_desc_dict["plot0"] = {"names":["Trace {}".format(i) for i in range (plot_descriptions)]}
 
     #Process string inputs
@@ -237,23 +270,29 @@
     
     #Send the category
     socket.send_string(SENDING_PLOT_UPDATE)
 
     #Send the description
     socket.send_json(plot_desc_dict)
 
+    #If we have a log name, then save the log
+    if log_name is not None:
+        create_local_log(log_name)
+
 
 def save_plot(log_name):
     """
     Tell the server to store the data that has been sent for the latest
     plot configuration
     
     Keyword Arguments
     log_name -- string, name of the file that will be stored
         
     """
-
-    #Indicate that we will send a plot save requset
+    # Indicate that we will send a plot save requset
     socket.send_string(SAVE_PLOT)
 
-    #Send the save plot name
-    socket.send_string(log_name)
+    # Send the save plot name
+    socket.send_string(log_name)
+
+    # Flush the file to ensure that all data is written
+    local_log_file.flush()
```

### Comparing `better_rtplot-0.1.4/rtplot/example_code.py` & `better_rtplot-0.1.5/rtplot/example_code.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,104 +3,87 @@
 import time
 
 
 #The first section is dedicated to configuring IP
 # You do NOT need to do this if the server.py is connecting to the pi
 # Uncomment "client.local_plot()" if you want to plot locally 
 
-#--------------------------------------------------------------------------------------------------
+#------------------------------------------------------------------------------
 #Change the ip address that you are going to send data to
-# In this example we configure it to plot locally (127.0.0.1 is the address of the local host)
+# In this example we configure it to plot locally (127.0.0.1 is the address of
+# the local host)
 # client.configure_ip("127.0.0.1")
 
 #Can also specify port, default is 5555
 # client.configure_ip("127.0.0.1:5555")
 # client.plot_to_neurobionics_tv()
 
-#If you want to plot locally, there is already a function that is equivalent to the above
+#If you want to plot locally, there is already a function that is equivalent 
+# to the above
 client.local_plot()
-#--------------------------------------------------------------------------------------------------
+#------------------------------------------------------------------------------
 
 
-#--------------------------------------------------------------------------------------------------
+#------------------------------------------------------------------------------
 #Initialize one plot with one trace
 client.initialize_plots()
 
 
 #Send 1000 data points
 for i in range(1000):
 
     #Send data
     client.send_array(np.random.randn())
 
     time.sleep(0.01)
-#--------------------------------------------------------------------------------------------------
-
-
-
+#------------------------------------------------------------------------------
 
 
 time.sleep(2)
 
 
-
-
-
-#--------------------------------------------------------------------------------------------------
+#------------------------------------------------------------------------------
 #Initialize one plot with 5 traces
 client.initialize_plots(5)
 
 
 #Send 1000 data points
 for i in range(1000):
 
     #Send data
     client.send_array(np.random.randn(5,1))
-#--------------------------------------------------------------------------------------------------
-
-
-
+#------------------------------------------------------------------------------
 
 
 time.sleep(2)
 
 
-
-
-
-#--------------------------------------------------------------------------------------------------
+#------------------------------------------------------------------------------
 #Initialize one plot with oen trace named 'test_trace'
 client.initialize_plots('test_trace')
 
 
 #Send 1000 data points
 for i in range(1000):
 
     #Send data
     client.send_array(np.random.randn(1,1))
-#--------------------------------------------------------------------------------------------------
-
-
-
+#------------------------------------------------------------------------------
 
 
 time.sleep(2)
 
 
-
-
-
-
-#--------------------------------------------------------------------------------------------------
+#------------------------------------------------------------------------------
 #Initialize one plot with three traces
 client.initialize_plots(['test 1', 'test2', 'test 5'])
 
 
 #Send 1000 data points
-for i in range(1000):
+for i in range(10000):
 
     #Generate Data -> (This would be your code)
     var1 = np.random.randn()
     var2 = np.random.randn()
     var3 = np.random.randn()
     
     #Create array (or numpy array) with data
@@ -108,27 +91,24 @@
 
     #Equivalently, send as columns vector
     #data = np.array([[var1],[var2],[var3]])
 
     #Send data
     client.send_array(data)
 
-#--------------------------------------------------------------------------------------------------
-
+    time.sleep(0.001)
 
 
+#------------------------------------------------------------------------------
 
 
 time.sleep(2)
 
 
-
-
-
-#--------------------------------------------------------------------------------------------------
+#------------------------------------------------------------------------------
 #Initialize three subplots with one trace each
 client.initialize_plots([['test 1'], ['test2'], ['test 5']])
 
 
 #Send 1000 data points
 for i in range(1000):
 
@@ -140,102 +120,112 @@
     #Create array (or numpy array) with data
     data = [var1,var2,var3]
     #Equivalently, send as columns vector
     #data = np.array([[var1],[var2],[var3]])
 
     #Send data
     client.send_array(data)
-#--------------------------------------------------------------------------------------------------
-
+#------------------------------------------------------------------------------
 
 
 time.sleep(2)
 
 
-
-#--------------------------------------------------------------------------------------------------
+#------------------------------------------------------------------------------
 #Initialize with more complex configuration
 
 #The only required field is 'names' 
 
 plot_config1 = {'names' : ['plot1_trace1', 'plot1_trace2'],
                 'colors' : ['r','b'],
                 'line_style': ['','-'],
                 'title' : "Plot 1 Title",
                 'ylabel': "Plot 1 y label",
                 'xlabel': "Plot 1 x label",
+                'line_width':[2,2],
                 'yrange': [-1,1]
                 }
 
 plot_config2 = {'names' : ['plot2_trace1'],
                 'colors' : ['r','b'],
                 'line_style': ['-',''],
                 'title' : "Plot 2 Title",
                 'ylabel': "Plot 2 y label",
                 'xlabel': "Plot 2 x label",
+                'line_width':[2],
                 'yrange': [-1,1]
                 }
 
 client.initialize_plots([plot_config1, plot_config2])
 
 
 #Send 1000 data points
-for i in range(1000):
+for i in range(100000):
 
     #Generate Data -> (This would be your code)
     var1 = np.random.randn()
     var2 = np.random.randn()
     var3 = np.random.randn()
 
     #Create array (or numpy array) with data
     data = [var1,var2,var3]
     #Equivalently, send as columns vector
     #data = np.array([[var1],[var2],[var3]])
 
     #Send data
     client.send_array(data)
-#--------------------------------------------------------------------------------------------------
 
+    time.sleep(1/3000)
+#------------------------------------------------------------------------------
 
-#--------------------------------------------------------------------------------------------------
-#Initialize with more complex configuration
 
-#The only required field is 'names' 
+time.sleep(2)
+
 
+#------------------------------------------------------------------------------
+#Send data that will not be plotted
 plot_config1 = {'names' : ['plot1_trace1', 'plot1_trace2'],
                 'colors' : ['r','b'],
                 'line_style': ['','-'],
-                'title' : "Plot 1 Title",
+                'title' : "Non plot test 1",
                 'ylabel': "Plot 1 y label",
                 'xlabel': "Plot 1 x label",
                 'yrange': [-1,1]
                 }
 
 plot_config2 = {'names' : ['plot2_trace1'],
                 'colors' : ['r','b'],
                 'line_style': ['-',''],
-                'title' : "Plot 2 Title",
+                'title' : "Non plot test 2",
                 'ylabel': "Plot 2 y label",
                 'xlabel': "Plot 2 x label",
                 'yrange': [-1,1],
                 'xrange':500
                 }
 
-client.initialize_plots([plot_config1, plot_config2])
+#Add non-plot data labels
+non_plot_config = {"non_plot_labels" : ['non_plot_test_data_1',
+                                        "non_plot_test_data_2"]}
+                
+client.initialize_plots([plot_config1, plot_config2,non_plot_config])
 
 
 #Send 1000 data points
 for i in range(1000):
 
     #Generate Data -> (This would be your code)
     var1 = np.random.randn()
     var2 = np.random.randn()
     var3 = np.random.randn()
+    var4 = np.random.randn()
+    var5 = np.random.randn()
 
     #Create array (or numpy array) with data
-    data = [var1,var2,var3]
+    data = [var1,var2,var3,var4,var5]
     #Equivalently, send as columns vector
     #data = np.array([[var1],[var2],[var3]])
 
     #Send data
     client.send_array(data)
-#--------------------------------------------------------------------------------------------------
+#------------------------------------------------------------------------------
+
+
```

### Comparing `better_rtplot-0.1.4/rtplot/server.py` & `better_rtplot-0.1.5/rtplot/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -78,14 +78,45 @@
     "--skip",
     help="Skip every n datapoints",
     action="store",
     type=int,
     default=1,
 )
 
+# Add argument to change the save directory
+parser.add_argument(
+    "-sd",
+    "--save-dir",
+    help="Directory to save the data to. Default is to save in \
+    the current directory",
+    action="store",
+    type=str,
+    default=os.getcwd(),
+)
+
+# Add argument to change the save name
+parser.add_argument(
+    "-sn",
+    "--save-name",
+    help="Name of the file to save the data to. Default is to save \
+    the data to the current directory",
+    action="store",
+    type=str,
+    default=None,
+)
+
+# Make the number of lines that the server plots at the same time be adaptable
+parser.add_argument(
+    "-a",
+    "--adaptable",
+    help='Adjusts how frequently the plotter will refresh the plot in order to consume the incoming data fast enough without filling a buffer.',
+    action="store_true",
+    default=False,
+)
+
 # Read in the arguments
 args = parser.parse_args()
 
 if args.plot_config is True:
     help_text = (
         "You can control the following things when calling"
         " client.initialize_plots() by passing in a dictionary:"
@@ -150,14 +181,31 @@
 
 # Define if debug text output is set on
 DEBUG_TEXT_ENABLED = args.debug
 
 # Define how many datapoints are skipped
 SKIP_PLOT_DATAPOINTS = args.skip
 
+# Determine if we want to adapt the number of skipped data points
+ADAPT_SKIP_PLOT_DATAPOINTS = args.adaptable
+
+# Define the save directory
+PLOT_SAVE_PATH = args.save_dir
+if PLOT_SAVE_PATH is not None:
+    # Make it absolute path
+    PLOT_SAVE_PATH = os.path.abspath(PLOT_SAVE_PATH)
+    # If the save directory doesn't exist, create it
+    if not os.path.exists(PLOT_SAVE_PATH):
+        os.makedirs(PLOT_SAVE_PATH)
+print(f"Plots will be saved in: {PLOT_SAVE_PATH}")
+
+
+# Define the save name
+PLOT_SAVE_NAME = args.save_name
+
 ###################
 # ZMQ Networking #
 ##################
 
 # Create connection layer
 context = zmq.Context()
 
@@ -184,15 +232,14 @@
     # Bind so that you can get more
     socket.bind("tcp://*:5555")
     print("Bounded every ip address on port :5555")
 
 # Initialize subscriber
 socket.setsockopt_string(zmq.SUBSCRIBE, "")
 
-
 ###############################
 # Local Storage Configuration #
 ###############################
 
 # Width of the window displaying the curve
 # NUM_DATAPOINTS_IN_PLOT = 200
 DEFAULT_NUM_DATAPOINTS_IN_PLOT = 200
@@ -209,17 +256,14 @@
 
 # Create an index to keep track where we are in the local storage buffer
 li = DEFAULT_NUM_DATAPOINTS_IN_PLOT
 
 # Set how many traces we have
 local_storage_buffer_num_trace = 1
 
-# Configure save path
-PLOT_SAVE_PATH = "saved_plots/"
-
 # We are going to use the traces per plot do add info to saved plots
 # since this is set below, initialize to none
 traces_per_plot = None
 trace_labels = None
 non_plot_labels = None
 
 # Create button callback method
@@ -240,30 +284,39 @@
         local_storage_buffer[i, li] = subplot_index
         # Get the number of subplots
         num_subplots = max(subplot_index, num_subplots)
         # Add trace name
         trace_names.append(trace_name)
     
     # Set the non-plot labels to have a index of -1
-    
+    local_storage_buffer[
+        local_storage_buffer_num_trace:local_storage_buffer_num_trace+num_non_plot_traces, 
+        li] = -1
 
     # Assign a new subplot for time
     num_traces = len(trace_labels)
     trace_names.append("Time(s)")
     local_storage_buffer[num_traces, li] = num_subplots + 1
 
+    # Get the timestamp for the plot name
+    timestamp = str(datetime.datetime.now())
+    # Remove colons from timestamp for windows file name compatibility
+    # Remove spaces for underscores so it looks nicer
+    timestamp = timestamp.replace(" ", "_").replace(":", "-")
+
     #Set the log name if it is not provided
     if log_name is None or log_name is False:
-
-        # Set the plot name as the current time
-        log_name = datetime.datetime.now()
-        #Remove spaces for underscores for no real reason
-        log_name = str(log_name).replace(" ", "_")
-        # Remove colons from timestamp for windows file name compatibility
-        log_name = log_name.replace(":", "-")
+        if PLOT_SAVE_NAME is not None:
+            log_name = PLOT_SAVE_NAME + "_"
+        else:
+            # Set the plot name as the current time
+            log_name = 'rtplot_' 
+    
+    #Add the timestamp to the log name
+    log_name += timestamp
 
     #Add to the save path for the datafiles
     total_name = os.path.join(
         PLOT_SAVE_PATH, log_name + ".parquet"
     )
     
     # Create the dataframe object so that we can add info about the subplot
@@ -276,15 +329,14 @@
         columns=trace_names + non_plot_labels,
     )
     df.to_parquet(total_name)
 
     # Output text confirming we saved
     print(f"Saved the plot as {total_name}")
 
-
 ###########################
 # PyQTgraph Configuration #
 ###########################
 
 # START QtApp
 # You MUST do this once to initialize pyqtgraph
 # app = QtWidgets.QApplication([])
@@ -446,18 +498,18 @@
             new_plot.setTitle("", **title_style)
 
         # Define default Style
         colors = ["r", "g", "b", "c", "m", "y"]
         if "colors" in plot_description:
             colors = plot_description["colors"]
 
-        line_style = [QtCore.Qt.SolidLine] * num_traces
+        line_style = [QtCore.Qt.PenStyle.SolidLine] * num_traces
         if "line_style" in plot_description:
             line_style = [
-                QtCore.Qt.DashLine if desc == "-" else QtCore.Qt.SolidLine
+                QtCore.Qt.PenStyle.DashLine if desc == "-" else QtCore.Qt.PenStyle.SolidLine
                 for desc 
                 in plot_description["line_style"]
             ]
 
         line_width = [1] * num_traces
         if "line_width" in plot_description:
             line_width = plot_description["line_width"]
@@ -475,15 +527,15 @@
             subplots_traces.append(new_curve)
             # Store the current trace name
             trace_info.append((trace_names[i], plot_num))
 
         # Add the new subplot
         subplots.append(new_plot)
 
-    print("Initialized Plot!")
+    print("Initialized Plot!                 ")
     return (
         traces_per_plot,
         subplots_traces,
         subplots,
         top_plot,
         top_plot_title,
         trace_info,
@@ -585,30 +637,39 @@
 subplots = None
 
 # Make sure that you don't try to plot data without having a plot
 initialized_plot = False
 
 # Create a counter that will be used in case we want to update the plot 
 # every X datapoints
-data_counter = 0
+data_between_plots_refresh = 0
 
 # Create a counter that will be used to determine if the incoming data is 
 # coming in faster than we can process it
 data_rate_counter = 0
 
+# Create a counter between adaptations
+data_between_adaptations = 0
+
 # Main code loop
 while True:
     # Receive the type of information
     category = rec_type()
 
     # Do not continue unless you have initialized the plot
     if category == RECEIVED_PLOT_UPDATE:
 
         # Reset the data counter to zero
-        data_counter = 0
+        data_between_plots_refresh = 0
+        data_rate_counter = 0
+        data_between_adaptations = 0
+
+        # If we are adapting the skip points, reset to one
+        if ADAPT_SKIP_PLOT_DATAPOINTS:
+            SKIP_PLOT_DATAPOINTS = 1
 
         # Receive plot configuration
         flags = 0
         plot_configuration = socket.recv_json(flags=flags)
 
         # Initialize plot
         (
@@ -712,32 +773,70 @@
             li : li + num_values
         ] = receive_np_array[
             local_storage_buffer_num_trace:local_storage_buffer_num_trace+num_non_plot_traces,:]
 
         # Increase the local storage index variable
         li += num_values
 
-        # Update fps in title
+        # Verify if we are processing data faster than we are getting it
         if data_rate_counter < 100:
-            color = "green"
+            # If we have recently taken a break, assume we are good
+            if ADAPT_SKIP_PLOT_DATAPOINTS is True \
+                and data_between_adaptations > 200\
+                and SKIP_PLOT_DATAPOINTS > 1:
+                
+                SKIP_PLOT_DATAPOINTS -= 1
+                print(f"Adapted skip points to be: {SKIP_PLOT_DATAPOINTS}    ",
+                      end="\r")
+                data_between_adaptations = 0
+
+            # Green good
+            title_color = "green"
         else:
-            color = "red"
-        top_plot.setTitle(top_plot_title + f" - FPS:{fps:.0f}", color=color)
+            # If we have processed 100 data points without tacking a break, 
+            # assume we are getting overwhelmed. If so, increase the datapoints 
+            # we skip. However, don't skip more than 30% of the datapoints in
+            # the plot since that would be way too choppy
+            skip_points_cutoff = int(num_datapoints_in_plot*0.3)
+            if ADAPT_SKIP_PLOT_DATAPOINTS is True \
+                and data_between_adaptations > 200\
+                and SKIP_PLOT_DATAPOINTS < skip_points_cutoff:
+                
+                SKIP_PLOT_DATAPOINTS += 1
+                print(f"Adapted skip points to be: {SKIP_PLOT_DATAPOINTS}    ",
+                      end="\r")
+                data_between_adaptations = 0
+
+            # Red bad
+            title_color = "red"
+        
+        # Update fps in title
+        # If we have non-plotting variables, add them the amount to the title
+        if num_non_plot_traces > 0:
+            non_plot_text = f" - Non Plot Trace: {num_non_plot_traces}"
+        else:
+            non_plot_text = ""
+        
+        fps_text = f" - FPS:{fps:.0f}"
+        # IF not, don't even include it
+        top_plot.setTitle(top_plot_title + non_plot_text + fps_text,
+                            color=title_color)
 
         # Update the data counter and data_rate counter
-        data_counter += 1
+        data_between_plots_refresh += 1
         data_rate_counter += 1
+        data_between_adaptations += 1
 
         # If you have reached the number of datapoints to update the plot
         # update the plot
-        if data_counter % SKIP_PLOT_DATAPOINTS == 0:
+        if data_between_plots_refresh % SKIP_PLOT_DATAPOINTS == 0:
             # Indicate you MUST process the plot now
             QtWidgets.QApplication.processEvents()
             # Reset the data counter
-            data_counter = 0
+            data_between_plots_refresh = 0
 
     elif category == SAVE_PLOT:
         #Get the log name
         log_name = socket.recv_string()
         #Save the plot with the log name
         save_current_plot(log_name)
```

