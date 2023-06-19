# Comparing `tmp/ortega-1.0.3.tar.gz` & `tmp/ortega-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ortega-1.0.3.tar", last modified: Tue Mar 21 17:22:32 2023, max compression
+gzip compressed data, was "ortega-1.0.4.tar", last modified: Mon Jun 19 03:00:36 2023, max compression
```

## Comparing `ortega-1.0.3.tar` & `ortega-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:22:32.530333 ortega-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-21 17:22:22.000000 ortega-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-21 17:22:32.530333 ortega-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-03-21 17:22:22.000000 ortega-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:22:32.530333 ortega-1.0.3/ortega/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-03-21 17:22:22.000000 ortega-1.0.3/ortega/STPoint.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-21 17:22:22.000000 ortega-1.0.3/ortega/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-21 17:22:22.000000 ortega-1.0.3/ortega/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-03-21 17:22:22.000000 ortega-1.0.3/ortega/ellipses.py
--rw-r--r--   0 runner    (1001) docker     (123)    20585 2023-03-21 17:22:22.000000 ortega-1.0.3/ortega/ortega.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-03-21 17:22:22.000000 ortega-1.0.3/ortega/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 17:22:32.530333 ortega-1.0.3/ortega.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-21 17:22:32.000000 ortega-1.0.3/ortega.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-21 17:22:32.000000 ortega-1.0.3/ortega.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 17:22:32.000000 ortega-1.0.3/ortega.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-21 17:22:32.000000 ortega-1.0.3/ortega.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-21 17:22:32.000000 ortega-1.0.3/ortega.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 17:22:32.530333 ortega-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-03-21 17:22:22.000000 ortega-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:00:36.054205 ortega-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-19 03:00:25.000000 ortega-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-19 03:00:36.054205 ortega-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-19 03:00:25.000000 ortega-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:00:36.050204 ortega-1.0.4/ortega/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-19 03:00:25.000000 ortega-1.0.4/ortega/STPoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-19 03:00:25.000000 ortega-1.0.4/ortega/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-19 03:00:25.000000 ortega-1.0.4/ortega/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-06-19 03:00:25.000000 ortega-1.0.4/ortega/ellipses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27029 2023-06-19 03:00:25.000000 ortega-1.0.4/ortega/ortega.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-19 03:00:25.000000 ortega-1.0.4/ortega/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:00:36.050204 ortega-1.0.4/ortega.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-19 03:00:35.000000 ortega-1.0.4/ortega.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-19 03:00:36.000000 ortega-1.0.4/ortega.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 03:00:35.000000 ortega-1.0.4/ortega.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-19 03:00:35.000000 ortega-1.0.4/ortega.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 03:00:35.000000 ortega-1.0.4/ortega.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 03:00:36.054205 ortega-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-19 03:00:25.000000 ortega-1.0.4/setup.py
```

### Comparing `ortega-1.0.3/LICENSE` & `ortega-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ortega-1.0.3/README.md` & `ortega-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ortega-1.0.3/ortega/STPoint.py` & `ortega-1.0.4/ortega/STPoint.py`

 * *Files identical despite different names*

### Comparing `ortega-1.0.3/ortega/ellipses.py` & `ortega-1.0.4/ortega/ellipses.py`

 * *Files identical despite different names*

### Comparing `ortega-1.0.3/ortega/ortega.py` & `ortega-1.0.4/ortega/ortega.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,47 +16,48 @@
     return (
             item.el.intersects(others.el)
             or item.geom.within(others.geom)
             or others.geom.within(item.geom)
     )
 
 
-def get_spatiotemporal_intersect_pairs(
-        ellipses_list_id1: List[Ellipse], ellipses_list_id2: List[Ellipse],
-        interaction_min_delay: float) -> List[Tuple[Ellipse, Ellipse]]:
-    """
-    Get spatially and temporally intersect PPA pairs
-    :param ellipses_list_id2:
-    :param ellipses_list_id1:
-    :param interaction_min_delay:
-    :return:
-    """
-    intersection_pairs = []
+def get_time_difference(
+        ellipses_list_id1: List[Ellipse], ellipses_list_id2: List[Ellipse]):
+    time_diff = []
     for count, item in enumerate(ellipses_list_id1, 1):
-        # temporal intersect
+        # spatial intersect
         sub_ellipses_list = []
         for item2 in ellipses_list_id2:
