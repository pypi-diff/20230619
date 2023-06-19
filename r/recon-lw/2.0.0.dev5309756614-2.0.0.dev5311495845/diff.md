# Comparing `tmp/recon_lw-2.0.0.dev5309756614.tar.gz` & `tmp/recon_lw-2.0.0.dev5311495845.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5309756614.tar", last modified: Mon Jun 19 08:47:29 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5311495845.tar", last modified: Mon Jun 19 11:53:20 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5309756614.tar` & `recon_lw-2.0.0.dev5311495845.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 08:47:29.000000 recon_lw-2.0.0.dev5309756614/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-19 08:47:29.000000 recon_lw-2.0.0.dev5309756614/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-19 08:46:58.000000 recon_lw-2.0.0.dev5309756614/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 08:47:29.000000 recon_lw-2.0.0.dev5309756614/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     4942 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    36026 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/recon_lw/recon_ob_cross_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     5995 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/recon_lw/recon_ob_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 08:47:29.000000 recon_lw-2.0.0.dev5309756614/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-19 08:47:29.000000 recon_lw-2.0.0.dev5309756614/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      481 2023-06-19 08:47:29.000000 recon_lw-2.0.0.dev5309756614/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-19 08:47:29.000000 recon_lw-2.0.0.dev5309756614/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-19 08:47:29.000000 recon_lw-2.0.0.dev5309756614/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-19 08:47:29.000000 recon_lw-2.0.0.dev5309756614/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-19 08:47:29.000000 recon_lw-2.0.0.dev5309756614/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 08:47:29.000000 recon_lw-2.0.0.dev5309756614/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 11:53:20.000000 recon_lw-2.0.0.dev5311495845/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-19 11:52:24.000000 recon_lw-2.0.0.dev5311495845/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-19 11:53:20.000000 recon_lw-2.0.0.dev5311495845/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-19 11:52:24.000000 recon_lw-2.0.0.dev5311495845/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-19 11:52:53.000000 recon_lw-2.0.0.dev5311495845/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 11:53:20.000000 recon_lw-2.0.0.dev5311495845/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-19 11:52:24.000000 recon_lw-2.0.0.dev5311495845/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4942 2023-06-19 11:52:24.000000 recon_lw-2.0.0.dev5311495845/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-19 11:52:24.000000 recon_lw-2.0.0.dev5311495845/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-06-19 11:52:24.000000 recon_lw-2.0.0.dev5311495845/recon_lw/SequenceCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-06-19 11:52:24.000000 recon_lw-2.0.0.dev5311495845/recon_lw/StateSequenceGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-19 11:52:24.000000 recon_lw-2.0.0.dev5311495845/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-19 11:52:24.000000 recon_lw-2.0.0.dev5311495845/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-06-19 11:52:24.000000 recon_lw-2.0.0.dev5311495845/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32855 2023-06-19 11:52:24.000000 recon_lw-2.0.0.dev5311495845/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-06-19 11:52:24.000000 recon_lw-2.0.0.dev5311495845/recon_lw/recon_ob_cross_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6018 2023-06-19 11:52:24.000000 recon_lw-2.0.0.dev5311495845/recon_lw/recon_ob_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 11:53:20.000000 recon_lw-2.0.0.dev5311495845/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-19 11:53:20.000000 recon_lw-2.0.0.dev5311495845/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-19 11:53:20.000000 recon_lw-2.0.0.dev5311495845/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-19 11:53:20.000000 recon_lw-2.0.0.dev5311495845/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-19 11:53:20.000000 recon_lw-2.0.0.dev5311495845/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-19 11:53:20.000000 recon_lw-2.0.0.dev5311495845/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-19 11:52:24.000000 recon_lw-2.0.0.dev5311495845/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-19 11:53:20.000000 recon_lw-2.0.0.dev5311495845/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-19 11:52:24.000000 recon_lw-2.0.0.dev5311495845/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 11:53:20.000000 recon_lw-2.0.0.dev5311495845/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-19 11:52:24.000000 recon_lw-2.0.0.dev5311495845/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5309756614/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5311495845/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5309756614/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5311495845/recon_lw/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5309756614/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5311495845/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5309756614/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5311495845/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5309756614/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5311495845/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5309756614/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5311495845/recon_lw/recon_ob.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,76 +1,16 @@
 from datetime import datetime, timedelta
 from sortedcontainers import SortedKeyList
 from th2_data_services.utils.message_utils import message_utils
 from recon_lw import recon_lw
 from th2_data_services.utils import time as time_utils
+from recon_lw.SequenceCache import SequenceCache
 import copy
 
 
