# Comparing `tmp/breeze_strategies-6.0.tar.gz` & `tmp/breeze_strategies-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breeze_strategies-6.0.tar", last modified: Fri Jun 16 10:00:09 2023, max compression
+gzip compressed data, was "breeze_strategies-6.0.1.tar", last modified: Mon Jun 19 08:00:15 2023, max compression
```

## Comparing `breeze_strategies-6.0.tar` & `breeze_strategies-6.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 10:00:09.883008 breeze_strategies-6.0/
--rw-rw-rw-   0        0        0     1113 2023-06-15 05:40:22.000000 breeze_strategies-6.0/LICENSE
--rw-rw-rw-   0        0        0     1470 2023-06-16 10:00:09.870088 breeze_strategies-6.0/PKG-INFO
--rw-rw-rw-   0        0        0      921 2023-06-16 10:00:00.000000 breeze_strategies-6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 10:00:08.835977 breeze_strategies-6.0/breeze_strategies/
--rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-6.0/breeze_strategies/__init__.py
--rw-rw-rw-   0        0        0    15678 2023-06-16 09:59:48.000000 breeze_strategies-6.0/breeze_strategies/breeze_strategies.py
-drwxrwxrwx   0        0        0        0 2023-06-16 10:00:09.867038 breeze_strategies-6.0/breeze_strategies.egg-info/
--rw-rw-rw-   0        0        0     1470 2023-06-16 10:00:08.000000 breeze_strategies-6.0/breeze_strategies.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-16 10:00:08.000000 breeze_strategies-6.0/breeze_strategies.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 10:00:08.000000 breeze_strategies-6.0/breeze_strategies.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-16 10:00:08.000000 breeze_strategies-6.0/breeze_strategies.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-16 10:00:08.000000 breeze_strategies-6.0/breeze_strategies.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 10:00:09.885007 breeze_strategies-6.0/setup.cfg
--rw-rw-rw-   0        0        0      815 2023-06-16 09:59:55.000000 breeze_strategies-6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:00:15.241980 breeze_strategies-6.0.1/
+-rw-rw-rw-   0        0        0     1113 2023-06-15 05:40:22.000000 breeze_strategies-6.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1135 2023-06-19 08:00:15.239978 breeze_strategies-6.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2023-06-19 07:58:59.000000 breeze_strategies-6.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 08:00:15.171666 breeze_strategies-6.0.1/breeze_strategies/
+-rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-6.0.1/breeze_strategies/__init__.py
+-rw-rw-rw-   0        0        0    18069 2023-06-19 07:58:03.000000 breeze_strategies-6.0.1/breeze_strategies/breeze_strategies.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:00:15.235990 breeze_strategies-6.0.1/breeze_strategies.egg-info/
+-rw-rw-rw-   0        0        0     1135 2023-06-19 08:00:15.000000 breeze_strategies-6.0.1/breeze_strategies.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-19 08:00:15.000000 breeze_strategies-6.0.1/breeze_strategies.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 08:00:15.000000 breeze_strategies-6.0.1/breeze_strategies.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-19 08:00:15.000000 breeze_strategies-6.0.1/breeze_strategies.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-19 08:00:15.000000 breeze_strategies-6.0.1/breeze_strategies.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 08:00:15.241980 breeze_strategies-6.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      817 2023-06-19 07:59:05.000000 breeze_strategies-6.0.1/setup.py
```

### Comparing `breeze_strategies-6.0/LICENSE` & `breeze_strategies-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `breeze_strategies-6.0/PKG-INFO` & `breeze_strategies-6.0.1/breeze_strategies.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: breeze_strategies
-Version: 6.0
+Name: breeze-strategies
+Version: 6.0.1
 Summary: ICICIDIRECT's breezeconnect strategies in python
 Home-page: https://github.com/Idirect-Tech/python_strategies/tree/master
 Author: ICICI Direct Breeze
 Author-email: breezeapi@icicisecurities.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,31 +17,28 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==6.0
+pip install breeze_strategies==6.0.1
 
 ```
 
 
 ## code usage
 
 ```python
 
 from breeze_strategies import Strategies
 
 
 obj = Strategies(app_key = "your app key",secret_key = "your secret key",api_session = "your api session",max_profit = "your max profit",max_loss = "your max loss")
 obj.long_straddle(stock_code = "NIFTY",strike_price = "18700",qty = "50",expiry_date = "2023-06-15T06:00:00.000Z")
-obj.stop()
+obj.stop() #for disconnection and exit of current strategy
 obj.get_pnl()
-obj.squareoff(exchange_code = "exchange_code", stock_code = "stock_code", product_type = "product_type", expiry_date = "expiry_date", strike_price = "strike_price", action = "buy", order_type = "market" , validity = "validity", stoploss, quantity = "quantity" , price = "executed price",validity_date = "validity_date", trade_password = "", disclosed_quantity = "0",right = "Call")
-
-
 
 ```