-            if __timedifcheck(item.t1, item2.t1) <= interaction_min_delay * 60:  # check temporal intersect
-                sub_ellipses_list.append(item2)
+            if __check_spatial_intersect(item, item2):
+                time_diff.append(__timedifcheck(item.t1, item2.t1))
+    return time_diff
 
-        if len(sub_ellipses_list) == 0:
-            continue
 
+def get_spatial_intersect_pairs(
+        ellipses_list_id1: List[Ellipse], ellipses_list_id2: List[Ellipse],
+        ) -> List[Tuple[Ellipse, Ellipse]]:
+    intersection_pairs = []
+    for count, item in enumerate(ellipses_list_id1, 1):
         # spatial intersect
-        intersection_pairs.extend(
-            [
-                (item, others)
-                for others in sub_ellipses_list
-                if __check_spatial_intersect(item, others)
-            ]
-        )
-
+        for item2 in ellipses_list_id2:
+            if __check_spatial_intersect(item, item2):
+                intersection_pairs.append((item, item2))
     return intersection_pairs
 
 
+def get_timedelay_pairs(intersection_df: List[Tuple[Ellipse, Ellipse]],
+                        interaction_min_delay: float, interaction_max_delay: float):
+    intersection_pair = []
+    for pair in intersection_df:
+        if (__timedifcheck(pair[0].t1, pair[1].t1) >= interaction_min_delay * 60) & (
+                __timedifcheck(pair[0].t1, pair[1].t1) <= interaction_max_delay * 60):
+            intersection_pair.append(pair)
+    return intersection_pair
+
+
 def intersect_ellipse_todataframe(intersection_df: List[Tuple[Ellipse, Ellipse]]):
     """
 
     :param intersection_df:
     :return:
     """
 
@@ -79,14 +80,91 @@
         [
             {**columns_names(item, 1), **columns_names(item2, 2)}
             for item, item2 in intersection_df
         ]
     )
 
 
+def check_continuous(df: pd.DataFrame, id1: int, id2: int):
+    p1start = df['P1_t_start'].tolist()
+    p1end = df['P1_t_end'].tolist()
+    p2start = df['P2_t_start'].tolist()
+    p2end = df['P2_t_end'].tolist()
+    p1_start_time, p1_end_time, p2_start_time, p2_end_time = [], [], [], []
+    p1_start_index, p1_end_index = [], []
+    p1_start_time.append(p1start[0])
+    p1_start_index.append(0)
+    for i in range(1, len(p1start)):
+        if datetime.strptime(str(p1start[i]), '%Y-%m-%d %H:%M:%S') == datetime.strptime(str(p1start[i - 1]),
+                                                                                        '%Y-%m-%d %H:%M:%S'):
+            continue
+        elif datetime.strptime(str(p1end[i - 1]), '%Y-%m-%d %H:%M:%S') == datetime.strptime(str(p1start[i]),
+                                                                                        '%Y-%m-%d %H:%M:%S'):
+            continue
+        else:
+            p1_end_time.append(p1end[i - 1])
+            p1_end_index.append(i - 1)
+            p1_start_time.append(p1start[i])
+            p1_start_index.append(i)
+    p1_end_time.append(p1end[len(p1end) - 1])
+    p1_end_index.append(len(p1end) - 1)
+    
+    p2_start_pool, p2_end_pool = [], []
+    p2_start_pool_list, p2_end_pool_list = [], []
+    
+    i = 0
+    for j in p1_end_index:
+        while i <= j:
+            p2_start_pool.append(p2start[i])
+            p2_end_pool.append(p2end[i])
+            i += 1
+        p2_start_pool.sort()
+        p2_end_pool.sort()
+        p2_start_pool_list.append(p2_start_pool)
+        p2_end_pool_list.append(p2_end_pool)
+        p2_start_pool, p2_end_pool = [], []
+
+    p2_start_time_list, p2_end_time_list = [], []
+    for k in range(0, len(p2_start_pool_list)):
+        p2_start_time.append((p2_start_pool_list[k])[0])
+        for m in range(1, len(p2_start_pool_list[k])):
+            if datetime.strptime(str((p2_start_pool_list[k])[m]), '%Y-%m-%d %H:%M:%S') \
+                    == datetime.strptime(str((p2_start_pool_list[k])[m - 1]), '%Y-%m-%d %H:%M:%S'):
+                continue
+            elif datetime.strptime(str((p2_end_pool_list[k])[m - 1]), '%Y-%m-%d %H:%M:%S') \
+                    == datetime.strptime(str((p2_start_pool_list[k])[m]), '%Y-%m-%d %H:%M:%S'):
+                continue
+            else:
+                p2_end_time.append((p2_end_pool_list[k])[m - 1])
+                p2_start_time.append((p2_start_pool_list[k])[m])
+        p2_end_time.append((p2_end_pool_list[k])[len((p2_end_pool_list[k])) - 1])
+        p2_start_time_list.append(p2_start_time)
+        p2_end_time_list.append(p2_end_time)
+        p2_start_time = []
+        p2_end_time = []
+
+    p1_start_column, p1_end_column, p2_start_column, p2_end_column = [], [], [], []
+    for i in range(0, len(p2_start_time_list)):
+        for j in range(0, len(p2_start_time_list[i])):
+            p1_start_column.append(p1_start_time[i])
+            p1_end_column.append(p1_end_time[i])
+            p2_start_column.append((p2_start_time_list[i])[j])
+            p2_end_column.append((p2_end_time_list[i])[j])
+
+    d = {'P1 start': p1_start_column, 'P1 end': p1_end_column,
+         'P2 start': p2_start_column, 'P2 end': p2_end_column}
+    df_new = pd.DataFrame(d)
+    diff_list = []
+    for i in range(0, len(p1_start_column)):
+        diff = pd.Timedelta(p2_start_column[i] - p1_start_column[i]).total_seconds()/60
+        diff_list.append(diff)
+    df_new['Difference'] = diff_list
+    return df_new
+
+
 def __merge_continuous_incident(df: pd.DataFrame, id1: int, id2: int):
     """
     Merge continuous interaction incidents after estimating duration
     :param df:
     :param id1:
     :param id2:
     :return:
@@ -139,29 +217,42 @@
     :return:
     """
     p1start = df['P1_t_start'].tolist()
     p1end = df['P1_t_end'].tolist()
     p2start = df['P2_t_start'].tolist()
     p2end = df['P2_t_end'].tolist()
     final_start, final_end, subsequenceOfInteraction = [], [], []
