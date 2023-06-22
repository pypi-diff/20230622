# Comparing `tmp/Signal8-4.1.tar.gz` & `tmp/Signal8-4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-4.1.tar", last modified: Wed Jun 21 21:43:48 2023, max compression
+gzip compressed data, was "Signal8-4.2.tar", last modified: Thu Jun 22 19:41:50 2023, max compression
```

## Comparing `Signal8-4.1.tar` & `Signal8-4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 21:43:47.993205 Signal8-4.1/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-4.1/LICENSE
--rw-rw-rw-   0        0        0     4763 2023-06-21 21:43:47.990205 Signal8-4.1/PKG-INFO
--rw-rw-rw-   0        0        0     4265 2023-06-20 21:50:49.000000 Signal8-4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 21:43:47.872205 Signal8-4.1/Signal8/
--rw-rw-rw-   0        0        0    11770 2023-06-21 21:42:34.000000 Signal8-4.1/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-4.1/Signal8/__init__.py
--rw-rw-rw-   0        0        0      242 2023-06-19 21:10:10.000000 Signal8-4.1/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-06-21 21:43:47.982206 Signal8-4.1/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-4.1/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5346 2023-06-14 03:28:36.000000 Signal8-4.1/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     1070 2023-06-20 21:36:24.000000 Signal8-4.1/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-4.1/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    11955 2023-06-21 21:40:30.000000 Signal8-4.1/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-4.1/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-06-21 21:43:47.947203 Signal8-4.1/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4763 2023-06-21 21:43:47.000000 Signal8-4.1/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2023-06-21 21:43:47.000000 Signal8-4.1/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 21:43:47.000000 Signal8-4.1/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-21 21:43:47.000000 Signal8-4.1/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 21:43:47.993205 Signal8-4.1/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-06-21 21:42:39.000000 Signal8-4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 19:41:50.663192 Signal8-4.2/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-4.2/LICENSE
+-rw-rw-rw-   0        0        0     4769 2023-06-22 19:41:50.660193 Signal8-4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4271 2023-06-22 19:39:26.000000 Signal8-4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 19:41:50.558191 Signal8-4.2/Signal8/
+-rw-rw-rw-   0        0        0    11825 2023-06-22 19:40:11.000000 Signal8-4.2/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-4.2/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      209 2023-06-22 19:39:06.000000 Signal8-4.2/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-06-22 19:41:50.648191 Signal8-4.2/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-4.2/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5346 2023-06-14 03:28:36.000000 Signal8-4.2/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2070 2023-06-22 19:25:12.000000 Signal8-4.2/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-4.2/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    11952 2023-06-22 19:39:57.000000 Signal8-4.2/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-4.2/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-06-22 19:41:50.598192 Signal8-4.2/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     4769 2023-06-22 19:41:49.000000 Signal8-4.2/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-06-22 19:41:50.000000 Signal8-4.2/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 19:41:49.000000 Signal8-4.2/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-22 19:41:49.000000 Signal8-4.2/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 19:41:50.664193 Signal8-4.2/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-06-22 19:41:08.000000 Signal8-4.2/setup.py
```

### Comparing `Signal8-4.1/LICENSE` & `Signal8-4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-4.1/PKG-INFO` & `Signal8-4.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 4.1
+Version: 4.2
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
@@ -37,15 +37,15 @@
 
 ## Usage
 
 ```
 import Signal8
 
 env = Signal8.env()
-env.reset(options={'problem_instance': 'corners'}))
+env.reset(options={'problem_instance': 'einstein_tile'}))
 observation, _, terminations, truncations, _ = env.last()
 env.step(action)
 env.close()
 ```
 
 ## List of Problem Instances
```

### Comparing `Signal8-4.1/README.md` & `Signal8-4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ## Usage
 
 ```
 import Signal8
 
 env = Signal8.env()
-env.reset(options={'problem_instance': 'corners'}))
+env.reset(options={'problem_instance': 'einstein_tile'}))
 observation, _, terminations, truncations, _ = env.last()
 env.step(action)
 env.close()
 ```
 
 ## List of Problem Instances
```

### Comparing `Signal8-4.1/Signal8/Signal8.py` & `Signal8-4.2/Signal8/Signal8.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,34 +99,37 @@
             enlarged_vertices = path.vertices + epsilon * (path.vertices - centroid)
             enlarged_paths.append(mpath.Path(enlarged_vertices))
         return not any(path.contains_points(point[None, :]) for path in enlarged_paths)
     
     def _outside_circle(self, point, center, radius, epsilon):
         return np.linalg.norm(point - center) > radius + epsilon
     
-    # Check if point is outside of rectangular obstacle regions
     def _outside_rectangle(self, point, x_constraints, y_constraints, epsilon):
-        return all(not (low - epsilon <= point[0] <= high + epsilon) for low, high in x_constraints) \
-            and all(not (low - epsilon <= point[1] <= high + epsilon) for low, high in y_constraints)
+        within_constraints = any(
+            (low_x - epsilon <= point[0] <= high_x + epsilon) and (low_y - epsilon <= point[1] <= high_y + epsilon)
+            for (low_x, high_x), (low_y, high_y) in zip(x_constraints, y_constraints)
+        )
+        return not within_constraints
+
     
     # Reset agents and goals to their initial positions
     def _reset_agents_and_goals(self, world, np_random, paths):
         epsilon = world.buffer_dist
         
