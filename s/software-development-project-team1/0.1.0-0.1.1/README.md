# Comparing `tmp/software_development_project_team1-0.1.0.tar.gz` & `tmp/software_development_project_team1-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "software_development_project_team1-0.1.0.tar", last modified: Thu Apr 11 16:35:18 2024, max compression
+gzip compressed data, was "software_development_project_team1-0.1.1.tar", last modified: Thu Apr 11 18:34:13 2024, max compression
```

## Comparing `software_development_project_team1-0.1.0.tar` & `software_development_project_team1-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 16:35:18.334616 software_development_project_team1-0.1.0/
--rw-rw-rw-   0        0        0     1086 2024-02-19 08:02:42.000000 software_development_project_team1-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      620 2024-04-11 16:35:18.332045 software_development_project_team1-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4244 2024-04-10 17:43:52.000000 software_development_project_team1-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-11 16:35:18.334616 software_development_project_team1-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      663 2024-04-11 16:35:15.000000 software_development_project_team1-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 16:35:18.332045 software_development_project_team1-0.1.0/software_development_project_team1.egg-info/
--rw-rw-rw-   0        0        0      620 2024-04-11 16:35:18.000000 software_development_project_team1-0.1.0/software_development_project_team1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-04-11 16:35:18.000000 software_development_project_team1-0.1.0/software_development_project_team1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 16:35:18.000000 software_development_project_team1-0.1.0/software_development_project_team1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 16:35:18.000000 software_development_project_team1-0.1.0/software_development_project_team1.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 18:34:13.418882 software_development_project_team1-0.1.1/
+-rw-rw-rw-   0        0        0     1086 2024-02-19 08:02:42.000000 software_development_project_team1-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      620 2024-04-11 18:34:13.416997 software_development_project_team1-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5226 2024-04-11 16:58:15.000000 software_development_project_team1-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-11 18:34:13.420390 software_development_project_team1-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      663 2024-04-11 18:31:58.000000 software_development_project_team1-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 18:34:13.404177 software_development_project_team1-0.1.1/software_development_project_team1/
+-rw-rw-rw-   0        0        0        0 2024-04-10 17:43:52.000000 software_development_project_team1-0.1.1/software_development_project_team1/__init__.py
+-rw-rw-rw-   0        0        0    11922 2024-04-11 16:55:28.000000 software_development_project_team1-0.1.1/software_development_project_team1/autoencoder.py
+-rw-rw-rw-   0        0        0    17650 2024-04-11 16:54:24.000000 software_development_project_team1-0.1.1/software_development_project_team1/genetic_algorithm.py
+-rw-rw-rw-   0        0        0    10170 2024-04-11 16:54:24.000000 software_development_project_team1-0.1.1/software_development_project_team1/identify_attacker.py
+-rw-rw-rw-   0        0        0    37373 2024-04-10 17:43:54.000000 software_development_project_team1-0.1.1/software_development_project_team1/projet_interface_class.py
+-rw-rw-rw-   0        0        0    15234 2024-04-10 17:43:54.000000 software_development_project_team1-0.1.1/software_development_project_team1/ui.py
+drwxrwxrwx   0        0        0        0 2024-04-11 18:34:13.415477 software_development_project_team1-0.1.1/software_development_project_team1.egg-info/
+-rw-rw-rw-   0        0        0      620 2024-04-11 18:34:13.000000 software_development_project_team1-0.1.1/software_development_project_team1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      569 2024-04-11 18:34:13.000000 software_development_project_team1-0.1.1/software_development_project_team1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 18:34:13.000000 software_development_project_team1-0.1.1/software_development_project_team1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-04-11 18:34:13.000000 software_development_project_team1-0.1.1/software_development_project_team1.egg-info/top_level.txt
```

### Comparing `software_development_project_team1-0.1.0/LICENSE` & `software_development_project_team1-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `software_development_project_team1-0.1.0/PKG-INFO` & `software_development_project_team1-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: software_development_project_team1
-Version: 0.1.0
+Version: 0.1.1
 Summary: Software to help victims portray a culprit using an autoencoder model trained on the CelebA dataset and a genetic algorithm
 Author: Laetitia Guérout, Théo Berthet, Lucas Bodelle & Synne Trettenes
 Author-email: laetitia.guerout@insa-lyon.fr, theo.berthet@insa-lyon.fr, lucas.bodelle@insa-lyon.fr, synne-moe.trettenes@insa-lyon.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `software_development_project_team1-0.1.0/README.md` & `software_development_project_team1-0.1.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,56 @@
 # BS-BMDEV
 
 ## How to run the project
 
+Open Docker Desktop on your computer. In the Dockerfile in this directory, put the name of the file that should be run when using the `./run.sh` command.
+
+Make `run.sh` executable: `chmod +x run.sh`
+
+Run `./run.sh`
+
 ## Identification software
 identify_attacker.py is a program that uses a combination of an autoencoder and a genetic algorithm to identify an "attacker" image from a set of images.
 
 The autoencoder is trained based on user input, with the option to train a new model or use an existing one. The model is then trained and its predictions are visualized.
 
 A population of images is initialized randomly from a batch. The user is then asked to select the image(s) that most resemble the attacker.
 
 The genetic algorithm and the autoencoder's encoder and decoder layers are used to identify the attacker. The algorithm initializes a random population, enters a loop for a maximum number of iterations, gets the victim's choice, encodes the victim's choice and the population, applies the genetic algorithm to generate a new population, decodes the new population, displays the new population, and updates the population.
 
 The main function of the script sets the parameters for the genetic algorithm, splits the data into a training set and a validation set, asks the user whether they want to train a model, and either trains a new model or loads an existing model and identifies the attacker.
 
