# Comparing `tmp/recon_lw-2.0.0.dev5222793001.tar.gz` & `tmp/recon_lw-2.0.0.dev5309756614.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5222793001.tar", last modified: Fri Jun  9 14:10:15 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5309756614.tar", last modified: Mon Jun 19 08:47:29 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5222793001.tar` & `recon_lw-2.0.0.dev5309756614.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:10:15.000000 recon_lw-2.0.0.dev5222793001/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-09 14:09:35.000000 recon_lw-2.0.0.dev5222793001/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-09 14:10:15.000000 recon_lw-2.0.0.dev5222793001/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-09 14:09:35.000000 recon_lw-2.0.0.dev5222793001/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-09 14:09:57.000000 recon_lw-2.0.0.dev5222793001/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:10:15.000000 recon_lw-2.0.0.dev5222793001/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-09 14:09:35.000000 recon_lw-2.0.0.dev5222793001/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-06-09 14:09:35.000000 recon_lw-2.0.0.dev5222793001/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-09 14:09:35.000000 recon_lw-2.0.0.dev5222793001/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-09 14:09:35.000000 recon_lw-2.0.0.dev5222793001/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-09 14:09:35.000000 recon_lw-2.0.0.dev5222793001/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-06-09 14:09:35.000000 recon_lw-2.0.0.dev5222793001/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    32850 2023-06-09 14:09:35.000000 recon_lw-2.0.0.dev5222793001/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    22335 2023-06-09 14:09:35.000000 recon_lw-2.0.0.dev5222793001/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:10:15.000000 recon_lw-2.0.0.dev5222793001/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-09 14:10:15.000000 recon_lw-2.0.0.dev5222793001/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-06-09 14:10:15.000000 recon_lw-2.0.0.dev5222793001/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 14:10:15.000000 recon_lw-2.0.0.dev5222793001/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-09 14:10:15.000000 recon_lw-2.0.0.dev5222793001/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-09 14:10:15.000000 recon_lw-2.0.0.dev5222793001/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-09 14:09:35.000000 recon_lw-2.0.0.dev5222793001/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-09 14:10:15.000000 recon_lw-2.0.0.dev5222793001/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-09 14:09:35.000000 recon_lw-2.0.0.dev5222793001/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:10:15.000000 recon_lw-2.0.0.dev5222793001/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-09 14:09:35.000000 recon_lw-2.0.0.dev5222793001/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 08:47:29.000000 recon_lw-2.0.0.dev5309756614/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-19 08:47:29.000000 recon_lw-2.0.0.dev5309756614/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-19 08:46:58.000000 recon_lw-2.0.0.dev5309756614/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 08:47:29.000000 recon_lw-2.0.0.dev5309756614/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4942 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36026 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/recon_lw/recon_ob_cross_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5995 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/recon_lw/recon_ob_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 08:47:29.000000 recon_lw-2.0.0.dev5309756614/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-19 08:47:29.000000 recon_lw-2.0.0.dev5309756614/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      481 2023-06-19 08:47:29.000000 recon_lw-2.0.0.dev5309756614/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-19 08:47:29.000000 recon_lw-2.0.0.dev5309756614/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-19 08:47:29.000000 recon_lw-2.0.0.dev5309756614/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-19 08:47:29.000000 recon_lw-2.0.0.dev5309756614/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-19 08:47:29.000000 recon_lw-2.0.0.dev5309756614/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 08:47:29.000000 recon_lw-2.0.0.dev5309756614/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-19 08:46:36.000000 recon_lw-2.0.0.dev5309756614/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5222793001/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5309756614/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5222793001/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5309756614/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5222793001/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5309756614/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5222793001/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5309756614/recon_lw/recon_lw.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,23 +307,27 @@
             scopes_streams[scope] += Data.from_cache_file(path.join(streams_path, f))
     for strm in scopes_streams.values():
         ts0 = {"epochSecond": 0, "nano": 0}
         streams.add((ts0, iter(strm), None))
     return streams
 
 
