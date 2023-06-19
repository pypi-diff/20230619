# Comparing `tmp/decoratory-0.1.2.3.tar.gz` & `tmp/decoratory-0.1.3.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoratory-0.1.2.3.tar", last modified: Sun Jun 18 17:23:04 2023, max compression
+gzip compressed data, was "decoratory-0.1.3.11.tar", last modified: Mon Jun 19 16:30:58 2023, max compression
```

## Comparing `decoratory-0.1.2.3.tar` & `decoratory-0.1.3.11.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 17:23:04.955683 decoratory-0.1.2.3/
--rw-rw-rw-   0        0        0     2550 2023-06-02 20:50:35.000000 decoratory-0.1.2.3/License.txt
--rw-rw-rw-   0        0        0    43195 2023-06-18 17:23:04.955683 decoratory-0.1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0    41570 2023-06-18 17:20:31.000000 decoratory-0.1.2.3/Readme.rst
--rw-rw-rw-   0        0        0        0 2023-06-10 04:00:34.000000 decoratory-0.1.2.3/Requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-18 17:23:04.902316 decoratory-0.1.2.3/Sources/
-drwxrwxrwx   0        0        0        0 2023-06-18 17:23:04.940058 decoratory-0.1.2.3/Sources/decoratory/
--rw-rw-rw-   0        0        0      249 2023-06-07 18:32:49.000000 decoratory-0.1.2.3/Sources/decoratory/__init__.py
--rw-rw-rw-   0        0        0     5466 2023-06-18 17:22:40.000000 decoratory-0.1.2.3/Sources/decoratory/__main__.py
--rw-rw-rw-   0        0        0     5490 2023-06-18 11:48:18.000000 decoratory-0.1.2.3/Sources/decoratory/banner.py
--rw-rw-rw-   0        0        0    14152 2023-06-17 09:30:05.000000 decoratory-0.1.2.3/Sources/decoratory/basic.py
--rw-rw-rw-   0        0        0    11946 2023-06-17 11:25:08.000000 decoratory-0.1.2.3/Sources/decoratory/multiton.py
--rw-rw-rw-   0        0        0    38712 2023-06-18 17:18:51.000000 decoratory-0.1.2.3/Sources/decoratory/observer.py
--rw-rw-rw-   0        0        0     7319 2023-06-17 11:25:08.000000 decoratory-0.1.2.3/Sources/decoratory/singleton.py
--rw-rw-rw-   0        0        0     9932 2023-06-17 11:25:08.000000 decoratory-0.1.2.3/Sources/decoratory/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:23:04.940058 decoratory-0.1.2.3/Sources/decoratory.egg-info/
--rw-rw-rw-   0        0        0    43195 2023-06-18 17:23:04.000000 decoratory-0.1.2.3/Sources/decoratory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      586 2023-06-18 17:23:04.000000 decoratory-0.1.2.3/Sources/decoratory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 17:23:04.000000 decoratory-0.1.2.3/Sources/decoratory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-18 17:23:04.000000 decoratory-0.1.2.3/Sources/decoratory.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-18 17:23:04.955683 decoratory-0.1.2.3/Unittest/
--rw-rw-rw-   0        0        0    24268 2023-06-18 11:03:38.000000 decoratory-0.1.2.3/Unittest/test_basic.py
--rw-rw-rw-   0        0        0    21811 2023-06-18 10:51:44.000000 decoratory-0.1.2.3/Unittest/test_multiton.py
--rw-rw-rw-   0        0        0    42465 2023-06-18 08:46:05.000000 decoratory-0.1.2.3/Unittest/test_observer.py
--rw-rw-rw-   0        0        0    10504 2023-06-18 13:26:28.000000 decoratory-0.1.2.3/Unittest/test_singleton.py
--rw-rw-rw-   0        0        0     9069 2023-06-18 11:03:38.000000 decoratory-0.1.2.3/Unittest/test_wrapper.py
--rw-rw-rw-   0        0        0       42 2023-06-18 17:23:04.955683 decoratory-0.1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     4446 2023-06-18 17:22:40.000000 decoratory-0.1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:30:58.817531 decoratory-0.1.3.11/
+-rw-rw-rw-   0        0        0     2550 2023-06-02 20:50:35.000000 decoratory-0.1.3.11/License.txt
+-rw-rw-rw-   0        0        0    42585 2023-06-19 16:30:58.817531 decoratory-0.1.3.11/PKG-INFO
+-rw-rw-rw-   0        0        0    40959 2023-06-19 15:52:43.000000 decoratory-0.1.3.11/Readme.rst
+-rw-rw-rw-   0        0        0        0 2023-06-10 04:00:34.000000 decoratory-0.1.3.11/Requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 16:30:58.755034 decoratory-0.1.3.11/Sources/
+drwxrwxrwx   0        0        0        0 2023-06-19 16:30:58.786288 decoratory-0.1.3.11/Sources/decoratory/
+-rw-rw-rw-   0        0        0      249 2023-06-07 18:32:49.000000 decoratory-0.1.3.11/Sources/decoratory/__init__.py
+-rw-rw-rw-   0        0        0     5467 2023-06-19 16:30:22.000000 decoratory-0.1.3.11/Sources/decoratory/__main__.py
+-rw-rw-rw-   0        0        0     5490 2023-06-19 15:55:21.000000 decoratory-0.1.3.11/Sources/decoratory/banner.py
+-rw-rw-rw-   0        0        0    14152 2023-06-19 15:55:21.000000 decoratory-0.1.3.11/Sources/decoratory/basic.py
+-rw-rw-rw-   0        0        0    11946 2023-06-19 15:55:21.000000 decoratory-0.1.3.11/Sources/decoratory/multiton.py
+-rw-rw-rw-   0        0        0    37282 2023-06-19 16:25:39.000000 decoratory-0.1.3.11/Sources/decoratory/observer.py
+-rw-rw-rw-   0        0        0     7319 2023-06-19 15:55:21.000000 decoratory-0.1.3.11/Sources/decoratory/singleton.py
+-rw-rw-rw-   0        0        0     9932 2023-06-19 15:55:21.000000 decoratory-0.1.3.11/Sources/decoratory/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-19 16:30:58.801921 decoratory-0.1.3.11/Sources/decoratory.egg-info/
+-rw-rw-rw-   0        0        0    42585 2023-06-19 16:30:58.000000 decoratory-0.1.3.11/Sources/decoratory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      586 2023-06-19 16:30:58.000000 decoratory-0.1.3.11/Sources/decoratory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 16:30:58.000000 decoratory-0.1.3.11/Sources/decoratory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 16:30:58.000000 decoratory-0.1.3.11/Sources/decoratory.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 16:30:58.817531 decoratory-0.1.3.11/Unittest/
+-rw-rw-rw-   0        0        0    24037 2023-06-19 16:25:39.000000 decoratory-0.1.3.11/Unittest/test_basic.py
+-rw-rw-rw-   0        0        0    21837 2023-06-19 16:04:04.000000 decoratory-0.1.3.11/Unittest/test_multiton.py
+-rw-rw-rw-   0        0        0    40092 2023-06-19 16:25:39.000000 decoratory-0.1.3.11/Unittest/test_observer.py
+-rw-rw-rw-   0        0        0    10504 2023-06-19 15:55:21.000000 decoratory-0.1.3.11/Unittest/test_singleton.py
+-rw-rw-rw-   0        0        0     9098 2023-06-19 16:25:39.000000 decoratory-0.1.3.11/Unittest/test_wrapper.py
+-rw-rw-rw-   0        0        0       42 2023-06-19 16:30:58.817531 decoratory-0.1.3.11/setup.cfg
+-rw-rw-rw-   0        0        0     4447 2023-06-19 16:30:22.000000 decoratory-0.1.3.11/setup.py
```

### Comparing `decoratory-0.1.2.3/License.txt` & `decoratory-0.1.3.11/License.txt`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.2.3/PKG-INFO` & `decoratory-0.1.3.11/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoratory
-Version: 0.1.2.3
+Version: 0.1.3.11
 Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
 Home-page: http://evation.eu
 Download-URL: http://evation.eu
 Author: Martin Abel
 Author-email: Martin Abel <python@evation.eu>
 Maintainer: Martin Abel
 Maintainer-email: Martin Abel <python@evation.eu>
@@ -343,18 +343,18 @@
 .. code-block:: python
 
     # *** example_multitonton.py - Accessibility to the internal directory
 
     # Case 7: with decoration @Multiton(key=lambda spec, name: 'a' in name,
     #                                   accessible=True)
     print(Animal.get_instances())   # {}
-    a = Animal('dog', name='Teddy') #
+    a = Animal('dog', name='Teddy') 
     print(Animal.get_instances())   # {False: Animal('dog', 'Teddy')}
-    b = Animal('cat', name='Molly') #
-    c = Animal('dog', name='Roxie') #
+    b = Animal('cat', name='Molly') 
+    c = Animal('dog', name='Roxie') 
     print(Animal.get_instances())   # {False: Animal('dog', 'Teddy'),
                                     #  True:  Animal('cat', 'Molly')}
 
 In situations where it might be useful to reset the multiton to express in
 code that instances are often retrieved but rarely modified, setting the
 decorator parameter ``resettable=True`` will expose the ``reset()`` method,
 by means of which the internal directory of instances can be completely cleared.
@@ -556,15 +556,15 @@
 * `Class Decoration`_
 * `Instance Decoration`_ 
 
 
 Observable Decoration
 ---------------------
 
-The simplest and at the same time the most Pythonic variant of decoration
+The simplest and at the same time the most pythonic variant of decoration
 is to decorate only the *observed* entities.
 
 .. code-block:: python
 
     # *** example_observer.py - observable decoration
 
     from decoratory.observer import Observable
@@ -585,30 +585,14 @@
 
 Obviously, the addressed observer, the person, must be declared before
 the observed dog. With the simpler decoration 
 ``@Observable(observers=person)`` the person would always respond with their 
 default action and say ``'Hello?'``. The usage of ``F`` enables the transfer 
 of individual parameters to the observer.
 
-To make the observers more visible in the code, an (optional) observer 
-decoration is supported, i.e.
-
-.. code-block:: python
-
-    # *** example_observer.py - observable decoration
-
-    from decoratory.observer import Observer
-
-    @Observer                       # Just for the clarity of the code!
-    def person(say: str = "Hello?"):
-        print(f"{person.__name__} says '{say}'")
-
-This makes person an ``Observer``, but here with the same result as in 
-``Case 1`` above.
-
 Due to hierarchies in stacked observer patterns, a more detailed management
 of the observed objects may be necessary.
 
 .. code-block:: python
 
     # *** example_observer.py - observable decoration
 
@@ -839,26 +823,24 @@
 
 The instantiation of ``Dog`` induced an instantiation of ``Person``.
 
 .. warning::
 
     Calling **__init__()** results in a new instance! This means calling 
     the observable induces instantiation of a new observer object, surely
-    in not any case this is the desired action...
+    in not any case this is the desired behavior...
 
 So the decoration should not address a class but one (or more) target 
-functions. As already mentioned, this is easy if this callback function 
-is a ``@staticmethod`` or ``@classmethod``.
+methods of the class. As already mentioned, this is easy if this callback 
+function is a ``@staticmethod`` or ``@classmethod``.
 
 .. code-block:: python
 
     # *** example_observer.py - class decoration
 
-    from decoratory.observer import Observable
-
     class Person:
         def __init__(self, name: str = "Jane Doe"):
             print(f"{name} arrived.")
 
         @staticmethod
         def action1(act: str = "Hello?"):
             print(f"Person says {act}")
@@ -874,31 +856,28 @@
 
     # Case 2: Dog is an observable to Person.action
     prs = Person()                  # Jane Doe arrived.
     dog = Dog()                     # Dog Teddy arrived.
                                     # Person says Hello?
                                     # Person says What's up?
 
-This way, *one action* of ``Dog`` triggers *many actions* at one ``Person``
-(or on each ``Person``).
+This is how it usually works: *one action* of the observed ``Dog``, here it's 
+the instantiation, triggers *many actions* at each observing ``Person``.
 
-But often an instance method is more interesting as a callback function.
+But often an instance method is also interesting as a callback function.
 If a *particular instance* ``prs = Person(name="John Doe")`` of a person 
 is meant, a decoration like ``@Observable(observers=prs.action)`` 
 can be applied to ``Dog``. And for *any instance* 
 ``@Observable(observers=Person().action)`` works. Even a list of ``F`` 
 structures would be possible to submit different parameters.
 
 .. code-block:: python
 
     # *** example_observer.py - class decoration
 
-    from decoratory.observer import Observable
-    from decoratory.basic import F
-
     class Person:
         def __init__(self, name: str = "Jane Doe"):
             self.name = name
             print(f"{name} arrived.")
 
         def action(self, act: str = "Hello?"):
             print(f"{self.name} says {act}")
@@ -912,33 +891,29 @@
             print(f"Dog {name} arrived.")
 
     # Case 3: Dog is an observable to actions of various person instances.
     dog = Dog()                     # Dog Teddy arrived.
                                     # Jane Doe says Hello?
                                     # John Doe says What's up?
 
-This way, *one action* of ``Dog`` triggers *one or many actions* at each 
-of the selected ``Person`` instances. In such situations, a late 
-`dynamic decoration <#dynamic-decoration>`_ of Dog could be a good idea.
-Additionally, in all these cases, for the sake of code clarity, an optional 
-empty decoration ``@Oberserver class Person`` or ``@Oberserver() class Person`` 
-is recommended.
+Here, *one action* of the observed ``Dog``, its instantiation, triggers 
+*many actions* at each of the observing decorated ``Person`` instances. 
+In such situations, a late `dynamic decoration <#dynamic-decoration>`_ 
+of Dog could be a good idea.
 
-So far, instantiating ``Dog`` resulted in an information with the following 
+So far, instantiating ``Dog`` resulted in an information and induced  
 action at ``Person``. If ``Dog`` has its own actions that need to be 
 selectively monitored, each of the selected actions can of course be decorated 
 individually as an ``Observable``. For the sake of a better overview, this 
 can also be done on the class itself.
 
 .. code-block:: python
 
     # *** example_observer.py - class decoration
 
-    from decoratory.observer import Observable
-
     class Person:
         def __init__(self, name: str = "Jane Doe"):
             self.name = name
             print(f"{name} arrived.")
 
         @classmethod
         def actionA(cls, act: str = "Hello?"):