+    time_difference = [(df['P2_t_start'] - df['P1_t_start']) / pd.Timedelta(hours=1)]
+    time_group, diff_mean = [], []
     for i in range(0, len(p1start) - 1):  # identify subsequence of continuous interaction
         if datetime.strptime(str(p1start[i]), '%Y-%m-%d %H:%M:%S') == datetime.strptime(str(p1start[i + 1]),
                                                                                         '%Y-%m-%d %H:%M:%S'):
             subsequenceOfInteraction.extend([p1start[i], p1end[i], p1end[i + 1], p2start[i], p2end[i], p2start[i + 1],
                                              p2end[i + 1]])  # append all time in a candidate pool
+            time_group.append(time_difference[0][i])
+
         elif datetime.strptime(str(p1end[i]), '%Y-%m-%d %H:%M:%S') == datetime.strptime(str(p1start[i + 1]),
                                                                                         '%Y-%m-%d %H:%M:%S'):
             subsequenceOfInteraction.extend([p1start[i], p1end[i], p1end[i + 1], p2start[i], p2end[i], p2start[i + 1],
                                              p2end[i + 1]])  # append all time in a candidate pool
+            time_group.append(time_difference[0][i])
         else:
             if len(subsequenceOfInteraction) == 0:
                 subsequenceOfInteraction.extend([p1start[i], p1end[i], p2start[i], p2end[i]])
             final_start.append(min(subsequenceOfInteraction))  # print(i,p1start[i],p1end[i],p1start[i+1],p1end[i+1])
             final_end.append(max(subsequenceOfInteraction))
             subsequenceOfInteraction = []
+            time_group.append(time_difference[0][i])
+            diff_mean.append(sum(time_group) / len(time_group))
+            time_group = []
+        if i == (len(p1start) - 2):
+            time_group.append(time_difference[0][i + 1])
+            diff_mean.append(sum(time_group) / len(time_group))
+            time_group = []
+
     if len(subsequenceOfInteraction) != 0:
         final_start.append(min(subsequenceOfInteraction))
         final_end.append(max(subsequenceOfInteraction))
     if len(p1start) == 1:
         i = 0
         subsequenceOfInteraction.extend(
             [p1start[i], p1end[i], p2start[i], p2end[i]])  # append all time in a candidate pool