+
 ## The autoencoder
 This Python script allows to create, train or load a variational antoencoder model for image reconstruction from celebA dataset. The autoencoder is built using Keras library with Tensorflow backend.
 
 The first step is the loading of the dataset and splitting in a training set and a validation set. The sets are tensor object containing Numpy arrays of a number of images determine by the batch size. The first images of each set are dipslayed to check the loading of data.
 
 Then you can choose to create a new variationnal autoencoder model. During the training the autoencoder is saved at the end of each epoch in the model file according to the name you entered and with a keras extension.
 
 To train a previously created model, enter the name of the .keras file presents in the model file without the .keras, the model will also be saved at the end of each epoch.
 At the end of the training, graph of loss value and val loss value can be displayed. Also the prediction on the validation set are displayed.
 
 A previously trained model can be loaded without training, enter the name as previously. Predictions on the validation by the autoencoder and by the encoder followin by the decoder set will be displayed in order to check the encoder and decoder have been loaded correcly. 
 
-## The Genetic algorithm
-This Python script employs a genetic algorithm to generate images that closely resemble a target image. The genetic algorithm, inspired by the process of natural selection, is used as an optimization technique to find the best solution to a problem.
 
-The script starts by initializing a population of random genomes, each representing a potential solution - in this case, an image. These genomes are decoded into images using an autoencoder. The fitness of each image in the population is then evaluated based on how closely it resembles the target image. This is done by comparing the mean squared error between the target image and the generated image.
+## The Genetic algorithm 
+This Python code includes three different implementations of genetic algorithms for image processing. Each algorithm uses a different fitness function to evaluate the quality of the images, and different methods for parent selection, crossover, mutation, and new population generation.
+
+Genetic Algorithm with Mean Squared Error (MSE)
+This algorithm uses the Mean Squared Error (MSE) as the fitness function. MSE is a popular method to measure the error of an estimator and is calculated as the average squared difference between the estimated values and the actual value. In this context, a lower MSE value indicates a better fit.
 
-The algorithm then enters a loop where it continually selects the best genomes based on their fitness scores, uses them to generate a new population, and introduces random mutations to create variations. This process of selection, crossover, and mutation is repeated for a specified number of iterations to continually refine the solutions.
+For parent selection, this algorithm selects the best genomes based on the lowest fitness score. It uses single point crossover for mating and normal distribution for mutation. The new population is generated with elitism, meaning the best individuals from the previous generation are included in the new population.
 
-A unique aspect of this script is the inclusion of a human-in-the-loop (HITL) function, which allows a human user to interactively select the image that most closely resembles the target image. This adds a level of subjective judgment to the otherwise purely mathematical optimization process.
+Genetic Algorithm with Peak Signal-to-Noise Ratio (PSNR)
+This algorithm uses the Peak Signal-to-Noise Ratio (PSNR) as the fitness function. PSNR is an engineering term for the ratio between the maximum possible power of a signal and the power of corrupting noise that affects the fidelity of its representation. In this context, a higher PSNR value indicates a better fit.
 
-The script concludes by setting parameters for the genetic algorithm, such as the size of the population, the maximum number of iterations, and the mutation rate, and then running the algorithm. It also loads a database of images that are used to initialize the population of genomes.
+For parent selection, this algorithm selects the best genomes based on the highest fitness score. It uses two-point crossover for mating and bit flip mutation for mutation. The new population is generated without elitism.
 
-## UI
-# Requirements :
-Tensorflow : 2.15.0
-Keras : 2.15.0
+Genetic Algorithm with Structural Similarity Index (SSIM)
+This algorithm uses the Structural Similarity Index (SSIM) as the fitness function. SSIM is a method for comparing similarities between two images. The SSIM index is a full reference metric; in other words, the measurement or prediction of image quality is based on an initial uncompressed or distortion-free image as reference. In this context, a higher SSIM value indicates a better fit.
 
+For parent selection, this algorithm uses roulette wheel selection, where the probability of an individual being selected is proportional to its fitness score. It uses uniform crossover for mating and bit flip mutation for mutation. The new population is generated without elitism.
 
+Each of these algorithms can be used depending on the specific requirements of your image processing task.
 
+## UI
```

### Comparing `software_development_project_team1-0.1.0/setup.py` & `software_development_project_team1-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
 name='software_development_project_team1',
-version='0.1.0',
+version='0.1.1',
 author='Laetitia Guérout, Théo Berthet, Lucas Bodelle & Synne Trettenes',
 author_email='laetitia.guerout@insa-lyon.fr, theo.berthet@insa-lyon.fr, lucas.bodelle@insa-lyon.fr, synne-moe.trettenes@insa-lyon.fr',
 description='Software to help victims portray a culprit using an autoencoder model trained on the CelebA dataset and a genetic algorithm',
 packages=find_packages(),
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
```

### Comparing `software_development_project_team1-0.1.0/software_development_project_team1.egg-info/PKG-INFO` & `software_development_project_team1-0.1.1/software_development_project_team1.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: software-development-project-team1
-Version: 0.1.0
+Version: 0.1.1
 Summary: Software to help victims portray a culprit using an autoencoder model trained on the CelebA dataset and a genetic algorithm
 Author: Laetitia Guérout, Théo Berthet, Lucas Bodelle & Synne Trettenes
 Author-email: laetitia.guerout@insa-lyon.fr, theo.berthet@insa-lyon.fr, lucas.bodelle@insa-lyon.fr, synne-moe.trettenes@insa-lyon.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

