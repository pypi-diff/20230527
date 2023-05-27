# Comparing `tmp/LegacyNeuralNetworks-0.0.1.tar.gz` & `tmp/LegacyNeuralNetworks-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LegacyNeuralNetworks-0.0.1.tar", last modified: Sat May 27 08:56:31 2023, max compression
+gzip compressed data, was "LegacyNeuralNetworks-0.0.2.tar", last modified: Sat May 27 10:23:00 2023, max compression
```

## Comparing `LegacyNeuralNetworks-0.0.1.tar` & `LegacyNeuralNetworks-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 08:56:31.133143 LegacyNeuralNetworks-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-27 08:56:31.122563 LegacyNeuralNetworks-0.0.1/LegacyNeuralNetworks/
--rw-rw-rw-   0        0        0    28773 2023-05-27 08:54:50.000000 LegacyNeuralNetworks-0.0.1/LegacyNeuralNetworks/Fill.py
--rw-rw-rw-   0        0        0    19189 2023-05-27 08:44:43.000000 LegacyNeuralNetworks-0.0.1/LegacyNeuralNetworks/LegacyNeuralNetworks.py
--rw-rw-rw-   0        0        0      101 2023-05-27 08:55:33.000000 LegacyNeuralNetworks-0.0.1/LegacyNeuralNetworks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 08:56:31.131097 LegacyNeuralNetworks-0.0.1/LegacyNeuralNetworks.egg-info/
--rw-rw-rw-   0        0        0      649 2023-05-27 08:56:31.000000 LegacyNeuralNetworks-0.0.1/LegacyNeuralNetworks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2023-05-27 08:56:31.000000 LegacyNeuralNetworks-0.0.1/LegacyNeuralNetworks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 08:56:31.000000 LegacyNeuralNetworks-0.0.1/LegacyNeuralNetworks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-05-27 08:56:31.000000 LegacyNeuralNetworks-0.0.1/LegacyNeuralNetworks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-27 08:56:31.000000 LegacyNeuralNetworks-0.0.1/LegacyNeuralNetworks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      649 2023-05-27 08:56:31.132104 LegacyNeuralNetworks-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-27 08:56:31.133143 LegacyNeuralNetworks-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      859 2023-05-27 07:10:58.000000 LegacyNeuralNetworks-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 10:23:00.710592 LegacyNeuralNetworks-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-05-27 10:23:00.700169 LegacyNeuralNetworks-0.0.2/LegacyNeuralNetworks/
+-rw-rw-rw-   0        0        0    31698 2023-05-27 10:22:37.000000 LegacyNeuralNetworks-0.0.2/LegacyNeuralNetworks/Fill.py
+-rw-rw-rw-   0        0        0    19189 2023-05-27 08:44:43.000000 LegacyNeuralNetworks-0.0.2/LegacyNeuralNetworks/LegacyNeuralNetworks.py
+-rw-rw-rw-   0        0        0      101 2023-05-27 08:55:33.000000 LegacyNeuralNetworks-0.0.2/LegacyNeuralNetworks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 10:23:00.707581 LegacyNeuralNetworks-0.0.2/LegacyNeuralNetworks.egg-info/
+-rw-rw-rw-   0        0        0      649 2023-05-27 10:23:00.000000 LegacyNeuralNetworks-0.0.2/LegacyNeuralNetworks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-05-27 10:23:00.000000 LegacyNeuralNetworks-0.0.2/LegacyNeuralNetworks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 10:23:00.000000 LegacyNeuralNetworks-0.0.2/LegacyNeuralNetworks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-05-27 10:23:00.000000 LegacyNeuralNetworks-0.0.2/LegacyNeuralNetworks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-27 10:23:00.000000 LegacyNeuralNetworks-0.0.2/LegacyNeuralNetworks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      649 2023-05-27 10:23:00.708593 LegacyNeuralNetworks-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      595 2023-05-27 09:13:04.000000 LegacyNeuralNetworks-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-27 10:23:00.710592 LegacyNeuralNetworks-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      859 2023-05-27 10:22:51.000000 LegacyNeuralNetworks-0.0.2/setup.py
```

### Comparing `LegacyNeuralNetworks-0.0.1/LegacyNeuralNetworks/Fill.py` & `LegacyNeuralNetworks-0.0.2/LegacyNeuralNetworks/Fill.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 import os
 
 # String holders for code
 activation_function = """
+import numpy as np
+import tensorflow as tf
+import matplotlib.pyplot as plt
+from sklearn.linear_model import Perceptron
+from sklearn.datasets import make_classification
+from sklearn.neural_network import MLPClassifier
+
 class ActivationFunction:
     def __init__(self, function_name, grid=False):
         self.function_name = function_name
         self.grid = grid
 
     def plot(self):
         if self.function_name == 'sigmoid':
@@ -75,14 +82,21 @@
 
 # Change activation function names
 activation_func = ActivationFunction('tanh')
 activation_func.plot()
 """
 
 mcculloh_pitt = """
+import numpy as np
+import tensorflow as tf
+import matplotlib.pyplot as plt
+from sklearn.linear_model import Perceptron
+from sklearn.datasets import make_classification
+from sklearn.neural_network import MLPClassifier
+
 class McCullochPittsNeuron:
     def __init__(self):
         pass
 
     def activate(self, inputs, weights, threshold=3):
         weighted_sum = sum(w * x for w, x in zip(weights, inputs))
         if weighted_sum >= threshold:
@@ -97,14 +111,21 @@
 neuron = McCullochPittsNeuron()
 weights = [1, 4]
 x1 = 0; x2 = 0
 output = neuron.andnot(x1, x2, weights)
 """
 
 ascii_perceptron = """ 
+import numpy as np
+import tensorflow as tf
+import matplotlib.pyplot as plt
+from sklearn.linear_model import Perceptron
+from sklearn.datasets import make_classification
+from sklearn.neural_network import MLPClassifier
+
 class Perceptron:
     def __init__(self, input_size):
         self.weights = np.random.rand(input_size)
         self.bias = np.random.rand()
 
     def activate(self, inputs):
         weighted_sum = np.dot(self.weights, inputs) + self.bias
@@ -150,14 +171,21 @@
 
 for number, prediction in zip(X_test, predictions):
     result = "Even" if prediction == 0 else "Odd"
     print(f"Number: {number[0]}, Prediction: {result}")
 """
 
 descision_region_perceptron = """ 
+import numpy as np
+import tensorflow as tf
+import matplotlib.pyplot as plt
+from sklearn.linear_model import Perceptron
+from sklearn.datasets import make_classification
+from sklearn.neural_network import MLPClassifier
+
 class PerceptronPlotter:
     def __init__(self, random_seed=42):
         self.random_seed = random_seed
         self.X_train = None
         self.y_train = None
         self.clf = None
 
@@ -187,14 +215,21 @@
         self.plot_decision_regions()
 
 plotter = PerceptronPlotter(random_seed=44)
 plotter.run()
 """
 
 recognize_5x3_matrix = """ 
+import numpy as np
+import tensorflow as tf
+import matplotlib.pyplot as plt
+from sklearn.linear_model import Perceptron
+from sklearn.datasets import make_classification
+from sklearn.neural_network import MLPClassifier
+
 class PerceptronNN:
     def __init__(self, nn=10):
         self.nn = nn
         self.clf = MLPClassifier(hidden_layer_sizes=(self.nn,), random_state=42)
         self.train_data = {
             0: [[1, 1, 1], [1, 0, 1], [1, 0, 1], [1, 0, 1], [1, 1, 1]],
             1: [[0, 1, 0], [0, 1, 0], [0, 1, 0], [0, 1, 0], [0, 1, 0]],
@@ -235,14 +270,21 @@
 recognizer = PerceptronNN(16)
 recognizer.train()
 test_data = np.array([test_data]).flatten()
 print(predictions)
 """
 
 ann_forward_backward = """ 
+import numpy as np
+import tensorflow as tf
+import matplotlib.pyplot as plt
+from sklearn.linear_model import Perceptron
+from sklearn.datasets import make_classification
+from sklearn.neural_network import MLPClassifier
+
 class NeuralNetwork:
     def __init__(self, input_size, hidden_size, output_size):
         self.input_size = input_size
         self.hidden_size = hidden_size
         self.output_size = output_size
         
         # Initialize weights and biases
@@ -344,14 +386,21 @@
 new_data = np.array([[0, 0], [0, 1], [1, 0], [1, 1]])
 predictions = nn.predict(new_data)
 
 print(predictions)
 """
 
 xor_backprop = """ 
+import numpy as np
+import tensorflow as tf
+import matplotlib.pyplot as plt
+from sklearn.linear_model import Perceptron
+from sklearn.datasets import make_classification
+from sklearn.neural_network import MLPClassifier
+
 class BackpropagationXOR:
     def __init__(self):
         # Initialize weights and biases
         self.W1 = np.random.randn(2, 2)
         self.b1 = np.zeros((1, 2))
         self.W2 = np.random.randn(2, 1)
         self.b2 = np.zeros((1, 1))
@@ -450,14 +499,21 @@
 predictions = xor_net.predict(new_data)
 
 # Print the predictions
 predictions
 """
 
 art_network = """ 
+import numpy as np
+import tensorflow as tf
+import matplotlib.pyplot as plt
+from sklearn.linear_model import Perceptron
+from sklearn.datasets import make_classification
+from sklearn.neural_network import MLPClassifier
+
 class ARTNeuralNetwork:
     def __init__(self, num_features, max_categories=100, rho=0.5, beta=1.0):
         self.num_features = num_features
         self.max_categories = max_categories
         self.rho = rho
         self.beta = beta
 
@@ -512,14 +568,21 @@
 
 # Predict categories for patterns
 predictions = art1.predict(patterns)
 print(f"Predicted categories: {predictions}")
 """
 
 hopfield_network = """ 
+import numpy as np
+import tensorflow as tf
+import matplotlib.pyplot as plt
+from sklearn.linear_model import Perceptron
+from sklearn.datasets import make_classification
+from sklearn.neural_network import MLPClassifier
+
 class HopfieldNetwork:
     def __init__(self, num_neurons):
         self.num_neurons = num_neurons
         self.weights = np.zeros((num_neurons, num_neurons))
 
     def train(self, training_vectors):
         num_vectors = len(training_vectors)
@@ -554,14 +617,21 @@
 recalled_vector = hopfield.recall(noisy_vector, steps=5)
 
 print(f"Noisy input:    {noisy_vector}")
 print(f"Recalled output: {recalled_vector.tolist()}")
 """
 
 cnn_object_detection = """ 
+import numpy as np
+import tensorflow as tf
+import matplotlib.pyplot as plt
+from sklearn.linear_model import Perceptron
+from sklearn.datasets import make_classification
+from sklearn.neural_network import MLPClassifier
+
 class CNNObjectDetection:
     def __init__(self, num_classes=10, filters=32, kernel=(3, 3), dense_nodes=64):
         self.filters = filters
         self.kernel = kernel
         self.dense_nodes = dense_nodes
         self.num_classes = num_classes
         self.model = self.create_model()
@@ -635,14 +705,21 @@
 cnn.run(X_train, y_train, 
         X_val, y_val, 
         X_test, y_test, 
         epochs=20, batch_size=128)
 """
 
 cnn_image_classification = """ 
+import numpy as np
+import tensorflow as tf
+import matplotlib.pyplot as plt
+from sklearn.linear_model import Perceptron
+from sklearn.datasets import make_classification
+from sklearn.neural_network import MLPClassifier
+
 class CNNObjectDetection:
     def __init__(self, num_classes=10, filters=32, kernel=(3, 3), dense_nodes=64):
         self.filters = filters
         self.kernel = kernel
         self.dense_nodes = dense_nodes
         self.num_classes = num_classes
         self.model = self.create_model()
@@ -717,14 +794,21 @@
         X_val, y_val, 
         X_test, y_test, 
         epochs=20, batch_size=128,
         plot=True)
 """
 
 cnn_tf_implementation = """
+import numpy as np
+import tensorflow as tf
+import matplotlib.pyplot as plt
+from sklearn.linear_model import Perceptron
+from sklearn.datasets import make_classification
+from sklearn.neural_network import MLPClassifier
+
 class CNNModel:
     def __init__(self, num_classes):
         self.num_classes = num_classes
         self.model = self.build_model()
 
     def build_model(self):
         model = tf.keras.Sequential([
@@ -759,14 +843,21 @@
 cnn_model = CNNModel(num_classes)
 cnn_model.train(X_train, y_train, epochs=10, batch_size=32)
 cnn_model.evaluate(X_test, y_test)
 predictions = cnn_model.predict(X_test)
 """
 
 mnist_detection = """ 
+import numpy as np
+import tensorflow as tf
+import matplotlib.pyplot as plt
+from sklearn.linear_model import Perceptron
+from sklearn.datasets import make_classification
+from sklearn.neural_network import MLPClassifier
+
 class MNISTClassifier:
     def __init__(self):
         self.model = self.build_model()
 
     def build_model(self):
         model = tf.keras.Sequential([
             tf.keras.layers.Flatten(input_shape=(28, 28)),
```

### Comparing `LegacyNeuralNetworks-0.0.1/LegacyNeuralNetworks/LegacyNeuralNetworks.py` & `LegacyNeuralNetworks-0.0.2/LegacyNeuralNetworks/LegacyNeuralNetworks.py`

 * *Files identical despite different names*

### Comparing `LegacyNeuralNetworks-0.0.1/LegacyNeuralNetworks.egg-info/PKG-INFO` & `LegacyNeuralNetworks-0.0.2/LegacyNeuralNetworks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LegacyNeuralNetworks
-Version: 0.0.1
+Version: 0.0.2
 Summary: Legacy Neural Networks
 Home-page: UNKNOWN
 Author: Hrushikesh Kachgunde
 Author-email: <hrushiskachgunde@gmail.com>
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python,neural networks,ann,mcculloh-pitt,ART neural network
```

### Comparing `LegacyNeuralNetworks-0.0.1/PKG-INFO` & `LegacyNeuralNetworks-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LegacyNeuralNetworks
-Version: 0.0.1
+Version: 0.0.2
 Summary: Legacy Neural Networks
 Home-page: UNKNOWN
 Author: Hrushikesh Kachgunde
 Author-email: <hrushiskachgunde@gmail.com>
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python,neural networks,ann,mcculloh-pitt,ART neural network
```

### Comparing `LegacyNeuralNetworks-0.0.1/setup.py` & `LegacyNeuralNetworks-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Legacy Neural Networks'
  
 # Setting up
 setup(
     name="LegacyNeuralNetworks",
     version=VERSION,
     author="Hrushikesh Kachgunde",
```

