# Comparing `tmp/Signal8-3.8.tar.gz` & `tmp/Signal8-3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-3.8.tar", last modified: Wed Jun 14 03:35:13 2023, max compression
+gzip compressed data, was "Signal8-3.9.tar", last modified: Mon Jun 19 21:14:32 2023, max compression
```

## Comparing `Signal8-3.8.tar` & `Signal8-3.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 03:35:13.658821 Signal8-3.8/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-3.8/LICENSE
--rw-rw-rw-   0        0        0     5356 2023-06-14 03:35:13.656821 Signal8-3.8/PKG-INFO
--rw-rw-rw-   0        0        0     4858 2023-06-12 22:34:01.000000 Signal8-3.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 03:35:13.423773 Signal8-3.8/Signal8/
--rw-rw-rw-   0        0        0    10451 2023-06-14 03:30:36.000000 Signal8-3.8/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       24 2023-06-12 18:52:22.000000 Signal8-3.8/Signal8/__init__.py
--rw-rw-rw-   0        0        0      214 2023-06-13 18:14:07.000000 Signal8-3.8/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:35:13.649822 Signal8-3.8/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-3.8/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5346 2023-06-14 03:28:36.000000 Signal8-3.8/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     1116 2023-06-12 21:36:47.000000 Signal8-3.8/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-3.8/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    11900 2023-06-14 03:32:30.000000 Signal8-3.8/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-3.8/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:35:13.579298 Signal8-3.8/Signal8.egg-info/
--rw-rw-rw-   0        0        0     5356 2023-06-14 03:35:11.000000 Signal8-3.8/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2023-06-14 03:35:12.000000 Signal8-3.8/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 03:35:11.000000 Signal8-3.8/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-14 03:35:11.000000 Signal8-3.8/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 03:35:13.658821 Signal8-3.8/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-06-14 03:33:47.000000 Signal8-3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 21:14:32.975725 Signal8-3.9/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-3.9/LICENSE
+-rw-rw-rw-   0        0        0     5357 2023-06-19 21:14:32.968726 Signal8-3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4859 2023-06-19 21:11:01.000000 Signal8-3.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 21:14:32.875723 Signal8-3.9/Signal8/
+-rw-rw-rw-   0        0        0    11779 2023-06-19 20:54:40.000000 Signal8-3.9/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       23 2023-06-19 19:29:34.000000 Signal8-3.9/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      242 2023-06-19 21:10:10.000000 Signal8-3.9/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-06-19 21:14:32.962724 Signal8-3.9/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-3.9/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5346 2023-06-14 03:28:36.000000 Signal8-3.9/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     1100 2023-06-19 19:38:38.000000 Signal8-3.9/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-3.9/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    11993 2023-06-19 21:07:54.000000 Signal8-3.9/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-3.9/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-06-19 21:14:32.924726 Signal8-3.9/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     5357 2023-06-19 21:14:32.000000 Signal8-3.9/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-06-19 21:14:32.000000 Signal8-3.9/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 21:14:32.000000 Signal8-3.9/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-19 21:14:32.000000 Signal8-3.9/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 21:14:32.976724 Signal8-3.9/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-06-19 21:12:06.000000 Signal8-3.9/setup.py
```

### Comparing `Signal8-3.8/LICENSE` & `Signal8-3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-3.8/PKG-INFO` & `Signal8-3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 3.8
+Version: 3.9
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
@@ -50,15 +50,15 @@
 ## List of Problem Instances
 
 | Problem Instance |                 Visualization                 |
 | :--------------: | :--------------------------------------------: |
 |  ``corners``Â   | ![1686604788813](image/README/1686604788813.png) |
 |   ``quarters``   | ![1686604799335](image/README/1686604799335.png) |
 |    ``cross``    | ![1686604808540](image/README/1686604808540.png) |
-|   ``cluster``   | ![1686604839072](image/README/1686604839072.png) |
+|    ``circle``    | ![1687209049891](image/README/1687209049891.png) |
 |     ``left``     | ![1686604845732](image/README/1686604845732.png) |
 |    ``right``    | ![1686604851758](image/README/1686604851758.png) |
 |      ``up``      | ![1686604859851](image/README/1686604859851.png) |
 |     ``down``     | ![1686604868138](image/README/1686604868138.png) |
 
 Each of the colored regions represents an area where the respective entity can be instantiated. Blue regions are starting regions, yellow regions represent goal regions and in the case of precision farming, if a goal region is not generated in the yellow region then changes to a static obstacle region but this is not the case for disaster response, instead the region where the goal was not instantiated does not impact the episode at all, the light red regions represent static obstacles, and dark red regions represent dynamic obstacles.
