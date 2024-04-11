# Comparing `tmp/polynomial_generator-0.1.0.tar.gz` & `tmp/polynomial_generator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polynomial_generator-0.1.0.tar", max compression
+gzip compressed data, was "polynomial_generator-0.1.1.tar", max compression
```

## Comparing `polynomial_generator-0.1.0.tar` & `polynomial_generator-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2024-04-11 10:53:22.170528 polynomial_generator-0.1.0/LICENSE
--rw-r--r--   0        0        0     2328 2024-04-11 10:53:22.174528 polynomial_generator-0.1.0/README.md
--rw-r--r--   0        0        0     2294 2024-04-11 10:53:22.170528 polynomial_generator-0.1.0/polynomial_generator/polynomial.py
--rw-r--r--   0        0        0     2823 2024-04-11 10:53:22.170528 polynomial_generator-0.1.0/polynomial_generator/polynomial_app.py
--rw-r--r--   0        0        0      780 2024-04-11 10:53:22.170528 polynomial_generator-0.1.0/polynomial_generator/polynomial_cli.py
--rw-r--r--   0        0        0      339 2024-04-11 10:53:22.170528 polynomial_generator-0.1.0/polynomial_generator/pyinstaller_script.py
--rw-r--r--   0        0        0      616 2024-04-11 10:53:22.170528 polynomial_generator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2956 1970-01-01 00:00:00.000000 polynomial_generator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-11 11:14:32.772378 polynomial_generator-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2398 2024-04-11 11:14:32.776378 polynomial_generator-0.1.1/README.md
+-rw-r--r--   0        0        0     2330 2024-04-11 11:14:32.784378 polynomial_generator-0.1.1/polynomial_generator/polynomial.py
+-rw-r--r--   0        0        0     2983 2024-04-11 11:14:32.784378 polynomial_generator-0.1.1/polynomial_generator/polynomial_app.py
+-rw-r--r--   0        0        0      879 2024-04-11 11:14:32.784378 polynomial_generator-0.1.1/polynomial_generator/polynomial_cli.py
+-rw-r--r--   0        0        0      599 2024-04-11 11:14:32.784378 polynomial_generator-0.1.1/polynomial_generator/pyinstaller_script.py
+-rw-r--r--   0        0        0      652 2024-04-11 11:14:59.848722 polynomial_generator-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3026 1970-01-01 00:00:00.000000 polynomial_generator-0.1.1/PKG-INFO
```

### Comparing `polynomial_generator-0.1.0/LICENSE` & `polynomial_generator-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `polynomial_generator-0.1.0/README.md` & `polynomial_generator-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: polynomial-generator
+Version: 0.1.1
+Summary: A Python package for generating polynomial expressions
+License: MIT
+Author: Hermann Agossou
+Author-email: agossouhermann7@gmail.com
+Requires-Python: >=3.8,<3.13
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
+
 # Polynomial Generator
 
 [![License](https://img.shields.io/github/license/hermann-web/polynomial-generator)](LICENSE)
 [![Release](https://img.shields.io/github/v/release/hermann-web/polynomial-generator)](https://github.com/hermann-web/polynomial-generator/releases)
 
 ## Overview
 
@@ -51,15 +68,15 @@
 
 ```bash
 polygenapp
 ```
 
 Enter the variables and degree for your polynomial, then click "Generate" to see the result.
 
-![GUI Frontend](./assets/polygenapp-example.png)
+![GUI Frontend](https://raw.githubusercontent.com/Hermann-web/polynomial-generator/main/assets/polygenapp-example.png)
 
 ## Contributing
 
 Contributions are welcome! If you'd like to contribute to this project, please follow these steps:
 
 1. Fork the repository.
 2. Create a new branch (`git checkout -b feature/improvement`).
@@ -71,7 +88,8 @@
 ## License
 
 This project is licensed under the [MIT License](LICENSE).
 
 ## Contact
 
 For any questions or feedback, feel free to contact [Hermann Agossou](mailto:agossouhermann7@gmail.com).
+
```

### Comparing `polynomial_generator-0.1.0/polynomial_generator/polynomial.py` & `polynomial_generator-0.1.1/polynomial_generator/polynomial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
-generate_polynomial_expression.py
+polynomial_generator/polynomial.py
 
 A Python module for generating polynomial expressions based on the specified variables and degree.
 
 Author: Hermann Agossou
-
+Date: 2024/04/11
 """
 
 from itertools import product
 
+
 def generate_polynomial_expression(variables, degree):
     """
     Generate a polynomial expression for a given list of variables and degree.
 
     Args:
         variables (list): A list of variable names as strings.
         degree (int): The degree of the polynomial.