-def sequence_cache_add(seq_num: int, ts: dict, m: dict, sequence_cache: dict) -> None:
-    seq_element = (seq_num, m)
-    sequence = sequence_cache["sequence"]
-    # gaps = sequence_cache["gaps"]
-    gap = {"gap": True}
-    duplicates = sequence_cache["duplicates"]
-    times = sequence_cache["times"]
-    if len(sequence) > 0:
-        last_elem = sequence[-1]
-        first_elem = sequence[0]
-        if seq_num > last_elem[0]:
-            sequence.add(seq_element)
-            sequence.update([(i, gap) for i in range(last_elem[0] + 1, seq_num)])
-            times.add((ts, seq_num))
-        elif seq_num < first_elem[0]:
-            #  radical difference means sequence Reset
-            if first_elem[0] - seq_num > 500:
-                raise Exception(f'Stream break detected: got{seq_num} vs {first_elem[0]}')
-            sequence.update([(i, gap) for i in range(seq_num + 1, first_elem[0])])
-            sequence.add(seq_element)
-            times.add((ts, seq_num))
-        else:
-            if "gap" in sequence[seq_num - first_elem[0]][1]:
-                del sequence[seq_num - first_elem[0]]
-                sequence.add(seq_element)
-                times.add((ts, seq_num))
-            else:
-                duplicates.add((seq_num, m["messageId"], sequence[seq_num - first_elem[0]][1]["messageId"]))
-    else:
-        sequence.add(seq_element)
-        times.add((ts, seq_num))
-
-
-def flush_sequence_get_collection(current_ts: dict, horizon_delay: int, sequence_cache: dict) -> SortedKeyList:
-    times = sequence_cache["times"]
-    sequence = sequence_cache["sequence"]
-    sub_seq = None
-    if current_ts is not None:
-        edge_timestamp = {"epochSecond": current_ts["epochSecond"] - horizon_delay,
-                          "nano": 0}
-        horizon_edge = times.bisect_key_left(recon_lw.time_stamp_key(edge_timestamp))
-        if horizon_edge < len(times):
-            seq_index = times[horizon_edge][1]
-            sub_seq = sequence.irange(None, (seq_index, None), (False, False))
-            for i in range(0, horizon_edge):
-                times.pop(0)
-        else:
-            sub_seq = sequence
-            times.clear()
-        return sub_seq
-    else:
-        times.clear()
-        return sequence
-
-
-def flush_sequence_clear_cache(processed_len: int, sequence_cache: dict) -> None:
-    sequence = sequence_cache["sequence"]
-    for i in range(0, processed_len):
-        sequence.pop(0)
-
-
 def combine_operations(operations_list):
     combined_operations = [[]]
     for operation_entry in operations_list:
         if len(combined_operations[-1]) == 0:
             combined_operations[-1].append(operation_entry)
         else:
             #if operation_entry[2]["messageId"] == combined_operations[-1][-1][2]["messageId"]:
@@ -278,115 +218,94 @@
         events.append(log_event)
 
     send_events_func(events)
     return n_processed
 
 
 def init_ob_stream(rule_settings: dict) -> None:
-    rule_settings["sequence_cache"] = {"sequence": SortedKeyList(key=lambda item: item[0]),
-                                       "times": SortedKeyList(key=lambda t: recon_lw.time_stamp_key(t[0])),
-                                       "duplicates": SortedKeyList(key=lambda item: item[0])}
+    rule_settings["sequence_cache"] = SequenceCache(rule_settings["horizon_delay"])
+        #{"sequence": SortedKeyList(key=lambda item: item[0]),
+        #                               "times": SortedKeyList(key=lambda t: recon_lw.time_stamp_key(t[0])),
+        #                               "duplicates": SortedKeyList(key=lambda item: item[0])}
     rule_settings["books_cache"] = {}
 
 
 def collect_ob_stream(next_batch: list, rule_dict: dict) -> None:
     sequence_cache = rule_dict["sequence_cache"]
     sequence_timestamp_extract = rule_dict["sequence_timestamp_extract"]
     for m in next_batch:
         seq_list = sequence_timestamp_extract(m)
-
-        # seq, ts = sequence_timestamp_extract(m)
         if seq_list is not None:
             for mess, seq, ts in seq_list:
                 try:
-                    sequence_cache_add(seq, ts, mess, sequence_cache)
+                    sequence_cache.add_object(seq, ts, mess)
+                    #sequence_cache_add(seq, ts, mess, sequence_cache)
                 except Exception as e:
                     print("Critical Error Detected: ", e)
                     print("sequence:  ", seq)
                     print("timestamp:  ", time_utils.extract_timestamp(ts))
                     print("mess:  ", mess)
                     raise e
 
 
 def flush_ob_stream(ts: dict, rule_settings: dict, event_sequence: dict, save_events_func) -> None:
-    seq_batch = flush_sequence_get_collection(ts, rule_settings["horizon_delay"], rule_settings["sequence_cache"])
+    #seq_batch = flush_sequence_get_collection(ts, rule_settings["horizon_delay"], rule_settings["sequence_cache"])
+    seq_batch = rule_settings["sequence_cache"].get_next_chunk(ts)
     n_processed = process_ob_rules(seq_batch,
                                    rule_settings["books_cache"],
                                    rule_settings["get_book_id"],
                                    rule_settings["update_book_rule"],
                                    rule_settings["check_book_rule"],
                                    event_sequence,
                                    save_events_func,
                                    rule_settings["rule_root_event"],
                                    rule_settings["initial_book_params"],
                                    rule_settings["log_books_filter"] if "log_books_filter" in rule_settings else None,
                                    rule_settings["aggregate_batch_updates"] if "aggregate_batch_updates" in rule_settings else False)
     ## Process duplicated