-def open_streams(streams_path, name_filter=None):
+def open_streams(streams_path, name_filter=None, expanded_messages=False):
     streams = SortedKeyList(key=lambda t: time_stamp_key(t[0]))
     files = listdir(streams_path)
     for f in files:
         if ".pickle" not in f:
             continue
         if name_filter is not None and not name_filter(f):
             continue
-        stream = Data.from_cache_file(path.join(streams_path, f))
+        data_object = Data.from_cache_file(path.join(streams_path, f))
+        if expanded_messages:
+            stream = (mm for m in data_object for mm in message_utils.expand_message(m))
+        else:
+            stream = Data.from_cache_file(path.join(streams_path, f))
         ts0 = {"epochSecond": 0, "nano": 0}
         streams.add((ts0, iter(stream), None))
 
     return streams
 
 
 def get_next_batch(streams, batch, b_len, get_timestamp_func):
```

### Comparing `recon_lw-2.0.0.dev5222793001/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5309756614/recon_lw/recon_ob.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from datetime import datetime, timedelta
 from sortedcontainers import SortedKeyList
 from th2_data_services.utils.message_utils import message_utils
 from recon_lw import recon_lw
+from th2_data_services.utils import time as time_utils
 import copy
 
 
 def sequence_cache_add(seq_num: int, ts: dict, m: dict, sequence_cache: dict) -> None:
     seq_element = (seq_num, m)
     sequence = sequence_cache["sequence"]
     # gaps = sequence_cache["gaps"]
@@ -16,14 +17,17 @@
         last_elem = sequence[-1]
         first_elem = sequence[0]
         if seq_num > last_elem[0]:
             sequence.add(seq_element)
             sequence.update([(i, gap) for i in range(last_elem[0] + 1, seq_num)])
             times.add((ts, seq_num))
         elif seq_num < first_elem[0]:
+            #  radical difference means sequence Reset
+            if first_elem[0] - seq_num > 500:
+                raise Exception(f'Stream break detected: got{seq_num} vs {first_elem[0]}')
             sequence.update([(i, gap) for i in range(seq_num + 1, first_elem[0])])
             sequence.add(seq_element)
             times.add((ts, seq_num))
         else:
             if "gap" in sequence[seq_num - first_elem[0]][1]:
                 del sequence[seq_num - first_elem[0]]
                 sequence.add(seq_element)
@@ -289,15 +293,22 @@
     sequence_timestamp_extract = rule_dict["sequence_timestamp_extract"]
     for m in next_batch:
         seq_list = sequence_timestamp_extract(m)
 
         # seq, ts = sequence_timestamp_extract(m)
         if seq_list is not None:
             for mess, seq, ts in seq_list:
-                sequence_cache_add(seq, ts, mess, sequence_cache)
+                try:
+                    sequence_cache_add(seq, ts, mess, sequence_cache)
+                except Exception as e:
+                    print("Critical Error Detected: ", e)
+                    print("sequence:  ", seq)
+                    print("timestamp:  ", time_utils.extract_timestamp(ts))
+                    print("mess:  ", mess)
+                    raise e
 
 
 def flush_ob_stream(ts: dict, rule_settings: dict, event_sequence: dict, save_events_func) -> None:
     seq_batch = flush_sequence_get_collection(ts, rule_settings["horizon_delay"], rule_settings["sequence_cache"])
     n_processed = process_ob_rules(seq_batch,
                                    rule_settings["books_cache"],
                                    rule_settings["get_book_id"],
@@ -537,15 +548,17 @@
     order_book["implied_only"] = (real_num_orders == 0)
 
     result_body = {}
     max_levels = order_book["aggr_max_levels"]
     side_key = side + "_aggr"
     new_index = level - 1
     if not 0 <= new_index <= len(order_book[side_key]):
-        result_body["error"] = "Unexpected level {0}, against existing {1}".format(level, len(order_book[side_key]))
+        result_body["error"] = "Unexpected level {0}, against existing {1} levels on {2} side".format(level,
+                                                                                                      len(order_book[side_key]),
+                                                                                                      side_key)
         return result_body, []
 
     new_level = {"price": price, "real_qty": real_qty, "real_num_orders": real_num_orders, "impl_qty": impl_qty,
                  "impl_num_orders": impl_num_orders}
     order_book[side_key].insert(new_index, new_level)
     if len(order_book[side_key]) == max_levels + 1:
         order_book[side_key].pop()
@@ -563,16 +576,17 @@
     else:
         reset_aggr_seq(order_book)
 
     result_body = {}
     side_key = side + "_aggr"
     del_index = level - 1
     if not 0 <= del_index < len(order_book[side_key]):
-        result_body["error"] = "Unexpected level {0}, against existing {1}".format(level, len(order_book[side_key]))
-        return result_body, []
+        result_body["error"] = "Unexpected level {0}, against existing {1} levels on {2} side".format(level,
+                                                                                                      len(order_book[side_key]),
+                                                                                                      side_key)
 
     #is it purely implied
     order_book["implied_only"] = (order_book[side_key][del_index]["real_num_orders"] == 0)
 
     order_book[side_key].pop(del_index)
 
     order_book["aggr_seq"]["top_delta"] = (del_index == 0)
@@ -591,15 +605,17 @@
         reset_aggr_seq(order_book)
 
     result_body = {}
     max_levels = order_book["aggr_max_levels"]
     side_key = side + "_aggr"
     update_index = level - 1
     if not 0 <= update_index < len(order_book[side_key]):
-        result_body["error"] = "Unexpected level {0}, against existing {1}".format(level, len(order_book[side_key]))
+        result_body["error"] = "Unexpected level {0}, against existing {1} levels on {2} side".format(level,
+                                                                                                      len(order_book[side_key]),
+                                                                                                      side_key)
         return result_body, []
 
     #is it purely implied
     order_book["implied_only"] = (order_book[side_key][update_index]["real_num_orders"] == real_num_orders) and \
                                  (order_book[side_key][update_index]["real_qty"] == real_qty)
 
 
@@ -648,25 +664,29 @@
 
     update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["top_delta"] = 1
 
     return {}, [copy.deepcopy(order_book)]
 
 
-def ob_indicative_market_data_trade(trade_price: float, str_time_of_event, order_book: dict):
+def ob_market_data_trade(trade_price: float, str_time_of_event, order_book: dict):
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
 
     order_book["last_price"] = trade_price
     if trade_price > order_book["max_price"]:
         order_book["max_price"] = trade_price
     if trade_price < order_book["min_price"]:
         order_book["min_price"] = trade_price
+    if "total_n_trades" not in order_book:
+        order_book["total_n_trades"] = 1
+    else:
+        order_book["total_n_trades"] += 1
 
     update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["top_delta"] = 0
     order_book["aggr_seq"]["limit_delta"] = 0
 
     return {}, [copy.deepcopy(order_book)]
 
@@ -760,7 +780,57 @@
     order_book["bid_real_n_orders"] = bid_real_n_orders
     order_book["bid_impl_n_orders"] = bid_impl_n_orders
 
     update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["top_delta"] = 1
 
     return {}, [copy.deepcopy(order_book)]
+
+
+def display_l1(order_book):
+    header = ["bid_price", "bid_real_qty", "bid_impl_qty", "bid_real_n_orders", "bid_impl_n_orders",
+              "ask_price", "ask_real_qty", "ask_impl_qty", "ask_real_n_orders", "ask_impl_n_orders"]
+    data = [order_book[col] for col in header]
+    return [header, data]
+
+
+def display_l2(order_book):
+    header = ["bid_price", "bid_real_qty", "bid_impl_qty", "bid_real_num_orders", "bid_impl_num_orders",
+              "ask_price", "ask_real_qty", "ask_impl_qty", "ask_real_num_orders", "ask_impl_num_orders"]
+    result = [header]
+    levels = max(len(order_book["bid_aggr"]), len(order_book["ask_aggr"]))
+    keys = ["bid_aggr","bid_aggr"]
+    shifts = [0,5]
+    for i in range(levels):
+        line = []
+        for key, shift in zip(keys, shifts):
+            if i < len(order_book[key]):
+                for j in range(5):
+                    line.append(order_book[key][i][header[j+shift]])
+            else:
+                line.extend([None]*5)
+        result.append(line)
+    return result
+
+
+def display_l3(order_book):
+    header = ["bid_price", "bid_qty", "bid_order_id",
+              "ask_price", "ask_qty", "ask_order_id"]
+    result = [header]
+    bid_prices = list(order_book["bid"])
+    bid_prices.sort()
+    bid_items = [[p, q, o_id] for p in bid_prices for o_id,q in order_book["bid"][p].items()]
+    ask_items = [[p, q, o_id] for p in bid_prices for o_id,q in order_book["ask"][p].items()]
+    levels = max(len(bid_items), len(ask_items))
+    for i in range(levels):
+        line = []
+        if i < len(bid_items):
+            line.extend(bid_items[i])
+        else:
+            line.extend([None]*3)
+        if i < len(ask_items):
+            line.extend(ask_items[i])
+        else:
+            line.extend([None]*3)
+        result.append(line)
+    return result
+
```

### Comparing `recon_lw-2.0.0.dev5222793001/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5309756614/recon_lw/recon_ob_cross_stream.py`

 * *Files 5% similar despite different names*

```diff
@@ -184,38 +184,38 @@
     return None, None, None
 
 
 def ob_compare_interpret_match_aggr(match, custom_settings, create_event, save_events):
     if match[0] is not None and match[1] is not None:
         comp_res = compare_full_vs_aggr(match[0]["body"], match[1]["body"])
         if len(comp_res) > 0:
-            error_event = create_event("StreamMismatchAggr",
-                                       "StreamMismatchAggr",
+            error_event = create_event("23:mismatch",
+                                       "23:mismatch",
                                        False,
                                        {"full_book_event": match[0]["eventId"],
                                         "aggr_book_event": match[1]["eventId"],
                                         "book_id": match[0]["body"]["book_id"],
                                         "time_of_event": match[0]["body"]["time_of_event"],
                                         "limit_v2": match[0]["body"]["aggr_seq"]["limit_v2"],
                                         "errors": comp_res})
             save_events([error_event])
     elif match[0] is not None:
         tech_info = ob_compare_get_timestamp_key1_key2_aggr(match[0], custom_settings)
-        error_event = create_event("StreamMismatchNoAggr",
-                                   "StreamMismatchNoAggr",
+        error_event = create_event("23:missing2",
+                                   "23:missing2",
                                    False,
                                    {"full_book_event": match[0]["eventId"],
                                     "book_id": match[0]["body"]["book_id"],
                                     "time_of_event": match[0]["body"]["time_of_event"],
                                     "limit_v2": match[0]["body"]["aggr_seq"]["limit_v2"],
                                     "sessionId": match[0]["body"]["sessionId"],
                                     "tech_info": tech_info})
         save_events([error_event])
     elif match[1] is not None:
-        e_type = "StreamMismatchNoFullvsAggrImpl" if match[1]["body"]["implied_only"] else "StreamMismatchNoFullvsAggr"
+        e_type = "23:missing3 impl" if match[1]["body"]["implied_only"] else "23:missing3"
         error_event = create_event(e_type,
                                    e_type,
                                    False,
                                    {"aggr_book_event": match[1]["eventId"],
                                     "book_id": match[1]["body"]["book_id"],
                                     "time_of_event": match[1]["body"]["time_of_event"],
                                    "limit_v2": match[1]["body"]["aggr_seq"]["limit_v2"],
@@ -223,36 +223,36 @@
         save_events([error_event])
 
 
 def ob_compare_interpret_match_top(match, custom_settings, create_event, save_events):
     if match[0] is not None and match[1] is not None:
         comp_res = compare_full_vs_top(match[0]["body"], match[1]["body"])
         if len(comp_res) > 0:
-            error_event = create_event("StreamMismatchTop",
-                                       "StreamMismatchTop",
+            error_event = create_event("13:mismatch",
+                                       "13:mismatch",
                                        False,
                                        {"full_book_event": match[0]["eventId"],
                                         "top_book_event": match[1]["eventId"],
                                         "book_id": match[0]["body"]["book_id"],
                                         "time_of_event": match[0]["body"]["time_of_event"],
                                         "top_v2": match[0]["body"]["aggr_seq"]["top_v2"],
                                         "errors": comp_res})
             save_events([error_event])
     elif match[0] is not None:
-        error_event = create_event("StreamMismatchNoTop",
-                                   "StreamMismatchNoTop",
+        error_event = create_event("13:missing1",
+                                   "13:missing1",
                                    False,
                                    {"full_book_event": match[0]["eventId"],
                                     "book_id": match[0]["body"]["book_id"],
                                     "time_of_event": match[0]["body"]["time_of_event"],
                                     "top_v2": match[0]["body"]["aggr_seq"]["top_v2"],
                                     "sessionId": match[0]["body"]["sessionId"]})
         save_events([error_event])
     elif match[1] is not None:
-        e_type = "StreamMismatchNoFullvsTopImpl" if match[1]["body"]["implied_only"] else "StreamMismatchNoFullvsTop"
+        e_type = "13:missing3 impl" if match[1]["body"]["implied_only"] else "13:missing3"
         error_event = create_event(e_type,
                                    e_type,
                                    False,
                                    {"top_book_event": match[1]["eventId"],
                                     "book_id": match[1]["body"]["book_id"],
                                     "time_of_event": match[1]["body"]["time_of_event"],
                                     "top_v2": match[1]["body"]["aggr_seq"]["top_v2"],
@@ -260,37 +260,37 @@
         save_events([error_event])
 
 
 def ob_compare_interpret_match_top_aggr(match, custom_settings, create_event, save_events):
     if match[0] is not None and match[1] is not None:
         comp_res = compare_aggr_vs_top(match[1]["body"], match[0]["body"])
         if len(comp_res) > 0:
-            error_event = create_event("StreamMismatchTopAggr",
-                                       "StreamMismatchTopAggr",
+            error_event = create_event("12:mismatch",
+                                       "12:mismatch",
                                        False,
                                        {"top_book_event": match[0]["eventId"],
                                         "aggr_book_event": match[1]["eventId"],
                                         "book_id": match[0]["body"]["book_id"],
                                         "time_of_event": match[0]["body"]["time_of_event"],
                                         "top_v2": match[0]["body"]["aggr_seq"]["top_v2"],
                                         "errors": comp_res})
             save_events([error_event])
     elif match[0] is not None:
-        error_event = create_event("StreamMismatchNoAggrVsTop",
-                                   "StreamMismatchNoAggrVsTop",
+        error_event = create_event("12:missing2",
+                                   "12:missing2",
                                    False,
                                    {"top_book_event": match[0]["eventId"],
                                     "book_id": match[0]["body"]["book_id"],
                                     "time_of_event": match[0]["body"]["time_of_event"],
                                     "top_v2": match[0]["body"]["aggr_seq"]["top_v2"],
                                     "sessionId": match[0]["body"]["sessionId"]})
         save_events([error_event])
     elif match[1] is not None:
-        error_event = create_event("StreamMismatchNoTopVsAggr",
-                                   "StreamMismatchNoTopVsAggr",
+        error_event = create_event("12:missing1",
+                                   "12:missing1",
                                    False,
                                    {"aggr_book_event": match[1]["eventId"],
                                     "book_id": match[1]["body"]["book_id"],
                                     "time_of_event": match[1]["body"]["time_of_event"],
                                     "limit_v2": match[1]["body"]["aggr_seq"]["limit_v2"],
                                     "sessionId": match[1]["body"]["sessionId"]})
         save_events([error_event])
```

### Comparing `recon_lw-2.0.0.dev5222793001/setup.py` & `recon_lw-2.0.0.dev5309756614/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5222793001/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5309756614/test/test_recon_ob.py`

 * *Files identical despite different names*