-        if world.problem_instance not in ['corners', 'circle']:
+        if world.problem_instance not in ['corners', 'einstein_tile', 'circle']:
             x_constraints = [constr[0] for constr in world.instance_constr]
             y_constraints = [constr[1] for constr in world.instance_constr]
 
         for i, agent in enumerate(world.agents):
             agent.goal = world.goals[i]
 
             agent.state.p_vel = np.zeros(world.dim_p)
             agent.goal.state.p_vel = np.zeros(world.dim_p)
 
-            if world.problem_instance == 'corners':
+            if world.problem_instance in ['corners', 'einstein_tile']:
                 condition = partial(
                     self._outside_triangle, 
                     paths=paths, 
                     epsilon=epsilon
                     )
             elif world.problem_instance == 'circle':
                 condition = partial(
@@ -159,15 +162,15 @@
                 
         occupied_triangles = set()
         for i, large_obstacle in enumerate(world.large_obstacles):            
             large_obstacle.state.p_vel = np.zeros(world.dim_p)
             idx = i % len(world.instance_constr)
             
             # Each corner may only have one large_obstacle in it
-            if world.problem_instance == 'corners':
+            if world.problem_instance in ['corners', 'einstein_tile']:
                 while True:
                     pos = self._generate_position(np_random, inside_triangle_condition)
                     triangle_idx = next((i for i, path in enumerate(paths) if path.contains_points(pos[None, :])), None)
                     if triangle_idx not in occupied_triangles:
                         large_obstacle.state.p_pos = pos
                         occupied_triangles.add(triangle_idx)
                         break
@@ -182,37 +185,37 @@
         agent_positions = [agent.state.p_pos for agent in world.agents]
         goal_positions = [goal.state.p_pos for goal in world.goals]
         large_obstacle_positions = [obstacle.state.p_pos for obstacle in world.large_obstacles]
 
         def safe_position(point):
             within_other_positions = any(np.linalg.norm(point - pos) <= epsilon for pos in agent_positions + goal_positions + large_obstacle_positions)
 
-            if world.problem_instance == 'corners':
+            if world.problem_instance in ['corners', 'einstein_tile']:
                 within_obstacle_constraints = any(path.contains_points(point[None, :]) for path in paths)
             elif world.problem_instance == 'circle':
                 center = world.instance_constr[0][0]
                 radius = world.instance_constr[0][1]
                 within_obstacle_constraints = np.linalg.norm(point - center) <= radius + epsilon
             else:
                 x_constraints = [constr[0] for constr in world.instance_constr]
                 y_constraints = [constr[1] for constr in world.instance_constr]
-                within_obstacle_constraints = any(low - epsilon <= point[0] <= high + epsilon for low, high in x_constraints) \
-                    or any(low - epsilon <= point[1] <= high + epsilon for low, high in y_constraints)
+                outside_rectangle = self._outside_rectangle(point, x_constraints, y_constraints, epsilon)
+                within_obstacle_constraints = not outside_rectangle
 
             return not (within_obstacle_constraints or within_other_positions)
 
         for small_obstacle in world.small_obstacles:
             small_obstacle.state.p_vel = np.zeros(world.dim_p)
             small_obstacle.state.p_pos = self._generate_position(np_random, safe_position)
 
     def reset_world(self, world, np_random, problem_instance):
         self._set_problem_instance(world, problem_instance)
         
         paths = [mpath.Path(np.array(triangle)) for triangle in world.instance_constr] \
-            if world.problem_instance == 'corners' else None
+            if world.problem_instance in ['corners', 'einstein_tile'] else None
             
         self._reset_agents_and_goals(world, np_random, paths)
         self._reset_large_obstacles(world, np_random, paths)
         self._reset_small_obstacles(world, np_random, paths)
     
     # Ground agents can only observe the positions of other agents, goals, and small obstacles
     def observation(self, agent, world):
```

### Comparing `Signal8-4.1/Signal8/utils/core.py` & `Signal8-4.2/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.1/Signal8/utils/simple_env.py` & `Signal8-4.2/Signal8/utils/simple_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         self._reset_called = False
 
         self.max_cycles = max_cycles
         self.scenario = scenario
         self.world = world
         self.local_ratio = local_ratio
 
-        self.scenario.reset_world(self.world, self.np_random, 'corners')
+        self.scenario.reset_world(self.world, self.np_random, 'left')
         self.agents = [agent.name for agent in self.world.agents]
         self.possible_agents = self.agents[:]
         self._index_map = {agent.name: idx for idx, agent in enumerate(self.world.agents)}
 
         self._agent_selector = agent_selector(self.agents)
 
         # set spaces
```

### Comparing `Signal8-4.1/Signal8/utils/test_dynamic_obs.py` & `Signal8-4.2/Signal8/utils/test_dynamic_obs.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.1/Signal8.egg-info/PKG-INFO` & `Signal8-4.2/Signal8.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 4.1
+Version: 4.2
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
@@ -37,15 +37,15 @@
 
 ## Usage
 
 ```
 import Signal8
 
 env = Signal8.env()
-env.reset(options={'problem_instance': 'corners'}))
+env.reset(options={'problem_instance': 'einstein_tile'}))
 observation, _, terminations, truncations, _ = env.last()
 env.step(action)
 env.close()
 ```
 
 ## List of Problem Instances
```

### Comparing `Signal8-4.1/setup.py` & `Signal8-4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="4.1",
+    version="4.2",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

