# Comparing `tmp/model_composer-0.2.0-py3-none-any.whl.zip` & `tmp/model_composer-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 11092 bytes, number of entries: 14
+Zip file size: 11509 bytes, number of entries: 14
 -rw-r--r--  2.0 unx     1074 b- defN 80-Jan-01 00:00 LICENSE.txt
--rw-r--r--  2.0 unx     3502 b- defN 80-Jan-01 00:00 README.md
+-rw-r--r--  2.0 unx     4239 b- defN 80-Jan-01 00:00 README.md
 -rw-r--r--  2.0 unx      227 b- defN 80-Jan-01 00:00 model_composer/__init__.py
 -rw-r--r--  2.0 unx     1757 b- defN 80-Jan-01 00:00 model_composer/_utils.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 model_composer/implementations/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 model_composer/implementations/tensorflow/__init__.py
 -rw-r--r--  2.0 unx    12061 b- defN 80-Jan-01 00:00 model_composer/implementations/tensorflow/composer.py
 -rw-r--r--  2.0 unx      763 b- defN 80-Jan-01 00:00 model_composer/interface.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 model_composer/py.typed
 -rw-r--r--  2.0 unx     2442 b- defN 80-Jan-01 00:00 model_composer/spec.py
--rw-r--r--  2.0 unx     1074 b- defN 80-Jan-01 00:00 model_composer-0.2.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     4512 b- defN 80-Jan-01 00:00 model_composer-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 model_composer-0.2.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1176 b- defN 16-Jan-01 00:00 model_composer-0.2.0.dist-info/RECORD
-14 files, 28676 bytes uncompressed, 9118 bytes compressed:  68.2%
+-rw-r--r--  2.0 unx     1074 b- defN 80-Jan-01 00:00 model_composer-0.3.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     5381 b- defN 80-Jan-01 00:00 model_composer-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 model_composer-0.3.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1176 b- defN 16-Jan-01 00:00 model_composer-0.3.0.dist-info/RECORD
+14 files, 30282 bytes uncompressed, 9535 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: model_composer/py.typed
 Comment: 
 
 Filename: model_composer/spec.py
 Comment: 
 
-Filename: model_composer-0.2.0.dist-info/LICENSE.txt
+Filename: model_composer-0.3.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: model_composer-0.2.0.dist-info/METADATA
+Filename: model_composer-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: model_composer-0.2.0.dist-info/WHEEL
+Filename: model_composer-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: model_composer-0.2.0.dist-info/RECORD
+Filename: model_composer-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## README.md

```diff
@@ -1,24 +1,33 @@
 # Model Composer
 
+<br>
+
+[![PyPI version shields.io](https://img.shields.io/pypi/v/model-composer.svg)](https://pypi.org/project/model-composer/)
+[![PyPI license](https://img.shields.io/pypi/l/model-composer.svg)](https://pypi.python.org/pypi/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/model-composer.svg)](https://pypi.python.org/pypi/model-composer/)
+[![Downloads](https://pepy.tech/badge/model-composer/month)](https://pepy.tech/project/model-composer)
+[![Downloads](https://pepy.tech/badge/model-composer)](https://pepy.tech/project/model-composer)
+
+
 ## Motivation
 
 This use-case prompted the development of `model-composer`:
 
 - You have two tensorflow models, one trained on weekday data and one trained on weekend data
 - You would like to compose a single tensorflow model that can be used to generate predictions for any day of the week.
 - You want the composed model to be natively defined in tensorflow - i.e. a single "computational graph" that can be easily loaded and used to make predictions.
 - You want a single composed model becasuse:
   - It is easier to maintain than having to implement the logic to compose the models in every service that needs to make predictions.
   - It ensures the performance of the composed model will remain consistent with a native tensorflow model of a similar complexity.
   - It is easier to deploy a single model than multiple models
 
 ## Documentation
 
-The official documentation is hosted on ReadTheDocs: https://model-composer.readthedocs.io
+The official documentation is hosted on ReadTheDocs: https://model-composer.readthedocs.io/
 
 ## Install
 
 Using pip:
 
 ```
 pip install model-composer
@@ -30,38 +39,19 @@
 
 ```bash
 pip install model-composer[tensorflow]  # compose tensorflow models
 pip install model-composer[cloudpathlib]  # load models from cloud storage
 pip install model-composer[all]  # all extras
 ```
 
-## Supported ML libraries
-
-- Tensorflow
-
-## Roadmap
-
-- Support for more ML frameworks:
-  - PyTorch
-  - Scikit-learn
-
-## How to setup
-
-```bash
-pip install model_composer
-```
-
 ## Quick start
 
-We define our composed model using a composed model spec which can be serialized in a human-readable file like yaml.
-
-```python
-import yaml
+Declare your composed model in a yaml file which defines the components and how they should be composed.
 
-example = """
+```yaml title="example.yaml"
 name: "ride_share_pricing"
 components:
   - name: weekday_model
     path: weekday_model.tf
     type: tensorflow
     where:
       input: is_weekday