```

### Comparing `breeze_strategies-6.0/breeze_strategies/breeze_strategies.py` & `breeze_strategies-6.0.1/breeze_strategies/breeze_strategies.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,14 +20,23 @@
         self.currentcall = 0
         self.currentput = 0
         self.flag = False
         self.client = BreezeConnect(app_key)
         self.client.generate_session(secret_key,api_session)
         self.client.ws_connect()
         self.quantity = 0
+        self.exchange_code = ""
+        self.stock_code = ""
+        self.product_type = ""
+        self.expiry_date = ""
+        self.strike_price = ""
+        self.order_type = ""
+        self.validity = ""
+        self.stoploss = ""
+        self.validity_date = ""
     
     def squareoff(self,exchange_code, stock_code, product_type, expiry_date, strike_price, action, order_type, validity, stoploss, quantity, price,validity_date, trade_password, disclosed_quantity,right):
         data = self.client.square_off(exchange_code=exchange_code,
                             product="options",
                             stock_code=stock_code,
                             expiry_date=expiry_date,
                             right=right,
@@ -63,34 +72,35 @@
         month = expiry_date[5:7]
         day = expiry_date[8:10]
         formatted_date = f"{day}-{month_names[month]}-{year}"
         return(formatted_date)
         
     def trigger(self,product_type, rightval, stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, call_execution,put_execution):
         net_gain_loss = (self.currentcall + self.currentput)*int(quantity)
-        print(f"net gain/loss received : {net_gain_loss}/- Rs")
+        print(f"net gain/loss  : {round(net_gain_loss,2)}/- Rs")
+        print("-------------------------------------------------------------------")
         formatted_date = self.get_date_format(expiry_date)
 
         if(net_gain_loss > 0 and net_gain_loss >= self.maxprofit):
             print("maxprofit has reached...")
             print("SquareOff operation on both contracts call and put begins....")
             
-            self.squareoff(exchange_code, stock_code, product_type, expiry_date, strike_price, order_type, validity, stoploss, quantity, call_price, validity_date, "", disclosed_quantity="0",right = "Call",action = "buy")
-            self.squareoff(exchange_code, stock_code, product_type, expiry_date, strike_price , order_type, validity, stoploss, quantity, put_price, validity_date, "", disclosed_quantity="0",right = "Put", action = "buy")
+            self.squareoff(exchange_code, stock_code, product_type, expiry_date, strike_price, order_type, validity, stoploss, quantity, validity_date, "", disclosed_quantity="0",right = "Call",action = "sell", price = "")
+            self.squareoff(exchange_code, stock_code, product_type, expiry_date, strike_price , order_type, validity, stoploss, quantity, validity_date, "", disclosed_quantity="0",right = "Put", action = "sell", price = "")
             
             self.client.unsubscribe_feeds(exchange_code=exchange_code, stock_code=stock_code, product_type="options", expiry_date= formatted_date, strike_price=strike_price, right="Call", get_exchange_quotes=True, get_market_depth=False)
             self.client.unsubscribe_feeds(exchange_code=exchange_code, stock_code=stock_code, product_type="options", expiry_date= formatted_date, strike_price=strike_price, right="Put", get_exchange_quotes=True, get_market_depth=False)
-            print("-------------END--------------")
+            print("-------------END------------------")
             self.flag = True
             return
         if(net_gain_loss < 0 and net_gain_loss <= self.maxloss):
             print("maxloss has reached...")
             print("SquareOff operation on both contracts call and put begins....")
-            self.squareoff(exchange_code, stock_code, product_type, expiry_date, strike_price, order_type, validity, stoploss, quantity, call_price, validity_date, "", disclosed_quantity="0",right = "Call",action = "buy")
-            self.squareoff(exchange_code, stock_code, product_type, expiry_date, strike_price, order_type, validity, stoploss, quantity, put_price, validity_date, "", disclosed_quantity="0",right = "Put",action = "buy")
+            self.squareoff(exchange_code, stock_code, product_type, expiry_date, strike_price, order_type, validity, stoploss, quantity, validity_date, "", disclosed_quantity="0",right = "Call",action = "sell",price = "")
+            self.squareoff(exchange_code, stock_code, product_type, expiry_date, strike_price, order_type, validity, stoploss, quantity, validity_date, "", disclosed_quantity="0",right = "Put",action = "sell",price = "")
 
             self.client.unsubscribe_feeds(exchange_code=exchange_code, stock_code=stock_code, product_type="options", expiry_date= formatted_date, strike_price=strike_price, right="Call", get_exchange_quotes=True, get_market_depth=False)
             self.client.unsubscribe_feeds(exchange_code=exchange_code, stock_code=stock_code, product_type="options", expiry_date= formatted_date, strike_price=strike_price, right="Put", get_exchange_quotes=True, get_market_depth=False)
             print("---------------END-----------------")
             self.flag = True
             return
 
@@ -101,34 +111,48 @@
         
         def on_ticks(data):
             
             value = data
             
             if(value['right'] == "Call"):
                 self.currentcall = round(float(value['last']) - float(call_execution), 2)
-                print(f"current Call gain  : {self.currentcall}/- Rs")
+                print(f"P & L (CALL)  : {self.currentcall * int(self.quantity)}/- Rs")
+                print("-------------------------------------------------------------------")
                 if(self.flag == False):
                     self.trigger(product_type, "Call", stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,call_execution,put_execution)
             
             if(value['right'] == "Put"):
                 self.currentput = round(float(value['last']) - float(put_execution), 2)
-                print(f"current Put gain :  {self.currentput}/- Rs")
+                print(f"P & L (PUT) :  {self.currentput * int(self.quantity)}/- Rs")
+                print("-------------------------------------------------------------------")
                 if(self.flag == False):
                     self.trigger(product_type, "Put", stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,call_execution,put_execution)
             
         self.client.on_ticks = on_ticks
         self.client.subscribe_feeds(exchange_code = exchange_code, stock_code = stock_code, product_type = product_type, expiry_date= formatted_date, strike_price=strike_price, right = "Call", get_exchange_quotes=True, get_market_depth=False)
         self.client.subscribe_feeds(exchange_code = exchange_code, stock_code = stock_code, product_type = product_type, expiry_date= formatted_date, strike_price=strike_price, right = "Put", get_exchange_quotes=True, get_market_depth=False) 
 
         
     def profit_and_loss(self,product_type, stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, orderids,call_execution,put_execution):
         self.calculate_current(product_type, stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, call_execution, put_execution,False)
             
     def long_straddle(self, stock_code, strike_price, qty, expiry_date, stoploss = "", put_price = "0", call_price = "0",product_type = "options", order_type = "market", validity = "day", validity_date = datetime.utcnow().strftime('%Y-%m-%dT%H:%M:%S.%fZ'), exchange_code = "NFO"):
+        
         self.quantity = qty
+        self.exchange_code = exchange_code 
+        self.stock_code = stock_code
+        self.product_type = product_type 
+        self.expiry_date = expiry_date  
+        self.strike_price = strike_price
+        self.order_type = order_type
+        self.validity = validity
+        self.stoploss = stoploss
+        self.quantity = quantity
+        self.validity_date = validity_date
+
         def place_order_method(stock_code,exchange_code,product,action,order_type,stoploss,quantity,price,validity,validity_date,expiry_date,right,strike_price,res_queue):
          
             data =  self.client.place_order(stock_code=stock_code,
                     exchange_code=exchange_code,
                     product="options",
                     action = "buy",
                     order_type=order_type,
@@ -156,125 +180,121 @@
         res_queue = queue.Queue()
         t2 = threading.Thread(target = place_order_method,args = (stock_code,exchange_code,"options","buy",order_type,stoploss,qty,put_price,validity,validity_date,expiry_date,"Put",strike_price,res_queue))
         t2.start()
         t2.join()
         secondresponse = res_queue.get()
         
         
-        #if one of the order fails then squareoff the other one which is successfull
+        #if one of the order fails then cancel the other one which is successfull
         if(firstresponse.get('Success',None)!=None and secondresponse.get('Success',None)==None):
-            
+            print("Put Order Failed....")
             order_id = firstresponse['Success']['order_id']
-            self.client.square_off(exchange_code="NFO",
-                    product = "options",
-                    stock_code = stock_code,
-                    expiry_date= expiry_date,
-                    right="Call",
-                    strike_price= strike_price,
-                    action="buy",
-                    order_type= order_type,
-                    validity = validity,
-                    stoploss="0",
-                    quantity = qty,
-                    price = price,
-                    validity_date = validity_date,
-                    trade_password="",
-                    disclosed_quantity="0")
-            
+            data  = self.client.cancel_order(exchange_code=exchange_code,
+                    order_id = order_id)
+
             if(data.get("Success",None) == None):
-                print("PUT Order SquareOff has not been successfull")
+                print("Call Order Cancellation has not been successfull")
                 print("----------END-------------------")
             else:
-                print("PUT Order SquareOff has  been successfull")
+                print("Call Order Cancellation has  been successfull")
                 print("----------END-------------------")
             
-            return("Call Order Failed...")
+            
         
         elif(secondresponse.get('Success',None)!=None and firstresponse.get('Success',None)==None):
-            
+            print("Call order failed....")
             order_id = secondresponse['Success']['order_id']
             
-            data = self.client.square_off(exchange_code="NFO",
-                    product = "options",
-                    stock_code = stock_code,
-                    expiry_date= expiry_date,
-                    right="Put",
-                    strike_price = strike_price,
-                    action="buy",
-                    order_type= order_type,
-                    validity = validity,
-                    stoploss="0",
-                    quantity = qty,
-                    price = price,
-                    validity_date = validity_date,
-                    trade_password="",
-                    disclosed_quantity="0")
+            data = self.client.cancel_order(exchange_code=exchange_code,
+                    order_id = order_id)
             
             if(data.get("Success",None) == None):
-                print("Call Order SquareOff has not been successfull")
+                print("Put Order Cancellation has not been successfull")
             else:
-                print("Call Order SquareOff has  been successfull")
-            return("Put order failed....")
+                print("Put Order Cancellation has  been successfull")
+            
         
         elif(firstresponse.get('Success',None)==None and secondresponse.get('Success',None)==None):
             print("both order call and put have failed")
             print("------------END----------------")
             
         
         else:
             orderids = [] #0th index will contain call order, #1st index will contain put order 
             orderids.append(firstresponse['Success']['order_id']) 
             orderids.append(secondresponse['Success']['order_id'])            
             #define a mechanism to get profit and loss
-            print("----lets wait for 15 seconds for getting the executed status---")
-            time.sleep(15)
+            print("----lets wait for 5 seconds for getting the executed status---")
+            time.sleep(5)
             details = self.client.get_order_detail(exchange_code=exchange_code,
                         order_id= orderids[0])
-            print(details)
+
+            call_status = None
+            put_status = None
+
+            #print(details)
             call_execution = -1
             put_execution = -1
             
             print(f"order ids are : {orderids}")
             for entry in details['Success']:
                 if(entry['status'] == "Executed"):
                     call_execution = entry['average_price']
+                    call_status = "Executed"
                     break
                     
             details = self.client.get_order_detail(exchange_code=exchange_code,
                         order_id= orderids[1])
-            print(details)
+            #print(details)
             for entry in details['Success']:
                 if(entry['status'] == "Executed"):
                     put_execution = entry['average_price']
+                    put_status = "Executed"
                     break
                     
             if(call_execution == -1 or put_execution == -1):
                 print("Dear User order could not execute within time limit ..cancelling it")
                 if(call_execution == -1 and put_execution == -1):
-                    pass
+                    print("Both Order Call and Put could not execute to so cancelling it ..... ")
+                    self.client.cancel_order(exchange_code=exchange_code,
+                    order_id = orderids[0])
+                    self.client.cancel_order(exchange_code=exchange_code,
+                    order_id = orderids[1])
 
                 elif(call_execution == -1):
                     #call cancel order api
                     print("call order could not execute due to some reason so cancelling order")
                     #self.squareoff(self,rightval,exchange_code, stock_code, product_type, expiry_date, right, strike_price, action, order_type, validity, stoploss, quantity, price,validity_date, trade_password, disclosed_quantity)
                     self.client.cancel_order(exchange_code=exchange_code,
                     order_id = orderids[0])
-                    
+
+                    print("put order is executed squaring off....")
+                    self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Put", action = "sell")
+
                 elif(put_execution == -1):
                     #call cancel order api
                     print("put order could not execute due to some reason so cancelling order")
                     status = self.client.cancel_order(exchange_code=exchange_code,
                     order_id = orderids[1])
+                    print("call order is executed squaring off....")
+                    self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Call", action = "sell")
                     
             else:
                 print("Call order got executed at price :{0} Rs and Put Order got executed at price : {1} Rs".format(call_execution,put_execution))
                 self.profit_and_loss(product_type, stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, orderids,call_execution,put_execution)
             
     def stop(self):
+
+        print("squaring off the contract and exiting strategy...")
+        self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Call", action = "sell")
+        self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Put", action = "sell")
+
         self.client.ws_disconnect()
 
     def get_pnl(self):
         print("- Negative indicates loss")
-        print(f"current call gain/loss per qty {self.currentcall}/- Rs")
-        print(f"current put gain/loss per qty {self.currentput}/- Rs")
+        print(f" P & L(CALL):  {self.currentcall}/- Rs")
+        print(f" P & L(PUT):  {self.currentput}/- Rs")
         outcome = (self.currentcall + self.currentput)*int(self.quantity)
         print(f"Total Profit/Loss for {self.quantity} is {outcome}/- Rs")
+
+        print("------------------------------------------------------------------------------")
```

### Comparing `breeze_strategies-6.0/breeze_strategies.egg-info/PKG-INFO` & `breeze_strategies-6.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: breeze-strategies
-Version: 6.0
+Name: breeze_strategies
+Version: 6.0.1
 Summary: ICICIDIRECT's breezeconnect strategies in python
 Home-page: https://github.com/Idirect-Tech/python_strategies/tree/master
 Author: ICICI Direct Breeze
 Author-email: breezeapi@icicisecurities.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,31 +17,28 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==6.0
+pip install breeze_strategies==6.0.1
 
 ```
 
 
 ## code usage
 
 ```python
 
 from breeze_strategies import Strategies
 
 
 obj = Strategies(app_key = "your app key",secret_key = "your secret key",api_session = "your api session",max_profit = "your max profit",max_loss = "your max loss")
 obj.long_straddle(stock_code = "NIFTY",strike_price = "18700",qty = "50",expiry_date = "2023-06-15T06:00:00.000Z")
-obj.stop()
+obj.stop() #for disconnection and exit of current strategy
 obj.get_pnl()
-obj.squareoff(exchange_code = "exchange_code", stock_code = "stock_code", product_type = "product_type", expiry_date = "expiry_date", strike_price = "strike_price", action = "buy", order_type = "market" , validity = "validity", stoploss, quantity = "quantity" , price = "executed price",validity_date = "validity_date", trade_password = "", disclosed_quantity = "0",right = "Call")
-
-
 
 ```
```

### Comparing `breeze_strategies-6.0/setup.py` & `breeze_strategies-6.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="breeze_strategies",
-    version="6.0",
+    version="6.0.1",
     author="ICICI Direct Breeze",
     author_email="breezeapi@icicisecurities.com",
     description="ICICIDIRECT's breezeconnect strategies in python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['breeze_connect==1.0.37','nest_asyncio'],
     url="https://github.com/Idirect-Tech/python_strategies/tree/master",
```