@@ -170,14 +261,15 @@
     df_new = pd.DataFrame(list(zip(final_start, final_end)), columns=['Start', 'End'])
     df_new['P1'] = id1
     df_new['P2'] = id2
     df_new['No'] = np.arange(df_new.shape[0]) + 1
     df_new['Duration'] = df_new['End'] - df_new['Start']
     df_new['Duration'] = df_new['Duration'].dt.total_seconds().div(60)
     df_new = __merge_continuous_incident(df_new, id1, id2)
+    #df_new['Mean_delay'] = diff_mean
     return df_new[['No', 'P1', 'P2', 'Start', 'End', 'Duration']]
 
 
 def interaction_compute_speed_diff(df: pd.DataFrame):
     """
     compute the percentage difference in speed between two moving entities
     this speed is based on the instant speed between two points not the average speed over a kernel
@@ -210,20 +302,27 @@
     #     return x
 
     df['diff_direction'] = df['P2_direction'] - df['P1_direction']
     df['diff_direction'] = df['diff_direction'].apply(math.cos)
     return df
 
 
+def interaction_compute_time_diff(df:pd.DataFrame):
+    df['diff_time'] = (df['P2_t_start'] - df['P1_t_start'])/ pd.Timedelta(hours=1)
+    return df
+
+
 class ORTEGA:
     # ORTEGA is the main class for interaction analysis, users need to initialize this object at the very beginning
     def __init__(
             self,
             data: pd.DataFrame,  # movement data of two entities
-            minute_delay: float,  # allowable delay for intersecting PPAs, in minute
+            # minute_delay: float,  # allowable delay for intersecting PPAs, in minute
+            minute_min_delay: float = 0,
+            minute_max_delay: float = 0,
             start_time: str = None,  # use this when users want to select a segment of movement data
             end_time: str = None,  # use this when users want to select a segment of movement data
             max_el_time_min: float = 10000,  # PPA's interval greater than this value will be eliminated, in minute
             latitude_field: str = "latitude",  # specify the latitude field name
             longitude_field: str = "longitude",  # specify the longitude field name
             id_field: str = "pid",  # specify the id field name
             time_field: str = "time_local",  # time_field must include month, day, year, hour, minute, second
@@ -233,33 +332,35 @@
         self.data = data
         self.start_time = start_time
         self.end_time = end_time
         self.latitude_field = latitude_field
         self.longitude_field = longitude_field
         self.id_field = id_field
         self.time_field = time_field
-        self.minute_delay = minute_delay
+        # self.minute_delay = minute_delay
+        self.minute_min_delay = minute_min_delay
+        self.minute_max_delay = minute_max_delay
         self.max_el_time_min = max_el_time_min
         self.speed_average = speed_average
         # self.kernel = kernel
         self.__validate()
         self.__start()
-
+    '''
     @property
     def minute_delay(self):
         return self._minute_delay
 
     @minute_delay.setter
     def minute_delay(self, value):
         if not isinstance(value, float) and not isinstance(value, int):
             raise TypeError("Parameter 'minute_delay' must be numeric!")
         if value <= 0:
             raise ValueError("Parameter 'minute_delay' must be greater than zero!")
         self._minute_delay = value
-
+    '''
     @property
     def max_el_time_min(self):
         return self._max_el_time_min
 
     @max_el_time_min.setter
     def max_el_time_min(self, value):
         if not isinstance(value, float) and not isinstance(value, int):
@@ -399,30 +500,56 @@
         """
         self.ellipses_list = self.__get_ellipse_list(self.df1, self.df2)  # all ellipses for two objects
         self.ellipses_list_id1 = [i for i in self.ellipses_list if i.pid == self.id1]
         self.ellipses_list_id2 = [i for i in self.ellipses_list if i.pid == self.id2]
         # these do not exclude large PPAs! Only after __get_spatiotemporal_intersect_pairs() we exclude large PPAs
         print(datetime.now(), 'Initialization success!')
 
+    def continues_analysis(self):
+        spatial_pairs = self.__get_spatial_intersect_pairs()
+        all_intersection_pairs = get_timedelay_pairs(spatial_pairs, self.minute_min_delay, self.minute_max_delay)
+
+        if not all_intersection_pairs:
+            print(datetime.now(), 'Complete! No interaction found!')
+            return None
+        else:
+
+            # convert the list of intersecting ellipses to dataframe format - df_all_intersection_pairs
+            df_all_intersection_pairs = intersect_ellipse_todataframe(all_intersection_pairs)
+            df_all_intersection_pairs = interaction_compute_speed_diff(df_all_intersection_pairs)
+            df_all_intersection_pairs = interaction_compute_direction_diff(df_all_intersection_pairs)
+            df_all_intersection_pairs = interaction_compute_time_diff(df_all_intersection_pairs)
+
+            # compute duration of interaction and output as a dataframe - df_duration
+            print(datetime.now(), 'Compute continues events...')
+            df_continues = check_continuous(df_all_intersection_pairs, self.id1, self.id2)
+            if df_continues.shape[0] != 0:
+                return df_continues
+            else:
+                return None
+
     def interaction_analysis(self):
 
         print(datetime.now(), 'Implement interaction analysis...')
         # get list of intersecting Ellipse objects - all_intersection_pairs