@@ -70,20 +60,24 @@
   - name: weekend_model
     path: weekend_model.tf
     type: tensorflow
     where:
       input: is_weekday
       operator: eq
       value: false
-"""
-with open("example.yaml", "w") as f:
-    f.write(example)
 ```
 
-We build each model separately and save it to disk.
+Each component needs to have the following properties:
+
+- `name`: The name of the component model
+- `path`: The path to the component model on disk
+- `type`: The type of the component model.
+- `where`: The condition at which the component model should be used.
+
+We build the weekend model and save it to disk.
 
 ```python
 import tensorflow as tf
 
 # Build the weekend model
 weekend_model = tf.keras.Sequential([
     tf.keras.layers.Input(shape=(1,), name="distance"),
@@ -94,16 +88,19 @@
 
 weekend_model.fit(
     x={"distance": tf.convert_to_tensor([10, 20], dtype=tf.float32)},
     y=tf.convert_to_tensor([10, 20], dtype=tf.float32),
     epochs=10
 )
 weekend_model.save("weekend_model.tf")
+```
 
+We build the weekday model and save it to disk.
 
+```python
 # Build the weekday model
 weekday_model = tf.keras.Sequential([
     tf.keras.layers.Input(shape=(1,), name="distance"),
     tf.keras.layers.Dense(1, name="price")
 ])
 
 weekday_model.compile(optimizer="adam", loss="mse")
@@ -114,24 +111,32 @@
     epochs=10
 )
 
 # Save the models
 weekday_model.save("weekday_model.tf")
 ```
 
-We can then load the composed model spec and use it to make predictions.
+We can now build our composed model from the example yaml spec.
 
 ```python
 import tensorflow as tf
 from model_composer import TensorflowModelComposer
 
 composed_model = TensorflowModelComposer().from_yaml("example.yaml")
 
+assert isinstance(composed_model, tf.keras.Model)
+
 composed_model.save("composed_model.tf")
 
 loaded_model = tf.keras.models.load_model("composed_model.tf")
 
 composed_model.predict({
   "is_weekday": tf.convert_to_tensor([True, False], dtype=tf.bool),
   "distance": tf.convert_to_tensor([10, 20], dtype=tf.float32)
 })
 ```
+
+## Roadmap
+
+- Support for more ML frameworks:
+  - PyTorch
+  - Scikit-learn
```

## Comparing `model_composer-0.2.0.dist-info/LICENSE.txt` & `model_composer-0.3.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `model_composer-0.2.0.dist-info/RECORD` & `model_composer-0.3.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 LICENSE.txt,sha256=Mnp2fKtOQumiboMO2u1yHN6pPUPHYZ8XlTZ5cyV6a_g,1074
-README.md,sha256=4SWdfcuXuuc4c6Z9-MvDoEEi6icUJVym8qQnOXmbhic,3502
+README.md,sha256=YoT3_RaU-DYVqL1dRceqpVo03nvKhfYrrBASExNy2Jk,4239
 model_composer/__init__.py,sha256=3TY3vgbb04IDlv9tRACzIxrBlrPJoJtkLWyumV1i-q4,227
 model_composer/_utils.py,sha256=EuHZfpvL2eiVpvvFt7dvolcBTQALRzQMKKCJuz616dA,1757
 model_composer/implementations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 model_composer/implementations/tensorflow/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 model_composer/implementations/tensorflow/composer.py,sha256=TiF5xON_MWu7Mij12EAwtrDnMiRMTrn458o8pgpzjrI,12061
 model_composer/interface.py,sha256=J9xcr6BQpOqUfKux0XoSM4it0z2FJ7WZMANenJoj5q4,763
 model_composer/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 model_composer/spec.py,sha256=oTskNRZxM1oQP4GqN4--T1-oq9zHRHSgHyJbpxhLAJA,2442
-model_composer-0.2.0.dist-info/LICENSE.txt,sha256=Mnp2fKtOQumiboMO2u1yHN6pPUPHYZ8XlTZ5cyV6a_g,1074
-model_composer-0.2.0.dist-info/METADATA,sha256=POmOn2MVFYuuMK8qrrcYynrt0Lb1OOXWAoYvdJLA-_U,4512
-model_composer-0.2.0.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
-model_composer-0.2.0.dist-info/RECORD,,
+model_composer-0.3.0.dist-info/LICENSE.txt,sha256=Mnp2fKtOQumiboMO2u1yHN6pPUPHYZ8XlTZ5cyV6a_g,1074
+model_composer-0.3.0.dist-info/METADATA,sha256=iAe6ZEM4o16-PZfndAGqLOvx9x6INf-Ymd_6zgFb8Zs,5381
+model_composer-0.3.0.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
+model_composer-0.3.0.dist-info/RECORD,,
```