-    duplicates = rule_settings["sequence_cache"]["duplicates"]
+    #duplicates = rule_settings["sequence_cache"]["duplicates"]
+    duplicates = rule_settings["sequence_cache"].get_duplicates_collection()
     n_dupl = len(duplicates)
     dupl_events = []
     for i in range(0, n_dupl):
         item = duplicates.pop(0)
         d_ev = recon_lw.create_event("Duplicate:" + rule_settings["rule_root_event"]["eventName"], "Duplicate",
                                      event_sequence,
                                      ok=False,
                                      body={"seq_num": item[0], "sessionId": rule_settings["sessionId"]},
                                      parentId=rule_settings["rule_root_event"]["eventId"])
-        d_ev["attachedMessageIds"] = [item[1], item[2]]
+        d_ev["attachedMessageIds"] = [item[1]["messageId"], item[2]["messageId"]]
         dupl_events.append(d_ev)
     save_events_func(dupl_events)
     duplicates.clear()
-    flush_sequence_clear_cache(n_processed, rule_settings["sequence_cache"])
+    rule_settings["sequence_cache"].clear_processed_chunk(n_processed)
+    #flush_sequence_clear_cache(n_processed, rule_settings["sequence_cache"])
 
 
 def init_aggr_seq(order_book: dict) -> None:
-    #order_book["aggr_seq"] = {"top_v": 0, "top_delta": 0, "limit_v": 0, "limit_delta": 0, "limit_v2" : 0, "top_v2" : 0, "affected_side": "na", "affected_level": -1}
     order_book["aggr_seq"] = {"top_delta": 0, "limit_delta": 0}
     order_book["implied_only"] = False
 
 
 def reset_aggr_seq(order_book):
     order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
     order_book["implied_only"] = False
 
 
 def reflect_price_update_in_version(side: str, price: float,str_time_of_event,order_book: dict):
     level = get_price_level(side, price, order_book)
-    #order_book["aggr_seq"]["affected_side"] = side
-    #order_book["aggr_seq"]["affected_level"] = level
 
     max_levels = order_book["aggr_max_levels"]
     if level <= max_levels:
-        #order_book["aggr_seq"]["limit_v"] += 1
         order_book["aggr_seq"]["limit_delta"] = 1
     if level == 1:
-        #order_book["aggr_seq"]["top_v"] += 1
         order_book["aggr_seq"]["top_delta"] = 1
 
     order_book["time_of_event"] = str_time_of_event
 
-        #order_book["aggr_seq"]["limit_v2"] = 0
-        #order_book["aggr_seq"]["limit_v2"] = 0
-    #else:
-    #    if str_time_of_event == order_book["time_of_event"]:
-    #        if level <= max_levels:
-    #            order_book["aggr_seq"]["limit_v2"] += 1
-    #        if level == 1:
-    #            order_book["aggr_seq"]["top_v2"] += 1
-    #    else:
-     #       order_book["time_of_event"] = str_time_of_event
-     #       if level <= max_levels:
-     #           order_book["aggr_seq"]["limit_v2"] = 0
-     #       else:
-     #           order_book["aggr_seq"]["limit_v2"] = -1
-     #       if level == 1:
-     #           order_book["aggr_seq"]["top_v2"] = 0
-     #       else:
-     #           order_book["aggr_seq"]["top_v2"] = -1
-
 
 def ob_add_order(order_id: str, price: float, size: int, side: str, str_time_of_event ,order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
```

### Comparing `recon_lw-2.0.0.dev5309756614/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5311495845/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5309756614/recon_lw/recon_ob_stats.py` & `recon_lw-2.0.0.dev5311495845/recon_lw/recon_ob_stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,15 +77,16 @@
             )
         processors.append(processor)
 
     streams = recon_lw.open_scoped_events_streams(source_ob_events_path, lambda n: "default_" not in n)
     streams2 = recon_lw.open_streams(source_stat_messages_path,
                                      lambda n: any(s in n for s in all_stat_sessions),
                                      expanded_messages=True)
-    streams.extend(streams2)
+    for elem in streams2:
+        streams.add(elem)
 
     message_buffer = [None] * 100
     buffer_len = 100
     while len(streams) > 0:
         next_batch_len = recon_lw.get_next_batch(streams, message_buffer, buffer_len, get_timestamp)
         buffer_to_process = message_buffer
         if next_batch_len < buffer_len:
```

### Comparing `recon_lw-2.0.0.dev5309756614/setup.py` & `recon_lw-2.0.0.dev5311495845/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5309756614/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5311495845/test/test_recon_ob.py`

 * *Files identical despite different names*

