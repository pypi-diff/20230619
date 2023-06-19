# Comparing `tmp/VLCDA-1.0.3.tar.gz` & `tmp/VLCDA-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VLCDA-1.0.3.tar", last modified: Fri Jun 16 00:39:44 2023, max compression
+gzip compressed data, was "VLCDA-1.0.4.tar", last modified: Sat Jun 17 19:00:36 2023, max compression
```

## Comparing `VLCDA-1.0.3.tar` & `VLCDA-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 00:39:44.281137 VLCDA-1.0.3/
--rw-rw-rw-   0        0        0     1077 2023-06-16 00:19:36.000000 VLCDA-1.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     2066 2023-06-16 00:39:44.280138 VLCDA-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1406 2023-06-16 00:33:20.000000 VLCDA-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 00:39:44.250584 VLCDA-1.0.3/VLCDA/
--rw-rw-rw-   0        0        0    19570 2023-06-16 00:20:07.000000 VLCDA-1.0.3/VLCDA/Logic_Circuits_Evolution.py
--rw-rw-rw-   0        0        0        0 2023-06-13 23:22:24.000000 VLCDA-1.0.3/VLCDA/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 00:39:44.277127 VLCDA-1.0.3/VLCDA.egg-info/
--rw-rw-rw-   0        0        0     2066 2023-06-16 00:39:42.000000 VLCDA-1.0.3/VLCDA.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-06-16 00:39:44.000000 VLCDA-1.0.3/VLCDA.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 00:39:43.000000 VLCDA-1.0.3/VLCDA.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 00:39:43.000000 VLCDA-1.0.3/VLCDA.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 00:39:44.281137 VLCDA-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      884 2023-06-16 00:39:39.000000 VLCDA-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 19:00:36.903096 VLCDA-1.0.4/
+-rw-rw-rw-   0        0        0     1077 2023-06-16 00:19:36.000000 VLCDA-1.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-17 19:00:36.902094 VLCDA-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1406 2023-06-16 00:33:20.000000 VLCDA-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 19:00:36.866977 VLCDA-1.0.4/VLCDA/
+-rw-rw-rw-   0        0        0    19674 2023-06-17 19:00:23.000000 VLCDA-1.0.4/VLCDA/Logic_Circuits_Evolution.py
+-rw-rw-rw-   0        0        0        0 2023-06-13 23:22:24.000000 VLCDA-1.0.4/VLCDA/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 19:00:36.877556 VLCDA-1.0.4/VLCDA.egg-info/
+-rw-rw-rw-   0        0        0     2066 2023-06-17 19:00:36.000000 VLCDA-1.0.4/VLCDA.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2023-06-17 19:00:36.000000 VLCDA-1.0.4/VLCDA.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 19:00:36.000000 VLCDA-1.0.4/VLCDA.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-17 19:00:36.000000 VLCDA-1.0.4/VLCDA.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 19:00:36.898568 VLCDA-1.0.4/dist/
+-rw-rw-rw-   0        0        0     7475 2023-06-16 00:24:22.000000 VLCDA-1.0.4/dist/VLCDA-1.0.0-py3-none-any.whl
+-rw-rw-rw-   0        0        0     7746 2023-06-16 00:24:20.000000 VLCDA-1.0.4/dist/VLCDA-1.0.0.tar.gz
+-rw-rw-rw-   0        0        0     7472 2023-06-16 00:29:29.000000 VLCDA-1.0.4/dist/VLCDA-1.0.1-py3-none-any.whl
+-rw-rw-rw-   0        0        0     7531 2023-06-16 00:29:28.000000 VLCDA-1.0.4/dist/VLCDA-1.0.1.tar.gz
+-rw-rw-rw-   0        0        0     8172 2023-06-16 00:39:38.000000 VLCDA-1.0.4/dist/VLCDA-1.0.2-py3-none-any.whl
+-rw-rw-rw-   0        0        0     8301 2023-06-16 00:39:37.000000 VLCDA-1.0.4/dist/VLCDA-1.0.2.tar.gz
+-rw-rw-rw-   0        0        0     8181 2023-06-17 18:55:00.000000 VLCDA-1.0.4/dist/VLCDA-1.0.3-py3-none-any.whl
+-rw-rw-rw-   0        0        0    50423 2023-06-17 18:54:59.000000 VLCDA-1.0.4/dist/VLCDA-1.0.3.tar.gz
+-rw-rw-rw-   0        0        0       42 2023-06-17 19:00:36.903096 VLCDA-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      884 2023-06-17 18:55:14.000000 VLCDA-1.0.4/setup.py
```

### Comparing `VLCDA-1.0.3/LICENSE.txt` & `VLCDA-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.3/PKG-INFO` & `VLCDA-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VLCDA
-Version: 1.0.3
+Version: 1.0.4
 Summary: Modulo Python dedicado a evolução de circuitos lógicos através de algoritmos genéticos
 Home-page: https://github.com/HumbertoTavora/Logic-Circuits-Evolution
 Download-URL: https://github.com/HumbertoTavora/Logic-Circuits-Evolution
 Author: Humberto Távora, Stefan Blawid, Yasmin Maria
 Author-email: humbertocctg@gmail.com
 License: MIT
 Keywords: Genetic,Algorithm,Logic Circuits,Evolution,Optimization
```

### Comparing `VLCDA-1.0.3/README.md` & `VLCDA-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.3/VLCDA/Logic_Circuits_Evolution.py` & `VLCDA-1.0.4/VLCDA/Logic_Circuits_Evolution.py`

 * *Files 6% similar despite different names*

```diff
@@ -236,17 +236,17 @@
           #print(fitness,"\n\n\n\n\n")
           listFitness.append(fitness)
         
         c = 0
         for fitness in listFitness:
           c += fitness
         print(listFitness)