```

### Comparing `Signal8-3.8/README.md` & `Signal8-3.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 ## List of Problem Instances
 
 | Problem Instance |                 Visualization                 |
 | :--------------: | :--------------------------------------------: |
 |  ``corners``   | ![1686604788813](image/README/1686604788813.png) |
 |   ``quarters``   | ![1686604799335](image/README/1686604799335.png) |
 |    ``cross``    | ![1686604808540](image/README/1686604808540.png) |
-|   ``cluster``   | ![1686604839072](image/README/1686604839072.png) |
+|    ``circle``    | ![1687209049891](image/README/1687209049891.png) |
 |     ``left``     | ![1686604845732](image/README/1686604845732.png) |
 |    ``right``    | ![1686604851758](image/README/1686604851758.png) |
 |      ``up``      | ![1686604859851](image/README/1686604859851.png) |
 |     ``down``     | ![1686604868138](image/README/1686604868138.png) |
 
 Each of the colored regions represents an area where the respective entity can be instantiated. Blue regions are starting regions, yellow regions represent goal regions and in the case of precision farming, if a goal region is not generated in the yellow region then changes to a static obstacle region but this is not the case for disaster response, instead the region where the goal was not instantiated does not impact the episode at all, the light red regions represent static obstacles, and dark red regions represent dynamic obstacles.
```

### Comparing `Signal8-3.8/Signal8/Signal8.py` & `Signal8-3.9/Signal8/Signal8.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import copy
 import numpy as np
 import matplotlib.path as mpath
 
 from functools import partial