@@ -970,36 +945,35 @@
                                     # Person says Hello?    (@classmethod)
                                     # Any Doe says Hello?   (Instance 'Any')
 
     Dog.action2(dog)                # Teddy acts Brrr!      (Instance 'Teddy')
                                     # Person says Hello?    (@classmethod)
                                     # Any Doe says Hello?   (Instance 'Any')
 
-This last line ``Dog.action2(dog)`` provides the instance of ``Teddy`` as the 
+The last line ``Dog.action2(dog)`` provides the instance of ``Teddy`` as the 
 first argument. This works because implicitly the *class method* ``Dog.action2`` 
-was registered. Therefore the call ``dog.action2`` fails because this 
-*instance method* was not registered. But, if this is what is to be achieved, 
-an instance method must first be created and registered, as above.
+was registered. On the other hand, the call ``dog.action2()`` fails because 
+this *instance method* was not registered. But, if this is what is to be 
+achieved, an instance method can first be created and registered, just as 
+seen above.
 
 
 Instance Decoration 
 -------------------
 
 The classic way to exchange information between objects with the observer 
 pattern is through the active use of the ``register``, ``dispatch``, and 
-``unregister`` methods that an observable exports. This way, information can 
+``unregister`` interface methods that an observable exposes. Information can 
 be given to the right recipients at the right places in the code. For this, 
-the classes are not decorated. The `dynamic decoration <#dynamic-decoration>`_ 
-comes into play. 
-
-For this, the classes remain undecorated. Dynamic decoration is used, often 
-also in connection with getter/setter/property constructions, since data 
-changes take place meaningfully over these methods.
+the classes are not decorated and `dynamic decoration <#dynamic-decoration>`_ 
+comes into play. Dynamic decoration is used, often also in connection with 
+getter/setter/property constructions, since data changes take place 
+meaningfully over these methods.
 
-Let's start with the simple classes:
+Let's consider two simple classes:
 
 .. code-block:: python
 
     # *** example_observer.py - instance decoration
 
     class Note:                             # Observer without decoration!
         def info(self, thing):
@@ -1012,68 +986,72 @@
             self._a += 1
         def get_a(self):
             return self._a
         def set_a(self, value):
             self._a = value
         a = property(get_a, set_a)
 
-Well, some typical actions might be:
+Initially, they are undecorated and typical actions might be:
 
 .. code-block:: python
 
     # *** example_observer.py - instance decoration
 
-    from decoratory.observer import Observable
-    from decoratory.basic import F
-
     # (1) Setup instances
     nti = Note()                    # Note instance
-    thg = Thing()                   # Thing instance
+    tgi = Thing()                   # Thing instance
 
     # (2) Dynamic decoration of some methods: Late binding
-    thg.inc = Observable(thg.inc)           # Late method decoration   
+    tgi.inc = Observable(tgi.inc)           # Late method decoration   
     Thing.set_a = Observable(Thing.set_a)   # Late property decoration 
     Thing.a = property(Thing.get_a, Thing.set_a)
 
     # (3) Register the observer (Note) with the observable (Thing)
-    thg.inc.observable.register(F(nti.info, thg))
-    thg.set_a.observable.register(F(nti.info, thing=thg))
+    tgi.inc.observable.register(F(nti.info, tgi))
+    tgi.set_a.observable.register(F(nti.info, thing=tgi))
 
     # Case 1: Change self.a = 0 using inc()
-    thg.inc()                       # Note.info: val = 1
+    tgi.inc()                       # Note.info: val = 1
 
     # Case 2: Change self.a = 1 using setter via property
-    thg.a = 2                       # Note.info: val = 2
+    tgi.a = 2                       # Note.info: val = 2
 
     # Case 3: Notification from inc() to nti.info() about Thing(3)
-    thg.inc.observable.dispatch(nti.info, Thing(3))
+    tgi.inc.observable.dispatch(nti.info, Thing(3))
                                     # Note.info: val = 3
 
     # Case 4: Notification from set_a() to nti.info() about Thing(4)
-    thg.set_a.observable.dispatch(nti.info, Thing(4))
+    tgi.set_a.observable.dispatch(nti.info, Thing(4))
                                     # Note.info: val = 4
 
-    # Case 5: Print the current value of thg.a
-    print(f"a = {thg.a}")           # a = 2     (no changes by notifications)
+    # Case 5: Print the current value of tgi.a
+    print(f"a = {tgi.a}")           # a = 2     (no changes by notification)
 
     # Case 6: Print list of all observers
-    print(thg.inc.observable.observers(classbased=True))
+    print(tgi.inc.observable.observers(classbased=True))
     # ---> {'Note': ['F(info, <__main__.Thing object at ..)']}   
-    print(thg.set_a.observable.observers(classbased=True))
+    print(tgi.set_a.observable.observers(classbased=True))
     # ---> {'Note': ['F(info, thing=<__main__.Thing object at ..)']}
 
-    # Case 7: Unregister nti.info from thg
-    thg.inc.observable.unregister(nti.info)
-    print(thg.inc.observable.observers(classbased=True))    # {}
+    # Case 7: Unregister nti.info from tgi
+    tgi.inc.observable.unregister(nti.info)
+    print(tgi.inc.observable.observers(classbased=True))    # {}
     
+This method of instance decoration is certainly the most flexible. However, 
+it bears the risk of losing track of all dependencies. 
 
+    
 ******************************************************************************
 Version History
 ******************************************************************************
 
+**Version: 0.1.3.*, Build: 2023-06-19**
+
+- Enhancements for module observer: test and documentation
+
 **Version: 0.1.2.*, Build: 2023-06-18**
 
 - Intergration of unit tests for modules singleton, multiton and wrapper
 - An overall unit test for the package decoratory
 - Documentation enhancements for module observer, t.b.c.
 
 **Version: 0.1.1.*, Build: 2023-06-16**
```

### Comparing `decoratory-0.1.2.3/Readme.rst` & `decoratory-0.1.3.11/Readme.rst`

 * *Files 1% similar despite different names*

```diff
@@ -304,18 +304,18 @@
 .. code-block:: python
 
     # *** example_multitonton.py - Accessibility to the internal directory
 
     # Case 7: with decoration @Multiton(key=lambda spec, name: 'a' in name,
     #                                   accessible=True)
     print(Animal.get_instances())   # {}
-    a = Animal('dog', name='Teddy') #
+    a = Animal('dog', name='Teddy') 
     print(Animal.get_instances())   # {False: Animal('dog', 'Teddy')}
-    b = Animal('cat', name='Molly') #
-    c = Animal('dog', name='Roxie') #
+    b = Animal('cat', name='Molly') 
+    c = Animal('dog', name='Roxie') 
     print(Animal.get_instances())   # {False: Animal('dog', 'Teddy'),
                                     #  True:  Animal('cat', 'Molly')}
 
 In situations where it might be useful to reset the multiton to express in
 code that instances are often retrieved but rarely modified, setting the
 decorator parameter ``resettable=True`` will expose the ``reset()`` method,
 by means of which the internal directory of instances can be completely cleared.
@@ -517,15 +517,15 @@
 * `Class Decoration`_
 * `Instance Decoration`_ 
 
 
 Observable Decoration
 ---------------------
 
-The simplest and at the same time the most Pythonic variant of decoration
+The simplest and at the same time the most pythonic variant of decoration
 is to decorate only the *observed* entities.
 
 .. code-block:: python
 
     # *** example_observer.py - observable decoration
 
     from decoratory.observer import Observable
@@ -546,30 +546,14 @@
 
 Obviously, the addressed observer, the person, must be declared before
 the observed dog. With the simpler decoration 
 ``@Observable(observers=person)`` the person would always respond with their 
 default action and say ``'Hello?'``. The usage of ``F`` enables the transfer 
 of individual parameters to the observer.
 
-To make the observers more visible in the code, an (optional) observer 
-decoration is supported, i.e.
-
-.. code-block:: python
-
-    # *** example_observer.py - observable decoration
-
-    from decoratory.observer import Observer
-
-    @Observer                       # Just for the clarity of the code!
-    def person(say: str = "Hello?"):
-        print(f"{person.__name__} says '{say}'")
-
-This makes person an ``Observer``, but here with the same result as in 
-``Case 1`` above.
-
 Due to hierarchies in stacked observer patterns, a more detailed management
 of the observed objects may be necessary.
 
 .. code-block:: python
 
     # *** example_observer.py - observable decoration
 
@@ -800,26 +784,24 @@
 
 The instantiation of ``Dog`` induced an instantiation of ``Person``.
 
 .. warning::
 
     Calling **__init__()** results in a new instance! This means calling 
     the observable induces instantiation of a new observer object, surely
-    in not any case this is the desired action...
+    in not any case this is the desired behavior...
 
 So the decoration should not address a class but one (or more) target 
-functions. As already mentioned, this is easy if this callback function 
-is a ``@staticmethod`` or ``@classmethod``.
+methods of the class. As already mentioned, this is easy if this callback 
+function is a ``@staticmethod`` or ``@classmethod``.
 
 .. code-block:: python
 
     # *** example_observer.py - class decoration
 
-    from decoratory.observer import Observable
-
     class Person:
         def __init__(self, name: str = "Jane Doe"):
             print(f"{name} arrived.")
 
         @staticmethod
         def action1(act: str = "Hello?"):
             print(f"Person says {act}")
@@ -835,31 +817,28 @@
 
     # Case 2: Dog is an observable to Person.action
     prs = Person()                  # Jane Doe arrived.
     dog = Dog()                     # Dog Teddy arrived.
                                     # Person says Hello?
                                     # Person says What's up?
 
-This way, *one action* of ``Dog`` triggers *many actions* at one ``Person``
-(or on each ``Person``).
+This is how it usually works: *one action* of the observed ``Dog``, here it's 
+the instantiation, triggers *many actions* at each observing ``Person``.
 
-But often an instance method is more interesting as a callback function.
+But often an instance method is also interesting as a callback function.
 If a *particular instance* ``prs = Person(name="John Doe")`` of a person 
 is meant, a decoration like ``@Observable(observers=prs.action)`` 
 can be applied to ``Dog``. And for *any instance* 
 ``@Observable(observers=Person().action)`` works. Even a list of ``F`` 
 structures would be possible to submit different parameters.
 
 .. code-block:: python
 
     # *** example_observer.py - class decoration
 
-    from decoratory.observer import Observable
-    from decoratory.basic import F
-
     class Person:
         def __init__(self, name: str = "Jane Doe"):
             self.name = name
             print(f"{name} arrived.")
 
         def action(self, act: str = "Hello?"):
             print(f"{self.name} says {act}")
@@ -873,33 +852,29 @@
             print(f"Dog {name} arrived.")
 
     # Case 3: Dog is an observable to actions of various person instances.
     dog = Dog()                     # Dog Teddy arrived.
                                     # Jane Doe says Hello?
                                     # John Doe says What's up?
 
-This way, *one action* of ``Dog`` triggers *one or many actions* at each 
-of the selected ``Person`` instances. In such situations, a late 
-`dynamic decoration <#dynamic-decoration>`_ of Dog could be a good idea.
-Additionally, in all these cases, for the sake of code clarity, an optional 
-empty decoration ``@Oberserver class Person`` or ``@Oberserver() class Person`` 
-is recommended.
+Here, *one action* of the observed ``Dog``, its instantiation, triggers 
+*many actions* at each of the observing decorated ``Person`` instances. 
+In such situations, a late `dynamic decoration <#dynamic-decoration>`_ 
+of Dog could be a good idea.
 
-So far, instantiating ``Dog`` resulted in an information with the following 
+So far, instantiating ``Dog`` resulted in an information and induced  
 action at ``Person``. If ``Dog`` has its own actions that need to be 
 selectively monitored, each of the selected actions can of course be decorated 
 individually as an ``Observable``. For the sake of a better overview, this 
 can also be done on the class itself.
 
 .. code-block:: python
 
     # *** example_observer.py - class decoration
 
-    from decoratory.observer import Observable
-
     class Person:
         def __init__(self, name: str = "Jane Doe"):
             self.name = name
             print(f"{name} arrived.")
 
         @classmethod
         def actionA(cls, act: str = "Hello?"):
@@ -931,36 +906,35 @@
                                     # Person says Hello?    (@classmethod)
                                     # Any Doe says Hello?   (Instance 'Any')
 
     Dog.action2(dog)                # Teddy acts Brrr!      (Instance 'Teddy')
                                     # Person says Hello?    (@classmethod)
                                     # Any Doe says Hello?   (Instance 'Any')
 
-This last line ``Dog.action2(dog)`` provides the instance of ``Teddy`` as the 
+The last line ``Dog.action2(dog)`` provides the instance of ``Teddy`` as the 
 first argument. This works because implicitly the *class method* ``Dog.action2`` 
-was registered. Therefore the call ``dog.action2`` fails because this 
-*instance method* was not registered. But, if this is what is to be achieved, 
-an instance method must first be created and registered, as above.
+was registered. On the other hand, the call ``dog.action2()`` fails because 
+this *instance method* was not registered. But, if this is what is to be 
+achieved, an instance method can first be created and registered, just as 
+seen above.
 
 
 Instance Decoration 
 -------------------
 
 The classic way to exchange information between objects with the observer 
 pattern is through the active use of the ``register``, ``dispatch``, and 
-``unregister`` methods that an observable exports. This way, information can 
+``unregister`` interface methods that an observable exposes. Information can 
 be given to the right recipients at the right places in the code. For this, 
-the classes are not decorated. The `dynamic decoration <#dynamic-decoration>`_ 
-comes into play. 
-
-For this, the classes remain undecorated. Dynamic decoration is used, often 
-also in connection with getter/setter/property constructions, since data 
-changes take place meaningfully over these methods.
+the classes are not decorated and `dynamic decoration <#dynamic-decoration>`_ 
+comes into play. Dynamic decoration is used, often also in connection with 
+getter/setter/property constructions, since data changes take place 
+meaningfully over these methods.
 
-Let's start with the simple classes:
+Let's consider two simple classes:
 
 .. code-block:: python
 
     # *** example_observer.py - instance decoration
 
     class Note:                             # Observer without decoration!
         def info(self, thing):
@@ -973,68 +947,72 @@
             self._a += 1
         def get_a(self):
             return self._a
         def set_a(self, value):
             self._a = value
         a = property(get_a, set_a)
 
-Well, some typical actions might be:
+Initially, they are undecorated and typical actions might be:
 
 .. code-block:: python
 
     # *** example_observer.py - instance decoration
 
-    from decoratory.observer import Observable
-    from decoratory.basic import F
-
     # (1) Setup instances
     nti = Note()                    # Note instance
-    thg = Thing()                   # Thing instance
+    tgi = Thing()                   # Thing instance
 
     # (2) Dynamic decoration of some methods: Late binding