-        print("\n\n\nFitness final: ", c/trys)
-        
-    def calculateFitness(self):
+        print("\n\n\nFitness final: ", c/trys)     
+
+    def calculateFitness(self,logicFuncion):
         self.identify_deadGenes()
         fitnessCounter = 0
         l = []
         dic =  dict() 
 
         for i in range(0,self.nInputs):
             subL = [0,1]
@@ -277,15 +277,15 @@
             valueList = []
             for m in range(0,self.nInputs):
               sm = str(m)
               value = dic[sm]
               valueList.append(value)
             outDicList = [str(x) for x in list(dic.values())[-self.nOutputs:]]
             outDic = ''.join(outDicList)
-            outexact = self.gpiNand(valueList)
+            outexact = logicFuncion(valueList)
             #print(valueList)
             #print("outDic:",type(outDic),"outexact:",type(outexact))
             #print('----------------------')
             if(outDic == outexact):
                 fitnessCounter += 1
                             
         self.fitness = float(fitnessCounter/self.possiblesOutputs)
@@ -392,19 +392,19 @@
         for child in listChild:
             if(child.fitness > bestChild.fitness):
                 bestChild = child
                 
         return bestChild
 
 
-    def evolution(self):
+    def evolution(self,logicFunction):
         
         bestParent = Genoma(self.numberOfGenes,self.nInputs,self.nOutputs) 
         bestParent.generate_parent() # Generate the first generation (The first Parent)
-        bestParent.calculateFitness()  # Get the first generation fitness
+        bestParent.calculateFitness(logicFunction)  # Get the first generation fitness
         bestParent.calculateNoiseFitness()
         self.display(bestParent.genotipo, bestParent.fitness,bestParent.noiseFitness, self.totalGeneration)
        
         listGenomes = []
         ffc = 0
         
         reference = Genoma(self.numberOfGenes,self.nInputs,self.nOutputs)
@@ -417,35 +417,35 @@
         while True:
             self.totalGeneration = self.totalGeneration + 1
             listGenomes.clear()
             
             if(stochasticFactor !=0):
               cf = 0
               for i in range(0,stochasticFactor):
-                  bestParent.calculateFitness()
+                  bestParent.calculateFitness(logicFunction)
                   cf = cf + bestParent.fitness
               bestParent.setFitness(cf/stochasticFactor)
             else:
-              bestParent.calculateFitness()  
+              bestParent.calculateFitness(logicFunction)  
             bestParent.calculateNoiseFitness()
             
             listGenomes.append(bestParent)
             
             for i in range(0, self.y):
                 child = Genoma(self.numberOfGenes,self.nInputs,self.nOutputs)
                 bestParent.mutate().copyGene(child) 
                 
                 if(stochasticFactor !=0):
                   cf = 0
                   for i in range(0,stochasticFactor):
-                      child.calculateFitness()
+                      child.calculateFitness(logicFunction)
                       cf = cf + child.fitness
                   child.setFitness(cf/stochasticFactor)
                 else:
-                  child.calculateFitness()
+                  child.calculateFitness(logicFunction)
                 
                 child.calculateNoiseFitness()
                 
                 listGenomes.append(child)
 
             self.getBestGenome(listGenomes).copyGene(bestParent)
             
@@ -456,15 +456,16 @@
                 break
             
             if (bestParent.fitness >= 1):
                 ffc += 1
                 if (ffc == 10000):
                     self.display(bestParent.genotipo,bestParent.fitness,bestParent.noiseFitness,self.totalGeneration)
                     bestParent.setFaultChance()
-                    bestParent.calculateFitness()
+                    bestParent.calculateFitness(logicFunction)
                     bestParent.calculateNoiseFitness()
                     print("Recalculating fitness without faults...")
                     self.display(bestParent.genotipo,bestParent.fitness,bestParent.noiseFitness,self.totalGeneration)
 
                     break
         timeDiff = datetime.datetime.now() - self.startTime
         print("The end in: ",str(timeDiff))
+
```

### Comparing `VLCDA-1.0.3/VLCDA.egg-info/PKG-INFO` & `VLCDA-1.0.4/VLCDA.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VLCDA
-Version: 1.0.3
+Version: 1.0.4
 Summary: Modulo Python dedicado a evolução de circuitos lógicos através de algoritmos genéticos
 Home-page: https://github.com/HumbertoTavora/Logic-Circuits-Evolution
 Download-URL: https://github.com/HumbertoTavora/Logic-Circuits-Evolution
 Author: Humberto Távora, Stefan Blawid, Yasmin Maria
 Author-email: humbertocctg@gmail.com
 License: MIT
 Keywords: Genetic,Algorithm,Logic Circuits,Evolution,Optimization
```

### Comparing `VLCDA-1.0.3/setup.py` & `VLCDA-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as rm:
     long_description = rm.read()
 
 setup(
     name = "VLCDA",
-    version = "1.0.3",
+    version = "1.0.4",
     license='MIT',
     description = "Modulo Python dedicado a evolução de circuitos lógicos através de algoritmos genéticos",
     author = "Humberto Távora, Stefan Blawid, Yasmin Maria",
     author_email = 'humbertocctg@gmail.com',
     long_description=long_description,
     long_description_content_type = "text/markdown",
     url = 'https://github.com/HumbertoTavora/Logic-Circuits-Evolution',
```