-from .utils.scenario import BaseScenario
-from .utils.simple_env import SimpleEnv, make_env
-from .utils.core import Agent, Goal, Obstacle, World
-from .utils.problems import get_problem_list, get_problem_instance
+from utils.scenario import BaseScenario
+from utils.simple_env import SimpleEnv, make_env
+from utils.core import Agent, Goal, Obstacle, World
+from utils.problems import get_problem_list, get_problem_instance
 
 from gymnasium.utils import EzPickle
 
 
 class raw_env(SimpleEnv, EzPickle):
     def __init__(
         self, 
@@ -76,40 +76,48 @@
     # Get constraints on entities given problem instance name
     def _set_problem_instance(self, world, instance_name):
         instance_constr = get_problem_instance(instance_name)
         world.problem_instance = instance_name
         world.instance_constr = instance_constr
     
     # Generate valid points according to some condition
-    def _generate_position(self, np_random, condition):
+    def _generate_position(self, np_random, condition, circle=False):
         while True:
-            point = np_random.uniform(-1, +1, 2)
+            if circle:
+                theta = np_random.uniform(0, 2*np.pi)
+                r = 0.5 * np.sqrt(np_random.uniform(0, 1))
+                point = np.array([r * np.cos(theta), r * np.sin(theta)])
+            else:
+                point = np_random.uniform(-1, +1, 2)
             if condition(point):
                 break
         return point
-    
-    # Check if point is outside of rectangular obstacle regions
-    def _safe_position(self, point, epsilon, x_constraints, y_constraints):
-        return all(not (low - epsilon <= point[0] <= high + epsilon) for low, high in x_constraints) \
-            and all(not (low - epsilon <= point[1] <= high + epsilon) for low, high in y_constraints)
 
     # Check if point is outside of triangular obstacle regions
     def _outside_triangle(self, point, paths, epsilon):
         enlarged_paths = []
         for path in paths:
             centroid = np.mean(path.vertices[:-1], axis=0)
             enlarged_vertices = path.vertices + epsilon * (path.vertices - centroid)
             enlarged_paths.append(mpath.Path(enlarged_vertices))
         return not any(path.contains_points(point[None, :]) for path in enlarged_paths)
     
+    def _outside_circle(self, point, center, radius, epsilon):
+        return np.linalg.norm(point - center) > radius + epsilon
+    
+    # Check if point is outside of rectangular obstacle regions
+    def _outside_rectangle(self, point, x_constraints, y_constraints, epsilon):
+        return all(not (low - epsilon <= point[0] <= high + epsilon) for low, high in x_constraints) \
+            and all(not (low - epsilon <= point[1] <= high + epsilon) for low, high in y_constraints)
+    
     # Reset agents and goals to their initial positions
     def _reset_agents_and_goals(self, world, np_random, paths):
         epsilon = world.buffer_dist
         
-        if paths is None:
+        if world.problem_instance not in ['corners', 'circle']:
             x_constraints = [constr[0] for constr in world.instance_constr]
             y_constraints = [constr[1] for constr in world.instance_constr]
 
         for i, agent in enumerate(world.agents):
             agent.goal = world.goals[i]
 
             agent.state.p_vel = np.zeros(world.dim_p)
@@ -117,29 +125,42 @@
 
             if world.problem_instance == 'corners':
                 condition = partial(
                     self._outside_triangle, 
                     paths=paths, 
                     epsilon=epsilon
                     )
+            elif world.problem_instance == 'circle':
+                condition = partial(
+                    self._outside_circle,
+                    center=world.instance_constr[0][0],
+                    radius=world.instance_constr[0][1],
+                    epsilon=epsilon
+                    )
             else:
                 condition = partial(
-                    self._safe_position, 
-                    epsilon=epsilon, 
+                    self._outside_rectangle, 
                     x_constraints=x_constraints, 
-                    y_constraints=y_constraints
+                    y_constraints=y_constraints,
+                    epsilon=epsilon, 
                     )
 
             agent.state.p_pos = self._generate_position(np_random, condition)
             agent.goal.state.p_pos = self._generate_position(np_random, condition)
     
     # Reset all large obstacles to a position that does not intersect with the agents
     def _reset_large_obstacles(self, world, np_random, paths):
         def inside_triangle_condition(point):
             return any(path.contains_points(point[None, :]) for path in paths)
+        
+        def inside_circle_condition(point):
+            epsilon = world.buffer_dist
+            center = world.instance_constr[0][0]
+            radius = world.instance_constr[0][1]
+            return np.linalg.norm(point - center) <= radius - epsilon
                 
         occupied_triangles = set()
         for i, large_obstacle in enumerate(world.large_obstacles):            
             large_obstacle.state.p_vel = np.zeros(world.dim_p)
             idx = i % len(world.instance_constr)
             
             # Each corner may only have one large_obstacle in it
@@ -147,56 +168,57 @@
                 while True:
                     pos = self._generate_position(np_random, inside_triangle_condition)
                     triangle_idx = next((i for i, path in enumerate(paths) if path.contains_points(pos[None, :])), None)
                     if triangle_idx not in occupied_triangles:
                         large_obstacle.state.p_pos = pos
                         occupied_triangles.add(triangle_idx)
                         break
+            elif world.problem_instance == 'circle':
+                    large_obstacle.state.p_pos = self._generate_position(np_random, inside_circle_condition, circle=True)
             else:                
                 large_obstacle.state.p_pos = np_random.uniform(*zip(*world.instance_constr[idx]))
     
-    # Reset all small obstacles to a position that does not intersect with the agents or the large obstacles
     def _reset_small_obstacles(self, world, np_random, paths):
         epsilon = world.small_obstacles[0].size + world.large_obstacles[0].size
-        
-        x_constraints = [constr[0] for constr in world.instance_constr]
-        y_constraints = [constr[1] for constr in world.instance_constr]
+
         agent_positions = [agent.state.p_pos for agent in world.agents]
         goal_positions = [goal.state.p_pos for goal in world.goals]
         large_obstacle_positions = [obstacle.state.p_pos for obstacle in world.large_obstacles]
-        
+
         def safe_position(point):
+            within_other_positions = any(np.linalg.norm(point - pos) <= epsilon for pos in agent_positions + goal_positions + large_obstacle_positions)
+
             if world.problem_instance == 'corners':
                 within_obstacle_constraints = any(path.contains_points(point[None, :]) for path in paths)
+            elif world.problem_instance == 'circle':
+                center = world.instance_constr[0][0]
+                radius = world.instance_constr[0][1]
+                within_obstacle_constraints = np.linalg.norm(point - center) <= radius + epsilon
             else:
+                x_constraints = [constr[0] for constr in world.instance_constr]
+                y_constraints = [constr[1] for constr in world.instance_constr]
                 within_obstacle_constraints = any(low - epsilon <= point[0] <= high + epsilon for low, high in x_constraints) \
                     or any(low - epsilon <= point[1] <= high + epsilon for low, high in y_constraints)
 
-            within_other_positions = any(np.linalg.norm(point - pos) <= epsilon for pos in agent_positions + goal_positions + large_obstacle_positions)
-
             return not (within_obstacle_constraints or within_other_positions)
-        
+
         for small_obstacle in world.small_obstacles:
             small_obstacle.state.p_vel = np.zeros(world.dim_p)
             small_obstacle.state.p_pos = self._generate_position(np_random, safe_position)
 
     def reset_world(self, world, np_random, problem_instance):
         self._set_problem_instance(world, problem_instance)
         
         paths = [mpath.Path(np.array(triangle)) for triangle in world.instance_constr] \
             if world.problem_instance == 'corners' else None
             
         self._reset_agents_and_goals(world, np_random, paths)
         self._reset_large_obstacles(world, np_random, paths)
         self._reset_small_obstacles(world, np_random, paths)
     
-    # Reward given by agents to agents for reaching their respective goals
-    def reward(self, agent, world):
-        return 0
-    
     # Ground agents can only observe the positions of other agents, goals, and small obstacles
     def observation(self, agent, world):
         agent_pos = agent.state.p_pos
         agent_vel = agent.state.p_vel
         
         num_agents = len(world.agents)
         num_small_obstacles = len(world.small_obstacles)
@@ -227,8 +249,12 @@
                 
         goal_pos = agent.goal.state.p_pos
         relative_goal_pos = goal_pos - agent_pos
         goal_dist = np.linalg.norm(relative_goal_pos)
         if goal_dist <= max_observable_dist:
             observed_goal = relative_goal_pos
         
-        return np.concatenate((agent_pos, agent_vel, np.concatenate(observed_obstacles, axis=0), observed_goal))
+        return np.concatenate((agent_pos, agent_vel, np.concatenate(observed_obstacles, axis=0), observed_goal))
+        
+    # Reward given by agents to agents for reaching their respective goals
+    def reward(self, agent, world):
+        return 0
```

### Comparing `Signal8-3.8/Signal8/utils/core.py` & `Signal8-3.9/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-3.8/Signal8/utils/problems.py` & `Signal8-3.9/Signal8/utils/problems.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,16 +14,16 @@
         ],
     'cross': [
         ((-0.1875, 0.1875), (0, 0.7)),
         ((-0.1875, 0.1875), (-0.7, 0)),
         ((-0.7, 0), (-0.1875, 0.1875)),
         ((0, 0.7), (-0.1875, 0.1875)),
         ],