-    thg.inc = Observable(thg.inc)           # Late method decoration   
+    tgi.inc = Observable(tgi.inc)           # Late method decoration   
     Thing.set_a = Observable(Thing.set_a)   # Late property decoration 
     Thing.a = property(Thing.get_a, Thing.set_a)
 
     # (3) Register the observer (Note) with the observable (Thing)
-    thg.inc.observable.register(F(nti.info, thg))
-    thg.set_a.observable.register(F(nti.info, thing=thg))
+    tgi.inc.observable.register(F(nti.info, tgi))
+    tgi.set_a.observable.register(F(nti.info, thing=tgi))
 
     # Case 1: Change self.a = 0 using inc()
-    thg.inc()                       # Note.info: val = 1
+    tgi.inc()                       # Note.info: val = 1
 
     # Case 2: Change self.a = 1 using setter via property
-    thg.a = 2                       # Note.info: val = 2
+    tgi.a = 2                       # Note.info: val = 2
 
     # Case 3: Notification from inc() to nti.info() about Thing(3)
-    thg.inc.observable.dispatch(nti.info, Thing(3))
+    tgi.inc.observable.dispatch(nti.info, Thing(3))
                                     # Note.info: val = 3
 
     # Case 4: Notification from set_a() to nti.info() about Thing(4)
-    thg.set_a.observable.dispatch(nti.info, Thing(4))
+    tgi.set_a.observable.dispatch(nti.info, Thing(4))
                                     # Note.info: val = 4
 
-    # Case 5: Print the current value of thg.a
-    print(f"a = {thg.a}")           # a = 2     (no changes by notifications)
+    # Case 5: Print the current value of tgi.a
+    print(f"a = {tgi.a}")           # a = 2     (no changes by notification)
 
     # Case 6: Print list of all observers
-    print(thg.inc.observable.observers(classbased=True))
+    print(tgi.inc.observable.observers(classbased=True))
     # ---> {'Note': ['F(info, <__main__.Thing object at ..)']}   
-    print(thg.set_a.observable.observers(classbased=True))
+    print(tgi.set_a.observable.observers(classbased=True))
     # ---> {'Note': ['F(info, thing=<__main__.Thing object at ..)']}
 
-    # Case 7: Unregister nti.info from thg
-    thg.inc.observable.unregister(nti.info)
-    print(thg.inc.observable.observers(classbased=True))    # {}
+    # Case 7: Unregister nti.info from tgi
+    tgi.inc.observable.unregister(nti.info)
+    print(tgi.inc.observable.observers(classbased=True))    # {}
     
+This method of instance decoration is certainly the most flexible. However, 
+it bears the risk of losing track of all dependencies. 
 
+    
 ******************************************************************************
 Version History
 ******************************************************************************
 
+**Version: 0.1.3.*, Build: 2023-06-19**
+
+- Enhancements for module observer: test and documentation
+
 **Version: 0.1.2.*, Build: 2023-06-18**
 
 - Intergration of unit tests for modules singleton, multiton and wrapper
 - An overall unit test for the package decoratory
 - Documentation enhancements for module observer, t.b.c.
 
 **Version: 0.1.1.*, Build: 2023-06-16**
