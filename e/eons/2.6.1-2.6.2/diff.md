# Comparing `tmp/eons-2.6.1.tar.gz` & `tmp/eons-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eons-2.6.1.tar", last modified: Thu Jun 15 02:51:36 2023, max compression
+gzip compressed data, was "eons-2.6.2.tar", last modified: Mon Jun 19 03:04:21 2023, max compression
```

## Comparing `eons-2.6.1.tar` & `eons-2.6.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:51:36.823963 eons-2.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-06-15 02:51:36.823963 eons-2.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-06-15 02:51:21.000000 eons-2.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:51:36.819963 eons-2.6.1/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:51:36.819963 eons-2.6.1/pkg/eons/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 02:51:28.000000 eons-2.6.1/pkg/eons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    89390 2023-06-15 02:51:28.000000 eons-2.6.1/pkg/eons/eons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:51:36.819963 eons-2.6.1/pkg/eons/method/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-15 02:51:13.000000 eons-2.6.1/pkg/eons/method/External.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 02:51:28.000000 eons-2.6.1/pkg/eons/method/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:51:36.823963 eons-2.6.1/pkg/eons/resolve/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 02:51:28.000000 eons-2.6.1/pkg/eons/resolve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-06-15 02:51:13.000000 eons-2.6.1/pkg/eons/resolve/resolve_find_by_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-15 02:51:13.000000 eons-2.6.1/pkg/eons/resolve/resolve_import_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-15 02:51:13.000000 eons-2.6.1/pkg/eons/resolve/resolve_install_from_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-15 02:51:13.000000 eons-2.6.1/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-15 02:51:13.000000 eons-2.6.1/pkg/eons/resolve/resolve_install_with_pip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:51:36.819963 eons-2.6.1/pkg/eons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-06-15 02:51:36.000000 eons-2.6.1/pkg/eons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-15 02:51:36.000000 eons-2.6.1/pkg/eons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 02:51:36.000000 eons-2.6.1/pkg/eons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 02:51:36.000000 eons-2.6.1/pkg/eons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 02:51:36.000000 eons-2.6.1/pkg/eons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-15 02:51:28.000000 eons-2.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-15 02:51:36.823963 eons-2.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:04:21.953782 eons-2.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-06-19 03:04:21.953782 eons-2.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-06-19 03:04:05.000000 eons-2.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:04:21.949782 eons-2.6.2/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:04:21.949782 eons-2.6.2/pkg/eons/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-19 03:04:13.000000 eons-2.6.2/pkg/eons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91950 2023-06-19 03:04:13.000000 eons-2.6.2/pkg/eons/eons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:04:21.949782 eons-2.6.2/pkg/eons/method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-19 03:03:55.000000 eons-2.6.2/pkg/eons/method/External.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 03:04:13.000000 eons-2.6.2/pkg/eons/method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:04:21.953782 eons-2.6.2/pkg/eons/resolve/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 03:04:13.000000 eons-2.6.2/pkg/eons/resolve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-06-19 03:03:55.000000 eons-2.6.2/pkg/eons/resolve/resolve_find_by_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-19 03:03:55.000000 eons-2.6.2/pkg/eons/resolve/resolve_import_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-19 03:03:55.000000 eons-2.6.2/pkg/eons/resolve/resolve_install_from_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-19 03:03:55.000000 eons-2.6.2/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-19 03:03:55.000000 eons-2.6.2/pkg/eons/resolve/resolve_install_with_pip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:04:21.949782 eons-2.6.2/pkg/eons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-06-19 03:04:21.000000 eons-2.6.2/pkg/eons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-19 03:04:21.000000 eons-2.6.2/pkg/eons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 03:04:21.000000 eons-2.6.2/pkg/eons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-19 03:04:21.000000 eons-2.6.2/pkg/eons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-19 03:04:21.000000 eons-2.6.2/pkg/eons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-19 03:04:13.000000 eons-2.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-19 03:04:21.953782 eons-2.6.2/setup.cfg
```

### Comparing `eons-2.6.1/PKG-INFO` & `eons-2.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.6.1
+Version: 2.6.2
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.6.1/README.md` & `eons-2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `eons-2.6.1/pkg/eons/eons.py` & `eons-2.6.2/pkg/eons/eons.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 import sys
 import pkgutil
 import importlib.machinery
 import importlib.util
 import types
 import traceback
 import jsonpickle
-from pathlib import Path
-from subprocess import Popen
-from subprocess import PIPE
-from subprocess import STDOUT
-import inspect
-import operator
-import re
 import argparse
 import requests
 import yaml
 from requests_futures.sessions import FuturesSession
+from pathlib import Path
 from tqdm import tqdm
 from zipfile import ZipFile
 from distutils.dir_util import mkpath
 from eot import EOT
+import operator
+from subprocess import Popen
+from subprocess import PIPE
+from subprocess import STDOUT
+import inspect
+import re
 
 ######## START CONTENT ########
 def INVALID_NAME():
 	return "INVALID_NAME"
 
 class ActualType(type):
 	def __repr__(self):
@@ -740,15 +740,17 @@
 		# In order for this to work properly, each method needs to be a distinct object; hence the need for deepcopy.
 		# In the future, we might be able to find a way to share code objects between Functors. However, for now we will allow each Functor to modify its classmethods as it pleases.
 
 		# We have to use util.___Attr() because some sources might have '.'s in them.
 
 		for source, honorPropagate in this.methodSources.items():
 			if (not util.HasAttr(this, source)):
+				logging.debug(f"Could not find {source}; will not pull in its methods.")
 				continue
+			logging.debug(f"Populating methods from {source}.")
 			for method in util.GetAttr(this, source).values():
 				if (honorPropagate and not method.propagate):
 					continue
 				if (method.name in this.methods.keys() and honorPropagate):
 					existingMethod = this.methods[method.name]
 					if (not existingMethod.inheritMethods):
 						continue
@@ -1116,403 +1118,14 @@
 			pass
 
 	@staticmethod
 	def GetLatest():
 		return ExecutorTracker.Instance().executors[-1]
 
 
-# Global Fetch() function.
-# Uses the latest registered Executor
-def Fetch(varName, default=None, fetchFrom=None, start=True, attempted=None):
-    return ExecutorTracker.GetLatest().Fetch(varName, default, fetchFrom, start, attempted)
-
-# Ease-of-use wrapper for the global Fetch()
-def f(varName, default=None, fetchFrom=None, start=True, attempted=None):
-    Fetch(varName, default, fetchFrom, start, attempted)
-
-def METHOD_PENDING_POPULATION(obj, *args, **kwargs):
-	raise MethodPendingPopulation("METHOD PENDING POPULATION")
-
-# Use the @method() decorator to turn any class function into an eons Method Functor.
-# Methods are Functors which can be implicitly transferred between classes (see Functor.PopulateMethods)
-# Using Methods also gives us full control over the execution of your code; meaning, we can change how Python interprets what you wrote!
-# All Methods will be stored in the method member of your Functor. However, you shouldn't need to access that.
-#
-# If you would like to specify a custom implementation, set the 'impl' kwarg (e.g. @method(impl='MyMethodImplementation'))
-# Beside 'impl', all key-word arguments provided to the @method() decorator will be set as member variables of the created Method.
-# For example, to set whether or not the Method should be propagated, you can use @method(propagate=True).
-# This means, you can create a custom means of interpreting your code with your own feature set and still use this @method decorator.
-# Perhaps you'd like something along the lines of: @method(impl='MakeAwesome', awesomeness=10000).
-# NOTE: in order for impl to work, the implementation class must already be Registered (or this must be called from an appropriate @recoverable function).
-def method(impl='Method', **kwargs):
-
-	# Class decorator with __set_name__, as described here: https://stackoverflow.com/questions/2366713/can-a-decorator-of-an-instance-method-access-the-class
-	class MethodDecorator:
-		def __init__(this, function):
-			this.function = function
-
-		# Apparently, this is called when the decorated function is constructed.
-		def __set_name__(this, cls, functionName):
-			logging.debug(f"Constructing new method for {this.function} in {cls}")
-
-			# Create and configure a new Method
-
-			method = SelfRegistering(impl)
-			method.Constructor(this.function, cls)
-			for key, value in kwargs.items():
-				setattr(method, key, value)
-
-			# Store the new method in the class
-			if (not hasattr(cls, 'classMethods') or not isinstance(cls.classMethods, dict)):
-				cls.classMethods = {}
-			cls.classMethods[functionName] = method
-
-			# Self-destruct by replacing the decorated function.
-			# We rely on Functor.PopulateMethods to re-establish the method as callable.
-			# It seems like this just outright removes the methods. There may be an issue with using __get__ this way.
-			# Regardless deleting the method is okay as long as we add it back before anyone notices.
-			setattr(cls, functionName, METHOD_PENDING_POPULATION.__get__(cls))
-
-	return MethodDecorator
-
-class Method(Functor):
-
-	def __init__(this, name=INVALID_NAME()):
-		super().__init__(name)
-
-		# Methods do not fetch from the environment by default.
-		this.fetchFrom.remove('environment')
-
-		# Whether or not *this should be combined with other Methods of the same name.
-		this.inheritMethods = True
-
-		# Where should inherited methods be inserted?
-		# First here means "before *this".
-		# If False, inherited code will be run after *this.
-		this.inheritedMethodsFirst = True # otherwise ...Last
-
-		# Propagation allows for Functors called after that which defines *this to also call *this.
-		# This system allows for partial, implicit inheritance.
-		# By default, Methods will not be propagated. Use @propagate to enable propagation.
-		this.propagate = False
-
-		# We don't care about these checks right now.
-		# Plus, we can't exactly wrap 2 functions even if we wanted to Rollback.
-		this.functionSucceeded = True
-		this.rollbackSucceeded = True
-		this.enableRollback = False
-
-		# The source code of the function we're implementing.
-		this.source = ""
-
-		# The instance of the class to which *this belongs.
-		# i.e. the object that called *this, aka 'owner', 'caller', etc.
-		this.object = None
-
-		this.original = util.DotDict()
-		this.original.cls = None
-		this.original.function = None
-
-
-	# Make *this execute the code in this.source
-	def UpdateSource(this):
-		wrappedFunctionName = f'_eons_method_{this.name}'
-		completeSource = f'''\
-def {wrappedFunctionName}(this):
-{this.source}
-'''
-		if (this.executor and this.executor.verbosity > 3):
-			logging.debug(f"Source for {this.name} is:\n{completeSource}")
-		code = compile(completeSource, '', 'exec')
-		exec(code)
-		exec(f'this.Function = {wrappedFunctionName}.__get__(this, this.__class__)')
-
-
-
-	# Parse arguments and update the source code
-	# TODO: Implement full python parser to avoid bad string replacement (e.g. "def func(self):... self.selfImprovement" => "... this.object.this.object.Improvement").
-	def PopulateFrom(this, function):
-		this.source = ':'.join(inspect.getsource(function).split(':')[1:]) #Remove the first function definition
-
-		args = inspect.signature(function, follow_wrapped=False).parameters
-		thisSymbol = next(iter(args))
-		#del args[thisSymbol] # ??? 'mappingproxy' object does not support item deletion
-		this.source = this.source.replace(thisSymbol, 'this.object')
-
-		first = True
-		for arg in args.values(): #args.values[1:] also doesn't work.
-			if (first):
-				first = False
-				continue
-
-			replaceWith = arg.name
-
-			if (arg.kind == inspect.Parameter.VAR_POSITIONAL):
-				replaceWith = 'this.args'
-
-			elif (arg.kind == inspect.Parameter.VAR_KEYWORD):
-				replaceWith = 'this.kwargs'
-
-			else:
-				if (arg.default != inspect.Parameter.empty):
-					this.optionalKWArgs[arg.name] = arg.default
-				else:
-					this.requiredKWArgs.append(arg.name)
-				replaceWith = f'this.{arg.name}'
-
-				if (arg.kind in [inspect.Parameter.POSITIONAL_OR_KEYWORD, inspect.Parameter.POSITIONAL_ONLY]):
-					this.argMapping.append(arg.name)
-
-			this.source = this.source.replace(arg.name, replaceWith)
-
-
-	# When properly constructing a Method, rely only on the function *this should implement.
-	# The class and all other properties are irrelevant. However, they are provided and intended for debugging only.
-	def Constructor(this, function, cls):
-		this.name = function.__name__
-		this.original.cls = cls
-		this.original.function = function
-
-		this.PopulateFrom(function)
-		
-		# UpdateSource is called by Functor.PopulateMethods()
-		# this.UpdateSource()
-
-
-	# Grab any known and necessary args from this.kwargs before any Fetch calls are made.
-	def PopulatePrecursor(this):
-		if (not this.object):
-			raise MissingArgumentError(f"Call {this.name} from a class instance: {this.original.cls.__name__}.{this.name}(...). Maybe Functor.PopulateMethods() hasn't been called yet?")
-
-		this.executor = this.object.executor
-
-		if ('precursor' in this.kwargs):
-			this.precursor = this.kwargs.pop('precursor')
-		else:
-			this.precursor = None
-
-
-	# Next is set by Functor.PopulateMethods.
-	# We  definitely don't want to Fetch 'next'.
-	def PopulateNext(this):
-		pass
-
-
-	# Method.next should be a list of other Methods, as opposed to the standard string; so, instead of Executor.Execute..., we can directly invoke whatever is next.
-	# We skip all validation here.
-	# We also don't pass any args that were given in the initial function call. Those can all be Fetched from 'precursor'.
-	def CallNext(this):
-		if (not this.next):
-			return None
-
-		for next in this.next:
-			next(precursor=this)
-
-
-# The standard Functor extends Functor to add a set of standard members and methods.
-# This is similar to the standard library in C and C++
-# You must inherit from *this if you would like to use the functionality *this provides. The methods defined will not be propagated.
-class StandardFunctor(Functor):
-	def __init__(this, name="Standard Functor"):
-		super().__init__(name)
-
-	# Override this and do whatever!
-	# This is purposefully vague.
-	def Function(this):
-		pass
-
-
-	# Undo any changes made by UserFunction.
-	# Please override this too!
-	def Rollback(this):
-		pass
-
-
-	# Override this to check results of operation and report on status.
-	# Override this to perform whatever success checks are necessary.
-	def DidFunctionSucceed(this):
-		return this.functionSucceeded
-
-
-	# RETURN whether or not the Rollback was successful.
-	# Override this to perform whatever success checks are necessary.
-	def DidRollbackSucceed(this):
-		return this.rollbackSucceeded
-
-
-	######## START: UTILITIES ########
-
-	# RETURNS: an opened file object for writing.
-	# Creates the path if it does not exist.
-	@method()
-	def CreateFile(this, file, mode="w+"):
-		Path(os.path.dirname(os.path.abspath(file))).mkdir(parents=True, exist_ok=True)
-		return open(file, mode)
-
-	# Copy a file or folder from source to destination.
-	# This really shouldn't be so hard...
-	# root allows us to interpret '/' as something other than the top of the filesystem.
-	@method()
-	def Copy(this, source, destination, root='/'):
-		if (source.startswith('/')):
-			source = str(Path(root).joinpath(source[1:]).resolve())
-		else:
-			source = str(Path(source).resolve())
-		
-		destination = str(Path(destination).resolve())
-		
-		Path(destination).parent.mkdir(parents=True, exist_ok=True)
-
-		if (os.path.isfile(source)):
-			logging.debug(f"Copying file {source} to {destination}")
-			try:
-				shutil.copy(source, destination)
-			except shutil.Error as exc:
-				errors = exc.args[0]
-				for error in errors:
-					src, dst, msg = error
-					logging.debug(f"{msg}")
-		elif (os.path.isdir(source)):
-			logging.debug(f"Copying directory {source} to {destination}")
-			try:
-				shutil.copytree(source, destination)
-			except shutil.Error as exc:
-				errors = exc.args[0]
-				for error in errors:
-					src, dst, msg = error
-					logging.debug(f"{msg}")
-		else:
-			logging.error(f"Could not find source to copy: {source}")
-
-	# Delete a file or folder
-	@method()
-	def Delete(this, target):
-		if (not os.path.exists(target)):
-			logging.debug(f"Unable to delete nonexistent target: {target}")
-			return
-		if (os.path.isfile(target)):
-			logging.debug(f"Deleting file {target}")
-			os.remove(target)
-		elif (os.path.isdir(target)):
-			logging.debug(f"Deleting directory {target}")
-			try:
-				shutil.rmtree(target)
-			except shutil.Error as exc:
-				errors = exc.args[0]
-				for error in errors:
-					src, dst, msg = error
-					logging.debug(f"{msg}")
-
-	# Run whatever.
-	# DANGEROUS!!!!!
-	# RETURN: Return value and, optionally, the output as a list of lines.
-	@method()
-	def RunCommand(this, command, saveout=False, raiseExceptions=True):
-		logging.debug(f"================ Running command: {command} ================")
-		process = Popen(command, stdout=PIPE, stderr=STDOUT, shell=True)
-		output = []
-		while process.poll() is None:
-			line = process.stdout.readline().decode('utf8')[:-1]
-			if (saveout):
-				output.append(line)
-			if (line):
-				logging.debug(f"| {line}")  # [:-1] to strip excessive new lines.
-
-		message = f"Command returned {process.returncode}: {command}"
-		logging.debug(message)
-		if (raiseExceptions and process.returncode is not None and process.returncode):
-			raise CommandUnsuccessful(message)
-		
-		logging.debug(f"================ Completed command: {command} ================")
-		if (saveout):
-			return process.returncode, output
-		
-		return process.returncode
-	######## END: UTILITIES ########
-
-#from .Executor import Executor # don't import this, it'll be circular!
-
-# @recoverable
-# Decorating another function with this method will engage the error recovery system provided by *this.
-# To use this, you must define a GetExecutor() method in your class and decorate the functions you want to recover from.
-# For more info, see Executor.ResolveError and the README.md
-def recoverable(function):
-	def RecoverableDecorator(obj, *args, **kwargs):
-		return RecoverableImplementation(obj, obj.GetExecutor(), function, *args, **kwargs)
-	return RecoverableDecorator
-
-
-# This needs to be recursive, so rather than having the recoverable decorator call or decorate itself, we just break the logic into this separate method.
-def RecoverableImplementation(obj, executor, function, *args, **kwargs):
-	try:
-		return function(obj, *args, **kwargs)
-	except FailedErrorResolution as fatal:
-		raise fatal
-	except Exception as e:
-		if (not executor.resolveErrors):
-			raise e
-		return Recover(e, obj, executor, function, *args, **kwargs)
-
-
-def Recover(error, obj, executor, function, *args, **kwargs):
-	logging.warning(f"Got error '{error}' from function ({function}) by {obj.name}.")
-	util.LogStack()
-
-	# We have to use str(e) instead of pointers to Exception objects because multiple Exceptions will have unique addresses but will still be for the same error, as defined by string comparison.
-	if (str(error) not in executor.errorResolutionStack.keys()):
-		executor.errorResolutionStack.update({str(error):[]})
-
-	# The executor.errorResolutionStack grows each time we invoke *this or (indirectly) executor.ResolveError().
-	# ResolveError is itself @recoverable.
-	# So, each time we hit this point, we should also hit a corresponding ClearErrorResolutionStack() call.
-	# If we do not, an exception is passed to the caller; if we do, the stack will be cleared upon the last resolution.
-	executor.errorRecursionDepth = executor.errorRecursionDepth + 1
-
-	if (executor.errorRecursionDepth > len(executor.errorResolutionStack.keys())+1):
-		raise FailedErrorResolution(f"Hit infinite loop trying to resolve errors. Recursion depth: {executor.errorRecursionDepth}; STACK: {executor.errorResolutionStack}.")
-
-	successfullyRecovered = False
-	ret = None
-	resolvedBy = None
-	for i, res in enumerate(executor.resolveErrorsWith):
-
-		logging.debug(f"Checking if {res} can fix '{error}'.")
-		if (not executor.ResolveError(error, i, obj, function)): # attempt to resolve the issue; might cause us to come back here with a new error.
-			# if no resolution was attempted, there's no need to re-run the function.
-			continue
-		try:
-			logging.debug(f"Trying function ({function}) again after applying {res}.")
-			resolvedBy = res
-			ret = function(obj, *args, **kwargs)
-			successfullyRecovered = True
-			break
-
-		except Exception as e2:
-			if (str(error) == str(e2)):
-				logging.debug(f"{res} failed with '{e2}'; will ignore and see if we can use another ErrorResolution to resolve '{error}'.")
-				# Resolution failed. That's okay. Let's try the next.
-				# Not all ErrorResolutions will apply to all errors, so we may have to try a few before we get one that works.
-				continue
-			else:
-				# The error changed, maybe we're making progress.
-				ret = Recover(e2, obj, executor, function, *args, **kwargs)
-				successfullyRecovered = True
-				break
-
-	if (successfullyRecovered):
-		executor.ClearErrorResolutionStack(str(error)) # success!
-		logging.recovery(f"{resolvedBy} successfully resolved '{error}'!")
-		logging.debug(f"Error stack is now: {executor.errorResolutionStack}")
-		return ret
-
-	#  We failed to resolve the error. Die
-	sys.tracebacklimit = 0 # traceback is NOT helpful here.
-	raise FailedErrorResolution(f"Tried and failed to resolve: {error} STACK: {executor.errorResolutionStack}. See earlier logs (in debug) for traceback.")
-
-
 # A DataContainer allows Data to be stored and worked with.
 # This class is intended to be derived from and added to.
 # Each DataContainer is comprised of multiple Data (see Datum.py for more).
 # NOTE: DataContainers are, themselves Data. Thus, you can nest your child classes however you would like.
 class DataContainer(Datum):
 
 	def __init__(this, name=INVALID_NAME()):
@@ -1663,166 +1276,92 @@
 	def ImportDataFrom(this, otherDataContainer, preventDuplicatesOf=None):
 		this.data.extend(otherDataContainer.data);
 		if (preventDuplicatesOf is not None):
 			return this.RemoveDuplicateDataOf(preventDuplicatesOf)
 		return []
 
 
+#from .Executor import Executor # don't import this, it'll be circular!
 
-# Use an ErrorStringParser for each "parsers" in order to avoid having to override the GetObjectFromError method and create a new class for every error you want to handle.
-# ErrorStringParsers enable ErrorResolutions to be created on a per-functionality, rather than per-error basis, reducing the total amount of duplicate code.
-# Each error has a different string. In order to get the object of the error, we have to know where the object starts and ends.
-# NOTE: this assumes only 1 object per string. Maybe fancier parsing logic can be added in the future.
-#
-# startPosition is always positive
-# endPosition is always negative
-class ErrorStringParser:
-
-	def __init__(this, applicableError, startPosition, endPosition):
-		this.applicableError = applicableError
-		this.startPosition = startPosition
-		this.endPosition = endPosition
-
-	def Parse(this, errorString):
-		end = this.endPosition
-		if (not end):
-			end = len(errorString)
-		return errorString[this.startPosition:end]
-
-
-# ErrorResolution is a Functor which can be executed when an Exception is raised.
-# The goal of this class is to do some kind of work that will fix the problem on the second try of whatever generated the error.
-class ErrorResolution(StandardFunctor):
-
-	def __init__(this, name=INVALID_NAME()):
-		super().__init__(name)
-
-		# What errors, as ErrorStringParser objects, is *this prepared to handle?
-		this.parsers = []
-
-		this.error = None
-		this.errorType = ""
-		this.errorString = ""
-		this.errorObject = ""
-		this.errorResolutionStack = {}
-
-		# Provided directly from the recoverable decorator.
-		this.optionalKWArgs["obj"] = None
-		this.optionalKWArgs["function"] = None
-
-		# We do want to know whether or not we should attempt to run whatever failed again.
-		# So, let's store that in functionSucceeded. Meaning if this.functionSucceeded, try the original method again.
-		# No rollback, by default and definitely don't throw Exceptions.
-		this.enableRollback = False
-		this.functionSucceeded = True
-		this.raiseExceptions = False
-
-		this.errorShouldBeResolved = False
-
-
+# @recoverable
+# Decorating another function with this method will engage the error recovery system provided by *this.
+# To use this, you must define a GetExecutor() method in your class and decorate the functions you want to recover from.
+# For more info, see Executor.ResolveError and the README.md
+def recoverable(function):
+	def RecoverableDecorator(obj, *args, **kwargs):
+		return RecoverableImplementation(obj, obj.GetExecutor(), function, *args, **kwargs)
+	return RecoverableDecorator
 
-	# Put your logic here!
-	def Resolve(this):
-		# You get the following members:
-		# this.error (an Exception)
-		# this.errorString (a string cast of the Exception)
-		# this.errorType (a string)
-		# this.errorObjet (a string or whatever you return from GetObjectFromError())
 
-		# You get the following guarantees:
-		# *this has not been called on this particular error before.
-		# the error given is applicable to *this per this.parsers
+# This needs to be recursive, so rather than having the recoverable decorator call or decorate itself, we just break the logic into this separate method.
+def RecoverableImplementation(obj, executor, function, *args, **kwargs):
+	try:
+		return function(obj, *args, **kwargs)
+	except FailedErrorResolution as fatal:
+		raise fatal
+	except Exception as e:
+		if (not executor.resolveErrors):
+			raise e
+		return Recover(e, obj, executor, function, *args, **kwargs)
 
-		###############################################
-		# Please throw errors if something goes wrong #
-		# Otherwise, set this.errorShouldBeResolved   #
-		###############################################
-		
-		pass
 
+def Recover(error, obj, executor, function, *args, **kwargs):
+	logging.warning(f"Got error '{error}' from function ({function}) by {obj.name}.")
+	util.LogStack()
 
+	# We have to use str(e) instead of pointers to Exception objects because multiple Exceptions will have unique addresses but will still be for the same error, as defined by string comparison.
+	if (str(error) not in executor.errorResolutionStack.keys()):
+		executor.errorResolutionStack.update({str(error):[]})
 
-	# Helper method for creating ErrorStringParsers
-	# To use this, simply take an example output and replace the object you want to extract with "OBJECT"
-	def ApplyTo(this, error, exampleString):
-		match = re.search('OBJECT', exampleString)
-		this.parsers.append(ErrorStringParser(error, match.start(), match.end() - len(exampleString)))
+	# The executor.errorResolutionStack grows each time we invoke *this or (indirectly) executor.ResolveError().
+	# ResolveError is itself @recoverable.
+	# So, each time we hit this point, we should also hit a corresponding ClearErrorResolutionStack() call.
+	# If we do not, an exception is passed to the caller; if we do, the stack will be cleared upon the last resolution.
+	executor.errorRecursionDepth = executor.errorRecursionDepth + 1
 
+	if (executor.errorRecursionDepth > len(executor.errorResolutionStack.keys())+1):
+		raise FailedErrorResolution(f"Hit infinite loop trying to resolve errors. Recursion depth: {executor.errorRecursionDepth}; STACK: {executor.errorResolutionStack}.")
 
-	# Get the type of this.error as a string.
-	def GetErrorType(this):
-		return type(this.error).__name__
+	successfullyRecovered = False
+	ret = None
+	resolvedBy = None
+	for i, res in enumerate(executor.resolveErrorsWith):
 
+		logging.debug(f"Checking if {res} can fix '{error}'.")
+		if (not executor.ResolveError(error, i, obj, function)): # attempt to resolve the issue; might cause us to come back here with a new error.
+			# if no resolution was attempted, there's no need to re-run the function.
+			continue
+		try:
+			logging.debug(f"Trying function ({function}) again after applying {res}.")
+			resolvedBy = res
+			ret = function(obj, *args, **kwargs)
+			successfullyRecovered = True
+			break
 
-	# Get an actionable object from the error.
-	# For example, if the error is 'ModuleNotFoundError', what is the module?
-	def GetObjectFromError(this):
-		for parser in this.parsers:
-			if (parser.applicableError != this.errorType):
+		except Exception as e2:
+			if (str(error) == str(e2)):
+				logging.debug(f"{res} failed with '{e2}'; will ignore and see if we can use another ErrorResolution to resolve '{error}'.")
+				# Resolution failed. That's okay. Let's try the next.
+				# Not all ErrorResolutions will apply to all errors, so we may have to try a few before we get one that works.
 				continue
+			else:
+				# The error changed, maybe we're making progress.
+				ret = Recover(e2, obj, executor, function, *args, **kwargs)
+				successfullyRecovered = True
+				break
 
-			this.errorObject = parser.Parse(this.errorString)
-			return
-
-		raise ErrorResolutionError(f"{this.name} cannot parse error object from ({this.errorType}): {str(this.error)}.")
-
-
-	# Determine if this resolution method is applicable.
-	def CanProcess(this):
-		return this.GetErrorType() in [parser.applicableError for parser in this.parsers]
-
-
-	# Grab any known and necessary args from this.kwargs before any Fetch calls are made.
-	def ParseInitialArgs(this):
-		super().ParseInitialArgs()
-		if ('error' in this.kwargs):
-			this.error = this.kwargs.pop('error')
-			# Just assume the error is an actual Exception object.
-		else:
-			raise ErrorResolutionError(f"{this.name} was not given an error to resolve.")
-
-		this.errorString = str(this.error)
-		this.errorType = this.GetErrorType()
-
-		# Internal member to avoid processing duplicates
-		this.errorResolutionStack = this.executor.errorResolutionStack
-
-
-	# Error resolution is unchained.
-	def PopulateNext(this):
-		this.next = []
-
-
-	# Override of Functor method.
-	# We'll keep calling this until an error is raised.
-	def Function(this):
-		this.functionSucceeded = True
-		this.errorShouldBeResolved = True
-		
-		if (not this.CanProcess()):
-			this.errorShouldBeResolved = False
-			return this.errorResolutionStack, this.errorShouldBeResolved
-
-		if (not this.errorString in this.errorResolutionStack.keys()):
-			this.errorResolutionStack.update({this.errorString:[]})
-		
-		if (this.name in this.errorResolutionStack[this.errorString]):
-			raise FailedErrorResolution(f"{this.name} already tried and failed to resolve {this.errorType}: {this.errorString}.")
-
-		this.GetObjectFromError()
+	if (successfullyRecovered):
+		executor.ClearErrorResolutionStack(str(error)) # success!
+		logging.recovery(f"{resolvedBy} successfully resolved '{error}'!")
+		logging.debug(f"Error stack is now: {executor.errorResolutionStack}")
+		return ret
 
-		try:
-			this.Resolve()
-		except Exception as e:
-			logging.error(f"Error resolution with {this.name} failed: {e}")
-			util.LogStack()
-			this.functionSucceeded = False
-		
-		this.errorResolutionStack[this.errorString].append(this.name)
-		return this.errorResolutionStack, this.errorShouldBeResolved
+	#  We failed to resolve the error. Die
+	sys.tracebacklimit = 0 # traceback is NOT helpful here.
+	raise FailedErrorResolution(f"Tried and failed to resolve: {error} STACK: {executor.errorResolutionStack}. See earlier logs (in debug) for traceback.")
 
 
 # Executor: a base class for user interfaces.
 # An Executor is a functor and can be executed as such.
 # For example
 #	class MyExecutor(Executor):
 #		def __init__(this):
@@ -1890,14 +1429,19 @@
 		# Where should we log to?
 		# Set by Fetch('log_file')
 		this.log_file = None
 
 		# All repository configuration.
 		this.repo = util.DotDict()
 
+		# Placement helps to construct the correct load order of Functors as they are installed.
+		this.placement = util.DotDict()
+		this.placement.max = 255
+		this.placement.session = util.DotDict()
+		
 		# Defaults.
 		# You probably want to configure these in your own Executors.
 		this.defaultRepoDirectory = os.path.abspath(os.path.join(os.getcwd(), "./eons/"))
 		this.registerDirectories = []
 		this.defaultConfigFile = None
 		this.defaultPackageType = ""
 
@@ -1913,14 +1457,15 @@
 
 		# We can't Fetch from everywhere while we're getting things going. However, these should be safe,
 		this.fetchFromDuringSetup = ['args', 'config', 'environment']
 
 		this.Configure()
 		this.RegisterIncludedClasses()
 		this.AddArgs()
+		this.ResetPlacementSession()
 
 
 	# Destructors do not work reliably in python.
 	# NOTE: you CANNOT delete *this without first Pop()ing it from the ExecutorTracker.
 	# def __del__(this):
 	# 	ExecutorTracker.Instance().Pop(this)
 
@@ -2091,14 +1636,55 @@
 		this.argparser.add_argument('--config', '-c', type=str, default=None, help='Path to configuration file containing only valid JSON.', dest='config')
 
 		# We'll use Fetch instead
 		# this.argparser.add_argument('--log', '-l', type=str, default=None, help='Path to log file.', dest='log')
 		# this.argparser.add_argument('--no-repo', action='store_true', default=False, help='prevents searching online repositories', dest='no_repo')
 
 
+	# End the current placement session (if any)
+	def ResetPlacementSession(this):
+		this.placement.session.active = False
+		this.placement.session.level = this.placement.max
+		this.placement.session.hierarchy = {}
+		this.placement.session.current = []
+
+	# Track to the current location in the placement hierarchy.
+	def GetPlacementSessionCurrentPosition(this):
+		if (not this.placement.session.active):
+			return None
+		ret = this.placement.session.hierarchy
+		for place in this.placement.session.hierarchy:
+			ret = ret[place]
+		return ret
+	
+	def BeginPlacing(this, toPlace):
+		if (not this.placement.session.active):
+			this.placement.session.active = True
+		hierarchy = this.GetPlacementSessionCurrentPosition()
+		hierarchy[toPlace] = {}
+		this.placement.session.current.append(toPlace)
+		this.placement.session.level -= 1
+
+	# Once the proper location of a Functor has been derived, remove it from the hierarchy.
+	# Additionally, if we're the last ones to play with the current session, reset it.
+	def ResolvePlacementOf(this, placed):
+		if (not this.placement.session.active):
+			return
+		try:
+			this.placement.session.current.remove(placed)
+		except:
+			pass # key errors when getting an existing Functor...
+		hierarchy = this.GetPlacementSessionCurrentPosition()
+		if (not len(this.placement.session.current)):
+			this.ResetPlacementSession()
+		elif (hierarchy and placed in hierarchy.keys()):
+			del hierarchy[placed]
+			this.placement.session.level += 1
+		
+
 	# Create any sub-class necessary for child-operations
 	# Does not RETURN anything.
 	def InitData(this):
 		pass
 
 
 	# Register included files early so that they can be used by the rest of the system.
@@ -2244,14 +1830,15 @@
 		this.PopulateConfig()
 		this.SetVerbosity()
 		this.SetLogFile()
 		logging.debug(f"<---- {this.name} (log level: {logging.getLogger().level}) ---->")
 		logging.debug(f"Got extra arguments: {this.extraArgs}") # has to be after verbosity setting
 		logging.debug(f"Got config contents: {this.config}")
 		this.PopulateRepoDetails()
+		this.placement.max = this.Fetch('placement_max', 255, this.fetchFromDuringSetup)
 
 
 	# Functor required method
 	# Override this with your own workflow.
 	def Function(this):
 		
 		# NOTE: class registration may instantiate other Executors.
@@ -2370,19 +1957,21 @@
 			raise PackageError(f"Package wrote {progressBar.n} / {packageSize} bytes")
 
 		packageZipContents.close()
 
 		if (not os.path.exists(packageZipPath)):
 			raise PackageError(f"Failed to create {packageZipPath}")
 
-		logging.debug(f"Extracting {packageZipPath}")
 		openArchive = ZipFile(packageZipPath, 'r')
 		extractLoc = this.repo.store
 		if (createSubDirectory):
 			extractLoc = os.path.join(extractLoc, packageName)
+		elif (this.placement.session.active):
+			extractLoc = os.path.join(extractLoc, str(this.placement.session.level))
+		logging.debug(f"Extracting {packageZipPath} to {extractLoc}")
 		openArchive.extractall(f"{extractLoc}")
 		openArchive.close()
 		os.remove(packageZipPath)
 
 		if (registerClasses):
 			this.RegisterAllClassesInDirectory(this.repo.store)
 
@@ -2394,19 +1983,21 @@
 	@recoverable
 	def GetRegistered(this,
 		registeredName,
 		packageType=""):
 
 		try:
 			registered = SelfRegistering(registeredName)
+			this.ResolvePlacementOf(registeredName)
 		except Exception as e:
 			# We couldn't get what was asked for. Let's try asking for help from the error resolution machinery.
 			packageName = registeredName
 			if (packageType):
 				packageName = f"{registeredName}.{packageType}"
+			this.BeginPlacing(registeredName)
 			logging.error(f"While trying to instantiate {packageName}, got: {e}")
 			raise HelpWantedWithRegistering(f"Trying to get SelfRegistering {packageName}")
 
 		# NOTE: Functors are Data, so they have an IsValid() method
 		if (not registered or not registered.IsValid()):
 			logging.error(f"No valid object: {registeredName}")
 			raise FatalCannotExecute(f"No valid object: {registeredName}")
@@ -2543,7 +2134,475 @@
 		for key, val in this.extraArgs.items():
 			if (key == varName):
 				return val, True
 		return default, False
 
 	######## END: Fetch Locations ########
 
+
+# Global Fetch() function.
+# Uses the latest registered Executor
+def Fetch(varName, default=None, fetchFrom=None, start=True, attempted=None):
+    return ExecutorTracker.GetLatest().Fetch(varName, default, fetchFrom, start, attempted)
+
+# Ease-of-use wrapper for the global Fetch()
+def f(varName, default=None, fetchFrom=None, start=True, attempted=None):
+    Fetch(varName, default, fetchFrom, start, attempted)
+
+def METHOD_PENDING_POPULATION(obj, *args, **kwargs):
+	raise MethodPendingPopulation("METHOD PENDING POPULATION")
+
+# Use the @method() decorator to turn any class function into an eons Method Functor.
+# Methods are Functors which can be implicitly transferred between classes (see Functor.PopulateMethods)
+# Using Methods also gives us full control over the execution of your code; meaning, we can change how Python interprets what you wrote!
+# All Methods will be stored in the method member of your Functor. However, you shouldn't need to access that.
+#
+# If you would like to specify a custom implementation, set the 'impl' kwarg (e.g. @method(impl='MyMethodImplementation'))
+# Beside 'impl', all key-word arguments provided to the @method() decorator will be set as member variables of the created Method.
+# For example, to set whether or not the Method should be propagated, you can use @method(propagate=True).
+# This means, you can create a custom means of interpreting your code with your own feature set and still use this @method decorator.
+# Perhaps you'd like something along the lines of: @method(impl='MakeAwesome', awesomeness=10000).
+# NOTE: in order for impl to work, the implementation class must already be Registered (or this must be called from an appropriate @recoverable function).
+def method(impl='Method', **kwargs):
+
+	# Class decorator with __set_name__, as described here: https://stackoverflow.com/questions/2366713/can-a-decorator-of-an-instance-method-access-the-class
+	class MethodDecorator:
+		def __init__(this, function):
+			this.function = function
+
+		# Apparently, this is called when the decorated function is constructed.
+		def __set_name__(this, cls, functionName):
+			logging.debug(f"Constructing new method for {this.function} in {cls}")
+
+			# Create and configure a new Method
+
+			method = SelfRegistering(impl)
+			method.Constructor(this.function, cls)
+			for key, value in kwargs.items():
+				setattr(method, key, value)
+
+			# Store the new method in the class
+			# There is a potential bug here: if the class derives from a class which already has the classMethods static member, this will add to the PARENT class's classMethods. Thus, 2 classes with different methods will share those methods via their shared parent.
+			if (not hasattr(cls, 'classMethods') or not isinstance(cls.classMethods, dict)):
+				cls.classMethods = {}
+			else:
+				# to account for the bug above, shadow classMethods out of the base class & into the derived.
+				setattr(cls, 'classMethods', getattr(cls, 'classMethods').copy())
+			
+			cls.classMethods[functionName] = method
+
+			# Self-destruct by replacing the decorated function.
+			# We rely on Functor.PopulateMethods to re-establish the method as callable.
+			# It seems like this just outright removes the methods. There may be an issue with using __get__ this way.
+			# Regardless deleting the method is okay as long as we add it back before anyone notices.
+			setattr(cls, functionName, METHOD_PENDING_POPULATION.__get__(cls))
+
+	return MethodDecorator
+
+class Method(Functor):
+
+	def __init__(this, name=INVALID_NAME()):
+		super().__init__(name)
+
+		# Methods do not fetch from the environment by default.
+		this.fetchFrom.remove('environment')
+
+		# Whether or not *this should be combined with other Methods of the same name.
+		this.inheritMethods = True
+
+		# Where should inherited methods be inserted?
+		# First here means "before *this".
+		# If False, inherited code will be run after *this.
+		this.inheritedMethodsFirst = True # otherwise ...Last
+
+		# Propagation allows for Functors called after that which defines *this to also call *this.
+		# This system allows for partial, implicit inheritance.
+		# By default, Methods will not be propagated. Use @propagate to enable propagation.
+		this.propagate = False
+
+		# We don't care about these checks right now.
+		# Plus, we can't exactly wrap 2 functions even if we wanted to Rollback.
+		this.functionSucceeded = True
+		this.rollbackSucceeded = True
+		this.enableRollback = False
+
+		# The source code of the function we're implementing.
+		this.source = ""
+
+		# The instance of the class to which *this belongs.
+		# i.e. the object that called *this, aka 'owner', 'caller', etc.
+		this.object = None
+
+		this.original = util.DotDict()
+		this.original.cls = None
+		this.original.function = None
+
+
+	# Make *this execute the code in this.source
+	def UpdateSource(this):
+		wrappedFunctionName = f'_eons_method_{this.name}'
+		completeSource = f'''\
+def {wrappedFunctionName}(this):
+{this.source}
+'''
+		if (this.executor and this.executor.verbosity > 3):
+			logging.debug(f"Source for {this.name} is:\n{completeSource}")
+		code = compile(completeSource, '', 'exec')
+		exec(code)
+		exec(f'this.Function = {wrappedFunctionName}.__get__(this, this.__class__)')
+
+
+
+	# Parse arguments and update the source code
+	# TODO: Implement full python parser to avoid bad string replacement (e.g. "def func(self):... self.selfImprovement" => "... this.object.this.object.Improvement").
+	def PopulateFrom(this, function):
+		this.source = ':'.join(inspect.getsource(function).split(':')[1:]) #Remove the first function definition
+
+		args = inspect.signature(function, follow_wrapped=False).parameters
+		thisSymbol = next(iter(args))
+		#del args[thisSymbol] # ??? 'mappingproxy' object does not support item deletion
+		this.source = this.source.replace(thisSymbol, 'this.object')
+
+		first = True
+		for arg in args.values(): #args.values[1:] also doesn't work.
+			if (first):
+				first = False
+				continue
+
+			replaceWith = arg.name
+
+			if (arg.kind == inspect.Parameter.VAR_POSITIONAL):
+				replaceWith = 'this.args'
+
+			elif (arg.kind == inspect.Parameter.VAR_KEYWORD):
+				replaceWith = 'this.kwargs'
+
+			else:
+				if (arg.default != inspect.Parameter.empty):
+					this.optionalKWArgs[arg.name] = arg.default
+				else:
+					this.requiredKWArgs.append(arg.name)
+				replaceWith = f'this.{arg.name}'
+
+				if (arg.kind in [inspect.Parameter.POSITIONAL_OR_KEYWORD, inspect.Parameter.POSITIONAL_ONLY]):
+					this.argMapping.append(arg.name)
+
+			this.source = this.source.replace(arg.name, replaceWith)
+
+
+	# When properly constructing a Method, rely only on the function *this should implement.
+	# The class and all other properties are irrelevant. However, they are provided and intended for debugging only.
+	def Constructor(this, function, cls):
+		this.name = function.__name__
+		this.original.cls = cls
+		this.original.function = function
+
+		this.PopulateFrom(function)
+		
+		# UpdateSource is called by Functor.PopulateMethods()
+		# this.UpdateSource()
+
+
+	# Grab any known and necessary args from this.kwargs before any Fetch calls are made.
+	def PopulatePrecursor(this):
+		if (not this.object):
+			raise MissingArgumentError(f"Call {this.name} from a class instance: {this.original.cls.__name__}.{this.name}(...). Maybe Functor.PopulateMethods() hasn't been called yet?")
+
+		this.executor = this.object.executor
+
+		if ('precursor' in this.kwargs):
+			this.precursor = this.kwargs.pop('precursor')
+		else:
+			this.precursor = None
+
+
+	# Next is set by Functor.PopulateMethods.
+	# We  definitely don't want to Fetch 'next'.
+	def PopulateNext(this):
+		pass
+
+
+	# Method.next should be a list of other Methods, as opposed to the standard string; so, instead of Executor.Execute..., we can directly invoke whatever is next.
+	# We skip all validation here.
+	# We also don't pass any args that were given in the initial function call. Those can all be Fetched from 'precursor'.
+	def CallNext(this):
+		if (not this.next):
+			return None
+
+		for next in this.next:
+			next(precursor=this)
+
+
+# The standard Functor extends Functor to add a set of standard members and methods.
+# This is similar to the standard library in C and C++
+# You must inherit from *this if you would like to use the functionality *this provides. The methods defined will not be propagated.
+class StandardFunctor(Functor):
+	def __init__(this, name="Standard Functor"):
+		super().__init__(name)
+
+	# Override this and do whatever!
+	# This is purposefully vague.
+	def Function(this):
+		pass
+
+
+	# Undo any changes made by UserFunction.
+	# Please override this too!
+	def Rollback(this):
+		pass
+
+
+	# Override this to check results of operation and report on status.
+	# Override this to perform whatever success checks are necessary.
+	def DidFunctionSucceed(this):
+		return this.functionSucceeded
+
+
+	# RETURN whether or not the Rollback was successful.
+	# Override this to perform whatever success checks are necessary.
+	def DidRollbackSucceed(this):
+		return this.rollbackSucceeded
+
+
+	######## START: UTILITIES ########
+
+	# RETURNS: an opened file object for writing.
+	# Creates the path if it does not exist.
+	@method()
+	def CreateFile(this, file, mode="w+"):
+		Path(os.path.dirname(os.path.abspath(file))).mkdir(parents=True, exist_ok=True)
+		return open(file, mode)
+
+	# Copy a file or folder from source to destination.
+	# This really shouldn't be so hard...
+	# root allows us to interpret '/' as something other than the top of the filesystem.
+	@method()
+	def Copy(this, source, destination, root='/'):
+		if (source.startswith('/')):
+			source = str(Path(root).joinpath(source[1:]).resolve())
+		else:
+			source = str(Path(source).resolve())
+		
+		destination = str(Path(destination).resolve())
+		
+		Path(destination).parent.mkdir(parents=True, exist_ok=True)
+
+		if (os.path.isfile(source)):
+			logging.debug(f"Copying file {source} to {destination}")
+			try:
+				shutil.copy(source, destination)
+			except shutil.Error as exc:
+				errors = exc.args[0]
+				for error in errors:
+					src, dst, msg = error
+					logging.debug(f"{msg}")
+		elif (os.path.isdir(source)):
+			logging.debug(f"Copying directory {source} to {destination}")
+			try:
+				shutil.copytree(source, destination)
+			except shutil.Error as exc:
+				errors = exc.args[0]
+				for error in errors:
+					src, dst, msg = error
+					logging.debug(f"{msg}")
+		else:
+			logging.error(f"Could not find source to copy: {source}")
+
+	# Delete a file or folder
+	@method()
+	def Delete(this, target):
+		if (not os.path.exists(target)):
+			logging.debug(f"Unable to delete nonexistent target: {target}")
+			return
+		if (os.path.isfile(target)):
+			logging.debug(f"Deleting file {target}")
+			os.remove(target)
+		elif (os.path.isdir(target)):
+			logging.debug(f"Deleting directory {target}")
+			try:
+				shutil.rmtree(target)
+			except shutil.Error as exc:
+				errors = exc.args[0]
+				for error in errors:
+					src, dst, msg = error
+					logging.debug(f"{msg}")
+
+	# Run whatever.
+	# DANGEROUS!!!!!
+	# RETURN: Return value and, optionally, the output as a list of lines.
+	@method()
+	def RunCommand(this, command, saveout=False, raiseExceptions=True):
+		logging.debug(f"================ Running command: {command} ================")
+		process = Popen(command, stdout=PIPE, stderr=STDOUT, shell=True)
+		output = []
+		while process.poll() is None:
+			line = process.stdout.readline().decode('utf8')[:-1]
+			if (saveout):
+				output.append(line)
+			if (line):
+				logging.debug(f"| {line}")  # [:-1] to strip excessive new lines.
+
+		message = f"Command returned {process.returncode}: {command}"
+		logging.debug(message)
+		if (raiseExceptions and process.returncode is not None and process.returncode):
+			raise CommandUnsuccessful(message)
+		
+		logging.debug(f"================ Completed command: {command} ================")
+		if (saveout):
+			return process.returncode, output
+		
+		return process.returncode
+	######## END: UTILITIES ########
+
+
+# Use an ErrorStringParser for each "parsers" in order to avoid having to override the GetObjectFromError method and create a new class for every error you want to handle.
+# ErrorStringParsers enable ErrorResolutions to be created on a per-functionality, rather than per-error basis, reducing the total amount of duplicate code.
+# Each error has a different string. In order to get the object of the error, we have to know where the object starts and ends.
+# NOTE: this assumes only 1 object per string. Maybe fancier parsing logic can be added in the future.
+#
+# startPosition is always positive
+# endPosition is always negative
+class ErrorStringParser:
+
+	def __init__(this, applicableError, startPosition, endPosition):
+		this.applicableError = applicableError
+		this.startPosition = startPosition
+		this.endPosition = endPosition
+
+	def Parse(this, errorString):
+		end = this.endPosition
+		if (not end):
+			end = len(errorString)
+		return errorString[this.startPosition:end]
+
+
+# ErrorResolution is a Functor which can be executed when an Exception is raised.
+# The goal of this class is to do some kind of work that will fix the problem on the second try of whatever generated the error.
+class ErrorResolution(StandardFunctor):
+
+	def __init__(this, name=INVALID_NAME()):
+		super().__init__(name)
+
+		# What errors, as ErrorStringParser objects, is *this prepared to handle?
+		this.parsers = []
+
+		this.error = None
+		this.errorType = ""
+		this.errorString = ""
+		this.errorObject = ""
+		this.errorResolutionStack = {}
+
+		# Provided directly from the recoverable decorator.
+		this.optionalKWArgs["obj"] = None
+		this.optionalKWArgs["function"] = None
+
+		# We do want to know whether or not we should attempt to run whatever failed again.
+		# So, let's store that in functionSucceeded. Meaning if this.functionSucceeded, try the original method again.
+		# No rollback, by default and definitely don't throw Exceptions.
+		this.enableRollback = False
+		this.functionSucceeded = True
+		this.raiseExceptions = False
+
+		this.errorShouldBeResolved = False
+
+
+
+	# Put your logic here!
+	def Resolve(this):
+		# You get the following members:
+		# this.error (an Exception)
+		# this.errorString (a string cast of the Exception)
+		# this.errorType (a string)
+		# this.errorObjet (a string or whatever you return from GetObjectFromError())
+
+		# You get the following guarantees:
+		# *this has not been called on this particular error before.
+		# the error given is applicable to *this per this.parsers
+
+		###############################################
+		# Please throw errors if something goes wrong #
+		# Otherwise, set this.errorShouldBeResolved   #
+		###############################################
+		
+		pass
+
+
+
+	# Helper method for creating ErrorStringParsers
+	# To use this, simply take an example output and replace the object you want to extract with "OBJECT"
+	def ApplyTo(this, error, exampleString):
+		match = re.search('OBJECT', exampleString)
+		this.parsers.append(ErrorStringParser(error, match.start(), match.end() - len(exampleString)))
+
+
+	# Get the type of this.error as a string.
+	def GetErrorType(this):
+		return type(this.error).__name__
+
+
+	# Get an actionable object from the error.
+	# For example, if the error is 'ModuleNotFoundError', what is the module?
+	def GetObjectFromError(this):
+		for parser in this.parsers:
+			if (parser.applicableError != this.errorType):
+				continue
+
+			this.errorObject = parser.Parse(this.errorString)
+			return
+
+		raise ErrorResolutionError(f"{this.name} cannot parse error object from ({this.errorType}): {str(this.error)}.")
+
+
+	# Determine if this resolution method is applicable.
+	def CanProcess(this):
+		return this.GetErrorType() in [parser.applicableError for parser in this.parsers]
+
+
+	# Grab any known and necessary args from this.kwargs before any Fetch calls are made.
+	def ParseInitialArgs(this):
+		super().ParseInitialArgs()
+		if ('error' in this.kwargs):
+			this.error = this.kwargs.pop('error')
+			# Just assume the error is an actual Exception object.
+		else:
+			raise ErrorResolutionError(f"{this.name} was not given an error to resolve.")
+
+		this.errorString = str(this.error)
+		this.errorType = this.GetErrorType()
+
+		# Internal member to avoid processing duplicates
+		this.errorResolutionStack = this.executor.errorResolutionStack
+
+
+	# Error resolution is unchained.
+	def PopulateNext(this):
+		this.next = []
+
+
+	# Override of Functor method.
+	# We'll keep calling this until an error is raised.
+	def Function(this):
+		this.functionSucceeded = True
+		this.errorShouldBeResolved = True
+		
+		if (not this.CanProcess()):
+			this.errorShouldBeResolved = False
+			return this.errorResolutionStack, this.errorShouldBeResolved
+
+		if (not this.errorString in this.errorResolutionStack.keys()):
+			this.errorResolutionStack.update({this.errorString:[]})
+		
+		if (this.name in this.errorResolutionStack[this.errorString]):
+			raise FailedErrorResolution(f"{this.name} already tried and failed to resolve {this.errorType}: {this.errorString}.")
+
+		this.GetObjectFromError()
+
+		try:
+			this.Resolve()
+		except Exception as e:
+			logging.error(f"Error resolution with {this.name} failed: {e}")
+			util.LogStack()
+			this.functionSucceeded = False
+		
+		this.errorResolutionStack[this.errorString].append(this.name)
+		return this.errorResolutionStack, this.errorShouldBeResolved
+
```