-    'cluster':  [
-        ((-0.50, 0.50), (-0.50, 0.50)),
+    'circle':  [
+        ((0, 0), (0.5)),
         ],
     'left': [
         ((-1, 0), (-1, 1))
         ],
     'right': [
         ((0, 1), (-1, 1))
         ],
```

### Comparing `Signal8-3.8/Signal8/utils/simple_env.py` & `Signal8-3.9/Signal8/utils/simple_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,19 +215,18 @@
         
         truncations = [(crossed_small or crossed_large) for crossed_small, crossed_large in zip(crossed_threshold_small, crossed_threshold_large)]
         truncations = [True] * self.num_agents if self.steps >= self.max_cycles else truncations
 
         terminations = [False] * self.num_agents
         for i, dist in enumerate(goal_dist):
             if dist <= goal_dist_threshold:
-                self.terminations[i] = True
+                terminations[i] = True
 
         return {'terminations': terminations, 'truncations': truncations}
 
-
     def step(self, action):
         if (
             self.terminations[self.agent_selection]
             or self.truncations[self.agent_selection]
         ):
             self._was_dead_step(action)
             return
@@ -237,16 +236,17 @@
         self.agent_selection = self._agent_selector.next()
         self.current_actions[current_idx] = action
 
         if next_idx == 0:
             self.steps += 1
             self._execute_world_step()
             status = self._episode_status()
-            self.terminations = status['terminations']
-            self.truncations = status['truncations']
+            for idx, agent in enumerate(self._index_map.keys()):
+                self.terminations[agent] = status['terminations'][idx]
+                self.truncations[agent] = status['truncations'][idx]  
 
         if self.render_mode == "human":
             self.render()
 
     def enable_render(self, mode="human"):
         if not self.renderOn and mode == "human":
             self.screen = pygame.display.set_mode(self.screen.get_size())
```

### Comparing `Signal8-3.8/Signal8/utils/test_dynamic_obs.py` & `Signal8-3.9/Signal8/utils/test_dynamic_obs.py`

 * *Files identical despite different names*

### Comparing `Signal8-3.8/Signal8.egg-info/PKG-INFO` & `Signal8-3.9/Signal8.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 3.8
+Version: 3.9
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
@@ -50,15 +50,15 @@
 ## List of Problem Instances
 
 | Problem Instance |                 Visualization                 |
 | :--------------: | :--------------------------------------------: |
 |  ``corners``Â   | ![1686604788813](image/README/1686604788813.png) |
 |   ``quarters``   | ![1686604799335](image/README/1686604799335.png) |
 |    ``cross``    | ![1686604808540](image/README/1686604808540.png) |
-|   ``cluster``   | ![1686604839072](image/README/1686604839072.png) |
+|    ``circle``    | ![1687209049891](image/README/1687209049891.png) |
 |     ``left``     | ![1686604845732](image/README/1686604845732.png) |
 |    ``right``    | ![1686604851758](image/README/1686604851758.png) |
 |      ``up``      | ![1686604859851](image/README/1686604859851.png) |
 |     ``down``     | ![1686604868138](image/README/1686604868138.png) |
 
 Each of the colored regions represents an area where the respective entity can be instantiated. Blue regions are starting regions, yellow regions represent goal regions and in the case of precision farming, if a goal region is not generated in the yellow region then changes to a static obstacle region but this is not the case for disaster response, instead the region where the goal was not instantiated does not impact the episode at all, the light red regions represent static obstacles, and dark red regions represent dynamic obstacles.
```

### Comparing `Signal8-3.8/setup.py` & `Signal8-3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="3.8",
+    version="3.9",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