```

### Comparing `decoratory-0.1.2.3/Sources/decoratory/__main__.py` & `decoratory-0.1.3.11/Sources/decoratory/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.2.3"
-__date__ = "2023-06-18"
-__time__ = "19:22:40"
+__version__ = "0.1.3.11"
+__date__ = "2023-06-19"
+__time__ = "18:30:22"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = []
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.1.2.3/Sources/decoratory/banner.py` & `decoratory-0.1.3.11/Sources/decoratory/banner.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.2.21"
-__date__ = "2023-06-18"
-__time__ = "13:48:16"
+__version__ = "0.1.3.23"
+__date__ = "2023-06-19"
+__time__ = "17:55:21"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["__banner"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.1.2.3/Sources/decoratory/basic.py` & `decoratory-0.1.3.11/Sources/decoratory/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.2.1"
-__date__ = "2023-06-17"
-__time__ = "11:30:04"
+__version__ = "0.1.3.3"
+__date__ = "2023-06-19"
+__time__ = "17:55:21"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["Activation", "Parser", "F", "X"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.1.2.3/Sources/decoratory/multiton.py` & `decoratory-0.1.3.11/Sources/decoratory/multiton.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,17 +117,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.2.5"
-__date__ = "2023-06-17"
-__time__ = "13:25:04"
+__version__ = "0.1.3.7"
+__date__ = "2023-06-19"
+__time__ = "17:55:21"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["Multiton"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.1.2.3/Sources/decoratory/observer.py` & `decoratory-0.1.3.11/Sources/decoratory/observer.py`

 * *Files 4% similar despite different names*

```diff
@@ -409,17 +409,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.2.11"
-__date__ = "2023-06-18"
-__time__ = "19:18:48"
+__version__ = "0.1.3.2"
+__date__ = "2023-06-19"
+__time__ = "18:25:39"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["Observer", "BaseObserver", "Observable", "BaseObservable"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
@@ -449,16 +449,16 @@
     method of class A or an instance a = A():
      - Registration call:   F(a.method, *args, **kwargs).eval()         or
                             F('method', a, *args, **kwargs).eval()      but not
      - Dynamic call:        F('method', *args, **kwargs).eval(obj=a)
     """
 
     def __init__(self, *args, **kwargs) -> None:
-        self.args = args
-        self.kwargs = kwargs
+        self.args = args or tuple()
+        self.kwargs = kwargs or dict()
 
         self.__observers = dict()  # dict of F-type observers: callee is key!
 
     # Methods of the Observer Pattern
     def register(self,
                  observer: Union[F, callable, str],
                  *observer_args,
@@ -632,25 +632,18 @@
         # --- Decorator Arguments Pattern (1/2)
         if self.__get__substitute() is not None:
             # Decoration without parameter(s)
             self.__set__substitute(
                 F(self.__get__substitute(), *args, **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
 
-            # Instance of BaseObservable
             self.__set__observable(Observable.BaseClass())
         else:
             # Decoration with parameter(s)
-            self.__set__decorator_args(args)
-            self.__set__decorator_kwargs(kwargs)
-
-            # Instance of BaseObservable
-            self.__set__observable(Observable.BaseClass(
-                *self.__get__decorator_args(),
-                **self.__get__decorator_kwargs()))
+            self.__set__observable(Observable.BaseClass(*args, **kwargs))
 
     def __call__(self, *args, **kwargs):
         # --- Decorator Arguments Pattern (2/2)
         if self.__get__substitute() is None:
             # Decoration with parameter(s)
             self.__set__substitute(F(args[0], *args[1:], **kwargs))
 
@@ -665,20 +658,20 @@
                     elif callable(mtd):
                         mtds = mtd.__name__
                         mtd0 = mtd
                     else:
                         raise TypeError(f"{mtd} is nor a string nor callable.")
                     # noinspection PyArgumentEqualDefault
                     mtd1 = Observable(
-                        None,  # Call with deco arguments (substitute is None)
-                        *self.__get__decorator_args(),
+                        None,  # Call with arguments (substitute is None)
+                        *self.observable.args,
                         observers=self.__get__observers(),
                         methods=None,  # Resolved, call to else part below!
                         activate=self.__get__activate(),
-                        **self.__get__decorator_kwargs())(
+                        **self.observable.kwargs)(
                         mtd0, *mtd_args, **mtd_kwargs)
                     setattr(subst, mtds, mtd1)
 
                 # Return the undecorated original class
                 return subst
             else:
                 # Setup observers
@@ -713,30 +706,14 @@
         return self.__substitute
 
     def __set__substitute(self, value):
         self.__substitute = value
 
     substitute = property(__get__substitute)
 
-    def __get__decorator_args(self):
-        return self.__decorator_args
-
-    def __set__decorator_args(self, value):
-        self.__decorator_args = value
-
-    decorator_args = property(__get__decorator_args)
-
-    def __get__decorator_kwargs(self):
-        return self.__decorator_kwargs
-
-    def __set__decorator_kwargs(self, value):
-        self.__decorator_kwargs = value
-
-    decorator_kwargs = property(__get__decorator_kwargs)
-
     def __get__observers(self):
         return self.__observers
 
     def __set__observers(self, value):
         self.__observers: list = Parser.eval(value)
 
     observers = property(__get__observers)
@@ -776,16 +753,16 @@
     callable as an observer is optional. If BaseObserver is overwritten and
     assigned to the observers BaseClass attribute all non captured decorator
     args & kwargs will be submitted to be used in customized class
     functionalities.
     """
 
     def __init__(self, *args, **kwargs):
-        self.args = args
-        self.kwargs = kwargs
+        self.args = args or tuple()
+        self.kwargs = kwargs or dict()
 
 
 class Observer:
     """**Observer** (Subscriber, Object)
 
     Creating an observer instantiates a callable object which exposes the
     original decorator arguments, if present, like the callable to be
@@ -834,25 +811,18 @@
         # --- Decorator Arguments Pattern (1/2)
         if self.__get__substitute() is not None:
             # Decoration without parameter(s)
             self.__set__substitute(
                 F(self.__get__substitute(), *args, **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
 
-            # Instance of BaseObserver
             self.__set__observer(Observer.BaseClass())
         else:
             # Decoration with parameter(s)
-            self.__set__decorator_args(args)
-            self.__set__decorator_kwargs(kwargs)
-
-            # Instance of BaseObserver
-            self.__set__observer(Observer.BaseClass(
-                *self.__get__decorator_args(),
-                **self.__get__decorator_kwargs()))
+            self.__set__observer(Observer.BaseClass(*args, **kwargs))
 
     def __call__(self, *args, **kwargs):
         # --- Decorator Arguments Pattern (2/2)
         if self.__get__substitute() is None:
             # Decoration with parameter(s)
             self.__set__substitute(F(args[0], *args[1:], **kwargs))
 
@@ -868,18 +838,18 @@
                         mtds = mtd.__name__
                         mtd0 = mtd
                     else:
                         raise TypeError(f"{mtd} is nor a string nor callable.")
                     # noinspection PyArgumentEqualDefault
                     mtd1 = Observer(
                         None,  # Call with deco arguments (substitute is None)
-                        *self.__get__decorator_args(),
+                        *self.observer.args,
                         observables=self.__get__observables(),
                         methods=None,  # Resolved, call to else part below!
-                        **self.__get__decorator_kwargs())(
+                        **self.observer.kwargs)(
                         mtd0, *mtd_args, **mtd_kwargs)
                     setattr(subst, mtds, mtd1)
 
                 # Return the undecorated original class
                 return subst
             else:
                 # Register self as a callable object for callback
@@ -914,30 +884,14 @@
         return self.__substitute
 
     def __set__substitute(self, value):
         self.__substitute = value
 
     substitute = property(__get__substitute)
 
-    def __get__decorator_args(self):
-        return self.__decorator_args
-
-    def __set__decorator_args(self, value):
-        self.__decorator_args = value
-
-    decorator_args = property(__get__decorator_args)
-
-    def __get__decorator_kwargs(self):
-        return self.__decorator_kwargs
-
-    def __set__decorator_kwargs(self, value):
-        self.__decorator_kwargs = value
-
-    decorator_kwargs = property(__get__decorator_kwargs)
-
     def __get__observables(self):
         return self.__observables
 
     def __set__observables(self, value):
         self.__observables: list = Parser.eval(value)
 
     observables = property(__get__observables)
```

### Comparing `decoratory-0.1.2.3/Sources/decoratory/singleton.py` & `decoratory-0.1.3.11/Sources/decoratory/singleton.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,17 +72,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.2.7"
-__date__ = "2023-06-17"
-__time__ = "13:25:04"
+__version__ = "0.1.3.9"
+__date__ = "2023-06-19"
+__time__ = "17:55:21"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["Singleton"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.1.2.3/Sources/decoratory/wrapper.py` & `decoratory-0.1.3.11/Sources/decoratory/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,17 +116,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.2.5"
-__date__ = "2023-06-17"
-__time__ = "13:25:04"
+__version__ = "0.1.3.7"
+__date__ = "2023-06-19"
+__time__ = "17:55:21"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["Wrapper"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.1.2.3/Sources/decoratory.egg-info/PKG-INFO` & `decoratory-0.1.3.11/Sources/decoratory.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoratory
-Version: 0.1.2.3
+Version: 0.1.3.11
 Summary: Decorators: Singleton, Multiton, Observer, Observable, generic Wrapper.
 Home-page: http://evation.eu
 Download-URL: http://evation.eu
 Author: Martin Abel
 Author-email: Martin Abel <python@evation.eu>
 Maintainer: Martin Abel
 Maintainer-email: Martin Abel <python@evation.eu>
@@ -343,18 +343,18 @@
 .. code-block:: python
 
     # *** example_multitonton.py - Accessibility to the internal directory
 
     # Case 7: with decoration @Multiton(key=lambda spec, name: 'a' in name,
     #                                   accessible=True)
     print(Animal.get_instances())   # {}
-    a = Animal('dog', name='Teddy') #
+    a = Animal('dog', name='Teddy') 
     print(Animal.get_instances())   # {False: Animal('dog', 'Teddy')}
-    b = Animal('cat', name='Molly') #
-    c = Animal('dog', name='Roxie') #
+    b = Animal('cat', name='Molly') 
+    c = Animal('dog', name='Roxie') 
     print(Animal.get_instances())   # {False: Animal('dog', 'Teddy'),
                                     #  True:  Animal('cat', 'Molly')}
 
 In situations where it might be useful to reset the multiton to express in
 code that instances are often retrieved but rarely modified, setting the
 decorator parameter ``resettable=True`` will expose the ``reset()`` method,
 by means of which the internal directory of instances can be completely cleared.
@@ -556,15 +556,15 @@
 * `Class Decoration`_
 * `Instance Decoration`_ 
 
 
 Observable Decoration
 ---------------------
 
-The simplest and at the same time the most Pythonic variant of decoration
+The simplest and at the same time the most pythonic variant of decoration
 is to decorate only the *observed* entities.
 
 .. code-block:: python
 
     # *** example_observer.py - observable decoration
 
     from decoratory.observer import Observable
@@ -585,30 +585,14 @@
 
 Obviously, the addressed observer, the person, must be declared before
 the observed dog. With the simpler decoration 
 ``@Observable(observers=person)`` the person would always respond with their 
 default action and say ``'Hello?'``. The usage of ``F`` enables the transfer 
 of individual parameters to the observer.
 
-To make the observers more visible in the code, an (optional) observer 
-decoration is supported, i.e.
-
-.. code-block:: python
-
-    # *** example_observer.py - observable decoration
-
-    from decoratory.observer import Observer
-
-    @Observer                       # Just for the clarity of the code!
-    def person(say: str = "Hello?"):
-        print(f"{person.__name__} says '{say}'")
-
-This makes person an ``Observer``, but here with the same result as in 
-``Case 1`` above.
-
 Due to hierarchies in stacked observer patterns, a more detailed management
 of the observed objects may be necessary.
 
 .. code-block:: python
 
     # *** example_observer.py - observable decoration
 
@@ -839,26 +823,24 @@
 
 The instantiation of ``Dog`` induced an instantiation of ``Person``.
 
 .. warning::
 
     Calling **__init__()** results in a new instance! This means calling 
     the observable induces instantiation of a new observer object, surely
-    in not any case this is the desired action...
+    in not any case this is the desired behavior...
 
 So the decoration should not address a class but one (or more) target 
-functions. As already mentioned, this is easy if this callback function 
-is a ``@staticmethod`` or ``@classmethod``.
+methods of the class. As already mentioned, this is easy if this callback 
+function is a ``@staticmethod`` or ``@classmethod``.
 
 .. code-block:: python
 
     # *** example_observer.py - class decoration
 
-    from decoratory.observer import Observable
-
     class Person:
         def __init__(self, name: str = "Jane Doe"):
             print(f"{name} arrived.")
 
         @staticmethod
         def action1(act: str = "Hello?"):
             print(f"Person says {act}")
@@ -874,31 +856,28 @@
 
     # Case 2: Dog is an observable to Person.action
     prs = Person()                  # Jane Doe arrived.
     dog = Dog()                     # Dog Teddy arrived.
                                     # Person says Hello?
                                     # Person says What's up?
 
-This way, *one action* of ``Dog`` triggers *many actions* at one ``Person``
-(or on each ``Person``).
+This is how it usually works: *one action* of the observed ``Dog``, here it's 
+the instantiation, triggers *many actions* at each observing ``Person``.
 
-But often an instance method is more interesting as a callback function.
+But often an instance method is also interesting as a callback function.
 If a *particular instance* ``prs = Person(name="John Doe")`` of a person 
 is meant, a decoration like ``@Observable(observers=prs.action)`` 
 can be applied to ``Dog``. And for *any instance* 
 ``@Observable(observers=Person().action)`` works. Even a list of ``F`` 
 structures would be possible to submit different parameters.
 
 .. code-block:: python
 
     # *** example_observer.py - class decoration
 
-    from decoratory.observer import Observable
-    from decoratory.basic import F
-
     class Person:
         def __init__(self, name: str = "Jane Doe"):
             self.name = name
             print(f"{name} arrived.")
 
         def action(self, act: str = "Hello?"):
             print(f"{self.name} says {act}")
@@ -912,33 +891,29 @@
             print(f"Dog {name} arrived.")
 
     # Case 3: Dog is an observable to actions of various person instances.
     dog = Dog()                     # Dog Teddy arrived.
                                     # Jane Doe says Hello?
                                     # John Doe says What's up?
 
-This way, *one action* of ``Dog`` triggers *one or many actions* at each 
-of the selected ``Person`` instances. In such situations, a late 
-`dynamic decoration <#dynamic-decoration>`_ of Dog could be a good idea.
-Additionally, in all these cases, for the sake of code clarity, an optional 
-empty decoration ``@Oberserver class Person`` or ``@Oberserver() class Person`` 
-is recommended.
+Here, *one action* of the observed ``Dog``, its instantiation, triggers 
+*many actions* at each of the observing decorated ``Person`` instances. 
+In such situations, a late `dynamic decoration <#dynamic-decoration>`_ 
+of Dog could be a good idea.
 
-So far, instantiating ``Dog`` resulted in an information with the following 
+So far, instantiating ``Dog`` resulted in an information and induced  
 action at ``Person``. If ``Dog`` has its own actions that need to be 
 selectively monitored, each of the selected actions can of course be decorated 
 individually as an ``Observable``. For the sake of a better overview, this 
 can also be done on the class itself.
 
 .. code-block:: python
 
     # *** example_observer.py - class decoration
 
-    from decoratory.observer import Observable
-
     class Person:
         def __init__(self, name: str = "Jane Doe"):
             self.name = name
             print(f"{name} arrived.")
 
         @classmethod
         def actionA(cls, act: str = "Hello?"):
@@ -970,36 +945,35 @@
                                     # Person says Hello?    (@classmethod)
                                     # Any Doe says Hello?   (Instance 'Any')
 
     Dog.action2(dog)                # Teddy acts Brrr!      (Instance 'Teddy')
                                     # Person says Hello?    (@classmethod)
                                     # Any Doe says Hello?   (Instance 'Any')
 
-This last line ``Dog.action2(dog)`` provides the instance of ``Teddy`` as the 
+The last line ``Dog.action2(dog)`` provides the instance of ``Teddy`` as the 
 first argument. This works because implicitly the *class method* ``Dog.action2`` 
-was registered. Therefore the call ``dog.action2`` fails because this 
-*instance method* was not registered. But, if this is what is to be achieved, 
-an instance method must first be created and registered, as above.
+was registered. On the other hand, the call ``dog.action2()`` fails because 
+this *instance method* was not registered. But, if this is what is to be 
+achieved, an instance method can first be created and registered, just as 
+seen above.
 
 
 Instance Decoration 
 -------------------
 
 The classic way to exchange information between objects with the observer 
 pattern is through the active use of the ``register``, ``dispatch``, and 
-``unregister`` methods that an observable exports. This way, information can 
+``unregister`` interface methods that an observable exposes. Information can 
 be given to the right recipients at the right places in the code. For this, 
-the classes are not decorated. The `dynamic decoration <#dynamic-decoration>`_ 
-comes into play. 
-
-For this, the classes remain undecorated. Dynamic decoration is used, often 
-also in connection with getter/setter/property constructions, since data 
-changes take place meaningfully over these methods.
+the classes are not decorated and `dynamic decoration <#dynamic-decoration>`_ 
+comes into play. Dynamic decoration is used, often also in connection with 
+getter/setter/property constructions, since data changes take place 
+meaningfully over these methods.
 
-Let's start with the simple classes:
+Let's consider two simple classes:
 
 .. code-block:: python
 
     # *** example_observer.py - instance decoration
 
     class Note:                             # Observer without decoration!
         def info(self, thing):
@@ -1012,68 +986,72 @@
             self._a += 1
         def get_a(self):
             return self._a
         def set_a(self, value):
             self._a = value
         a = property(get_a, set_a)
 
-Well, some typical actions might be:
+Initially, they are undecorated and typical actions might be:
 
 .. code-block:: python
 
     # *** example_observer.py - instance decoration
 
-    from decoratory.observer import Observable
-    from decoratory.basic import F
-
     # (1) Setup instances
     nti = Note()                    # Note instance
-    thg = Thing()                   # Thing instance
+    tgi = Thing()                   # Thing instance
 
     # (2) Dynamic decoration of some methods: Late binding
-    thg.inc = Observable(thg.inc)           # Late method decoration   
+    tgi.inc = Observable(tgi.inc)           # Late method decoration   
     Thing.set_a = Observable(Thing.set_a)   # Late property decoration 
     Thing.a = property(Thing.get_a, Thing.set_a)
 
     # (3) Register the observer (Note) with the observable (Thing)
-    thg.inc.observable.register(F(nti.info, thg))
-    thg.set_a.observable.register(F(nti.info, thing=thg))
+    tgi.inc.observable.register(F(nti.info, tgi))
+    tgi.set_a.observable.register(F(nti.info, thing=tgi))
 
     # Case 1: Change self.a = 0 using inc()
-    thg.inc()                       # Note.info: val = 1
+    tgi.inc()                       # Note.info: val = 1
 
     # Case 2: Change self.a = 1 using setter via property
-    thg.a = 2                       # Note.info: val = 2
+    tgi.a = 2                       # Note.info: val = 2
 
     # Case 3: Notification from inc() to nti.info() about Thing(3)
-    thg.inc.observable.dispatch(nti.info, Thing(3))
+    tgi.inc.observable.dispatch(nti.info, Thing(3))
                                     # Note.info: val = 3
 
     # Case 4: Notification from set_a() to nti.info() about Thing(4)
-    thg.set_a.observable.dispatch(nti.info, Thing(4))
+    tgi.set_a.observable.dispatch(nti.info, Thing(4))
                                     # Note.info: val = 4
 
-    # Case 5: Print the current value of thg.a
-    print(f"a = {thg.a}")           # a = 2     (no changes by notifications)
+    # Case 5: Print the current value of tgi.a
+    print(f"a = {tgi.a}")           # a = 2     (no changes by notification)
 
     # Case 6: Print list of all observers
-    print(thg.inc.observable.observers(classbased=True))
+    print(tgi.inc.observable.observers(classbased=True))
     # ---> {'Note': ['F(info, <__main__.Thing object at ..)']}   
-    print(thg.set_a.observable.observers(classbased=True))
+    print(tgi.set_a.observable.observers(classbased=True))
     # ---> {'Note': ['F(info, thing=<__main__.Thing object at ..)']}
 
-    # Case 7: Unregister nti.info from thg
-    thg.inc.observable.unregister(nti.info)
-    print(thg.inc.observable.observers(classbased=True))    # {}
+    # Case 7: Unregister nti.info from tgi
+    tgi.inc.observable.unregister(nti.info)
+    print(tgi.inc.observable.observers(classbased=True))    # {}
     
+This method of instance decoration is certainly the most flexible. However, 
+it bears the risk of losing track of all dependencies. 
 
+    
 ******************************************************************************
 Version History
 ******************************************************************************
 
+**Version: 0.1.3.*, Build: 2023-06-19**
+
+- Enhancements for module observer: test and documentation
+
 **Version: 0.1.2.*, Build: 2023-06-18**
 
 - Intergration of unit tests for modules singleton, multiton and wrapper
 - An overall unit test for the package decoratory
 - Documentation enhancements for module observer, t.b.c.
 
 **Version: 0.1.1.*, Build: 2023-06-16**
```

### Comparing `decoratory-0.1.2.3/Sources/decoratory.egg-info/SOURCES.txt` & `decoratory-0.1.3.11/Sources/decoratory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.2.3/Unittest/test_basic.py` & `decoratory-0.1.3.11/Unittest/test_basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,28 +13,35 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.2.3"
-__date__ = "2023-06-18"
-__time__ = "13:03:35"
+__version__ = "0.1.3.6"
+__date__ = "2023-06-19"
+__time__ = "18:25:39"
 __state__ = "Beta"
 __license__ = "PSF"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
 
 from decoratory.basic import (Activation, F, Parser, X)
 
 
 # -----------------------------------------------------------------------------
+# Test functions
+def cmp(f: F, t: tuple):
+    """Compare F with tuple"""
+    return (x == y for x, y in zip(f, t))
+
+
+# -----------------------------------------------------------------------------
 # Test Class
 # noinspection PyPep8Naming,PyArgumentEqualDefault
 class TestDecotools(unittest.TestCase):
 
     def setUp(self):
         """Preparation"""
         pass
@@ -59,19 +66,14 @@
 
         self.assertEqual(Activation.BEFORE_AND_AFTER,
                          Activation.BEFORE | Activation.AFTER)
 
     def test_F(self):
         """Unittest: F wrapper"""
 
-        # Helper
-        def cmp(F: F, t: tuple):
-            """Compare F with tuple"""
-            return (x == y for x, y in zip(F, t))
-
         # A callable
         def function(x, y):
             """Test function"""
             return x + y
 
         # ---------------------------------------------------------------------
         # Test
@@ -291,19 +293,14 @@
         self.assertTupleEqual(f.callee_args, (2, 3, 4))
         f.callee_kwargs = {'x': 2, 'y': 3, 'z': 4}
         self.assertDictEqual(f.callee_kwargs, {'x': 2, 'y': 3, 'z': 4})
 
     def test_X(self):
         """Unittest: X wrapper"""
 
-        # Helper
-        def cmp(X: X, t: tuple):
-            """Compare X with tuple"""
-            return (x == y for x, y in zip(X, t))
-
         # A callable
         def function(x, y):
             """Test function"""
             return int(x) + int(y)
 
         # ---------------------------------------------------------------------
         # Test
@@ -523,19 +520,14 @@
         self.assertTupleEqual(x.callee_args, (2, 3, 4))
         x.callee_kwargs = {'x': 2, 'y': 3, 'z': 4}
         self.assertDictEqual(x.callee_kwargs, {'x': 2, 'y': 3, 'z': 4})
 
     def test_Parser(self):
         """Unittest: Parser"""
 
-        # Helper
-        def cmp(F: F, t: tuple):
-            """Compare F with tuple"""
-            return (x == y for x, y in zip(F, t))
-
         # A callable
         def function(x, y):
             """Test function"""
             return x + y
 
         # ---------------------------------------------------------------------
         # Unittest: Parser.tuple
```

### Comparing `decoratory-0.1.2.3/Unittest/test_multiton.py` & `decoratory-0.1.3.11/Unittest/test_multiton.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.2.5"
-__date__ = "2023-06-18"
-__time__ = "12:51:41"
+__version__ = "0.1.3.9"
+__date__ = "2023-06-19"
+__time__ = "18:04:04"
 __state__ = "Beta"
 __license__ = "PSF"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
 
@@ -63,15 +63,17 @@
         pass
 
     def tearDown(self):
         """Shutdown"""
         pass
 
     def test_decoration_without_brackets(self):
-        """Unittest: Decoration without brackets --> No key: Multiton == Singleton"""
+        """Unittest: Decoration without brackets
+            --> No key: Multiton == Singleton
+        """
 
         TestClass = TestMultiton.TestClass
         TestClassMultiton = Multiton(TestClass)
 
         # Instances
         a = TestClassMultiton(name="a")  # New single object a
         b = TestClassMultiton(name="b")  # Multiton: b is a
@@ -149,15 +151,15 @@
         self.assertEqual(b, c)
         self.assertEqual(TestClass.__doc__, TestClassMultiton.__doc__)
         self.assertEqual(TestClass.__doc__, a.__doc__)
         self.assertEqual(TestClass.__doc__, b.__doc__)
         self.assertEqual(TestClass.__doc__, c.__doc__)
 
     def test_decoration_with_empty_brackets(self):
-        """Unittest: Decoration without brackets
+        """Unittest: Decoration with empty brackets
             --> No key: Multiton == Singleton
         """
         TestClass = TestMultiton.TestClass
         TestClassMultiton = Multiton()(TestClass)
 
         # Instances
         a = TestClassMultiton(name="a")  # New single object a
```

### Comparing `decoratory-0.1.2.3/Unittest/test_observer.py` & `decoratory-0.1.3.11/Unittest/test_observer.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,27 +13,46 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.2.2"
-__date__ = "2023-06-18"
-__time__ = "10:46:02"
+__version__ = "0.1.3.7"
+__date__ = "2023-06-19"
+__time__ = "18:25:39"
 __state__ = "Beta"
 __license__ = "PSF"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
 
 from decoratory.observer import (BaseObservable, BaseObserver,
-                                         Observable, Observer,
-                                         Activation, F, X)
+                                 Observable, Observer)
+from decoratory.basic import Activation, F, X
+
+
+# -----------------------------------------------------------------------------
+# Test functions
+def cmp(iter1, iter2):
+    """Compare *all* elements of F with a tuple"""
+    if len(iter1) != len(iter2):
+        return False
+    else:
+        iter1 = list(iter1)
+        iter2 = list(iter2)
+        iter1.sort()
+        iter2.sort()
+        for left, right in zip(iter1, iter2):
+            if left.callee != right.callee or \
+                    left.callee_args != right.callee_args or \
+                    left.callee_kwargs != right.callee_kwargs:
+                return False
+        return True
 
 
 # -----------------------------------------------------------------------------
 # Test Class
 # noinspection PyPep8Naming
 # noinspection PyUnresolvedReferences
 # noinspection PyArgumentEqualDefault
@@ -44,16 +63,16 @@
         """Preparation"""
         pass
 
     def tearDown(self):
         """Wrap-up"""
         pass
 
-    def test_basics_nodecos_noparams_without_brackets(self):
-        """Unittest: Observable & Observer - nodecos, noparams, nobrackets"""
+    def test_nodecoration_noparams_without_brackets(self):
+        """Unittest: Functions: no decoration, no parameters, no brackets"""
 
         # Result list
         res = list()
 
         # Observable
         def dog(act: str = "Brrr!") -> None:
             """A dog function"""
@@ -61,66 +80,74 @@
 
         # Observer
         def person(say: str = "Hello?") -> None:
             """A person function"""
             res.append(f"{person.__name__} says '{say}'")
 
         # ---------------------------------------------------------------------
-        # Test setup: Decoration
-        Dog = Observable(dog)
-        Person = Observer(person)
+        # Test setup: Observable, only
+        dog_obsl = Observable(dog)
+
+        # Checks for dog_obsl
+        self.assertTrue(isinstance(dog_obsl, Observable))
+        self.assertIs(dog_obsl.BaseClass, BaseObservable)
+        self.assertTrue(isinstance(dog_obsl.observable, dog_obsl.BaseClass))
+        self.assertTrue(hasattr(dog_obsl.observable, 'register'))
+        self.assertTrue(hasattr(dog_obsl.observable, 'unregister'))
+        self.assertTrue(hasattr(dog_obsl.observable, 'dispatch'))
+        self.assertTrue(hasattr(dog_obsl.observable, 'observers'))
+        self.assertTupleEqual(dog_obsl.observable.args, ())
+        self.assertDictEqual(dog_obsl.observable.kwargs, {})
+        self.assertIs(dog_obsl.activate, Activation.AFTER)
+        self.assertListEqual(dog_obsl.methods, [])
+        self.assertIs(dog_obsl.substitute.callee, dog)
+        self.assertTupleEqual(dog_obsl.substitute.callee_args, ())
+        self.assertDictEqual(dog_obsl.substitute.callee_kwargs, {})
+        self.assertIs(dog_obsl.__annotations__, dog.__annotations__)
+        self.assertIs(dog_obsl.__doc__, dog.__doc__)
+        self.assertIs(dog_obsl.__name__, dog.__name__)
+
+        # Calls
+        res.clear()
+        person()
+        self.assertListEqual(res, ["person says 'Hello?'"])
+        res.clear()
+        dog_obsl()
+        self.assertListEqual(res, ["dog acts 'Brrr!'"])
+
+        # ---------------------------------------------------------------------
+        # Test setup: Observable & Observer
+        prs_obsr = Observer(person)
 
-        # Basic checks for Dog
-        self.assertTrue(isinstance(Dog, Observable))
-        self.assertIs(Dog.BaseClass, BaseObservable)
-        self.assertTrue(isinstance(Dog.observable, Dog.BaseClass))
-        self.assertTrue(hasattr(Dog.observable, 'register'))
-        self.assertTrue(hasattr(Dog.observable, 'unregister'))
-        self.assertTrue(hasattr(Dog.observable, 'dispatch'))
-        self.assertTrue(hasattr(Dog.observable, 'observers'))
-        self.assertTupleEqual(Dog.observable.args, ())
-        self.assertDictEqual(Dog.observable.kwargs, {})
-        self.assertIs(Dog.activate, Activation.AFTER)
-        self.assertFalse(hasattr(Dog, 'decorator_args'))
-        self.assertFalse(hasattr(Dog, 'decorator_kwargs'))
-        self.assertListEqual(Dog.methods, [])
-        self.assertIs(Dog.substitute.callee, dog)
-        self.assertTupleEqual(Dog.substitute.callee_args, ())
-        self.assertDictEqual(Dog.substitute.callee_kwargs, {})
-        self.assertIs(Dog.__annotations__, dog.__annotations__)
-        self.assertIs(Dog.__doc__, dog.__doc__)
-        self.assertIs(Dog.__name__, dog.__name__)
-
-        # Basic checks for Person
-        self.assertTrue(isinstance(Person, Observer))
-        self.assertIs(Person.BaseClass, BaseObserver)
-        self.assertTrue(isinstance(Person.observer, Person.BaseClass))
-        self.assertTupleEqual(Person.observer.args, ())
-        self.assertDictEqual(Person.observer.kwargs, {})
-        self.assertFalse(hasattr(Person, 'decorator_args'))
-        self.assertFalse(hasattr(Person, 'decorator_kwargs'))
-        self.assertListEqual(Person.methods, [])
-        self.assertListEqual(Person.observables, [])
-        self.assertIs(Person.substitute.callee, person)
-        self.assertTupleEqual(Person.substitute.callee_args, ())
-        self.assertDictEqual(Person.substitute.callee_kwargs, {})
-        self.assertIs(Person.__annotations__, person.__annotations__)
-        self.assertIs(Person.__doc__, person.__doc__)
-        self.assertIs(Person.__name__, person.__name__)
+        # Checks for prs_obsr
+        self.assertTrue(isinstance(prs_obsr, Observer))
+        self.assertIs(prs_obsr.BaseClass, BaseObserver)
+        self.assertTrue(isinstance(prs_obsr.observer, prs_obsr.BaseClass))
+        self.assertTupleEqual(prs_obsr.observer.args, ())
+        self.assertDictEqual(prs_obsr.observer.kwargs, {})
+        self.assertListEqual(prs_obsr.methods, [])
+        self.assertListEqual(prs_obsr.observables, [])
+        self.assertIs(prs_obsr.substitute.callee, person)
+        self.assertTupleEqual(prs_obsr.substitute.callee_args, ())
+        self.assertDictEqual(prs_obsr.substitute.callee_kwargs, {})
+        self.assertIs(prs_obsr.__annotations__, person.__annotations__)
+        self.assertIs(prs_obsr.__doc__, person.__doc__)
+        self.assertIs(prs_obsr.__name__, person.__name__)
 
-        # Basic calls deliver function defaults
+        # ---------------------------------------------------------------------
+        # Calls
         res.clear()
-        Person()
+        prs_obsr()
         self.assertListEqual(res, ["person says 'Hello?'"])
         res.clear()
-        Dog()
+        dog_obsl()
         self.assertListEqual(res, ["dog acts 'Brrr!'"])
 
-    def test_basics_nodecos_noparams_with_empty_brackets(self):
-        """Unittest: Observable & Observer - nodecos, noparams, brackets"""
+    def test_nodecoration_noparams_with_empty_brackets(self):
+        """Unittest: Functions: no decoration, no parameters, empty brackets"""
 
         # Result list
         res = list()
 
         # Observable
         def dog(act: str = "Brrr!") -> None:
             """A dog function"""
@@ -128,66 +155,74 @@
 
         # Observer
         def person(say: str = "Hello?") -> None:
             """A person function"""
             res.append(f"{person.__name__} says '{say}'")
 
         # ---------------------------------------------------------------------
-        # Test setup: Decoration
-        Dog = Observable()(dog)
-        Person = Observer()(person)
+        # Test setup: Observable, only
+        dog_obsl = Observable()(dog)
+
+        # Checks for dog_obsl
+        self.assertTrue(isinstance(dog_obsl, Observable))
+        self.assertIs(dog_obsl.BaseClass, BaseObservable)
+        self.assertTrue(isinstance(dog_obsl.observable, dog_obsl.BaseClass))
+        self.assertTrue(hasattr(dog_obsl.observable, 'register'))
+        self.assertTrue(hasattr(dog_obsl.observable, 'unregister'))
+        self.assertTrue(hasattr(dog_obsl.observable, 'dispatch'))
+        self.assertTrue(hasattr(dog_obsl.observable, 'observers'))
+        self.assertTupleEqual(dog_obsl.observable.args, ())
+        self.assertDictEqual(dog_obsl.observable.kwargs, {})
+        self.assertIs(dog_obsl.activate, Activation.AFTER)
+        self.assertListEqual(dog_obsl.methods, [])
+        self.assertIs(dog_obsl.substitute.callee, dog)
+        self.assertTupleEqual(dog_obsl.substitute.callee_args, ())
+        self.assertDictEqual(dog_obsl.substitute.callee_kwargs, {})
+        self.assertIs(dog_obsl.__annotations__, dog.__annotations__)
+        self.assertIs(dog_obsl.__doc__, dog.__doc__)
+        self.assertIs(dog_obsl.__name__, dog.__name__)
+
+        # Calls
+        res.clear()
+        person()
+        self.assertListEqual(res, ["person says 'Hello?'"])
+        res.clear()
+        dog_obsl()
+        self.assertListEqual(res, ["dog acts 'Brrr!'"])
+
+        # ---------------------------------------------------------------------
+        # Test setup: Observable & Observer
+        prs_obsr = Observer()(person)
 
-        # Basic checks for Dog
-        self.assertTrue(isinstance(Dog, Observable))
-        self.assertIs(Dog.BaseClass, BaseObservable)
-        self.assertTrue(isinstance(Dog.observable, Dog.BaseClass))
-        self.assertTrue(hasattr(Dog.observable, 'register'))
-        self.assertTrue(hasattr(Dog.observable, 'unregister'))
-        self.assertTrue(hasattr(Dog.observable, 'dispatch'))
-        self.assertTrue(hasattr(Dog.observable, 'observers'))
-        self.assertTupleEqual(Dog.observable.args, ())
-        self.assertDictEqual(Dog.observable.kwargs, {})
-        self.assertIs(Dog.activate, Activation.AFTER)
-        self.assertTupleEqual(Dog.observable.args, ())
-        self.assertDictEqual(Dog.observable.kwargs, {})
-        self.assertListEqual(Dog.methods, [])
-        self.assertIs(Dog.substitute.callee, dog)
-        self.assertTupleEqual(Dog.substitute.callee_args, ())
-        self.assertDictEqual(Dog.substitute.callee_kwargs, {})
-        self.assertIs(Dog.__annotations__, dog.__annotations__)
-        self.assertIs(Dog.__doc__, dog.__doc__)
-        self.assertIs(Dog.__name__, dog.__name__)
-
-        # Basic checks for Person
-        self.assertTrue(isinstance(Person, Observer))
-        self.assertIs(Person.BaseClass, BaseObserver)
-        self.assertTrue(isinstance(Person.observer, Person.BaseClass))
-        self.assertTupleEqual(Person.observer.args, ())
-        self.assertDictEqual(Person.observer.kwargs, {})
-        self.assertTupleEqual(Person.observer.args, ())
-        self.assertDictEqual(Person.observer.kwargs, {})
-        self.assertListEqual(Person.methods, [])
-        self.assertListEqual(Person.observables, [])
-        self.assertIs(Person.substitute.callee, person)
-        self.assertTupleEqual(Person.substitute.callee_args, ())
-        self.assertDictEqual(Person.substitute.callee_kwargs, {})
-        self.assertIs(Person.__annotations__, person.__annotations__)
-        self.assertIs(Person.__doc__, person.__doc__)
-        self.assertIs(Person.__name__, person.__name__)
+        # Checks for prs_obsr
+        self.assertTrue(isinstance(prs_obsr, Observer))
+        self.assertIs(prs_obsr.BaseClass, BaseObserver)
+        self.assertTrue(isinstance(prs_obsr.observer, prs_obsr.BaseClass))
+        self.assertTupleEqual(prs_obsr.observer.args, ())
+        self.assertDictEqual(prs_obsr.observer.kwargs, {})
+        self.assertListEqual(prs_obsr.methods, [])
+        self.assertListEqual(prs_obsr.observables, [])
+        self.assertIs(prs_obsr.substitute.callee, person)
+        self.assertTupleEqual(prs_obsr.substitute.callee_args, ())
+        self.assertDictEqual(prs_obsr.substitute.callee_kwargs, {})
+        self.assertIs(prs_obsr.__annotations__, person.__annotations__)
+        self.assertIs(prs_obsr.__doc__, person.__doc__)
+        self.assertIs(prs_obsr.__name__, person.__name__)
 
-        # Basic calls deliver function defaults
+        # ---------------------------------------------------------------------
+        # Calls
         res.clear()
-        Person()
+        prs_obsr()
         self.assertListEqual(res, ["person says 'Hello?'"])
         res.clear()
-        Dog()
+        dog_obsl()
         self.assertListEqual(res, ["dog acts 'Brrr!'"])
 
-    def test_basics_nodecos_params(self):
-        """Unittest: Observable & Observer - nodecos, params"""
+    def test_nodecoration_params(self):
+        """Unittest: Functions: no decoration, parameters"""
 
         # Result list
         res = list()
 
         # Observable
         def dog(act1: str = "Brrr", act2: str = "!") -> None:
             """A dog function"""
@@ -195,66 +230,76 @@
 
         # Observer
         def person(say1: str = "Hello", say2: str = "?") -> None:
             """A person function"""
             res.append(f"{person.__name__} says '{say1}{say2}'")
 
         # ---------------------------------------------------------------------
-        # Test setup: Decoration
-        Dog = Observable(dog, 'Woof,', act2='Woof!')
-        Person = Observer(person, 'Ooops', say2='!')
+        # Test setup: Observable, only
+        dog_obsl = Observable(dog, 'Woof, ', act2='Woof!')
+
+        # Checks for dog_obsl
+        self.assertTrue(isinstance(dog_obsl, Observable))
+        self.assertIs(dog_obsl.BaseClass, BaseObservable)
+        self.assertTrue(isinstance(dog_obsl.observable, dog_obsl.BaseClass))
+        self.assertTrue(hasattr(dog_obsl.observable, 'register'))
+        self.assertTrue(hasattr(dog_obsl.observable, 'unregister'))
+        self.assertTrue(hasattr(dog_obsl.observable, 'dispatch'))
+        self.assertTrue(hasattr(dog_obsl.observable, 'observers'))
+        self.assertTupleEqual(dog_obsl.observable.args, ())
+        self.assertDictEqual(dog_obsl.observable.kwargs, {})
+        self.assertIs(dog_obsl.activate, Activation.AFTER)
+        self.assertListEqual(dog_obsl.methods, [])
+        self.assertIs(dog_obsl.substitute.callee, dog)
+        self.assertTupleEqual(dog_obsl.substitute.callee_args, ('Woof, ',))
+        self.assertDictEqual(dog_obsl.substitute.callee_kwargs,
+                             {'act2': 'Woof!'})
+        self.assertIs(dog_obsl.__annotations__, dog.__annotations__)
+        self.assertIs(dog_obsl.__doc__, dog.__doc__)
+        self.assertIs(dog_obsl.__name__, dog.__name__)
+
+        # ---------------------------------------------------------------------
+        # Calls
+        res.clear()
+        person()
+        self.assertListEqual(res, ["person says 'Hello?'"])
+        res.clear()
+        dog_obsl()
+        self.assertListEqual(res, ["dog acts 'Woof, Woof!'"])
+
+        # ---------------------------------------------------------------------
+        # Test setup: Observable & Observer
+        prs_obsr = Observer(person, 'Ooops', say2='!')
 
-        # Basic checks for Dog
-        self.assertTrue(isinstance(Dog, Observable))
-        self.assertIs(Dog.BaseClass, BaseObservable)
-        self.assertTrue(isinstance(Dog.observable, Dog.BaseClass))
-        self.assertTrue(hasattr(Dog.observable, 'register'))
-        self.assertTrue(hasattr(Dog.observable, 'unregister'))
-        self.assertTrue(hasattr(Dog.observable, 'dispatch'))
-        self.assertTrue(hasattr(Dog.observable, 'observers'))
-        self.assertTupleEqual(Dog.observable.args, ())
-        self.assertDictEqual(Dog.observable.kwargs, {})
-        self.assertIs(Dog.activate, Activation.AFTER)
-        self.assertFalse(hasattr(Dog, 'decorator_args'))
-        self.assertFalse(hasattr(Dog, 'decorator_kwargs'))
-        self.assertListEqual(Dog.methods, [])
-        self.assertIs(Dog.substitute.callee, dog)
-        self.assertTupleEqual(Dog.substitute.callee_args, ('Woof,',))
-        self.assertDictEqual(Dog.substitute.callee_kwargs, {'act2': 'Woof!'})
-        self.assertIs(Dog.__annotations__, dog.__annotations__)
-        self.assertIs(Dog.__doc__, dog.__doc__)
-        self.assertIs(Dog.__name__, dog.__name__)
-
-        # Basic checks for Person
-        self.assertTrue(isinstance(Person, Observer))
-        self.assertIs(Person.BaseClass, BaseObserver)
-        self.assertTrue(isinstance(Person.observer, Person.BaseClass))
-        self.assertTupleEqual(Person.observer.args, ())
-        self.assertDictEqual(Person.observer.kwargs, {})
-        self.assertFalse(hasattr(Person, 'decorator_args'))
-        self.assertFalse(hasattr(Person, 'decorator_kwargs'))
-        self.assertListEqual(Person.methods, [])
-        self.assertListEqual(Person.observables, [])
-        self.assertIs(Person.substitute.callee, person)
-        self.assertTupleEqual(Person.substitute.callee_args, ('Ooops',))
-        self.assertDictEqual(Person.substitute.callee_kwargs, {'say2': '!'})
-        self.assertIs(Person.__annotations__, person.__annotations__)
-        self.assertIs(Person.__doc__, person.__doc__)
-        self.assertIs(Person.__name__, person.__name__)
+        # Checks for prs_obsr
+        self.assertTrue(isinstance(prs_obsr, Observer))
+        self.assertIs(prs_obsr.BaseClass, BaseObserver)
+        self.assertTrue(isinstance(prs_obsr.observer, prs_obsr.BaseClass))
+        self.assertTupleEqual(prs_obsr.observer.args, ())
+        self.assertDictEqual(prs_obsr.observer.kwargs, {})
+        self.assertListEqual(prs_obsr.methods, [])
+        self.assertListEqual(prs_obsr.observables, [])
+        self.assertIs(prs_obsr.substitute.callee, person)
+        self.assertTupleEqual(prs_obsr.substitute.callee_args, ('Ooops',))
+        self.assertDictEqual(prs_obsr.substitute.callee_kwargs, {'say2': '!'})
+        self.assertIs(prs_obsr.__annotations__, person.__annotations__)
+        self.assertIs(prs_obsr.__doc__, person.__doc__)
+        self.assertIs(prs_obsr.__name__, person.__name__)
 
-        # Basic calls deliver decorator defaults
+        # ---------------------------------------------------------------------
+        # Calls
         res.clear()
-        Person()
+        prs_obsr()
         self.assertListEqual(res, ["person says 'Ooops!'"])
         res.clear()
-        Dog()
-        self.assertListEqual(res, ["dog acts 'Woof,Woof!'"])
+        dog_obsl()
+        self.assertListEqual(res, ["dog acts 'Woof, Woof!'"])
 
-    def test_basics_decos_noparams(self):
-        """Unittest: Observable & Observer - decos, noparams"""
+    def test_decoration_noparams(self):
+        """Unittest: Functions: decoration, no parameters"""
 
         # Result list
         res = list()
 
         # Observable
         def dog(act: str = "Brrr!") -> None:
             """A dog function"""
@@ -262,66 +307,74 @@
 
         # Observer
         def person(say: str = "Hello?") -> None:
             """A person function"""
             res.append(f"{person.__name__} says '{say}'")
 
         # ---------------------------------------------------------------------
-        # Test setup: Decoration
-        Dog = Observable(None, 'deco_arg', kw='deco_kwarg')(dog)
-        Person = Observer(None, 'deco_arg', kw='deco_kwarg')(person)
+        # Test setup: Observable, only
+        dog_obsl = Observable(None, 'deco_arg', kw='deco_kwarg')(dog)
+
+        # Checks for dog_obsl
+        self.assertTrue(isinstance(dog_obsl, Observable))
+        self.assertIs(dog_obsl.BaseClass, BaseObservable)
+        self.assertTrue(isinstance(dog_obsl.observable, dog_obsl.BaseClass))
+        self.assertTrue(hasattr(dog_obsl.observable, 'register'))
+        self.assertTrue(hasattr(dog_obsl.observable, 'unregister'))
+        self.assertTrue(hasattr(dog_obsl.observable, 'dispatch'))
+        self.assertTrue(hasattr(dog_obsl.observable, 'observers'))
+        self.assertTupleEqual(dog_obsl.observable.args, ('deco_arg',))
+        self.assertDictEqual(dog_obsl.observable.kwargs, {'kw': 'deco_kwarg'})
+        self.assertIs(dog_obsl.activate, Activation.AFTER)
+        self.assertListEqual(dog_obsl.methods, [])
+        self.assertIs(dog_obsl.substitute.callee, dog)
+        self.assertTupleEqual(dog_obsl.substitute.callee_args, ())
+        self.assertDictEqual(dog_obsl.substitute.callee_kwargs, {})
+        self.assertIs(dog_obsl.__annotations__, dog.__annotations__)
+        self.assertIs(dog_obsl.__doc__, dog.__doc__)
+        self.assertIs(dog_obsl.__name__, dog.__name__)
+
+        # Calls
+        res.clear()
+        person()
+        self.assertListEqual(res, ["person says 'Hello?'"])
+        res.clear()
+        dog_obsl()
+        self.assertListEqual(res, ["dog acts 'Brrr!'"])
+
+        # ---------------------------------------------------------------------
+        # Test setup: Observable & Observer
+        prs_obsr = Observer(None, 'deco_arg', kw='deco_kwarg')(person)
 
-        # Basic checks for Dog
-        self.assertTrue(isinstance(Dog, Observable))
-        self.assertIs(Dog.BaseClass, BaseObservable)
-        self.assertTrue(isinstance(Dog.observable, Dog.BaseClass))
-        self.assertTrue(hasattr(Dog.observable, 'register'))
-        self.assertTrue(hasattr(Dog.observable, 'unregister'))
-        self.assertTrue(hasattr(Dog.observable, 'dispatch'))
-        self.assertTrue(hasattr(Dog.observable, 'observers'))
-        self.assertTupleEqual(Dog.observable.args, ('deco_arg',))
-        self.assertDictEqual(Dog.observable.kwargs, {'kw': 'deco_kwarg'})
-        self.assertIs(Dog.activate, Activation.AFTER)
-        self.assertTupleEqual(Dog.decorator_args, ('deco_arg',))
-        self.assertDictEqual(Dog.decorator_kwargs, {'kw': 'deco_kwarg'})
-        self.assertListEqual(Dog.methods, [])
-        self.assertIs(Dog.substitute.callee, dog)
-        self.assertTupleEqual(Dog.substitute.callee_args, ())
-        self.assertDictEqual(Dog.substitute.callee_kwargs, {})
-        self.assertIs(Dog.__annotations__, dog.__annotations__)
-        self.assertIs(Dog.__doc__, dog.__doc__)
-        self.assertIs(Dog.__name__, dog.__name__)
-
-        # Basic checks for Person
-        self.assertTrue(isinstance(Person, Observer))
-        self.assertIs(Person.BaseClass, BaseObserver)
-        self.assertTrue(isinstance(Person.observer, Person.BaseClass))
-        self.assertTupleEqual(Person.observer.args, ('deco_arg',))
-        self.assertDictEqual(Person.observer.kwargs, {'kw': 'deco_kwarg'})
-        self.assertTupleEqual(Person.decorator_args, ('deco_arg',))
-        self.assertDictEqual(Person.decorator_kwargs, {'kw': 'deco_kwarg'})
-        self.assertListEqual(Person.methods, [])
-        self.assertListEqual(Person.observables, [])
-        self.assertIs(Person.substitute.callee, person)
-        self.assertTupleEqual(Person.substitute.callee_args, ())
-        self.assertDictEqual(Person.substitute.callee_kwargs, {})
-        self.assertIs(Person.__annotations__, person.__annotations__)
-        self.assertIs(Person.__doc__, person.__doc__)
-        self.assertIs(Person.__name__, person.__name__)
+        # Checks for prs_obsr
+        self.assertTrue(isinstance(prs_obsr, Observer))
+        self.assertIs(prs_obsr.BaseClass, BaseObserver)
+        self.assertTrue(isinstance(prs_obsr.observer, prs_obsr.BaseClass))
+        self.assertTupleEqual(prs_obsr.observer.args, ('deco_arg',))
+        self.assertDictEqual(prs_obsr.observer.kwargs, {'kw': 'deco_kwarg'})
+        self.assertListEqual(prs_obsr.methods, [])
+        self.assertListEqual(prs_obsr.observables, [])
+        self.assertIs(prs_obsr.substitute.callee, person)
+        self.assertTupleEqual(prs_obsr.substitute.callee_args, ())
+        self.assertDictEqual(prs_obsr.substitute.callee_kwargs, {})
+        self.assertIs(prs_obsr.__annotations__, person.__annotations__)
+        self.assertIs(prs_obsr.__doc__, person.__doc__)
+        self.assertIs(prs_obsr.__name__, person.__name__)
 
-        # Basic calls deliver function defaults
+        # ---------------------------------------------------------------------
+        # Calls
         res.clear()
-        Person()
+        prs_obsr()
         self.assertListEqual(res, ["person says 'Hello?'"])
         res.clear()
-        Dog()
+        dog_obsl()
         self.assertListEqual(res, ["dog acts 'Brrr!'"])
 
-    def test_basics_decos_params(self):
-        """Unittest: Observable & Observer - decos, params"""
+    def test_decoration_params(self):
+        """Unittest: Functions: decoration, parameters"""
 
         # Result list
         res = list()
 
         # Observable
         def dog(act1: str = "Brrr", act2: str = "!") -> None:
             """A dog function"""
@@ -329,69 +382,78 @@
 
         # Observer
         def person(say1: str = "Hello", say2: str = "?") -> None:
             """A person function"""
             res.append(f"{person.__name__} says '{say1}{say2}'")
 
         # ---------------------------------------------------------------------
-        # Test setup: Decoration
-        Dog = Observable(None, 'deco_arg', kw='deco_kwarg')(
-            dog, 'Woof,', act2='Woof!')
-        Person = Observer(None, 'deco_arg', kw='deco_kwarg')(
+        # Test setup: Observable, only
+        dog_obsl = Observable(None, 'deco_arg', kw='deco_kwarg')(
+            dog, 'Woof, ', act2='Woof!')
+
+        # Checks for dog_obsl
+        self.assertTrue(isinstance(dog_obsl, Observable))
+        self.assertIs(dog_obsl.BaseClass, BaseObservable)
+        self.assertTrue(isinstance(dog_obsl.observable, dog_obsl.BaseClass))
+        self.assertTrue(hasattr(dog_obsl.observable, 'register'))
+        self.assertTrue(hasattr(dog_obsl.observable, 'unregister'))
+        self.assertTrue(hasattr(dog_obsl.observable, 'dispatch'))
+        self.assertTrue(hasattr(dog_obsl.observable, 'observers'))
+        self.assertTupleEqual(dog_obsl.observable.args, ('deco_arg',))
+        self.assertDictEqual(dog_obsl.observable.kwargs, {'kw': 'deco_kwarg'})
+        self.assertIs(dog_obsl.activate, Activation.AFTER)
+        self.assertListEqual(dog_obsl.methods, [])
+        self.assertIs(dog_obsl.substitute.callee, dog)
+        self.assertTupleEqual(dog_obsl.substitute.callee_args, ('Woof, ',))
+        self.assertDictEqual(dog_obsl.substitute.callee_kwargs,
+                             {'act2': 'Woof!'})
+        self.assertIs(dog_obsl.__annotations__, dog.__annotations__)
+        self.assertIs(dog_obsl.__doc__, dog.__doc__)
+        self.assertIs(dog_obsl.__name__, dog.__name__)
+
+        # ---------------------------------------------------------------------
+        # Calls
+        res.clear()
+        person()
+        self.assertListEqual(res, ["person says 'Hello?'"])
+        res.clear()
+        dog_obsl()
+        self.assertListEqual(res, ["dog acts 'Woof, Woof!'"])
+
+        # ---------------------------------------------------------------------
+        # Test setup: Observable & Observer
+        prs_obsr = Observer(None, 'deco_arg', kw='deco_kwarg')(
             person, 'Ooops', say2='!')
 
-        # Basic checks for Dog
-        self.assertTrue(isinstance(Dog, Observable))
-        self.assertIs(Dog.BaseClass, BaseObservable)
-        self.assertTrue(isinstance(Dog.observable, Dog.BaseClass))
-        self.assertTrue(hasattr(Dog.observable, 'register'))
-        self.assertTrue(hasattr(Dog.observable, 'unregister'))
-        self.assertTrue(hasattr(Dog.observable, 'dispatch'))
-        self.assertTrue(hasattr(Dog.observable, 'observers'))
-        self.assertTupleEqual(Dog.observable.args, ('deco_arg',))
-        self.assertDictEqual(Dog.observable.kwargs, {'kw': 'deco_kwarg'})
-        self.assertIs(Dog.activate, Activation.AFTER)
-        self.assertTupleEqual(Dog.decorator_args, ('deco_arg',))
-        self.assertDictEqual(Dog.decorator_kwargs, {'kw': 'deco_kwarg'})
-        self.assertListEqual(Dog.methods, [])
-        self.assertIs(Dog.substitute.callee, dog)
-        self.assertTupleEqual(Dog.substitute.callee_args, ('Woof,',))
-        self.assertDictEqual(Dog.substitute.callee_kwargs, {'act2': 'Woof!'})
-        self.assertIs(Dog.__annotations__, dog.__annotations__)
-        self.assertIs(Dog.__doc__, dog.__doc__)
-        self.assertIs(Dog.__name__, dog.__name__)
-
-        # Basic checks for Person
-        self.assertTrue(isinstance(Person, Observer))
-        self.assertIs(Person.BaseClass, BaseObserver)
-        self.assertTrue(isinstance(Person.observer, Person.BaseClass))
-        self.assertTupleEqual(Person.observer.args, ('deco_arg',))
-        self.assertDictEqual(Person.observer.kwargs, {'kw': 'deco_kwarg'})
-        self.assertTupleEqual(Person.decorator_args, ('deco_arg',))
-        self.assertDictEqual(Person.decorator_kwargs, {'kw': 'deco_kwarg'})
-        self.assertListEqual(Person.methods, [])
-        self.assertListEqual(Person.observables, [])
-        self.assertIs(Person.substitute.callee, person)
-        self.assertTupleEqual(Person.substitute.callee_args, ('Ooops',))
-        self.assertDictEqual(Person.substitute.callee_kwargs, {'say2': '!'})
-        self.assertIs(Person.__annotations__, person.__annotations__)
-        self.assertIs(Person.__doc__, person.__doc__)
-        self.assertIs(Person.__name__, person.__name__)
+        # Checks for prs_obsr
+        self.assertTrue(isinstance(prs_obsr, Observer))
+        self.assertIs(prs_obsr.BaseClass, BaseObserver)
+        self.assertTrue(isinstance(prs_obsr.observer, prs_obsr.BaseClass))
+        self.assertTupleEqual(prs_obsr.observer.args, ('deco_arg',))
+        self.assertDictEqual(prs_obsr.observer.kwargs, {'kw': 'deco_kwarg'})
+        self.assertListEqual(prs_obsr.methods, [])
+        self.assertListEqual(prs_obsr.observables, [])
+        self.assertIs(prs_obsr.substitute.callee, person)
+        self.assertTupleEqual(prs_obsr.substitute.callee_args, ('Ooops',))
+        self.assertDictEqual(prs_obsr.substitute.callee_kwargs, {'say2': '!'})
+        self.assertIs(prs_obsr.__annotations__, person.__annotations__)
+        self.assertIs(prs_obsr.__doc__, person.__doc__)
+        self.assertIs(prs_obsr.__name__, person.__name__)
 
-        # Basic calls deliver decorator defaults
+        # ---------------------------------------------------------------------
+        # Calls
         res.clear()
-        Person()
+        prs_obsr()
         self.assertListEqual(res, ["person says 'Ooops!'"])
-
         res.clear()
-        Dog()
-        self.assertListEqual(res, ["dog acts 'Woof,Woof!'"])
+        dog_obsl()
+        self.assertListEqual(res, ["dog acts 'Woof, Woof!'"])
 
-    def test_basics_observable_activation(self):
-        """Unittest: Observable & Observer - Activation"""
+    def test_observable_activation(self):
+        """Unittest: Functions: Activation"""
 
         # Result list
         res = list()
 
         # Observable
         def dog(act: str = "Brrr!") -> None:
             """A dog function"""
@@ -414,78 +476,61 @@
         self.assertNotEqual(Activation.AFTER, Activation.BEFORE_AND_AFTER)
 
         self.assertEqual(Activation.BEFORE_AND_AFTER,
                          Activation.BEFORE | Activation.AFTER)
 
         # ---------------------------------------------------------------------
         # Decoration
-        Dog = Observable(dog)
-        Person = Observer(observables=Dog)(person)
+        dog_obsl = Observable(dog)
+        prs_obsr = Observer(observables=dog_obsl)(person)
 
         # Person says default
         res.clear()
-        Person()
+        prs_obsr()
         self.assertListEqual(res, ["person says 'Hello?'"])
 
         # ---------------------------------------------------------------------
 
         # Default activation is AFTER
-        self.assertIs(Dog.activate, Activation.AFTER)
+        self.assertIs(dog_obsl.activate, Activation.AFTER)
 
         # Activation: NONE
-        Dog.activate = Activation.NONE
+        dog_obsl.activate = Activation.NONE
         res.clear()
-        Dog()
+        dog_obsl()
         self.assertListEqual(res, ["dog acts 'Brrr!'"])
 
         # Activation: BEFORE
-        Dog.activate = Activation.BEFORE
+        dog_obsl.activate = Activation.BEFORE
         res.clear()
-        Dog()
+        dog_obsl()
         self.assertListEqual(res, ["person says 'Hello?'",
                                    "dog acts 'Brrr!'"])
 
         # Activation: AFTER
-        Dog.activate = Activation.AFTER
+        dog_obsl.activate = Activation.AFTER
         res.clear()
-        Dog()
+        dog_obsl()
         self.assertListEqual(res, ["dog acts 'Brrr!'",
                                    "person says 'Hello?'"])
 
         # Activation: BEFORE & AFTER
-        Dog.activate = Activation.BEFORE_AND_AFTER
+        dog_obsl.activate = Activation.BEFORE_AND_AFTER
         res.clear()
-        Dog()
+        dog_obsl()
         self.assertListEqual(res, ["person says 'Hello?'",
                                    "dog acts 'Brrr!'",
                                    "person says 'Hello?'"])
 
     def test_observable_functions(self):
-        """Unittest: Observable & Observer - Functions"""
+        """Unittest: Functions: Interface register, unregister, dispatch"""
 
         # Result list
         res = list()
 
-        # Helper
-        def cmp(iter1, iter2):
-            """Compare *all* elements of F with a tuple"""
-            if len(iter1) != len(iter2):
-                return False
-            else:
-                iter1 = list(iter1)
-                iter2 = list(iter2)
-                iter1.sort()
-                iter2.sort()
-                for left, right in zip(iter1, iter2):
-                    if left.callee != right.callee or \
-                            left.callee_args != right.callee_args or \
-                            left.callee_kwargs != right.callee_kwargs:
-                        return False
-                return True
-
         # Observable
         def dog(act: str = "Woof!") -> None:
             """A dog function"""
             res.append(f"{dog.__name__} acts '{act}'")
 
         # Observer
         def person(say: str = "Hello?") -> None:
@@ -592,493 +637,394 @@
             self.assertListEqual(res, ["person says 'What's up?'",
                                        "dog acts 'Brrr!'",
                                        "person says 'What's up?'"])
 
             Dog.activate = Activation.AFTER
 
         # ---------------------------------------------------------------------
-        # Test: Decoration via Observer
-        Dog = Observable(dog)
-        Person = Observer(observables=X(Dog, say="What's up?"))(person)
-        test(Person, Dog)
+        # Test: Decoration via Observable
+        prs_obsr = Observer(person)
+        dog_obsl = Observable(observers=F(prs_obsr, say="What's up?"))(dog)
+        test(prs_obsr, dog_obsl)
 
         # ---------------------------------------------------------------------
-        # Test: Decoration via Observable
-        Person = Observer(person)
-        Dog = Observable(observers=F(Person, say="What's up?"))(dog)
-        test(Person, Dog)
+        # Test: Decoration via Observer
+        dog_obsl = Observable(dog)
+        prs_obsr = Observer(observables=X(dog_obsl, say="What's up?"))(person)
+        test(prs_obsr, dog_obsl)
 
     def test_observable_class_init(self):
-        """Unittest: Observable & Observer - class init"""
+        """Unittest: Class: init()"""
 
         # Result list
         res = list()
 
         # Observable
-        class dog:
+        class Dog:
             """A Dog Type"""
 
             def __init__(self, name: str = "DOG"):
                 self.name = name
                 res.append(f"{self.name} acts 'INIT'")
 
             def untouched(self):
                 """Untouched by decoration"""
                 res.append(f"{self.name} is untouched")
 
         # Observer
-        class person:
+        class Person:
             """A Person Type"""
 
             def __init__(self, name: str = "PERSON"):
                 self.name = name
                 res.append(f"{self.name} says 'INIT'")
 
             def untouched(self):
                 """Untouched by decoration"""
                 res.append(f"{self.name} is untouched")
 
         # ---------------------------------------------------------------------
         # Test setup: Decoration
-        Person = Observer(person)
-        Dog = Observable(observers=Person)(dog)
+        Prs_obsr = Observer(Person)
+        Dog_obsl = Observable(observers=Prs_obsr)(Dog)
 
         # Person registered as an observer of dog by decorations above
-        self.assertDictEqual(Dog.observable.observers(),
-                             {F(Person): F(Person)})
+        self.assertDictEqual(Dog_obsl.observable.observers(),
+                             {F(Prs_obsr): F(Prs_obsr)})
 
         # Init a Person
         res.clear()
-        p = Person()
+        p = Prs_obsr()
         self.assertListEqual(res, ["PERSON says 'INIT'"])
 
         # Init a Dog with Person as an observer
         res.clear()
-        d = Dog()
+        d = Dog_obsl()
         self.assertListEqual(res, ["DOG acts 'INIT'", "PERSON says 'INIT'"])
 
         # The untouchables
         res.clear()
         p.untouched()
         self.assertEqual(res, ['PERSON is untouched'])
         res.clear()
         d.untouched()
         self.assertEqual(res, ['DOG is untouched'])
 
     def test_observable_class_staticmethod01(self):
-        """Unittest: Observable & Observer - static methods"""
+        """Unittest: Class: staticmethod()"""
 
         # Result list
         res = list()
 
-        # Helper
-        def cmp(iter1, iter2):
-            """Compare *all* elements of F with a tuple"""
-            if len(iter1) != len(iter2):
-                return False
-            else:
-                iter1 = list(iter1)
-                iter2 = list(iter2)
-                iter1.sort()
-                iter2.sort()
-                for left, right in zip(iter1, iter2):
-                    if left.callee != right.callee or \
-                            left.callee_args != right.callee_args or \
-                            left.callee_kwargs != right.callee_kwargs:
-                        return False
-                return True
-
         # Observable
-        class dog:
+        class Dog:
             """A Dog Type"""
 
             @staticmethod
             def static_method(act: str = 'Woof!'):
                 """To be decorated"""
-                res.append(f"dog act '{act}'")
+                res.append(f"Dog act '{act}'")
 
             @staticmethod
             def static_untouched():
                 """Untouched by decoration"""
-                res.append(f"dog is untouched")
+                res.append(f"Dog is untouched")
 
         # Observer
-        class person:
+        class Person:
             """A Person Type"""
 
             @staticmethod
             def static_method(say: str = 'Hello?'):
                 """To be decorated"""
-                res.append(f"person say '{say}'")
+                res.append(f"Person say '{say}'")
 
             @staticmethod
             def static_untouched():
                 """Untouched by decoration"""
-                res.append(f"person is untouched")
+                res.append(f"Person is untouched")
 
         # ---------------------------------------------------------------------
         # Test: function decoration
-        person.static_method = Observer(person.static_method)
-        dog.static_method = Observable(
-            observers=F(person.static_method, say="What's up?"))(
-            dog.static_method)
+        Person.static_method = Observer(Person.static_method)
+        Dog.static_method = Observable(
+            observers=F(Person.static_method, say="What's up?"))(
+            Dog.static_method)
 
         # Person registered as an observer of dog by decorations above
-        self.assertTrue(cmp(dog.static_method.observable.observers().values(),
-                            {F(person.static_method, say="What's up?")}))
+        self.assertTrue(cmp(Dog.static_method.observable.observers().values(),
+                            {F(Person.static_method, say="What's up?")}))
 
         # Person
         res.clear()
-        person.static_method()
-        self.assertListEqual(res, ["person say 'Hello?'"])
+        Person.static_method()
+        self.assertListEqual(res, ["Person say 'Hello?'"])
 
         # Dog with Person as an observer
         res.clear()
-        dog.static_method()
-        self.assertListEqual(res, ["dog act 'Woof!'",
-                                   "person say 'What's up?'"])
+        Dog.static_method()
+        self.assertListEqual(res, ["Dog act 'Woof!'",
+                                   "Person say 'What's up?'"])
 
         # The untouchables
         res.clear()
-        person.static_untouched()
-        self.assertEqual(res, ['person is untouched'])
+        Person.static_untouched()
+        self.assertEqual(res, ['Person is untouched'])
         res.clear()
-        dog.static_untouched()
-        self.assertEqual(res, ['dog is untouched'])
+        Dog.static_untouched()
+        self.assertEqual(res, ['Dog is untouched'])
 
     def test_observable_class_staticmethod02(self):
-        """Unittest: Observable & Observer - static methods"""
+        """Unittest: Class: staticmethod()"""
 
         # Result list
         res = list()
 
-        # Helper
-        def cmp(iter1, iter2):
-            """Compare *all* elements of F with a tuple"""
-            if len(iter1) != len(iter2):
-                return False
-            else:
-                iter1 = list(iter1)
-                iter2 = list(iter2)
-                iter1.sort()
-                iter2.sort()
-                for left, right in zip(iter1, iter2):
-                    if left.callee != right.callee or \
-                            left.callee_args != right.callee_args or \
-                            left.callee_kwargs != right.callee_kwargs:
-                        return False
-                return True
-
         # Observable
-        class dog:
+        class Dog:
             """A Dog Type"""
 
             @staticmethod
             def static_method(act: str = 'Woof!'):
                 """To be decorated"""
-                res.append(f"dog act '{act}'")
+                res.append(f"Dog act '{act}'")
 
             @staticmethod
             def static_untouched():
                 """Untouched by decoration"""
-                res.append(f"dog is untouched")
+                res.append(f"Dog is untouched")
 
         # Observer
-        class person:
+        class Person:
             """A Person Type"""
 
             @staticmethod
             def static_method(say: str = 'Hello?'):
                 """To be decorated"""
-                res.append(f"person say '{say}'")
+                res.append(f"Person say '{say}'")
 
             @staticmethod
             def static_untouched():
                 """Untouched by decoration"""
-                res.append(f"person is untouched")
+                res.append(f"Person is untouched")
 
         # ---------------------------------------------------------------------
         # Test: class decoration
-        Person = Observer(methods=person.static_method)(person)
+        Person = Observer(methods=Person.static_method)(Person)
         Dog = Observable(observers=F(Person.static_method, say="What's up?"),
-                         methods=dog.static_method)(dog)
+                         methods=Dog.static_method)(Dog)
 
         # Person registered as an observer of dog by decorations above
         self.assertTrue(cmp(Dog.static_method.observable.observers().values(),
                             {F(Person.static_method, say="What's up?")}))
 
         # Person
         res.clear()
         Person.static_method()
-        self.assertListEqual(res, ["person say 'Hello?'"])
+        self.assertListEqual(res, ["Person say 'Hello?'"])
 
         # Dog with Person as an observer
         res.clear()
         Dog.static_method()
-        self.assertListEqual(res, ["dog act 'Woof!'",
-                                   "person say 'What's up?'"])
+        self.assertListEqual(res, ["Dog act 'Woof!'",
+                                   "Person say 'What's up?'"])
 
         # The untouchables
         res.clear()
-        person.static_untouched()
-        self.assertEqual(res, ['person is untouched'])
+        Person.static_untouched()
+        self.assertEqual(res, ['Person is untouched'])
         res.clear()
-        dog.static_untouched()
-        self.assertEqual(res, ['dog is untouched'])
+        Dog.static_untouched()
+        self.assertEqual(res, ['Dog is untouched'])
 
     def test_observable_class_classmethod01(self):
-        """Unittest: Observable & Observer - class methods"""
+        """Unittest: Class: classmethod()"""
 
         # Result list
         res = list()
 
-        # Helper
-        def cmp(iter1, iter2):
-            """Compare *all* elements of F with a tuple"""
-            if len(iter1) != len(iter2):
-                return False
-            else:
-                iter1 = list(iter1)
-                iter2 = list(iter2)
-                iter1.sort()
-                iter2.sort()
-                for left, right in zip(iter1, iter2):
-                    if left.callee != right.callee or \
-                            left.callee_args != right.callee_args or \
-                            left.callee_kwargs != right.callee_kwargs:
-                        return False
-                return True
-
         # Observable
-        class dog:
+        class Dog:
             """A Dog Type"""
 
             @classmethod
             def class_method(cls, act: str = 'Woof!'):
                 """A classmethod"""
                 res.append(f"{cls.__name__} act '{act}'")
 
         # Observer
-        class person:
+        class Person:
             """A Person Type"""
 
             @classmethod
             def class_method(cls, say: str = 'Hello?'):
                 """A classmethod"""
                 res.append(f"{cls.__name__} say '{say}'")
 
         # ---------------------------------------------------------------------
         # Test: function decoration
-        person.class_method = Observer(person.class_method)
-        dog.class_method = Observable(
-            observers=F(person.class_method, say="What's up?"))(
-            dog.class_method)
+        Person.class_method = Observer(Person.class_method)
+        Dog.class_method = Observable(
+            observers=F(Person.class_method, say="What's up?"))(
+            Dog.class_method)
 
         # Person registered as an observer of dog by decorations above
-        self.assertTrue(cmp(dog.class_method.observable.observers().values(),
-                            {F(person.class_method, say="What's up?")}))
+        self.assertTrue(cmp(Dog.class_method.observable.observers().values(),
+                            {F(Person.class_method, say="What's up?")}))
 
         # Person
         res.clear()
-        person.class_method()
-        self.assertListEqual(res, ["person say 'Hello?'"])
+        Person.class_method()
+        self.assertListEqual(res, ["Person say 'Hello?'"])
 
         # Dog with Person as an observer
         res.clear()
-        dog.class_method()
-        self.assertListEqual(res, ["dog act 'Woof!'",
-                                   "person say 'What's up?'"])
+        Dog.class_method()
+        self.assertListEqual(res, ["Dog act 'Woof!'",
+                                   "Person say 'What's up?'"])
 
     def test_observable_class_classmethod02(self):
-        """Unittest: Observable & Observer - class methods"""
+        """Unittest: Class: classmethod()"""
 
         # Result list
         res = list()
 
-        # Helper
-        def cmp(iter1, iter2):
-            """Compare *all* elements of F with a tuple"""
-            if len(iter1) != len(iter2):
-                return False
-            else:
-                iter1 = list(iter1)
-                iter2 = list(iter2)
-                iter1.sort()
-                iter2.sort()
-                for left, right in zip(iter1, iter2):
-                    if left.callee != right.callee or \
-                            left.callee_args != right.callee_args or \
-                            left.callee_kwargs != right.callee_kwargs:
-                        return False
-                return True
-
         # Observable
-        class dog:
+        class Dog:
             """A Dog Type"""
 
             @classmethod
             def class_method(cls, act: str = 'Woof!'):
                 """A classmethod"""
                 res.append(f"{cls.__name__} act '{act}'")
 
         # Observer
-        class person:
+        class Person:
             """A Person Type"""
 
             @classmethod
             def class_method(cls, say: str = 'Hello?'):
                 """A classmethod"""
                 res.append(f"{cls.__name__} say '{say}'")
 
         # ---------------------------------------------------------------------
         # Test: class decoration
-        Person = Observer(methods=person.class_method)(person)
+        Person = Observer(methods=Person.class_method)(Person)
         Dog = Observable(observers=F(Person.class_method, say="What's up?"),
-                         methods=dog.class_method)(dog)
+                         methods=Dog.class_method)(Dog)
 
         # Person registered as an observer of dog by decorations above
         self.assertTrue(cmp(Dog.class_method.observable.observers().values(),
                             {F(Person.class_method, say="What's up?")}))
 
         # Person
         res.clear()
         Person.class_method()
-        self.assertListEqual(res, ["person say 'Hello?'"])
+        self.assertListEqual(res, ["Person say 'Hello?'"])
 
         # Dog with Person as an observer
         res.clear()
         Dog.class_method()
-        self.assertListEqual(res, ["dog act 'Woof!'",
-                                   "person say 'What's up?'"])
+        self.assertListEqual(res, ["Dog act 'Woof!'",
+                                   "Person say 'What's up?'"])
 
     def test_observable_class_objectmethod01(self):
-        """Unittest: Observable & Observer - object methods"""
+        """Unittest: Class: object method()"""
 
         # Result list
         res = list()
 
-        # Helper
-        def cmp(iter1, iter2):
-            """Compare *all* elements of F with a tuple"""
-            if len(iter1) != len(iter2):
-                return False
-            else:
-                iter1 = list(iter1)
-                iter2 = list(iter2)
-                iter1.sort()
-                iter2.sort()
-                for left, right in zip(iter1, iter2):
-                    if left.callee != right.callee or \
-                            left.callee_args != right.callee_args or \
-                            left.callee_kwargs != right.callee_kwargs:
-                        return False
-                return True
-
         # Observable
-        class dog:
+        class Dog:
             """A Dog Type"""
 
             def object_method(self, act: str = 'Woof!'):
                 """An objectmethod"""
                 res.append(f"{self.__class__.__name__} act '{act}'")
 
         # Observer
-        class person:
+        class Person:
             """A Person Type"""
 
             def object_method(self, say: str = 'Hello?'):
                 """An objectmethod"""
                 res.append(f"{self.__class__.__name__} say '{say}'")
 
         # ---------------------------------------------------------------------
         # Test: function decoration
-        Person = person()
-        Dog = dog()
+        Per_obsr = Person()
+        Dog_obsl = Dog()
 
-        Person.object_method = Observer(Person.object_method)
-        Dog.object_method = Observable(
-            observers=F(Person.object_method, say="What's up?"))(
-            Dog.object_method)
+        Per_obsr.object_method = Observer(Per_obsr.object_method)
+        Dog_obsl.object_method = Observable(
+            observers=F(Per_obsr.object_method, say="What's up?"))(
+            Dog_obsl.object_method)
 
         # Person registered as an observer of dog by decorations above
-        self.assertTrue(cmp(Dog.object_method.observable.observers().values(),
-                            {F(Person.object_method, say="What's up?")}))
+        self.assertTrue(
+            cmp(Dog_obsl.object_method.observable.observers().values(),
+                {F(Per_obsr.object_method, say="What's up?")}))
 
         # Person
         res.clear()
-        Person.object_method()
-        self.assertListEqual(res, ["person say 'Hello?'"])
+        Per_obsr.object_method()
+        self.assertListEqual(res, ["Person say 'Hello?'"])
 
         # Dog with Person as an observer
         res.clear()
-        Dog.object_method()
-        self.assertListEqual(res, ["dog act 'Woof!'",
-                                   "person say 'What's up?'"])
+        Dog_obsl.object_method()
+        self.assertListEqual(res, ["Dog act 'Woof!'",
+                                   "Person say 'What's up?'"])
 
     def test_observable_class_objectmethod02(self):
-        """Unittest: Observable & Observer - object methods"""
+        """Unittest: Class: object method()"""
 
         # Result list
         res = list()
 
-        # Helper
-        def cmp(iter1, iter2):
-            """Compare *all* elements of F with a tuple"""
-            if len(iter1) != len(iter2):
-                return False
-            else:
-                iter1 = list(iter1)
-                iter2 = list(iter2)
-                iter1.sort()
-                iter2.sort()
-                for left, right in zip(iter1, iter2):
-                    if left.callee != right.callee or \
-                            left.callee_args != right.callee_args or \
-                            left.callee_kwargs != right.callee_kwargs:
-                        return False
-                return True
-
         # Observable
-        class dog:
+        class Dog:
             """A Dog Type"""
 
             def object_method(self, act: str = 'Woof!'):
                 """An objectmethod"""
                 res.append(f"{self.__class__.__name__} act '{act}'")
 
         # Observer
-        class person:
+        class Person:
             """A Person Type"""
 
             def object_method(self, say: str = 'Hello?'):
                 """An objectmethod"""
                 res.append(f"{self.__class__.__name__} say '{say}'")
 
         # ---------------------------------------------------------------------
         # Test: object decoration
-        Person = person()
-        Dog = dog()
+        Per_obsr = Person()
+        Dog_obsl = Dog()
 
-        Person = Observer(methods=X('object_method'))(Person)
-        Dog = Observable(observers=F(Person.object_method, say="What's up?"),
-                         methods=F('object_method'))(Dog)
+        Per_obsr = Observer(methods=X('object_method'))(Per_obsr)
+        Dog_obsl = Observable(
+            observers=F(Per_obsr.object_method, say="What's up?"),
+            methods=F('object_method'))(Dog_obsl)
 
         # Person registered as an observer of dog by decorations above
-        self.assertTrue(cmp(Dog.object_method.observable.observers().values(),
-                            {F(Person.object_method, say="What's up?")}))
+        self.assertTrue(
+            cmp(Dog_obsl.object_method.observable.observers().values(),
+                {F(Per_obsr.object_method, say="What's up?")}))
 
         # Person
         res.clear()
-        Person.object_method()
-        self.assertListEqual(res, ["person say 'Hello?'"])
+        Per_obsr.object_method()
+        self.assertListEqual(res, ["Person say 'Hello?'"])
 
         # Dog with Person as an observer
         res.clear()
-        Dog.object_method()
-        self.assertListEqual(res, ["dog act 'Woof!'",
-                                   "person say 'What's up?'"])
+        Dog_obsl.object_method()
+        self.assertListEqual(res, ["Dog act 'Woof!'",
+                                   "Person say 'What's up?'"])
 
 
 # -----------------------------------------------------------------------------
 # Execution
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `decoratory-0.1.2.3/Unittest/test_singleton.py` & `decoratory-0.1.3.11/Unittest/test_singleton.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.2.6"
-__date__ = "2023-06-18"
-__time__ = "15:26:25"
+__version__ = "0.1.3.8"
+__date__ = "2023-06-19"
+__time__ = "17:55:21"
 __state__ = "Beta"
 __license__ = "PSF"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
```

### Comparing `decoratory-0.1.2.3/Unittest/test_wrapper.py` & `decoratory-0.1.3.11/Unittest/test_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,25 +13,26 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.2.4"
-__date__ = "2023-06-18"
-__time__ = "13:03:35"
+__version__ = "0.1.3.7"
+__date__ = "2023-06-19"
+__time__ = "18:25:39"
 __state__ = "Beta"
 __license__ = "PSF"
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
 import unittest
 
-from decoratory.wrapper import Wrapper, F
+from decoratory.wrapper import Wrapper
+from decoratory.basic import F
 
 
 # -----------------------------------------------------------------------------
 # Test Class
 # noinspection PyPep8Naming
 class TestWrapper(unittest.TestCase):
```

### Comparing `decoratory-0.1.2.3/setup.py` & `decoratory-0.1.3.11/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.2.3"
-__date__ = "2023-06-18"
-__time__ = "19:22:40"
+__version__ = "0.1.3.11"
+__date__ = "2023-06-19"
+__time__ = "18:30:22"
 __state__ = "Beta"
 __license__ = "PSF"
 
 # -----------------------------------------------------------------------------
 # Libraries
 from os.path import join
 from setuptools import setup, find_packages
```