-        all_intersection_pairs = self.__get_spatiotemporal_intersect_pairs()
+        # all_intersection_pairs = self.__get_spatiotemporal_intersect_pairs()
+        spatial_pairs = self.__get_spatial_intersect_pairs()
+        all_intersection_pairs = get_timedelay_pairs(spatial_pairs, self.minute_min_delay, self.minute_max_delay)
 
         if not all_intersection_pairs:
             print(datetime.now(), 'Complete! No interaction found!')
             return None, None, None
         else:
             print(datetime.now(), f'Complete! {len(all_intersection_pairs)} pairs of intersecting PPAs found!')
 
             # convert the list of intersecting ellipses to dataframe format - df_all_intersection_pairs
             df_all_intersection_pairs = intersect_ellipse_todataframe(all_intersection_pairs)
             df_all_intersection_pairs = interaction_compute_speed_diff(df_all_intersection_pairs)
             df_all_intersection_pairs = interaction_compute_direction_diff(df_all_intersection_pairs)
+            df_all_intersection_pairs = interaction_compute_time_diff(df_all_intersection_pairs)
 
             # compute duration of interaction and output as a dataframe - df_duration
             print(datetime.now(), 'Compute duration of interaction...')
             df_duration = durationEstimator(df_all_intersection_pairs, self.id1, self.id2)
             print(datetime.now(), f'Complete! {df_duration.shape[0]} interaction events identified!')
             if df_duration.shape[0] != 0:
                 return all_intersection_pairs, df_all_intersection_pairs, df_duration
@@ -438,25 +565,30 @@
         """
         print(datetime.now(), "Generate PPA list for the two moving entities...")
         ellipses_list_gen = EllipseList(self.latitude_field, self.longitude_field, self.id_field, self.time_field)
 
         # create PPA for df1, skip PPAs with large time interval
         ellipses_list_gen.generate(df1, max_el_time_min=self.max_el_time_min, speed_average=self.speed_average)
         # append PPA based on df2 to the above ellipses_list_gen object
-        allPPAlist = ellipses_list_gen.generate(df2, max_el_time_min=self.max_el_time_min, speed_average=self.speed_average)
+        allPPAlist = ellipses_list_gen.generate(df2, max_el_time_min=self.max_el_time_min,
+                                                speed_average=self.speed_average)
         print(datetime.now(), "Generating PPA list completed!")
 
         return allPPAlist  # return the whole list of PPAs
-
+    '''
     def __get_spatiotemporal_intersect_pairs(self):
         print(datetime.now(), "Getting spatial and temporal intersection pairs...")
         intersection_pairs = get_spatiotemporal_intersect_pairs(self.ellipses_list_id1, self.ellipses_list_id2,
                                                                 self.minute_delay)
         print(datetime.now(), "Getting spatial and temporal intersection pairs completed!")
         return intersection_pairs
+    '''
+    def __get_spatial_intersect_pairs(self):
+        intersection_pairs = get_spatial_intersect_pairs(self.ellipses_list_id1, self.ellipses_list_id2)
+        return intersection_pairs
 
     def compute_ppa_speed(self):
         speed_list = [
             [e.speed for e in self.ellipses_list_id1],
             [e.speed for e in self.ellipses_list_id2]
         ]
         print(f"Descriptive statistics of PPA ellipses length for id {self.id1}:")
```

### Comparing `ortega-1.0.3/ortega/visualization.py` & `ortega-1.0.4/ortega/visualization.py`

 * *Files identical despite different names*

### Comparing `ortega-1.0.3/setup.py` & `ortega-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 if __name__ == "__main__":
     setup(
         name='ortega',
-        version='1.0.3',
+        version='1.0.4',
         author='MOVE lab@UCSB',
         author_email="rongxiangsu@ucsb.edu",
         packages=["ortega"],
         url='https://github.com/move-ucsb/ORTEGA',
         license='MIT',
         description='ORTEGA',
         install_requires=[
```