@@ -27,38 +28,42 @@
         "('x + y + z)^2', 'x^2 + x*y + x*z + y^2 + y*z + z^2'"
     """
 
     variables = [elt.strip() for elt in variables]
 
     # Generate all possible combinations of exponents for the variables
     combinations = product(range(degree + 1), repeat=len(variables))
-    
+
     # Filter combinations to include only those whose exponents sum up to the given degree
     combinations = filter(lambda x: sum(x) == degree, combinations)
 
     # Initialize the polynomial expression
     expression = ""
 
     # Iterate over each combination of exponents
     for combination in combinations:
         # Generate terms for the current combination
-        terms = [f"{var}" if exp == 1 else f"{var}^{exp}" if exp > 1 else None for (exp, var) in zip(combination, variables)]
+        terms = [
+            f"{var}" if exp == 1 else f"{var}^{exp}" if exp > 1 else None
+            for (exp, var) in zip(combination, variables)
+        ]
         terms = filter(lambda x: x, terms)  # Remove None values
         # Join the terms with '*' and add them to the polynomial expression
         expression = "*".join(terms) + " + " + expression
-    
+
     # Removing the trailing " + " from the last term
     expression = expression.rstrip("+ ")
-    
+
     # Generate the first term of the polynomial
     first_term = f"({' + '.join(variables)})^{degree}"
-    
+
     return first_term, expression
 
+
 # Example usage:
 if __name__ == "__main__":
-    variables = ['x', 'y', 'z', 't']
+    variables = ["x", "y", "z", "t"]
     nb_var = 3
     variables = variables[:nb_var]
     degree = 2
     first_term, expression = generate_polynomial_expression(variables, degree)
-    print(f"{first_term} = {expression}" )
+    print(f"{first_term} = {expression}")
```

### Comparing `polynomial_generator-0.1.0/polynomial_generator/polynomial_app.py` & `polynomial_generator-0.1.1/polynomial_generator/polynomial_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """
+polynomial_generator/polynomial_app.py
+
 Polynomial Generator Application
 
 This application allows users to generate polynomial expressions based on specified variables and degree.
 
-Author: [Your Name]
-Date: [Current Date]
+Author: Hermann Agossou
+Date: 2024/04/11
 """
 
 import tkinter as tk
 from tkinter import ttk
+
 from polynomial_generator.polynomial import generate_polynomial_expression
 
 
 class PolynomialGeneratorApp:
     """
     GUI application for generating polynomial expressions.
     """
@@ -41,29 +44,39 @@
         self.degree_label = ttk.Label(root, text="Degree:")
         self.degree_label.grid(row=1, column=0, padx=5, pady=5)
         self.degree_entry = ttk.Entry(root, text=self.default_degree)
         self.degree_entry.insert(0, self.default_degree)
         self.degree_entry.grid(row=1, column=1, padx=5, pady=5)
 
         # Button for generating polynomial
-        self.generate_button = ttk.Button(root, text="Generate", command=self.generate_polynomial)
+        self.generate_button = ttk.Button(
+            root, text="Generate", command=self.generate_polynomial
+        )
         self.generate_button.grid(row=2, column=0, columnspan=2, padx=5, pady=5)
 
         # Label and Text widget for displaying result polynomial
         self.result_label = ttk.Label(root, text="Polynomial:")
         self.result_label.grid(row=3, column=0, padx=5, pady=5)
         self.result_text = tk.Text(root, height=4, width=50)
         self.result_text.grid(row=3, column=1, padx=5, pady=5)
 
     def generate_polynomial(self):
         """
         Generate polynomial expression based on user input variables and degree.
         """
-        variables = self.variables_entry.get().split(",") if self.variables_entry.get() else self.default_variables.split(",")
-        degree = int(self.degree_entry.get()) if self.degree_entry.get() else int(self.default_degree)
+        variables = (
+            self.variables_entry.get().split(",")
+            if self.variables_entry.get()
+            else self.default_variables.split(",")
+        )
+        degree = (
+            int(self.degree_entry.get())
+            if self.degree_entry.get()
+            else int(self.default_degree)
+        )
 
         first_term, polynomial = generate_polynomial_expression(variables, degree)
 
         self.result_text.delete(1.0, tk.END)
         self.result_text.insert(tk.END, first_term + " --> " + polynomial)
 
 
@@ -71,9 +84,10 @@
     """
     Main function to create and run the PolynomialGeneratorApp.
     """
     root = tk.Tk()
     app = PolynomialGeneratorApp(root)
     root.mainloop()
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `polynomial_generator-0.1.0/pyproject.toml` & `polynomial_generator-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [tool.poetry]
 name = "polynomial-generator"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Python package for generating polynomial expressions"
 authors = ["Hermann Agossou <agossouhermann7@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13"
 
 [tool.poetry.group.dev.dependencies]
 pyinstaller = "^6.5.0"
+isort = "^5.13.2"
+black = "^24.3.0"
 
 [tool.poetry.scripts]
 polygen = "polynomial_generator.polynomial_cli:main"
 polygenapp = "polynomial_generator.polynomial_app:main"
 build = "polynomial_generator.pyinstaller_script:install"
 
 [build-system]
```

### Comparing `polynomial_generator-0.1.0/PKG-INFO` & `polynomial_generator-0.1.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: polynomial-generator
-Version: 0.1.0
-Summary: A Python package for generating polynomial expressions
-License: MIT
-Author: Hermann Agossou
-Author-email: agossouhermann7@gmail.com
-Requires-Python: >=3.8,<3.13
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Description-Content-Type: text/markdown
-
 # Polynomial Generator
 
 [![License](https://img.shields.io/github/license/hermann-web/polynomial-generator)](LICENSE)
 [![Release](https://img.shields.io/github/v/release/hermann-web/polynomial-generator)](https://github.com/hermann-web/polynomial-generator/releases)
 
 ## Overview
 
@@ -68,15 +51,15 @@
 
 ```bash
 polygenapp
 ```
 
 Enter the variables and degree for your polynomial, then click "Generate" to see the result.
 
-![GUI Frontend](./assets/polygenapp-example.png)
+![GUI Frontend](https://raw.githubusercontent.com/Hermann-web/polynomial-generator/main/assets/polygenapp-example.png)
 
 ## Contributing
 
 Contributions are welcome! If you'd like to contribute to this project, please follow these steps:
 
 1. Fork the repository.
 2. Create a new branch (`git checkout -b feature/improvement`).
@@ -88,8 +71,7 @@
 ## License
 
 This project is licensed under the [MIT License](LICENSE).
 
 ## Contact
 
 For any questions or feedback, feel free to contact [Hermann Agossou](mailto:agossouhermann7@gmail.com).
-
```