### Comparing `eons-2.6.1/pkg/eons/method/External.py` & `eons-2.6.2/pkg/eons/method/External.py`

 * *Files identical despite different names*

### Comparing `eons-2.6.1/pkg/eons/resolve/resolve_find_by_fetch.py` & `eons-2.6.2/pkg/eons/resolve/resolve_find_by_fetch.py`

 * *Files identical despite different names*

### Comparing `eons-2.6.1/pkg/eons/resolve/resolve_import_module.py` & `eons-2.6.2/pkg/eons/resolve/resolve_import_module.py`

 * *Files identical despite different names*

### Comparing `eons-2.6.1/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py` & `eons-2.6.2/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py`

 * *Files identical despite different names*

### Comparing `eons-2.6.1/pkg/eons.egg-info/PKG-INFO` & `eons-2.6.2/pkg/eons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.6.1
+Version: 2.6.2
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.6.1/pkg/eons.egg-info/SOURCES.txt` & `eons-2.6.2/pkg/eons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eons-2.6.1/setup.cfg` & `eons-2.6.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eons
-version = 2.6.1
+version = 2.6.2
 author = Eons
 author_email = support@eons.llc
 description = Eons Python Framework
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/eons.lib
@@ -18,20 +18,20 @@
 
 [options]
 package_dir = 
 	= pkg
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	jsonpickle
 	requests
+	requests_futures
 	tqdm
 	pyyaml
+	jsonpickle
 	eot
-	requests_futures
 
 [options.packages.find]
 where = pkg
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

