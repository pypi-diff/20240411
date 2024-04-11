# Comparing `tmp/AsyncPayments-1.4.1.tar.gz` & `tmp/AsyncPayments-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AsyncPayments-1.4.1.tar", last modified: Sat Mar 23 08:23:39 2024, max compression
+gzip compressed data, was "AsyncPayments-1.4.2.tar", last modified: Thu Apr 11 20:39:24 2024, max compression
```

## Comparing `AsyncPayments-1.4.1.tar` & `AsyncPayments-1.4.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-03-23 08:23:39.083926 AsyncPayments-1.4.1/
-drwxrwxrwx   0        0        0        0 2024-03-23 08:23:38.856516 AsyncPayments-1.4.1/AsyncPayments/
--rw-rw-rw-   0        0        0        0 2023-12-28 23:00:34.000000 AsyncPayments-1.4.1/AsyncPayments/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-23 08:23:38.908453 AsyncPayments-1.4.1/AsyncPayments/aaio/
--rw-rw-rw-   0        0        0       26 2023-12-26 23:20:58.000000 AsyncPayments-1.4.1/AsyncPayments/aaio/__init__.py
--rw-rw-rw-   0        0        0     8004 2024-03-23 08:21:44.000000 AsyncPayments-1.4.1/AsyncPayments/aaio/api.py
--rw-rw-rw-   0        0        0     1689 2024-01-16 12:10:35.000000 AsyncPayments-1.4.1/AsyncPayments/aaio/models.py
-drwxrwxrwx   0        0        0        0 2024-03-23 08:23:38.954821 AsyncPayments-1.4.1/AsyncPayments/cryptoBot/
--rw-rw-rw-   0        0        0       31 2023-12-27 20:19:43.000000 AsyncPayments-1.4.1/AsyncPayments/cryptoBot/__init__.py
--rw-rw-rw-   0        0        0    17487 2024-01-03 21:56:52.000000 AsyncPayments-1.4.1/AsyncPayments/cryptoBot/api.py
--rw-rw-rw-   0        0        0     1964 2023-12-30 01:52:20.000000 AsyncPayments-1.4.1/AsyncPayments/cryptoBot/models.py
-drwxrwxrwx   0        0        0        0 2024-03-23 08:23:39.008469 AsyncPayments-1.4.1/AsyncPayments/crystalPay/
--rw-rw-rw-   0        0        0       32 2023-12-27 00:02:38.000000 AsyncPayments-1.4.1/AsyncPayments/crystalPay/__init__.py
--rw-rw-rw-   0        0        0    13934 2024-01-03 21:56:52.000000 AsyncPayments-1.4.1/AsyncPayments/crystalPay/api.py
--rw-rw-rw-   0        0        0     3113 2023-12-30 01:52:20.000000 AsyncPayments-1.4.1/AsyncPayments/crystalPay/models.py
-drwxrwxrwx   0        0        0        0 2024-03-23 08:23:39.018444 AsyncPayments-1.4.1/AsyncPayments/exceptions/
--rw-rw-rw-   0        0        0       34 2023-12-26 22:50:08.000000 AsyncPayments-1.4.1/AsyncPayments/exceptions/__init__.py
--rw-rw-rw-   0        0        0       88 2024-01-09 16:36:13.000000 AsyncPayments-1.4.1/AsyncPayments/exceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-03-23 08:23:39.053883 AsyncPayments-1.4.1/AsyncPayments/lolz/
--rw-rw-rw-   0        0        0       43 2023-12-28 21:57:07.000000 AsyncPayments-1.4.1/AsyncPayments/lolz/__init__.py
--rw-rw-rw-   0        0        0     6460 2024-02-28 14:34:32.000000 AsyncPayments-1.4.1/AsyncPayments/lolz/api.py
--rw-rw-rw-   0        0        0      222 2023-12-30 01:52:20.000000 AsyncPayments-1.4.1/AsyncPayments/lolz/models.py
--rw-rw-rw-   0        0        0     2573 2024-01-09 11:57:47.000000 AsyncPayments-1.4.1/AsyncPayments/requests.py
-drwxrwxrwx   0        0        0        0 2024-03-23 08:23:39.081931 AsyncPayments-1.4.1/AsyncPayments/ruKassa/
--rw-rw-rw-   0        0        0       29 2024-01-03 21:42:57.000000 AsyncPayments-1.4.1/AsyncPayments/ruKassa/__init__.py
--rw-rw-rw-   0        0        0     6558 2024-01-16 11:58:18.000000 AsyncPayments-1.4.1/AsyncPayments/ruKassa/api.py
--rw-rw-rw-   0        0        0      744 2024-01-04 15:25:38.000000 AsyncPayments-1.4.1/AsyncPayments/ruKassa/models.py
-drwxrwxrwx   0        0        0        0 2024-03-23 08:23:39.082928 AsyncPayments-1.4.1/AsyncPayments.egg-info/
--rw-rw-rw-   0        0        0     7875 2024-03-23 08:23:38.000000 AsyncPayments-1.4.1/AsyncPayments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      816 2024-03-23 08:23:38.000000 AsyncPayments-1.4.1/AsyncPayments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-23 08:23:38.000000 AsyncPayments-1.4.1/AsyncPayments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-03-23 08:23:38.000000 AsyncPayments-1.4.1/AsyncPayments.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-23 08:23:38.000000 AsyncPayments-1.4.1/AsyncPayments.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1080 2023-12-28 23:17:29.000000 AsyncPayments-1.4.1/LICENSE
--rw-rw-rw-   0        0        0     7875 2024-03-23 08:23:39.082928 AsyncPayments-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     6802 2024-03-23 08:21:44.000000 AsyncPayments-1.4.1/README.md
--rw-rw-rw-   0        0        0     1209 2024-03-23 08:21:44.000000 AsyncPayments-1.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-23 08:23:39.083926 AsyncPayments-1.4.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-11 20:39:24.458159 AsyncPayments-1.4.2/
+drwxrwxrwx   0        0        0        0 2024-04-11 20:39:24.420248 AsyncPayments-1.4.2/AsyncPayments/
+-rw-rw-rw-   0        0        0        0 2024-03-30 19:36:47.000000 AsyncPayments-1.4.2/AsyncPayments/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 20:39:24.434210 AsyncPayments-1.4.2/AsyncPayments/aaio/
+-rw-rw-rw-   0        0        0       26 2024-03-30 19:36:47.000000 AsyncPayments-1.4.2/AsyncPayments/aaio/__init__.py
+-rw-rw-rw-   0        0        0     7777 2024-03-30 19:36:47.000000 AsyncPayments-1.4.2/AsyncPayments/aaio/api.py
+-rw-rw-rw-   0        0        0     1635 2024-04-11 20:35:33.000000 AsyncPayments-1.4.2/AsyncPayments/aaio/models.py
+drwxrwxrwx   0        0        0        0 2024-04-11 20:39:24.436205 AsyncPayments-1.4.2/AsyncPayments/cryptoBot/
+-rw-rw-rw-   0        0        0       31 2024-03-30 19:36:47.000000 AsyncPayments-1.4.2/AsyncPayments/cryptoBot/__init__.py
+-rw-rw-rw-   0        0        0    17152 2024-03-30 19:36:47.000000 AsyncPayments-1.4.2/AsyncPayments/cryptoBot/api.py
+-rw-rw-rw-   0        0        0     1883 2024-03-30 19:36:47.000000 AsyncPayments-1.4.2/AsyncPayments/cryptoBot/models.py
+drwxrwxrwx   0        0        0        0 2024-04-11 20:39:24.437202 AsyncPayments-1.4.2/AsyncPayments/crystalPay/
+-rw-rw-rw-   0        0        0       32 2024-03-30 19:36:47.000000 AsyncPayments-1.4.2/AsyncPayments/crystalPay/__init__.py
+-rw-rw-rw-   0        0        0    13571 2024-03-30 19:36:47.000000 AsyncPayments-1.4.2/AsyncPayments/crystalPay/api.py
+-rw-rw-rw-   0        0        0     2973 2024-03-30 19:36:47.000000 AsyncPayments-1.4.2/AsyncPayments/crystalPay/models.py
+drwxrwxrwx   0        0        0        0 2024-04-11 20:39:24.439197 AsyncPayments-1.4.2/AsyncPayments/exceptions/
+-rw-rw-rw-   0        0        0       68 2024-03-30 19:36:47.000000 AsyncPayments-1.4.2/AsyncPayments/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      127 2024-03-30 19:36:47.000000 AsyncPayments-1.4.2/AsyncPayments/exceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-11 20:39:24.441192 AsyncPayments-1.4.2/AsyncPayments/lolz/
+-rw-rw-rw-   0        0        0       43 2024-03-30 19:36:47.000000 AsyncPayments-1.4.2/AsyncPayments/lolz/__init__.py
+-rw-rw-rw-   0        0        0     6493 2024-03-30 19:36:47.000000 AsyncPayments-1.4.2/AsyncPayments/lolz/api.py
+-rw-rw-rw-   0        0        0      209 2024-03-30 19:36:47.000000 AsyncPayments-1.4.2/AsyncPayments/lolz/models.py
+-rw-rw-rw-   0        0        0     2421 2024-03-30 19:36:47.000000 AsyncPayments-1.4.2/AsyncPayments/requests.py
+drwxrwxrwx   0        0        0        0 2024-04-11 20:39:24.442191 AsyncPayments-1.4.2/AsyncPayments/ruKassa/
+-rw-rw-rw-   0        0        0       29 2024-03-30 19:36:47.000000 AsyncPayments-1.4.2/AsyncPayments/ruKassa/__init__.py
+-rw-rw-rw-   0        0        0     6371 2024-03-30 19:36:47.000000 AsyncPayments-1.4.2/AsyncPayments/ruKassa/api.py
+-rw-rw-rw-   0        0        0      701 2024-03-30 19:36:47.000000 AsyncPayments-1.4.2/AsyncPayments/ruKassa/models.py
+drwxrwxrwx   0        0        0        0 2024-04-11 20:39:24.443186 AsyncPayments-1.4.2/AsyncPayments.egg-info/
+-rw-rw-rw-   0        0        0     7845 2024-04-11 20:39:24.000000 AsyncPayments-1.4.2/AsyncPayments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      816 2024-04-11 20:39:24.000000 AsyncPayments-1.4.2/AsyncPayments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 20:39:24.000000 AsyncPayments-1.4.2/AsyncPayments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-11 20:39:24.000000 AsyncPayments-1.4.2/AsyncPayments.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-11 20:39:24.000000 AsyncPayments-1.4.2/AsyncPayments.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1080 2023-12-28 23:17:29.000000 AsyncPayments-1.4.2/LICENSE
+-rw-rw-rw-   0        0        0     7845 2024-04-11 20:39:24.457157 AsyncPayments-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6582 2024-03-30 19:36:47.000000 AsyncPayments-1.4.2/README.md
+-rw-rw-rw-   0        0        0     1209 2024-04-11 20:38:49.000000 AsyncPayments-1.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 20:39:24.458159 AsyncPayments-1.4.2/setup.cfg
```

### Comparing `AsyncPayments-1.4.1/AsyncPayments/aaio/api.py` & `AsyncPayments-1.4.2/AsyncPayments/aaio/api.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,228 +1,228 @@
-from AsyncPayments.requests import RequestsClient
-from .models import Order, OrderMethod, WithdrawalMethod, CreateWithdrawalInfo, Withdrawal, Balance
-from typing import Optional, Union, List
-from urllib.parse import urlencode
-
-import hashlib
-
-
-class AsyncAaio(RequestsClient):
-    API_HOST: str = "https://aaio.so"
-
-    def __init__(self,
-            apikey: str,
-            shopid: Optional[str] = None,
-            secretkey: Optional[str] = None,
-            ) -> None:
-        '''
-        Initialize Aaio API client
-        :param apikey: Your API Key
-        :param shopid: Your Shop ID
-        :param secretkey: Your Secretkey №1
-        '''
-        super().__init__()
-        self.__api_key = apikey
-        self.__shop_id = shopid
-        self.__secret_key = secretkey
-        self.__headers = {
-            "Accept": "application/json",
-            "X-Api-Key": self.__api_key,
-        }
-        self.__post_method = "POST"
-        self.__payment_name = "aaio"
-        self.check_values()
-
-    def check_values(self):
-        if not self.__secret_key or not self.__shop_id:
-            raise ValueError('No SecretKey or ShopID specified')
-
-    def __create_sign(self, amount: Union[float, int], currency: str, order_id: str) -> str:
-        params_for_sing = ':'.join(map(
-            str,
-            [self.__shop_id, amount, currency, self.__secret_key, order_id])
-        )
-
-        return hashlib.sha256(params_for_sing.encode('utf-8')).hexdigest()
-
-    async def create_payment_url(
-            self,
-            amount: float,
-            order_id: Union[int, str],
-            currency: Optional[str] = 'RUB',
-            method: Optional[str] = None,
-            desc: Optional[str] = None,
-            email: Optional[str] = None,
-            lang: Optional[str] = None,
-            referal: Optional[str] = None,
-            us_key: Optional[str] = None,
-    ) -> str:
-
-        """Generate payment url.
-
-        Docs: https://wiki.aaio.so/priem-platezhei/sozdanie-zakaza
-
-        :param amount: Order amount.
-        :param order_id: Order number, which unique in your system, up to 16 characters, without spaces (aA-zZ, 0-9, :, -, _, [, ] , |)
-        :param currency: Currency. Default to 'RUB' (RUB, UAH, EUR, USD)
-        :param method: Payment Aaio system code name
-        :param desc: Order description
-        :param email: Buyer mail
-        :param lang: Interface language. Default to 'ru' (ru, en)
-        :param referal: Referral code
-        :param us_key: Parameter that you want to get in the notification"""
-
-        params = {
-            'merchant_id': self.__shop_id,
-            'amount': amount,
-            'order_id': order_id,
-            'currency': currency,
-            'method': method,
-            'desc': desc,
-            'email': email,
-            'lang': lang,
-            'referal': referal,
-            'us_key': us_key,
-            'sign': self.__create_sign(amount, currency, order_id),
-        }
-
-        for key, value in params.copy().items():
-            if value is None:
-                params.pop(key)
-
-        return f"{self.API_HOST}/merchant/pay?" + urlencode(params)
-
-    async def get_balance(self) -> Balance:
-        """Get available, referal and hold balance.
-
-        Docs: https://wiki.aaio.so/api/poluchenie-balansa"""
-
-        url = f'{self.API_HOST}/api/balance'
-
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers)
-
-        return Balance(**response)
-
-    async def get_order_info(self,
-                           order_id: Union[int, str]
-                           ) -> Order:
-
-        """Get information about an order by OrderID.
-
-        Docs: https://wiki.aaio.so/api/informaciya-o-zakaze
-
-        :param order_id: OrderID (in your system)"""
-
-        url = f'{self.API_HOST}/api/info-pay'
-
-        params = {
-            'merchant_id': self.__shop_id,
-            'order_id': order_id,
-        }
-
-        for key, value in params.copy().items():
-            if value is None:
-                params.pop(key)
-
-        response = await self._request(self.__payment_name, self.__post_method, url, data=params, headers=self.__headers)
-
-        return Order(**response)
-
-    async def get_withdrawal_methods(self,
-                                method: Optional[str] = None
-                                ) -> Union[List[WithdrawalMethod], WithdrawalMethod]:
-
-        """Get available methods for withdrawal.
-
-        If method is None -> return dict with all methods.
-
-        If a specific method -> return info about only this method.
-
-        Docs: https://wiki.aaio.so/api/dostupnye-metody-dlya-vyvoda-sredstv
-
-        :param method: Specific method. Default is None"""
-
-        url = f'{self.API_HOST}/api/methods-payoff'
-
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers)
-
-        if method is not None:
-            return WithdrawalMethod(**response['list'][method])
-        return [WithdrawalMethod(**method) for method in response["list"].values()]
-
-    async def get_order_methods(self,
-                           method: Optional[str] = None
-                           ) -> Union[List[OrderMethod], OrderMethod]:
-
-        """Get available methods for order.
-
-        If method is None -> return dict with all methods.
-
-        If a specific method -> return info about only this method.
-
-        Docs: https://wiki.aaio.so/api/dostupnye-metody-dlya-sozdaniya-zakaza
-
-        :param method: Specific method. Default is None"""
-
-        url = f'{self.API_HOST}/api/methods-pay'
-
-        params = {
-            'merchant_id': self.__shop_id,
-        }
-
-        response = await self._request(self.__payment_name, self.__post_method, url, data=params, headers=self.__headers)
-
-        if method is not None:
-            return OrderMethod.model_validate(response['list'][method])
-        return [OrderMethod(**method) for method in response["list"].values()]
-
-    async def get_withdrawal_info(self,
-                                my_id: Union[int, str],
-                                ) -> Withdrawal:
-
-        """Get information about a withdrawal by WithdrawalID.
-
-        Docs: https://wiki.aaio.so/api/informaciya-o-zayavke-na-vyvod-sredstv
-
-        :param my_id: WithdrawalID (in your system)"""
-
-        url = f'{self.API_HOST}/api/info-payoff'
-
-        params = {
-            'my_id': my_id,
-        }
-
-        response = await self._request(self.__payment_name, self.__post_method, url, data=params, headers=self.__headers)
-
-        return Withdrawal(**response)
-
-    async def create_withdrawal(self,
-                               my_id: Union[int, str],
-                               method: str,
-                               amount: float,
-                               wallet: str,
-                               commission_type: Optional[int] = 0
-                               ) -> CreateWithdrawalInfo:
-
-        """Create withdrawal.
-
-        Docs: https://wiki.aaio.so/api/vyvod-sredstv
-
-        :param my_id: WithdrawalID (in your system)
-        :param method: Specific method for withdrawal
-        :param amount: Withdrawal amount
-        :param wallet: Wallet or number for withdrawal (Without +, " ", and separators)
-        :param commission_type: Withdrawal commission type. Default to 0 (from the payment amount)"""
-
-        url = f'{self.API_HOST}/api/create-payoff'
-
-        params = {
-            'my_id': my_id,
-            'method': method,
-            'amount': amount,
-            'wallet': wallet,
-            'commission_type': commission_type,
-        }
-
-        response = await self._request(self.__payment_name, self.__post_method, url, data=params, headers=self.__headers)
-
+from AsyncPayments.requests import RequestsClient
+from .models import Order, OrderMethod, WithdrawalMethod, CreateWithdrawalInfo, Withdrawal, Balance
+from typing import Optional, Union, List
+from urllib.parse import urlencode
+
+import hashlib
+
+
+class AsyncAaio(RequestsClient):
+    API_HOST: str = "https://aaio.so"
+
+    def __init__(self,
+            apikey: str,
+            shopid: Optional[str] = None,
+            secretkey: Optional[str] = None,
+            ) -> None:
+        '''
+        Initialize Aaio API client
+        :param apikey: Your API Key
+        :param shopid: Your Shop ID
+        :param secretkey: Your Secretkey №1
+        '''
+        super().__init__()
+        self.__api_key = apikey
+        self.__shop_id = shopid
+        self.__secret_key = secretkey
+        self.__headers = {
+            "Accept": "application/json",
+            "X-Api-Key": self.__api_key,
+        }
+        self.__post_method = "POST"
+        self.__payment_name = "aaio"
+        self.check_values()
+
+    def check_values(self):
+        if not self.__secret_key or not self.__shop_id:
+            raise ValueError('No SecretKey or ShopID specified')
+
+    def __create_sign(self, amount: Union[float, int], currency: str, order_id: str) -> str:
+        params_for_sing = ':'.join(map(
+            str,
+            [self.__shop_id, amount, currency, self.__secret_key, order_id])
+        )
+
+        return hashlib.sha256(params_for_sing.encode('utf-8')).hexdigest()
+
+    async def create_payment_url(
+            self,
+            amount: float,
+            order_id: Union[int, str],
+            currency: Optional[str] = 'RUB',
+            method: Optional[str] = None,
+            desc: Optional[str] = None,
+            email: Optional[str] = None,
+            lang: Optional[str] = None,
+            referal: Optional[str] = None,
+            us_key: Optional[str] = None,
+    ) -> str:
+
+        """Generate payment url.
+
+        Docs: https://wiki.aaio.so/priem-platezhei/sozdanie-zakaza
+
+        :param amount: Order amount.
+        :param order_id: Order number, which unique in your system, up to 16 characters, without spaces (aA-zZ, 0-9, :, -, _, [, ] , |)
+        :param currency: Currency. Default to 'RUB' (RUB, UAH, EUR, USD)
+        :param method: Payment Aaio system code name
+        :param desc: Order description
+        :param email: Buyer mail
+        :param lang: Interface language. Default to 'ru' (ru, en)
+        :param referal: Referral code
+        :param us_key: Parameter that you want to get in the notification"""
+
+        params = {
+            'merchant_id': self.__shop_id,
+            'amount': amount,
+            'order_id': order_id,
+            'currency': currency,
+            'method': method,
+            'desc': desc,
+            'email': email,
+            'lang': lang,
+            'referal': referal,
+            'us_key': us_key,
+            'sign': self.__create_sign(amount, currency, order_id),
+        }
+
+        for key, value in params.copy().items():
+            if value is None:
+                params.pop(key)
+
+        return f"{self.API_HOST}/merchant/pay?" + urlencode(params)
+
+    async def get_balance(self) -> Balance:
+        """Get available, referal and hold balance.
+
+        Docs: https://wiki.aaio.so/api/poluchenie-balansa"""
+
+        url = f'{self.API_HOST}/api/balance'
+
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers)
+
+        return Balance(**response)
+
+    async def get_order_info(self,
+                           order_id: Union[int, str]
+                           ) -> Order:
+
+        """Get information about an order by OrderID.
+
+        Docs: https://wiki.aaio.so/api/informaciya-o-zakaze
+
+        :param order_id: OrderID (in your system)"""
+
+        url = f'{self.API_HOST}/api/info-pay'
+
+        params = {
+            'merchant_id': self.__shop_id,
+            'order_id': order_id,
+        }
+
+        for key, value in params.copy().items():
+            if value is None:
+                params.pop(key)
+
+        response = await self._request(self.__payment_name, self.__post_method, url, data=params, headers=self.__headers)
+
+        return Order(**response)
+
+    async def get_withdrawal_methods(self,
+                                method: Optional[str] = None
+                                ) -> Union[List[WithdrawalMethod], WithdrawalMethod]:
+
+        """Get available methods for withdrawal.
+
+        If method is None -> return dict with all methods.
+
+        If a specific method -> return info about only this method.
+
+        Docs: https://wiki.aaio.so/api/dostupnye-metody-dlya-vyvoda-sredstv
+
+        :param method: Specific method. Default is None"""
+
+        url = f'{self.API_HOST}/api/methods-payoff'
+
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers)
+
+        if method is not None:
+            return WithdrawalMethod(**response['list'][method])
+        return [WithdrawalMethod(**method) for method in response["list"].values()]
+
+    async def get_order_methods(self,
+                           method: Optional[str] = None
+                           ) -> Union[List[OrderMethod], OrderMethod]:
+
+        """Get available methods for order.
+
+        If method is None -> return dict with all methods.
+
+        If a specific method -> return info about only this method.
+
+        Docs: https://wiki.aaio.so/api/dostupnye-metody-dlya-sozdaniya-zakaza
+
+        :param method: Specific method. Default is None"""
+
+        url = f'{self.API_HOST}/api/methods-pay'
+
+        params = {
+            'merchant_id': self.__shop_id,
+        }
+
+        response = await self._request(self.__payment_name, self.__post_method, url, data=params, headers=self.__headers)
+
+        if method is not None:
+            return OrderMethod.model_validate(response['list'][method])
+        return [OrderMethod(**method) for method in response["list"].values()]
+
+    async def get_withdrawal_info(self,
+                                my_id: Union[int, str],
+                                ) -> Withdrawal:
+
+        """Get information about a withdrawal by WithdrawalID.
+
+        Docs: https://wiki.aaio.so/api/informaciya-o-zayavke-na-vyvod-sredstv
+
+        :param my_id: WithdrawalID (in your system)"""
+
+        url = f'{self.API_HOST}/api/info-payoff'
+
+        params = {
+            'my_id': my_id,
+        }
+
+        response = await self._request(self.__payment_name, self.__post_method, url, data=params, headers=self.__headers)
+
+        return Withdrawal(**response)
+
+    async def create_withdrawal(self,
+                               my_id: Union[int, str],
+                               method: str,
+                               amount: float,
+                               wallet: str,
+                               commission_type: Optional[int] = 0
+                               ) -> CreateWithdrawalInfo:
+
+        """Create withdrawal.
+
+        Docs: https://wiki.aaio.so/api/vyvod-sredstv
+
+        :param my_id: WithdrawalID (in your system)
+        :param method: Specific method for withdrawal
+        :param amount: Withdrawal amount
+        :param wallet: Wallet or number for withdrawal (Without +, " ", and separators)
+        :param commission_type: Withdrawal commission type. Default to 0 (from the payment amount)"""
+
+        url = f'{self.API_HOST}/api/create-payoff'
+
+        params = {
+            'my_id': my_id,
+            'method': method,
+            'amount': amount,
+            'wallet': wallet,
+            'commission_type': commission_type,
+        }
+
+        response = await self._request(self.__payment_name, self.__post_method, url, data=params, headers=self.__headers)
+
         return CreateWithdrawalInfo(**response)
```

### Comparing `AsyncPayments-1.4.1/AsyncPayments/aaio/models.py` & `AsyncPayments-1.4.2/AsyncPayments/aaio/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,75 +1,81 @@
-from pydantic import BaseModel
-from typing import Union, Optional
-
-
-class Balance(BaseModel):
-    balance: float
-    referral: float
-    hold: float
-
-class Order(BaseModel):
-    id: str
-    order_id: Union[int, str]
-    desc: str
-    merchant_id: str
-    merchant_domain: str
-    method: Optional[str] = None
-    amount: float
-    currency: str
-    profit: Optional[float] = None
-    commission: Optional[float] = None
-    commission_client: Optional[float] = None
-    commission_type: Optional[str] = None
-    email: Optional[str] = None
-    status: str
-    date: str
-    expired_date: str
-    complete_date: Optional[str] = None
-    us_vars: dict
-
-class OrderMethodCurrencies(BaseModel):
-    RUB: float
-    UAH: float
-    USD: float
-    EUR: float
-
-class OrderMethod(BaseModel):
-    name: str
-    min: OrderMethodCurrencies
-    max: OrderMethodCurrencies
-    commission_percent: float
-
-class Withdrawal(BaseModel):
-    id: str
-    my_id: Union[int, str]
-    method: str
-    wallet: str
-    amount: float
-    amount_down: float
-    commission: float
-    commission_type: int
-    status: str
-    cancel_message: Optional[str] = None
-    date: str
-    complete_date: Optional[str] = None
-
-class WithdrawalMethod(BaseModel):
-    name: str
-    min: float
-    max: float
-    commission_percent: float
-    commission_sum: float
-
-class CreateWithdrawalInfo(BaseModel):
-    id: str
-    my_id: Union[str, int]
-    method: str
-    wallet: str
-    amount: float
-    amount_in_currency: float
-    amount_currency: str
-    amount_rate: float
-    amount_down: float
-    commission: float
-    commission_type: int
-    status: str
+from pydantic import BaseModel
+from typing import Union, Optional
+
+
+class Balance(BaseModel):
+    balance: float
+    referral: float
+    hold: float
+
+
+class Order(BaseModel):
+    id: str
+    order_id: Union[int, str]
+    desc: str
+    merchant_id: str
+    merchant_domain: str
+    method: Optional[str] = None
+    amount: float
+    currency: str
+    profit: Optional[float] = None
+    commission: Optional[float] = None
+    commission_client: Optional[float] = None
+    commission_type: Optional[str] = None
+    email: Optional[str] = None
+    status: str
+    date: str
+    expired_date: str
+    complete_date: Optional[str] = None
+    us_vars: dict | str | list
+
+
+class OrderMethodCurrencies(BaseModel):
+    RUB: float
+    UAH: float
+    USD: float
+    EUR: float
+
+
+class OrderMethod(BaseModel):
+    name: str
+    min: OrderMethodCurrencies
+    max: OrderMethodCurrencies
+    commission_percent: float
+
+
+class Withdrawal(BaseModel):
+    id: str
+    my_id: Union[int, str]
+    method: str
+    wallet: str
+    amount: float
+    amount_down: float
+    commission: float
+    commission_type: int
+    status: str
+    cancel_message: Optional[str] = None
+    date: str
+    complete_date: Optional[str] = None
+
+
+class WithdrawalMethod(BaseModel):
+    name: str
+    min: float
+    max: float
+    commission_percent: float
+    commission_sum: float
+
+
+class CreateWithdrawalInfo(BaseModel):
+    id: str
+    my_id: Union[str, int]
+    method: str
+    wallet: str
+    amount: float
+    amount_in_currency: float
+    amount_currency: str
+    amount_rate: float
+    amount_down: float
+    commission: float
+    commission_type: int
+    status: str
```

### Comparing `AsyncPayments-1.4.1/AsyncPayments/cryptoBot/api.py` & `AsyncPayments-1.4.2/AsyncPayments/cryptoBot/api.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,336 +1,336 @@
-from AsyncPayments.requests import RequestsClient
-from typing import Optional, Union, List
-
-from .models import Invoice, MeInfo, Transfer, Balance, Check, ExchangeRate, Currency
-
-
-class AsyncCryptoBot(RequestsClient):
-    API_HOST: str = "https://t.me/Cryptobot"
-
-    def __init__(self, token: str) -> None:
-        """
-        Initialize CryptoBot API client
-        :param token: Your Token
-        """
-        super().__init__()
-        self.__token = token
-        self.__headers = {
-            'Crypto-Pay-API-Token': self.__token,
-        }
-        self.__base_url = "https://pay.crypt.bot/api"
-        self.__post_method = "POST"
-        self.__payment_name = "cryptoBot"
-        self.check_values()
-
-    def check_values(self):
-        if not self.__token:
-            raise ValueError('No Token specified')
-
-    async def get_me(self) -> MeInfo:
-        """Use this method to test your app's authentication token. Requires no parameters. On success, returns basic information about an app.
-
-        Docs: https://help.crypt.bot/crypto-pay-api#getMe"""
-
-        url = f'{self.__base_url}/getMe/'
-
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers)
-
-        return MeInfo(**response['result'])
-
-    async def create_invoice(self, amount: Union[int, float], currency_type: Optional[str] = None,
-                             asset: Optional[str] = None, fiat: Optional[str] = None,
-                             accepted_assets: Optional[list] = None, description: Optional[str] = None,
-                             hidden_message: Optional[str] = None, paid_btn_name: Optional[str] = None,
-                             paid_btn_url: Optional[str] = None, payload: Optional[str] = None,
-                             allow_comments: Optional[bool] = True, allow_anonymous: Optional[bool] = True,
-                             expires_in: Optional[int] = 3600) -> Invoice:
-        """Use this method to create a new invoice.
-
-        Docs: https://help.crypt.bot/crypto-pay-api#createInvoice
-
-        :param amount: Amount of the invoice in float. For example: 125.50
-        :param currency_type: Optional. Type of the price, can be “crypto” or “fiat”. Defaults to crypto.
-        :param asset: Optional. Required if currency_type is “crypto”. Cryptocurrency alphabetic code. Supported assets: “USDT”, “TON”, “BTC”, “ETH”, “LTC”, “BNB”, “TRX” and “USDC”.
-        :param fiat: Optional. Required if currency_type is “fiat”. Fiat currency code. Supported fiat currencies: “USD”, “EUR”, “RUB”, “BYN”, “UAH”, “GBP”, “CNY”, “KZT”, “UZS”, “GEL”, “TRY”, “AMD”, “THB”, “INR”, “BRL”, “IDR”, “AZN”, “AED”, “PLN” and “ILS".
-        :param accepted_assets: Optional. List of cryptocurrency alphabetic codes separated comma. Assets which can be used to pay the invoice. Available only if currency_type is “fiat”. Supported assets: “USDT”, “TON”, “BTC”, “ETH”, “LTC”, “BNB”, “TRX” and “USDC” (and “JET” for testnet). Defaults to all currencies.
-        :param description: Optional. Description for the invoice. User will see this description when they pay the invoice. Up to 1024 characters.
-        :param hidden_message: Optional. Text of the message which will be presented to a user after the invoice is paid. Up to 2048 characters.
-        :param paid_btn_name: Optional. Label of the button which will be presented to a user after the invoice is paid. Supported names:
-viewItem – “View Item”
-openChannel – “View Channel”
-openBot – “Open Bot”
-callback – “Return”
-        :param paid_btn_url: Optional. Required if paid_btn_name is specified. URL opened using the button which will be presented to a user after the invoice is paid. You can set any callback link (for example, a success link or link to homepage). Starts with https or http.
-        :param payload: Optional. Any data you want to attach to the invoice (for example, user ID, payment ID, ect). Up to 4kb.
-        :param allow_comments: Optional. Allow a user to add a comment to the payment. Defaults to True.
-        :param allow_anonymous: Optional. Allow a user to pay the invoice anonymously. Defaults to True.
-        :param expires_in: Optional. You can set a payment time limit for the invoice in seconds. Values between 1-2678400 are accepted. Defaults to 3600
-        """
-
-
-        url = f'{self.__base_url}/createInvoice/'
-
-        if accepted_assets and type(accepted_assets) == list:
-            accepted_assets = ",".join(map(str, accepted_assets))
-
-        params = {
-            "asset": asset,
-            "amount": amount,
-            "description": description,
-            "hidden_message": hidden_message,
-            "paid_btn_name": paid_btn_name,
-            "paid_btn_url": paid_btn_url,
-            "payload": payload,
-            "allow_comments": allow_comments,
-            "allow_anonymous": allow_anonymous,
-            "expires_in": expires_in,
-            "fiat": fiat,
-            "currency_type": currency_type,
-            "accepted_assets": accepted_assets,
-        }
-
-        for key, value in params.copy().items():
-            if isinstance(value, bool):
-                params[key] = str(value).lower()
-            if value is None:
-                params.pop(key)
-
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers,
-                                       params=params)
-
-        return Invoice(**response['result'])
-
-    async def delete_invoice(self, invoice_id: int) -> bool:
-        """Use this method to delete invoices created by your app. Returns True on success.
-
-        Docs: https://help.crypt.bot/crypto-pay-api#deleteInvoice
-
-        :param invoice_id: Invoice ID"""
-
-        url = f'{self.__base_url}/deleteInvoice/'
-        params = {
-            "invoice_id": invoice_id,
-        }
-
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers,
-                                       params=params)
-
-        return bool(response['result'])
-
-    async def create_check(self, amount: Union[float, int], asset: str) -> Check:
-        """Use this method to create a new check.
-
-        Docs: https://help.crypt.bot/crypto-pay-api#createCheck
-
-        :param amount: Amount of the invoice in float. For example: 125.50
-        :param asset: Cryptocurrency alphabetic code. Supported assets: “USDT”, “TON”, “BTC”, “ETH”, “LTC”, “BNB”, “TRX” and “USDC” (and “JET” for testnet).
-        """
-
-
-        url = f'{self.__base_url}/createCheck/'
-
-        params = {
-            "amount": amount,
-            "asset": asset,
-        }
-
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers,
-                                       params=params)
-
-        return Check(**response['result'])
-
-    async def delete_check(self, check_id: int) -> bool:
-        """Use this method to delete checks created by your app. Returns True on success.
-
-        Docs: https://help.crypt.bot/crypto-pay-api#deleteCheck
-
-        :param check_id: Check ID"""
-
-        url = f'{self.__base_url}/deleteCheck/'
-
-        params = {
-            "check_id": check_id,
-        }
-
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers,
-                                       params=params)
-
-        return bool(response['result'])
-
-    async def transfer(self, user_id: int, asset: str, amount: Union[float, int], spend_id: str,
-                       comment: Optional[str] = None, disable_send_notification: Optional[bool] = False) -> Transfer:
-        """Use this method to send coins from your app's balance to a user. This method must first be enabled in the security settings of your app. Open @CryptoBot (@CryptoTestnetBot for testnet), go to CryptoPay → MyApps, choose an app, then go to Security -> Transfers... and tap Enable.
-
-        Docs: https://help.crypt.bot/crypto-pay-api#transfer
-
-        :param user_id: User ID in Telegram. User must have previously used @CryptoBot (@CryptoTestnetBot for testnet).
-        :param asset: Cryptocurrency alphabetic code. Supported assets: “USDT”, “TON”, “BTC”, “ETH”, “LTC”, “BNB”, “TRX” and “USDC” (and “JET” for testnet).
-        :parameter amount: Amount of the transfer in float. The minimum and maximum amount limits for each of the supported assets roughly correspond to 1-25000 USD. Use get_exchange_rates() to convert amounts. For example: 125.50
-        :param spend_id: Random UTF-8 string unique per transfer for idempotent requests. The same spend_id can be accepted only once from your app. Up to 64 symbols.
-        :param comment: Optional. Comment for the transfer. Users will see this comment in the notification about the transfer. Up to 1024 symbols.
-        :param disable_send_notification: Optional. Pass true to not send to the user the notification about the transfer. Defaults to false.
-        """
-
-        url = f'{self.__base_url}/transfer/'
-
-        params = {
-            "user_id": user_id,
-            "asset": asset,
-            "amount": amount,
-            "spend_id": spend_id,
-            "comment": comment,
-            "disable_send_notification": disable_send_notification,
-        }
-
-        for key, value in params.copy().items():
-            if isinstance(value, bool):
-                params[key] = str(value).lower()
-            if value is None:
-                params.pop(key)
-
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers,
-                                       params=params)
-
-        return Transfer(**response['result'])
-
-    async def get_invoices(self, asset: Optional[str] = None, fiat: Optional[str] = None,
-                           invoice_ids: Optional[list] = None, status: Optional[str] = None,
-                           offset: Optional[int] = None, count: Optional[int] = None) -> Union[Invoice, List[Invoice]]:
-        """Use this method to get invoices created by your app.
-
-        Docs: https://help.crypt.bot/crypto-pay-api#getInvoices
-
-        :param asset: Optional. Cryptocurrency alphabetic code. Supported assets: “USDT”, “TON”, “BTC”, “ETH”, “LTC”, “BNB”, “TRX” and “USDC” (and “JET” for testnet). Defaults to all currencies.
-        :param fiat: Optional. Fiat currency code. Supported fiat currencies: “USD”, “EUR”, “RUB”, “BYN”, “UAH”, “GBP”, “CNY”, “KZT”, “UZS”, “GEL”, “TRY”, “AMD”, “THB”, “INR”, “BRL”, “IDR”, “AZN”, “AED”, “PLN” and “ILS". Defaults to all currencies.
-        :param invoice_ids: Optional. List of invoice IDs.
-        :param status: Optional. Status of invoices to be returned. Available statuses: “active” and “paid”. Defaults to all statuses.
-        :param offset: Optional. Offset needed to return a specific subset of invoices. Defaults to 0.
-        :param count: Optional. Number of invoices to be returned. Values between 1-1000 are accepted. Defaults to 100.
-        """
-
-        url = f"{self.__base_url}/getInvoices"
-
-        if invoice_ids and type(invoice_ids) == list:
-            invoice_ids = ",".join(map(str, invoice_ids))
-
-        params = {
-            "asset": asset,
-            "invoice_ids": invoice_ids,
-            "fiat": fiat,
-            "status": status,
-            "offset": offset,
-            "count": count,
-        }
-
-        for key, value in params.copy().items():
-            if value is None:
-                params.pop(key)
-
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers,
-                                       params=params)
-
-        if len(response["result"]["items"]) > 0:
-            if invoice_ids and isinstance(invoice_ids, int):
-                return Invoice(**response["result"]["items"][0])
-            return [Invoice(**invoice) for invoice in response["result"]["items"]]
-
-    async def get_transfers(self, asset: Optional[str] = None, transfer_ids: Optional[list] = None,
-                            offset: Optional[int] = None, count: Optional[int] = None) -> Union[Transfer, List[Transfer]]:
-        """Use this method to get transfers created by your app.
-
-        Docs: https://help.crypt.bot/crypto-pay-api#getTransfers
-
-        :param asset: Optional. Cryptocurrency alphabetic code. Supported assets: “USDT”, “TON”, “BTC”, “ETH”, “LTC”, “BNB”, “TRX” and “USDC” (and “JET” for testnet). Defaults to all currencies.
-        :param transfer_ids: Optional. List of transfer IDs.
-        :param offset: Optional. Offset needed to return a specific subset of transfers. Defaults to 0.
-        :param count: Optional. Number of transfers to be returned. Values between 1-1000 are accepted. Defaults to 100.
-        """
-        url = f"{self.__base_url}/getTransfers"
-
-        if transfer_ids and type(transfer_ids) == list:
-            transfer_ids = ",".join(map(str, transfer_ids))
-
-        params = {
-            "asset": asset,
-            "transfer_ids": transfer_ids,
-            "offset": offset,
-            "count": count,
-        }
-
-        for key, value in params.copy().items():
-            if value is None:
-                params.pop(key)
-
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers,
-                                       params=params)
-
-        if len(response["result"]["items"]) > 0:
-            if transfer_ids and isinstance(transfer_ids, int):
-                return Transfer(**response["result"]["items"][0])
-            return [Transfer(**transfer) for transfer in response["result"]["items"]]
-
-    async def get_checks(self, asset: Optional[str] = None, check_ids: Optional[list] = None,
-                         status: Optional[str] = None, offset: Optional[int] = None,
-                         count: Optional[int] = None) -> Union[Check, List[Check]]:
-        """Use this method to get checks created by your app.
-
-        Docs: https://help.crypt.bot/crypto-pay-api#getChecks
-
-        :param asset: Optional. Cryptocurrency alphabetic code. Supported assets: “USDT”, “TON”, “BTC”, “ETH”, “LTC”, “BNB”, “TRX” and “USDC” (and “JET” for testnet). Defaults to all currencies.
-        :param check_ids: Optional. List of check IDs.
-        :param status: Optional. Status of check to be returned. Available statuses: “active” and “activated”. Defaults to all statuses.
-        :param offset: Optional. Offset needed to return a specific subset of check. Defaults to 0.
-        :param count: Optional. Number of check to be returned. Values between 1-1000 are accepted. Defaults to 100.
-        """
-        url = f"{self.__base_url}/getChecks"
-
-        if check_ids and type(check_ids) == list:
-            check_ids = ",".join(map(str, check_ids))
-
-        params = {
-            "asset": asset,
-            "check_ids": check_ids,
-            "status": status,
-            "offset": offset,
-            "count": count,
-        }
-
-        for key, value in params.copy().items():
-            if value is None:
-                params.pop(key)
-
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers,
-                                       params=params)
-
-        if len(response["result"]["items"]) > 0:
-            if check_ids and isinstance(check_ids, int):
-                return Check(**response["result"]["items"][0])
-            return [Check(**check) for check in response["result"]["items"]]
-
-    async def get_balance(self) -> List[Balance]:
-        """Use this method to get balances of your app.
-
-        Docs: https://help.crypt.bot/crypto-pay-api#getBalance"""
-        url = f"{self.__base_url}/getBalance"
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers)
-
-        return [Balance(**balance) for balance in response["result"]]
-
-    async def get_exchange_rates(self) -> List[ExchangeRate]:
-        """Use this method to get exchange rates of supported currencies.
-
-        Docs: https://help.crypt.bot/crypto-pay-api#getExchangeRates"""
-        url = f"{self.__base_url}/getExchangeRates"
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers)
-
-        return [ExchangeRate(**rate) for rate in response["result"]]
-
-    async def get_currencies(self) -> List[Currency]:
-        """Use this method to get a list of supported currencies.
-
-        Docs: https://help.crypt.bot/crypto-pay-api#getCurrencies"""
-        url = f"{self.__base_url}/getCurrencies"
-
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers)
-
+from AsyncPayments.requests import RequestsClient
+from typing import Optional, Union, List
+
+from .models import Invoice, MeInfo, Transfer, Balance, Check, ExchangeRate, Currency
+
+
+class AsyncCryptoBot(RequestsClient):
+    API_HOST: str = "https://t.me/Cryptobot"
+
+    def __init__(self, token: str) -> None:
+        """
+        Initialize CryptoBot API client
+        :param token: Your Token
+        """
+        super().__init__()
+        self.__token = token
+        self.__headers = {
+            'Crypto-Pay-API-Token': self.__token,
+        }
+        self.__base_url = "https://pay.crypt.bot/api"
+        self.__post_method = "POST"
+        self.__payment_name = "cryptoBot"
+        self.check_values()
+
+    def check_values(self):
+        if not self.__token:
+            raise ValueError('No Token specified')
+
+    async def get_me(self) -> MeInfo:
+        """Use this method to test your app's authentication token. Requires no parameters. On success, returns basic information about an app.
+
+        Docs: https://help.crypt.bot/crypto-pay-api#getMe"""
+
+        url = f'{self.__base_url}/getMe/'
+
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers)
+
+        return MeInfo(**response['result'])
+
+    async def create_invoice(self, amount: Union[int, float], currency_type: Optional[str] = None,
+                             asset: Optional[str] = None, fiat: Optional[str] = None,
+                             accepted_assets: Optional[list] = None, description: Optional[str] = None,
+                             hidden_message: Optional[str] = None, paid_btn_name: Optional[str] = None,
+                             paid_btn_url: Optional[str] = None, payload: Optional[str] = None,
+                             allow_comments: Optional[bool] = True, allow_anonymous: Optional[bool] = True,
+                             expires_in: Optional[int] = 3600) -> Invoice:
+        """Use this method to create a new invoice.
+
+        Docs: https://help.crypt.bot/crypto-pay-api#createInvoice
+
+        :param amount: Amount of the invoice in float. For example: 125.50
+        :param currency_type: Optional. Type of the price, can be “crypto” or “fiat”. Defaults to crypto.
+        :param asset: Optional. Required if currency_type is “crypto”. Cryptocurrency alphabetic code. Supported assets: “USDT”, “TON”, “BTC”, “ETH”, “LTC”, “BNB”, “TRX” and “USDC”.
+        :param fiat: Optional. Required if currency_type is “fiat”. Fiat currency code. Supported fiat currencies: “USD”, “EUR”, “RUB”, “BYN”, “UAH”, “GBP”, “CNY”, “KZT”, “UZS”, “GEL”, “TRY”, “AMD”, “THB”, “INR”, “BRL”, “IDR”, “AZN”, “AED”, “PLN” and “ILS".
+        :param accepted_assets: Optional. List of cryptocurrency alphabetic codes separated comma. Assets which can be used to pay the invoice. Available only if currency_type is “fiat”. Supported assets: “USDT”, “TON”, “BTC”, “ETH”, “LTC”, “BNB”, “TRX” and “USDC” (and “JET” for testnet). Defaults to all currencies.
+        :param description: Optional. Description for the invoice. User will see this description when they pay the invoice. Up to 1024 characters.
+        :param hidden_message: Optional. Text of the message which will be presented to a user after the invoice is paid. Up to 2048 characters.
+        :param paid_btn_name: Optional. Label of the button which will be presented to a user after the invoice is paid. Supported names:
+viewItem – “View Item”
+openChannel – “View Channel”
+openBot – “Open Bot”
+callback – “Return”
+        :param paid_btn_url: Optional. Required if paid_btn_name is specified. URL opened using the button which will be presented to a user after the invoice is paid. You can set any callback link (for example, a success link or link to homepage). Starts with https or http.
+        :param payload: Optional. Any data you want to attach to the invoice (for example, user ID, payment ID, ect). Up to 4kb.
+        :param allow_comments: Optional. Allow a user to add a comment to the payment. Defaults to True.
+        :param allow_anonymous: Optional. Allow a user to pay the invoice anonymously. Defaults to True.
+        :param expires_in: Optional. You can set a payment time limit for the invoice in seconds. Values between 1-2678400 are accepted. Defaults to 3600
+        """
+
+
+        url = f'{self.__base_url}/createInvoice/'
+
+        if accepted_assets and type(accepted_assets) == list:
+            accepted_assets = ",".join(map(str, accepted_assets))
+
+        params = {
+            "asset": asset,
+            "amount": amount,
+            "description": description,
+            "hidden_message": hidden_message,
+            "paid_btn_name": paid_btn_name,
+            "paid_btn_url": paid_btn_url,
+            "payload": payload,
+            "allow_comments": allow_comments,
+            "allow_anonymous": allow_anonymous,
+            "expires_in": expires_in,
+            "fiat": fiat,
+            "currency_type": currency_type,
+            "accepted_assets": accepted_assets,
+        }
+
+        for key, value in params.copy().items():
+            if isinstance(value, bool):
+                params[key] = str(value).lower()
+            if value is None:
+                params.pop(key)
+
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers,
+                                       params=params)
+
+        return Invoice(**response['result'])
+
+    async def delete_invoice(self, invoice_id: int) -> bool:
+        """Use this method to delete invoices created by your app. Returns True on success.
+
+        Docs: https://help.crypt.bot/crypto-pay-api#deleteInvoice
+
+        :param invoice_id: Invoice ID"""
+
+        url = f'{self.__base_url}/deleteInvoice/'
+        params = {
+            "invoice_id": invoice_id,
+        }
+
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers,
+                                       params=params)
+
+        return bool(response['result'])
+
+    async def create_check(self, amount: Union[float, int], asset: str) -> Check:
+        """Use this method to create a new check.
+
+        Docs: https://help.crypt.bot/crypto-pay-api#createCheck
+
+        :param amount: Amount of the invoice in float. For example: 125.50
+        :param asset: Cryptocurrency alphabetic code. Supported assets: “USDT”, “TON”, “BTC”, “ETH”, “LTC”, “BNB”, “TRX” and “USDC” (and “JET” for testnet).
+        """
+
+
+        url = f'{self.__base_url}/createCheck/'
+
+        params = {
+            "amount": amount,
+            "asset": asset,
+        }
+
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers,
+                                       params=params)
+
+        return Check(**response['result'])
+
+    async def delete_check(self, check_id: int) -> bool:
+        """Use this method to delete checks created by your app. Returns True on success.
+
+        Docs: https://help.crypt.bot/crypto-pay-api#deleteCheck
+
+        :param check_id: Check ID"""
+
+        url = f'{self.__base_url}/deleteCheck/'
+
+        params = {
+            "check_id": check_id,
+        }
+
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers,
+                                       params=params)
+
+        return bool(response['result'])
+
+    async def transfer(self, user_id: int, asset: str, amount: Union[float, int], spend_id: str,
+                       comment: Optional[str] = None, disable_send_notification: Optional[bool] = False) -> Transfer:
+        """Use this method to send coins from your app's balance to a user. This method must first be enabled in the security settings of your app. Open @CryptoBot (@CryptoTestnetBot for testnet), go to CryptoPay → MyApps, choose an app, then go to Security -> Transfers... and tap Enable.
+
+        Docs: https://help.crypt.bot/crypto-pay-api#transfer
+
+        :param user_id: User ID in Telegram. User must have previously used @CryptoBot (@CryptoTestnetBot for testnet).
+        :param asset: Cryptocurrency alphabetic code. Supported assets: “USDT”, “TON”, “BTC”, “ETH”, “LTC”, “BNB”, “TRX” and “USDC” (and “JET” for testnet).
+        :parameter amount: Amount of the transfer in float. The minimum and maximum amount limits for each of the supported assets roughly correspond to 1-25000 USD. Use get_exchange_rates() to convert amounts. For example: 125.50
+        :param spend_id: Random UTF-8 string unique per transfer for idempotent requests. The same spend_id can be accepted only once from your app. Up to 64 symbols.
+        :param comment: Optional. Comment for the transfer. Users will see this comment in the notification about the transfer. Up to 1024 symbols.
+        :param disable_send_notification: Optional. Pass true to not send to the user the notification about the transfer. Defaults to false.
+        """
+
+        url = f'{self.__base_url}/transfer/'
+
+        params = {
+            "user_id": user_id,
+            "asset": asset,
+            "amount": amount,
+            "spend_id": spend_id,
+            "comment": comment,
+            "disable_send_notification": disable_send_notification,
+        }
+
+        for key, value in params.copy().items():
+            if isinstance(value, bool):
+                params[key] = str(value).lower()
+            if value is None:
+                params.pop(key)
+
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers,
+                                       params=params)
+
+        return Transfer(**response['result'])
+
+    async def get_invoices(self, asset: Optional[str] = None, fiat: Optional[str] = None,
+                           invoice_ids: Optional[list] = None, status: Optional[str] = None,
+                           offset: Optional[int] = None, count: Optional[int] = None) -> Union[Invoice, List[Invoice]]:
+        """Use this method to get invoices created by your app.
+
+        Docs: https://help.crypt.bot/crypto-pay-api#getInvoices
+
+        :param asset: Optional. Cryptocurrency alphabetic code. Supported assets: “USDT”, “TON”, “BTC”, “ETH”, “LTC”, “BNB”, “TRX” and “USDC” (and “JET” for testnet). Defaults to all currencies.
+        :param fiat: Optional. Fiat currency code. Supported fiat currencies: “USD”, “EUR”, “RUB”, “BYN”, “UAH”, “GBP”, “CNY”, “KZT”, “UZS”, “GEL”, “TRY”, “AMD”, “THB”, “INR”, “BRL”, “IDR”, “AZN”, “AED”, “PLN” and “ILS". Defaults to all currencies.
+        :param invoice_ids: Optional. List of invoice IDs.
+        :param status: Optional. Status of invoices to be returned. Available statuses: “active” and “paid”. Defaults to all statuses.
+        :param offset: Optional. Offset needed to return a specific subset of invoices. Defaults to 0.
+        :param count: Optional. Number of invoices to be returned. Values between 1-1000 are accepted. Defaults to 100.
+        """
+
+        url = f"{self.__base_url}/getInvoices"
+
+        if invoice_ids and type(invoice_ids) == list:
+            invoice_ids = ",".join(map(str, invoice_ids))
+
+        params = {
+            "asset": asset,
+            "invoice_ids": invoice_ids,
+            "fiat": fiat,
+            "status": status,
+            "offset": offset,
+            "count": count,
+        }
+
+        for key, value in params.copy().items():
+            if value is None:
+                params.pop(key)
+
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers,
+                                       params=params)
+
+        if len(response["result"]["items"]) > 0:
+            if invoice_ids and isinstance(invoice_ids, int):
+                return Invoice(**response["result"]["items"][0])
+            return [Invoice(**invoice) for invoice in response["result"]["items"]]
+
+    async def get_transfers(self, asset: Optional[str] = None, transfer_ids: Optional[list] = None,
+                            offset: Optional[int] = None, count: Optional[int] = None) -> Union[Transfer, List[Transfer]]:
+        """Use this method to get transfers created by your app.
+
+        Docs: https://help.crypt.bot/crypto-pay-api#getTransfers
+
+        :param asset: Optional. Cryptocurrency alphabetic code. Supported assets: “USDT”, “TON”, “BTC”, “ETH”, “LTC”, “BNB”, “TRX” and “USDC” (and “JET” for testnet). Defaults to all currencies.
+        :param transfer_ids: Optional. List of transfer IDs.
+        :param offset: Optional. Offset needed to return a specific subset of transfers. Defaults to 0.
+        :param count: Optional. Number of transfers to be returned. Values between 1-1000 are accepted. Defaults to 100.
+        """
+        url = f"{self.__base_url}/getTransfers"
+
+        if transfer_ids and type(transfer_ids) == list:
+            transfer_ids = ",".join(map(str, transfer_ids))
+
+        params = {
+            "asset": asset,
+            "transfer_ids": transfer_ids,
+            "offset": offset,
+            "count": count,
+        }
+
+        for key, value in params.copy().items():
+            if value is None:
+                params.pop(key)
+
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers,
+                                       params=params)
+
+        if len(response["result"]["items"]) > 0:
+            if transfer_ids and isinstance(transfer_ids, int):
+                return Transfer(**response["result"]["items"][0])
+            return [Transfer(**transfer) for transfer in response["result"]["items"]]
+
+    async def get_checks(self, asset: Optional[str] = None, check_ids: Optional[list] = None,
+                         status: Optional[str] = None, offset: Optional[int] = None,
+                         count: Optional[int] = None) -> Union[Check, List[Check]]:
+        """Use this method to get checks created by your app.
+
+        Docs: https://help.crypt.bot/crypto-pay-api#getChecks
+
+        :param asset: Optional. Cryptocurrency alphabetic code. Supported assets: “USDT”, “TON”, “BTC”, “ETH”, “LTC”, “BNB”, “TRX” and “USDC” (and “JET” for testnet). Defaults to all currencies.
+        :param check_ids: Optional. List of check IDs.
+        :param status: Optional. Status of check to be returned. Available statuses: “active” and “activated”. Defaults to all statuses.
+        :param offset: Optional. Offset needed to return a specific subset of check. Defaults to 0.
+        :param count: Optional. Number of check to be returned. Values between 1-1000 are accepted. Defaults to 100.
+        """
+        url = f"{self.__base_url}/getChecks"
+
+        if check_ids and type(check_ids) == list:
+            check_ids = ",".join(map(str, check_ids))
+
+        params = {
+            "asset": asset,
+            "check_ids": check_ids,
+            "status": status,
+            "offset": offset,
+            "count": count,
+        }
+
+        for key, value in params.copy().items():
+            if value is None:
+                params.pop(key)
+
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers,
+                                       params=params)
+
+        if len(response["result"]["items"]) > 0:
+            if check_ids and isinstance(check_ids, int):
+                return Check(**response["result"]["items"][0])
+            return [Check(**check) for check in response["result"]["items"]]
+
+    async def get_balance(self) -> List[Balance]:
+        """Use this method to get balances of your app.
+
+        Docs: https://help.crypt.bot/crypto-pay-api#getBalance"""
+        url = f"{self.__base_url}/getBalance"
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers)
+
+        return [Balance(**balance) for balance in response["result"]]
+
+    async def get_exchange_rates(self) -> List[ExchangeRate]:
+        """Use this method to get exchange rates of supported currencies.
+
+        Docs: https://help.crypt.bot/crypto-pay-api#getExchangeRates"""
+        url = f"{self.__base_url}/getExchangeRates"
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers)
+
+        return [ExchangeRate(**rate) for rate in response["result"]]
+
+    async def get_currencies(self) -> List[Currency]:
+        """Use this method to get a list of supported currencies.
+
+        Docs: https://help.crypt.bot/crypto-pay-api#getCurrencies"""
+        url = f"{self.__base_url}/getCurrencies"
+
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers)
+
         return [Currency(**currency) for currency in response["result"]]
```

### Comparing `AsyncPayments-1.4.1/AsyncPayments/crystalPay/api.py` & `AsyncPayments-1.4.2/AsyncPayments/crystalPay/api.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,364 +1,364 @@
-from AsyncPayments.requests import RequestsClient
-from typing import Optional, Union
-from .models import CreatePayment, CassaInfo, PayoffCreate, Balances, TickersRate, PaymentsMethods, PayoffRequest, \
-                    PaymentInfo, GeneralStats
-
-import json
-import hashlib
-
-
-
-class AsyncCrystalPay(RequestsClient):
-    API_HOST: str = "https://crystalpay.io"
-
-    def __init__(self, login: str, secret: str, salt: str) -> None:
-        """
-        Initialize CrystalPay API client
-        :param login: Your Login
-        :param secret: Your Secret
-        :param salt: Your Salt
-        """
-        super().__init__()
-        self.__login = login
-        self.__secret = secret
-        self.__salt = salt
-        self.__headers = {
-            'Content-Type': 'application/json',
-        }
-        self.__base_url = "https://api.crystalpay.io/v2"
-        self.__post_method = "POST"
-        self.__payment_name = "crystalPay"
-        self.check_values()
-
-    def check_values(self):
-        if not self.__login or not self.__secret or not self.__salt:
-            raise ValueError('No Secret, Login or Salt specified')
-
-    async def get_cassa_info(self, hide_empty: Optional[bool]= False) -> CassaInfo:
-        """Get cash info.
-
-        Docs: https://docs.crystalpay.io/api/kassa/poluchenie-informacii-o-kasse
-
-        :param hide_empty: Hide empty balances"""
-
-        url = f'{self.__base_url}/me/info/'
-
-        params = {
-            "auth_login": self.__login,
-            "auth_secret": self.__secret,
-            "hide_empty": hide_empty,
-        }
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
-
-        return CassaInfo(**response)
-
-    async def get_balance(self) -> Balances:
-        """Get cash balance.
-
-        Docs: https://docs.crystalpay.io/api/balans/poluchenie-balansa-kassy"""
-
-        url = f'{self.__base_url}/balance/info/'
-
-        params = {
-            "auth_login": self.__login,
-            "auth_secret": self.__secret,
-        }
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
-
-        return Balances(**response['balances'])
-
-    async def get_payment_methods(self) -> PaymentsMethods:
-        """Get payment methods.
-
-        Docs: https://docs.crystalpay.io/api/metody-oplaty/poluchenie-informacii-o-metodakh-oplaty"""
-
-        url = f'{self.__base_url}/method/list/'
-
-        params = {
-            "auth_login": self.__login,
-            "auth_secret": self.__secret,
-        }
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
-
-        return PaymentsMethods(**response['methods'])
-
-    async def edit_payment_method(self, method: str, extra_commission_percent: Union[int, float], enabled: bool) -> bool:
-        """Edit payment method
-
-        Dosc: https://docs.crystalpay.io/api/metody-oplaty/izmenenie-nastroek-metoda-oplaty
-
-        :param method: Payment method, for example: LZTMARKET, BITCOIN
-        :param extra_commission_percent: Additional cash desk commission for payment method, in percent
-        :param enabled: Enable/Disable payment method
-
-        :return: True if successful, else exception BadRequest
-        """
-
-        url = f'{self.__base_url}/method/edit/'
-
-        params = {
-            "auth_login": self.__login,
-            "auth_secret": self.__secret,
-            "method": method,
-            "extra_commission_percent": extra_commission_percent,
-            "enabled": enabled,
-        }
-
-        await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
-
-        return True
-
-    async def create_payment(
-            self, amount: Union[int, float], amount_currency: Optional[str] = "RUB", required_methods: Optional[str] = None,
-            type: Optional[str] = "purchase", description: Optional[str] = None, redirect_url: Optional[str] = None,
-            callback_url: Optional[str] = None, extra: Optional[str] = None, payer_details: Optional[str] = None,
-            lifetime: Optional[int] = 60) -> CreatePayment:
-        """Generate payment url.
-
-        Docs: https://docs.crystalpay.io/api/oplata/vystavlenie-schyota
-
-        :param amount: Order amount.
-        :param amount_currency: Currency. Default to 'RUB', for example: USD, BTC, ETH
-        :param required_methods: Pre-selected payment method, for example: LZTMARKET, BITCOIN
-        :param type: Invoice type. possible options: purchase, topup
-        :param description: The description or purpose of the payment is displayed to the payer on the payment page, for example: Account purchase #12345678
-        :param redirect_url: Redirect link after payment
-        :param callback_url: Link for HTTP Callback notification after successful payment
-        :param extra: Any internal data, for example: Payment ID in your system
-        :param payer_details: Payer email
-        :param lifetime: Invoice lifetime in minutes, maximum - 4320. Default to 60"""
-
-        url = f'{self.__base_url}/invoice/create/'
-
-        params = {
-            "auth_login": self.__login,
-            "auth_secret": self.__secret,
-            "amount": amount,
-            "amount_currency": amount_currency,
-            "required_methods": required_methods,
-            "type": type,
-            "description": description,
-            "redirect_url": redirect_url,
-            "callback_url": callback_url,
-            "extra": extra,
-            "payer_details": payer_details,
-            "lifetime": lifetime,
-        }
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
-
-        return CreatePayment(**response)
-
-    async def get_payment_info(self, invoice_id: str) -> PaymentInfo:
-        """Get info about payment.
-
-        Docs: https://docs.crystalpay.io/api/oplata/poluchenie-informacii-o-schyote
-
-        :param invoice_id: Invoice ID"""
-
-        url = f'{self.__base_url}/invoice/info/'
-
-        params = {
-            "auth_login": self.__login,
-            "auth_secret": self.__secret,
-            "id": invoice_id,
-        }
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
-
-        return PaymentInfo(**response)
-
-    async def create_payoff(self, amount: Union[int, float], method: str, wallet: str, subtract_from: str,
-                            amount_currency: Optional[str] = None, callback_url: Optional[str] = None,
-                            extra: Optional[str] = None) -> PayoffCreate:
-        """Create payoff request.
-
-        Docs: https://docs.crystalpay.io/api/vyvod/sozdanie-zayavki
-
-        :param amount: Payoff amount, for example: 10, 0.0015
-        :param amount_currency: The currency of the amount is automatically converted into the currency of the withdrawal method, for example: RUB, USD, BTC
-        :param method: Payoff method, for example: LZTMARKET, BITCOIN
-        :param wallet: Recipient's wallet details
-        :param subtract_from: Where to write off the commission amount, possible options: balance, amount
-        :param callback_url: Link for HTTP Callback notification after output is complete
-        :param extra: Any internal data, for example: Payment ID in your system
-
-        More about subtract_from:
-
-        amount - The commission will be deducted from the withdrawal amount. The amount will be credited to your wallet.
-        balance - The commission will be deducted from the balance. The exact amount will be sent to your wallet."""
-
-        url = f'{self.__base_url}/payoff/create/'
-
-        signature = hashlib.sha1(str.encode(f"{amount}:{method}:{wallet}:{self.__salt}")).hexdigest()
-
-        params = {
-            "auth_login": self.__login,
-            "auth_secret": self.__secret,
-            "signature": signature,
-            "amount": amount,
-            "amount_currency": amount_currency,
-            "method": method,
-            "wallet": wallet,
-            "subtract_from": subtract_from,
-            "callback_url": callback_url,
-            "extra": extra,
-        }
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
-
-        return PayoffCreate(**response)
-
-    async def submit_payoff(self, payoff_id: str) -> PayoffRequest:
-        """Submit payoff request
-
-        Docs: https://docs.crystalpay.io/api/vyvod/podtverzhdenie-zayavki
-
-        :param payoff_id: Payoff ID"""
-
-        signature = hashlib.sha1(str.encode(f"{payoff_id}:{self.__salt}")).hexdigest()
-
-        url = f"{self.__base_url}/payoff/submit/"
-
-        params = {
-            "auth_login": self.__login,
-            "auth_secret": self.__secret,
-            "signature": signature,
-            "id": payoff_id,
-        }
-
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
-
-        return PayoffRequest(**response)
-
-
-    async def cancel_payoff(self, payoff_id: str) -> PayoffRequest:
-        """Cancel payoff request
-
-        Docs: https://docs.crystalpay.io/api/vyvod/otmena-zayavki
-
-        :param payoff_id: Payoff ID"""
-
-        signature = hashlib.sha1(str.encode(f"{payoff_id}:{self.__salt}")).hexdigest()
-
-        url = f"{self.__base_url}/payoff/cancel/"
-
-        params = {
-            "auth_login": self.__login,
-            "auth_secret": self.__secret,
-            "signature": signature,
-            "id": payoff_id,
-        }
-
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
-
-        return PayoffRequest(**response)
-
-    async def get_payoff(self, payoff_id: str) -> PayoffRequest:
-        """Get info about payoff request
-
-        Docs: https://docs.crystalpay.io/api/vyvod/poluchenie-informacii-o-zayavke
-
-        :param payoff_id: Payoff ID"""
-
-        url = f"{self.__base_url}/payoff/info/"
-
-        params = {
-            "auth_login": self.__login,
-            "auth_secret": self.__secret,
-            "id": payoff_id,
-        }
-
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
-
-        return PayoffRequest(**response)
-
-    async def get_tickers_list(self) -> list:
-        """Get a list of available currencies
-
-        Dosc: https://docs.crystalpay.io/api/valyuty/poluchenie-spiska-dostupnykh-valyut"""
-
-        url = f"{self.__base_url}/ticker/list/"
-
-        params = {
-            "auth_login": self.__login,
-            "auth_secret": self.__secret,
-        }
-
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
-
-        return list(response['tickers'])
-
-    async def get_tickers_rate(self, tickers: list) -> TickersRate:
-        """Get the exchange rate against RUB
-
-        Docs: https://docs.crystalpay.io/api/valyuty/poluchenie-kursa-valyut
-
-        :param tickers: Array of currencies, for example: [“BTC”, “LTC”]"""
-
-        url = f"{self.__base_url}/ticker/get/"
-
-        params = {
-            "auth_login": self.__login,
-            "auth_secret": self.__secret,
-            "tickers": tickers,
-        }
-
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
-
-        return TickersRate(**response)
-
-    async def get_history_payments(self, page: int, items: int) -> list:
-        """Get payment history
-
-        Docs: https://docs.crystalpay.io/api/otchyoty/poluchenie-istorii-platezhei
-
-        :param page: Page number, for example: 1, 2, 3
-        :param items: Number of elements per page, maximum - 100"""
-
-        url = f"{self.__base_url}/history/payments/"
-
-        params = {
-            "auth_login": self.__login,
-            "auth_secret": self.__secret,
-            "page": page,
-            "items": items,
-        }
-
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
-
-        return list(response['payments'])
-
-    async def get_payoff_history(self, page: int, items: int) -> list:
-        """Getting withdrawal history
-
-        Docs: https://docs.crystalpay.io/api/otchyoty/poluchenie-istorii-vyvodov
-
-        :param page: Page number, for example: 1, 2, 3
-        :param items: Number of elements per page, maximum - 100"""
-
-        url = f"{self.__base_url}/history/payoffs/"
-
-        params = {
-            "auth_login": self.__login,
-            "auth_secret": self.__secret,
-            "page": page,
-            "items": items,
-        }
-
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
-
-        return list(response['payoffs'])
-
-    async def get_general_stats(self) -> GeneralStats:
-        """Get general statistics
-
-        Dosc: https://docs.crystalpay.io/api/otchyoty/poluchenie-obshei-statistiki"""
-
-        url = f"{self.__base_url}/history/summary/"
-
-        params = {
-            "auth_login": self.__login,
-            "auth_secret": self.__secret,
-        }
-
-        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
-
+from AsyncPayments.requests import RequestsClient
+from typing import Optional, Union
+from .models import CreatePayment, CassaInfo, PayoffCreate, Balances, TickersRate, PaymentsMethods, PayoffRequest, \
+                    PaymentInfo, GeneralStats
+
+import json
+import hashlib
+
+
+
+class AsyncCrystalPay(RequestsClient):
+    API_HOST: str = "https://crystalpay.io"
+
+    def __init__(self, login: str, secret: str, salt: str) -> None:
+        """
+        Initialize CrystalPay API client
+        :param login: Your Login
+        :param secret: Your Secret
+        :param salt: Your Salt
+        """
+        super().__init__()
+        self.__login = login
+        self.__secret = secret
+        self.__salt = salt
+        self.__headers = {
+            'Content-Type': 'application/json',
+        }
+        self.__base_url = "https://api.crystalpay.io/v2"
+        self.__post_method = "POST"
+        self.__payment_name = "crystalPay"
+        self.check_values()
+
+    def check_values(self):
+        if not self.__login or not self.__secret or not self.__salt:
+            raise ValueError('No Secret, Login or Salt specified')
+
+    async def get_cassa_info(self, hide_empty: Optional[bool]= False) -> CassaInfo:
+        """Get cash info.
+
+        Docs: https://docs.crystalpay.io/api/kassa/poluchenie-informacii-o-kasse
+
+        :param hide_empty: Hide empty balances"""
+
+        url = f'{self.__base_url}/me/info/'
+
+        params = {
+            "auth_login": self.__login,
+            "auth_secret": self.__secret,
+            "hide_empty": hide_empty,
+        }
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
+
+        return CassaInfo(**response)
+
+    async def get_balance(self) -> Balances:
+        """Get cash balance.
+
+        Docs: https://docs.crystalpay.io/api/balans/poluchenie-balansa-kassy"""
+
+        url = f'{self.__base_url}/balance/info/'
+
+        params = {
+            "auth_login": self.__login,
+            "auth_secret": self.__secret,
+        }
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
+
+        return Balances(**response['balances'])
+
+    async def get_payment_methods(self) -> PaymentsMethods:
+        """Get payment methods.
+
+        Docs: https://docs.crystalpay.io/api/metody-oplaty/poluchenie-informacii-o-metodakh-oplaty"""
+
+        url = f'{self.__base_url}/method/list/'
+
+        params = {
+            "auth_login": self.__login,
+            "auth_secret": self.__secret,
+        }
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
+
+        return PaymentsMethods(**response['methods'])
+
+    async def edit_payment_method(self, method: str, extra_commission_percent: Union[int, float], enabled: bool) -> bool:
+        """Edit payment method
+
+        Dosc: https://docs.crystalpay.io/api/metody-oplaty/izmenenie-nastroek-metoda-oplaty
+
+        :param method: Payment method, for example: LZTMARKET, BITCOIN
+        :param extra_commission_percent: Additional cash desk commission for payment method, in percent
+        :param enabled: Enable/Disable payment method
+
+        :return: True if successful, else exception BadRequest
+        """
+
+        url = f'{self.__base_url}/method/edit/'
+
+        params = {
+            "auth_login": self.__login,
+            "auth_secret": self.__secret,
+            "method": method,
+            "extra_commission_percent": extra_commission_percent,
+            "enabled": enabled,
+        }
+
+        await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
+
+        return True
+
+    async def create_payment(
+            self, amount: Union[int, float], amount_currency: Optional[str] = "RUB", required_methods: Optional[str] = None,
+            type: Optional[str] = "purchase", description: Optional[str] = None, redirect_url: Optional[str] = None,
+            callback_url: Optional[str] = None, extra: Optional[str] = None, payer_details: Optional[str] = None,
+            lifetime: Optional[int] = 60) -> CreatePayment:
+        """Generate payment url.
+
+        Docs: https://docs.crystalpay.io/api/oplata/vystavlenie-schyota
+
+        :param amount: Order amount.
+        :param amount_currency: Currency. Default to 'RUB', for example: USD, BTC, ETH
+        :param required_methods: Pre-selected payment method, for example: LZTMARKET, BITCOIN
+        :param type: Invoice type. possible options: purchase, topup
+        :param description: The description or purpose of the payment is displayed to the payer on the payment page, for example: Account purchase #12345678
+        :param redirect_url: Redirect link after payment
+        :param callback_url: Link for HTTP Callback notification after successful payment
+        :param extra: Any internal data, for example: Payment ID in your system
+        :param payer_details: Payer email
+        :param lifetime: Invoice lifetime in minutes, maximum - 4320. Default to 60"""
+
+        url = f'{self.__base_url}/invoice/create/'
+
+        params = {
+            "auth_login": self.__login,
+            "auth_secret": self.__secret,
+            "amount": amount,
+            "amount_currency": amount_currency,
+            "required_methods": required_methods,
+            "type": type,
+            "description": description,
+            "redirect_url": redirect_url,
+            "callback_url": callback_url,
+            "extra": extra,
+            "payer_details": payer_details,
+            "lifetime": lifetime,
+        }
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
+
+        return CreatePayment(**response)
+
+    async def get_payment_info(self, invoice_id: str) -> PaymentInfo:
+        """Get info about payment.
+
+        Docs: https://docs.crystalpay.io/api/oplata/poluchenie-informacii-o-schyote
+
+        :param invoice_id: Invoice ID"""
+
+        url = f'{self.__base_url}/invoice/info/'
+
+        params = {
+            "auth_login": self.__login,
+            "auth_secret": self.__secret,
+            "id": invoice_id,
+        }
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
+
+        return PaymentInfo(**response)
+
+    async def create_payoff(self, amount: Union[int, float], method: str, wallet: str, subtract_from: str,
+                            amount_currency: Optional[str] = None, callback_url: Optional[str] = None,
+                            extra: Optional[str] = None) -> PayoffCreate:
+        """Create payoff request.
+
+        Docs: https://docs.crystalpay.io/api/vyvod/sozdanie-zayavki
+
+        :param amount: Payoff amount, for example: 10, 0.0015
+        :param amount_currency: The currency of the amount is automatically converted into the currency of the withdrawal method, for example: RUB, USD, BTC
+        :param method: Payoff method, for example: LZTMARKET, BITCOIN
+        :param wallet: Recipient's wallet details
+        :param subtract_from: Where to write off the commission amount, possible options: balance, amount
+        :param callback_url: Link for HTTP Callback notification after output is complete
+        :param extra: Any internal data, for example: Payment ID in your system
+
+        More about subtract_from:
+
+        amount - The commission will be deducted from the withdrawal amount. The amount will be credited to your wallet.
+        balance - The commission will be deducted from the balance. The exact amount will be sent to your wallet."""
+
+        url = f'{self.__base_url}/payoff/create/'
+
+        signature = hashlib.sha1(str.encode(f"{amount}:{method}:{wallet}:{self.__salt}")).hexdigest()
+
+        params = {
+            "auth_login": self.__login,
+            "auth_secret": self.__secret,
+            "signature": signature,
+            "amount": amount,
+            "amount_currency": amount_currency,
+            "method": method,
+            "wallet": wallet,
+            "subtract_from": subtract_from,
+            "callback_url": callback_url,
+            "extra": extra,
+        }
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
+
+        return PayoffCreate(**response)
+
+    async def submit_payoff(self, payoff_id: str) -> PayoffRequest:
+        """Submit payoff request
+
+        Docs: https://docs.crystalpay.io/api/vyvod/podtverzhdenie-zayavki
+
+        :param payoff_id: Payoff ID"""
+
+        signature = hashlib.sha1(str.encode(f"{payoff_id}:{self.__salt}")).hexdigest()
+
+        url = f"{self.__base_url}/payoff/submit/"
+
+        params = {
+            "auth_login": self.__login,
+            "auth_secret": self.__secret,
+            "signature": signature,
+            "id": payoff_id,
+        }
+
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
+
+        return PayoffRequest(**response)
+
+
+    async def cancel_payoff(self, payoff_id: str) -> PayoffRequest:
+        """Cancel payoff request
+
+        Docs: https://docs.crystalpay.io/api/vyvod/otmena-zayavki
+
+        :param payoff_id: Payoff ID"""
+
+        signature = hashlib.sha1(str.encode(f"{payoff_id}:{self.__salt}")).hexdigest()
+
+        url = f"{self.__base_url}/payoff/cancel/"
+
+        params = {
+            "auth_login": self.__login,
+            "auth_secret": self.__secret,
+            "signature": signature,
+            "id": payoff_id,
+        }
+
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
+
+        return PayoffRequest(**response)
+
+    async def get_payoff(self, payoff_id: str) -> PayoffRequest:
+        """Get info about payoff request
+
+        Docs: https://docs.crystalpay.io/api/vyvod/poluchenie-informacii-o-zayavke
+
+        :param payoff_id: Payoff ID"""
+
+        url = f"{self.__base_url}/payoff/info/"
+
+        params = {
+            "auth_login": self.__login,
+            "auth_secret": self.__secret,
+            "id": payoff_id,
+        }
+
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
+
+        return PayoffRequest(**response)
+
+    async def get_tickers_list(self) -> list:
+        """Get a list of available currencies
+
+        Dosc: https://docs.crystalpay.io/api/valyuty/poluchenie-spiska-dostupnykh-valyut"""
+
+        url = f"{self.__base_url}/ticker/list/"
+
+        params = {
+            "auth_login": self.__login,
+            "auth_secret": self.__secret,
+        }
+
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
+
+        return list(response['tickers'])
+
+    async def get_tickers_rate(self, tickers: list) -> TickersRate:
+        """Get the exchange rate against RUB
+
+        Docs: https://docs.crystalpay.io/api/valyuty/poluchenie-kursa-valyut
+
+        :param tickers: Array of currencies, for example: [“BTC”, “LTC”]"""
+
+        url = f"{self.__base_url}/ticker/get/"
+
+        params = {
+            "auth_login": self.__login,
+            "auth_secret": self.__secret,
+            "tickers": tickers,
+        }
+
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
+
+        return TickersRate(**response)
+
+    async def get_history_payments(self, page: int, items: int) -> list:
+        """Get payment history
+
+        Docs: https://docs.crystalpay.io/api/otchyoty/poluchenie-istorii-platezhei
+
+        :param page: Page number, for example: 1, 2, 3
+        :param items: Number of elements per page, maximum - 100"""
+
+        url = f"{self.__base_url}/history/payments/"
+
+        params = {
+            "auth_login": self.__login,
+            "auth_secret": self.__secret,
+            "page": page,
+            "items": items,
+        }
+
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
+
+        return list(response['payments'])
+
+    async def get_payoff_history(self, page: int, items: int) -> list:
+        """Getting withdrawal history
+
+        Docs: https://docs.crystalpay.io/api/otchyoty/poluchenie-istorii-vyvodov
+
+        :param page: Page number, for example: 1, 2, 3
+        :param items: Number of elements per page, maximum - 100"""
+
+        url = f"{self.__base_url}/history/payoffs/"
+
+        params = {
+            "auth_login": self.__login,
+            "auth_secret": self.__secret,
+            "page": page,
+            "items": items,
+        }
+
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
+
+        return list(response['payoffs'])
+
+    async def get_general_stats(self) -> GeneralStats:
+        """Get general statistics
+
+        Dosc: https://docs.crystalpay.io/api/otchyoty/poluchenie-obshei-statistiki"""
+
+        url = f"{self.__base_url}/history/summary/"
+
+        params = {
+            "auth_login": self.__login,
+            "auth_secret": self.__secret,
+        }
+
+        response = await self._request(self.__payment_name, self.__post_method, url, headers=self.__headers, data=json.dumps(params))
+
         return GeneralStats(**response)
```

### Comparing `AsyncPayments-1.4.1/AsyncPayments/crystalPay/models.py` & `AsyncPayments-1.4.2/AsyncPayments/crystalPay/models.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-from pydantic import BaseModel
-from typing import Optional
-
-
-class CassaInfo(BaseModel):
-    id: int
-    name: str
-    status_level: int
-    created_at: str
-
-class CreatePayment(BaseModel):
-    id: str
-    url: str
-    amount: float
-    type: str
-
-class Balance(BaseModel):
-    amount: float
-    currency: str
-
-class Balances(BaseModel):
-    BITCOIN: Balance
-    BITCOINCASH: Balance
-    BNBCRYPTOBOT: Balance
-    BNBSMARTCHAIN: Balance
-    BTCBANKER: Balance
-    BTCCHATEX: Balance
-    BTCCRYPTOBOT: Balance
-    CARDRUBP2P: Balance
-    CARDTRYP2P: Balance
-    DASH: Balance
-    DOGECOIN: Balance
-    ETHBANKER: Balance
-    ETHCRYPTOBOT: Balance
-    ETHEREUM: Balance
-    LITECOIN: Balance
-    LTCBANKER: Balance
-    LZTMARKET: Balance
-    POLYGON: Balance
-    TONCRYPTOBOT: Balance
-    TRON: Balance
-    USDCTRC: Balance
-    USDTBANKER: Balance
-    USDTCHATEX: Balance
-    USDTCRYPTOBOT: Balance
-    USDTTRC: Balance
-
-class PaymentMethod(BaseModel):
-    name: str
-    enabled: bool
-    extra_commission_percent: float
-    minimal_status_level: int
-    currency: str
-    commission_percent: float
-    commission: float
-
-class PaymentsMethods(BaseModel):
-    CRYSTALPAY: PaymentMethod
-    TEST: PaymentMethod
-    CARDRUBP2P: PaymentMethod
-    CARDTRYP2P: PaymentMethod
-    LZTMARKET: PaymentMethod
-    BITCOIN: PaymentMethod
-    BITCOINCASH: PaymentMethod
-    DASH: PaymentMethod
-    DOGECOIN: PaymentMethod
-    ETHEREUM: PaymentMethod
-    LITECOIN: PaymentMethod
-    BNBSMARTCHAIN: PaymentMethod
-    POLYGON: PaymentMethod
-    TRON: PaymentMethod
-    USDCTRC: PaymentMethod
-    USDTTRC: PaymentMethod
-    BNBCRYPTOBOT: PaymentMethod
-    BTCCRYPTOBOT: PaymentMethod
-    ETHCRYPTOBOT: PaymentMethod
-    TONCRYPTOBOT: PaymentMethod
-    USDTCRYPTOBOT: PaymentMethod
-
-class PaymentInfo(BaseModel):
-    id: str
-    url: str
-    state: str
-    type: str
-    method: Optional[str] = None
-    required_method: str
-    currency: str
-    service_commission: float
-    extra_commission: float
-    amount: float
-    pay_amount: float
-    remaining_amount: float
-    balance_amount: float
-    description: str
-    redirect_url: str
-    callback_url: str
-    extra: str
-    created_at: str
-    expired_at: str
-
-class PayoffCreate(BaseModel):
-    id: str
-    method: str
-    commission: float
-    amount: float
-    rub_amount: float
-    receive_amount: float
-    deduction_amount: float
-    subtract_from: str
-    currency: str
-
-class PayoffRequest(BaseModel):
-    id: str
-    state: str
-    method: str
-    currency: str
-    commission: float
-    amount: float
-    rub_amount: float
-    receive_amount: float
-    deduction_amount: float
-    subtract_from: str
-    wallet: str
-    message: str
-    callback_url: str
-    extra: str
-    created_at: str
-
-class TickersRate(BaseModel):
-    base_currency: str
-    currencies: dict
-
-class Stats(BaseModel):
-    payed_amount: float
-    total_count: int
-    payed_count: int
-
-class GeneralStats(BaseModel):
-    incoming: Stats
-    outgoing: Stats
+from pydantic import BaseModel
+from typing import Optional
+
+
+class CassaInfo(BaseModel):
+    id: int
+    name: str
+    status_level: int
+    created_at: str
+
+class CreatePayment(BaseModel):
+    id: str
+    url: str
+    amount: float
+    type: str
+
+class Balance(BaseModel):
+    amount: float
+    currency: str
+
+class Balances(BaseModel):
+    BITCOIN: Balance
+    BITCOINCASH: Balance
+    BNBCRYPTOBOT: Balance
+    BNBSMARTCHAIN: Balance
+    BTCBANKER: Balance
+    BTCCHATEX: Balance
+    BTCCRYPTOBOT: Balance
+    CARDRUBP2P: Balance
+    CARDTRYP2P: Balance
+    DASH: Balance
+    DOGECOIN: Balance
+    ETHBANKER: Balance
+    ETHCRYPTOBOT: Balance
+    ETHEREUM: Balance
+    LITECOIN: Balance
+    LTCBANKER: Balance
+    LZTMARKET: Balance
+    POLYGON: Balance
+    TONCRYPTOBOT: Balance
+    TRON: Balance
+    USDCTRC: Balance
+    USDTBANKER: Balance
+    USDTCHATEX: Balance
+    USDTCRYPTOBOT: Balance
+    USDTTRC: Balance
+
+class PaymentMethod(BaseModel):
+    name: str
+    enabled: bool
+    extra_commission_percent: float
+    minimal_status_level: int
+    currency: str
+    commission_percent: float
+    commission: float
+
+class PaymentsMethods(BaseModel):
+    CRYSTALPAY: PaymentMethod
+    TEST: PaymentMethod
+    CARDRUBP2P: PaymentMethod
+    CARDTRYP2P: PaymentMethod
+    LZTMARKET: PaymentMethod
+    BITCOIN: PaymentMethod
+    BITCOINCASH: PaymentMethod
+    DASH: PaymentMethod
+    DOGECOIN: PaymentMethod
+    ETHEREUM: PaymentMethod
+    LITECOIN: PaymentMethod
+    BNBSMARTCHAIN: PaymentMethod
+    POLYGON: PaymentMethod
+    TRON: PaymentMethod
+    USDCTRC: PaymentMethod
+    USDTTRC: PaymentMethod
+    BNBCRYPTOBOT: PaymentMethod
+    BTCCRYPTOBOT: PaymentMethod
+    ETHCRYPTOBOT: PaymentMethod
+    TONCRYPTOBOT: PaymentMethod
+    USDTCRYPTOBOT: PaymentMethod
+
+class PaymentInfo(BaseModel):
+    id: str
+    url: str
+    state: str
+    type: str
+    method: Optional[str] = None
+    required_method: str
+    currency: str
+    service_commission: float
+    extra_commission: float
+    amount: float
+    pay_amount: float
+    remaining_amount: float
+    balance_amount: float
+    description: str
+    redirect_url: str
+    callback_url: str
+    extra: str
+    created_at: str
+    expired_at: str
+
+class PayoffCreate(BaseModel):
+    id: str
+    method: str
+    commission: float
+    amount: float
+    rub_amount: float
+    receive_amount: float
+    deduction_amount: float
+    subtract_from: str
+    currency: str
+
+class PayoffRequest(BaseModel):
+    id: str
+    state: str
+    method: str
+    currency: str
+    commission: float
+    amount: float
+    rub_amount: float
+    receive_amount: float
+    deduction_amount: float
+    subtract_from: str
+    wallet: str
+    message: str
+    callback_url: str
+    extra: str
+    created_at: str
+
+class TickersRate(BaseModel):
+    base_currency: str
+    currencies: dict
+
+class Stats(BaseModel):
+    payed_amount: float
+    total_count: int
+    payed_count: int
+
+class GeneralStats(BaseModel):
+    incoming: Stats
+    outgoing: Stats
```

### Comparing `AsyncPayments-1.4.1/AsyncPayments/ruKassa/api.py` & `AsyncPayments-1.4.2/AsyncPayments/ruKassa/api.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,187 +1,187 @@
-from AsyncPayments.requests import RequestsClient
-from typing import Optional, Union
-from .models import Balance, CreatePayment, Payment, CreateWithdrawRequest, CancelWithdrawRequest, WithdrawRequest
-
-import time
-import secrets
-import random
-
-
-class AsyncRuKassa(RequestsClient):
-    API_HOST: str = "https://ruks.pro"
-
-    def __init__(self, api_token: str, shop_id: int, email: str, password: str) -> None:
-        """
-        Initialize RuKassa API client
-        :param api_token: Your RuKassa API-Token
-        :param shop_id: Your RuKassa ShopID
-        :param email: Your Email, which you pointed to RuKassa
-        :param password: Your Password, which you pointed to RuKassa
-        """
-        super().__init__()
-        self.__token = api_token
-        self.__shop_id = shop_id
-        self.__email = email
-        self.__password = password
-        self.__base_url = "https://lk.rukassa.is/api/v1"
-        self.__post_method = "POST"
-        self.__payment_name = "ruKassa"
-        self.check_values()
-
-    def check_values(self):
-        if not self.__token or not self.__shop_id or not self.__email or not self.__password:
-            raise ValueError('No Api-Token, ShopID, Email or Password specified')
-
-    async def get_balance(self) -> Balance:
-        """Get User Balance
-
-        :return: Balance Object"""
-
-        url = f'{self.__base_url}/getBalance'
-
-        params = {
-            "email": self.__email,
-            "password": self.__password,
-        }
-
-        response = await self._request(self.__payment_name, self.__post_method, url, data=params)
-
-        return Balance(**response)
-
-    def __get_random_string(self):
-        return f'{time.time()}_{secrets.token_hex(random.randint(5, 10))}'
-
-    async def create_payment(self, amount: Union[int, float], currency: Optional[str] = "RUB",
-                             method: Optional[str] = None, data: Optional[str] = None,
-                             orderId: Optional[int] = None) -> CreatePayment:
-        """Create a payment
-
-        :param amount: Amount of payment.
-        :param currency: Optional. In what currency are you specifying the amount parameter? Default RUB. Currencies: RUB, USD
-        :param method: Optional. Payment method, if you want payment to be made through a specific method. Methods: card, card_byn, card_kzt, card_uah, card_uzs, qiwi, yandexmoney, payeer, crypta, sbp,
-        :param data: Optional. String sent to the server along with a notification of a successful payment.
-        :param orderId: Optional. A unique payment number in your system. If not specified, a random string will be generated.
-
-        :return: CreatePayment object
-        """
-
-        url = f'{self.__base_url}/create'
-
-        if not orderId:
-            orderId = self.__get_random_string()
-
-        params = {
-            "shop_id": self.__shop_id,
-            "order_id": orderId,
-            "amount": amount,
-            "token": self.__token,
-            "data": data,
-            "method": method,
-            "currency": currency,
-        }
-
-        for key, value in params.copy().items():
-            if value is None:
-                params.pop(key)
-
-        response = await self._request(self.__payment_name, self.__post_method, url, data=params)
-
-        return CreatePayment(**response)
-
-    async def get_info_payment(self, id: int) -> Payment:
-        """
-        Get payment information
-
-        :param id: Transaction (entry) number in our system.
-
-        :return: Payment object
-        """
-
-        url = f"{self.__base_url}/getPayInfo"
-
-        params = {
-            "id": id,
-            "shop_id": self.__shop_id,
-            "token": self.__token,
-        }
-
-        response = await self._request(self.__payment_name, self.__post_method, url, data=params)
-
-        return Payment(**response)
-
-    async def create_withdraw(self, way: str, wallet: str, amount: Union[float, int], orderId: str = None,
-                              check_from: Optional[str] = "BASE_RUB", who_fee: Optional[int] = 0,
-                              bank: Optional[int] = None) -> CreateWithdrawRequest:
-        """
-        Create withdraw request
-
-        :param way: Payment system for withdrawal. Systems: CARD, QIWI, YOOMONEY, USDT, SBP.
-        :param wallet: The number of the wallet or card where the funds will be sent.
-        :param amount: Amount to withdraw.
-        :param orderId: ID in the merchant system.
-        :param check_from: Account for debiting funds. Default: BASE_RUB. (BASE_RUB, BASE_USD).
-        :param who_fee: Where to write off the commission. Default: 0. (0 - from account, 1 - from balance).
-        :param bank: Only for SBP. Bank number.
-
-        :return: CreateWithdrawRequest object
-        """
-
-        url = f"{self.__base_url}/createWithdraw"
-
-        params = {
-            "email": self.__email,
-            "password": self.__password,
-            "way": way,
-            "wallet": wallet,
-            "amount": amount,
-            "order_id": orderId,
-            "from": check_from,
-            "who_fee": who_fee,
-            "bank": bank,
-        }
-
-        response = await self._request(self.__payment_name, self.__post_method, url, data=params)
-
-        return CreateWithdrawRequest(**response)
-
-    async def cancel_withdraw(self, id: int) -> CancelWithdrawRequest:
-        """
-        Cancel withdraw request
-
-        :param id: Payment ID in our system.
-
-        :return: CancelWithdrawRequest object
-        """
-
-        url = f"{self.__base_url}/cancelWithdraw"
-
-        params = {
-            "email": self.__email,
-            "password": self.__password,
-            "id": id,
-        }
-
-        response = await self._request(self.__payment_name, self.__post_method, url, data=params)
-
-        return CancelWithdrawRequest(**response)
-
-    async def get_info_withdraw(self, id: int) -> WithdrawRequest:
-        """
-        Get info about withdraw request
-
-        :param id: The number of the operation (withdrawal) in our system.
-
-        :return: WithdrawRequest object
-        """
-
-        url = f"{self.__base_url}/getWithdrawInfo"
-
-        params = {
-            "token": self.__token,
-            "shop_id": self.__shop_id,
-            "id": id,
-        }
-
-        response = await self._request(self.__payment_name, self.__post_method, url, data=params)
-
-        return WithdrawRequest(**response)
+from AsyncPayments.requests import RequestsClient
+from typing import Optional, Union
+from .models import Balance, CreatePayment, Payment, CreateWithdrawRequest, CancelWithdrawRequest, WithdrawRequest
+
+import time
+import secrets
+import random
+
+
+class AsyncRuKassa(RequestsClient):
+    API_HOST: str = "https://ruks.pro"
+
+    def __init__(self, api_token: str, shop_id: int, email: str, password: str) -> None:
+        """
+        Initialize RuKassa API client
+        :param api_token: Your RuKassa API-Token
+        :param shop_id: Your RuKassa ShopID
+        :param email: Your Email, which you pointed to RuKassa
+        :param password: Your Password, which you pointed to RuKassa
+        """
+        super().__init__()
+        self.__token = api_token
+        self.__shop_id = shop_id
+        self.__email = email
+        self.__password = password
+        self.__base_url = "https://lk.rukassa.is/api/v1"
+        self.__post_method = "POST"
+        self.__payment_name = "ruKassa"
+        self.check_values()
+
+    def check_values(self):
+        if not self.__token or not self.__shop_id or not self.__email or not self.__password:
+            raise ValueError('No Api-Token, ShopID, Email or Password specified')
+
+    async def get_balance(self) -> Balance:
+        """Get User Balance
+
+        :return: Balance Object"""
+
+        url = f'{self.__base_url}/getBalance'
+
+        params = {
+            "email": self.__email,
+            "password": self.__password,
+        }
+
+        response = await self._request(self.__payment_name, self.__post_method, url, data=params)
+
+        return Balance(**response)
+
+    def __get_random_string(self):
+        return f'{time.time()}_{secrets.token_hex(random.randint(5, 10))}'
+
+    async def create_payment(self, amount: Union[int, float], currency: Optional[str] = "RUB",
+                             method: Optional[str] = None, data: Optional[str] = None,
+                             orderId: Optional[int] = None) -> CreatePayment:
+        """Create a payment
+
+        :param amount: Amount of payment.
+        :param currency: Optional. In what currency are you specifying the amount parameter? Default RUB. Currencies: RUB, USD
+        :param method: Optional. Payment method, if you want payment to be made through a specific method. Methods: card, card_byn, card_kzt, card_uah, card_uzs, qiwi, yandexmoney, payeer, crypta, sbp,
+        :param data: Optional. String sent to the server along with a notification of a successful payment.
+        :param orderId: Optional. A unique payment number in your system. If not specified, a random string will be generated.
+
+        :return: CreatePayment object
+        """
+
+        url = f'{self.__base_url}/create'
+
+        if not orderId:
+            orderId = self.__get_random_string()
+
+        params = {
+            "shop_id": self.__shop_id,
+            "order_id": orderId,
+            "amount": amount,
+            "token": self.__token,
+            "data": data,
+            "method": method,
+            "currency": currency,
+        }
+
+        for key, value in params.copy().items():
+            if value is None:
+                params.pop(key)
+
+        response = await self._request(self.__payment_name, self.__post_method, url, data=params)
+
+        return CreatePayment(**response)
+
+    async def get_info_payment(self, id: int) -> Payment:
+        """
+        Get payment information
+
+        :param id: Transaction (entry) number in our system.
+
+        :return: Payment object
+        """
+
+        url = f"{self.__base_url}/getPayInfo"
+
+        params = {
+            "id": id,
+            "shop_id": self.__shop_id,
+            "token": self.__token,
+        }
+
+        response = await self._request(self.__payment_name, self.__post_method, url, data=params)
+
+        return Payment(**response)
+
+    async def create_withdraw(self, way: str, wallet: str, amount: Union[float, int], orderId: str = None,
+                              check_from: Optional[str] = "BASE_RUB", who_fee: Optional[int] = 0,
+                              bank: Optional[int] = None) -> CreateWithdrawRequest:
+        """
+        Create withdraw request
+
+        :param way: Payment system for withdrawal. Systems: CARD, QIWI, YOOMONEY, USDT, SBP.
+        :param wallet: The number of the wallet or card where the funds will be sent.
+        :param amount: Amount to withdraw.
+        :param orderId: ID in the merchant system.
+        :param check_from: Account for debiting funds. Default: BASE_RUB. (BASE_RUB, BASE_USD).
+        :param who_fee: Where to write off the commission. Default: 0. (0 - from account, 1 - from balance).
+        :param bank: Only for SBP. Bank number.
+
+        :return: CreateWithdrawRequest object
+        """
+
+        url = f"{self.__base_url}/createWithdraw"
+
+        params = {
+            "email": self.__email,
+            "password": self.__password,
+            "way": way,
+            "wallet": wallet,
+            "amount": amount,
+            "order_id": orderId,
+            "from": check_from,
+            "who_fee": who_fee,
+            "bank": bank,
+        }
+
+        response = await self._request(self.__payment_name, self.__post_method, url, data=params)
+
+        return CreateWithdrawRequest(**response)
+
+    async def cancel_withdraw(self, id: int) -> CancelWithdrawRequest:
+        """
+        Cancel withdraw request
+
+        :param id: Payment ID in our system.
+
+        :return: CancelWithdrawRequest object
+        """
+
+        url = f"{self.__base_url}/cancelWithdraw"
+
+        params = {
+            "email": self.__email,
+            "password": self.__password,
+            "id": id,
+        }
+
+        response = await self._request(self.__payment_name, self.__post_method, url, data=params)
+
+        return CancelWithdrawRequest(**response)
+
+    async def get_info_withdraw(self, id: int) -> WithdrawRequest:
+        """
+        Get info about withdraw request
+
+        :param id: The number of the operation (withdrawal) in our system.
+
+        :return: WithdrawRequest object
+        """
+
+        url = f"{self.__base_url}/getWithdrawInfo"
+
+        params = {
+            "token": self.__token,
+            "shop_id": self.__shop_id,
+            "id": id,
+        }
+
+        response = await self._request(self.__payment_name, self.__post_method, url, data=params)
+
+        return WithdrawRequest(**response)
```

### Comparing `AsyncPayments-1.4.1/AsyncPayments.egg-info/PKG-INFO` & `AsyncPayments-1.4.2/AsyncPayments.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AsyncPayments
-Version: 1.4.1
+Version: 1.4.2
 Summary: Add payment acceptance to your projects.
 Author: ToSa
 Maintainer: ToSa
 License: MIT License
 Project-URL: Homepage, https://github.com/I-ToSa-I/AsyncPayments
 Project-URL: Repository, https://github.com/I-ToSa-I/AsyncPayments
 Project-URL: Issues, https://github.com/I-ToSa-I/AsyncPayments/issues
@@ -26,27 +26,27 @@
 Requires-Dist: aiohttp
 
 # AsyncPayments
 > Add payment acceptance to your projects.
 ## Installing
     pip install AsyncPayments
 ## Version
-    v1.4.1
+    v1.4.2
 ## Code example
 ```python
 import asyncio
 
 from AsyncPayments.ruKassa import AsyncRuKassa
 from AsyncPayments.lolz import AsyncLolzteamMarketPayment
 from AsyncPayments.aaio import AsyncAaio
 from AsyncPayments.cryptoBot import AsyncCryptoBot
 from AsyncPayments.crystalPay import AsyncCrystalPay
 
 ruKassa = AsyncRuKassa("Api-Token", 1, "Email", "Password") # 1 - ShopID
-lolz = AsyncLolzteamMarketPayment("Token", 1, "UserNickname") # 1 - UserID
+lolz = AsyncLolzteamMarketPayment("Token")
 aaio = AsyncAaio("ApiKey", "ShopId", "SecretKey")
 cryptoBot = AsyncCryptoBot("Token")
 crystalPay = AsyncCrystalPay("Login", "Secret", "Salt")
 
 async def main():
     balance_rukassa = await ruKassa.get_balance()
     balance_lolz = await lolz.get_me()
@@ -175,15 +175,15 @@
 Доступно USDCTRC: 0.0  USDC
 Доступно USDTBANKER: 0.0  RUB
 Доступно USDTCHATEX: 0.0  RUB
 Доступно USDTCRYPTOBOT: 0.144637  USDT
 Доступно USDTTRC: 0.0  USDT
 ------------------------------------------
 RuKassa:  https://pay.ruks.pro/?hash=435fc3cee737f9dac2b34c9ba9311eae
-Lolz:  https://lzt.market/balance/transfer?username=ToSa&hold=0&amount=15&comment=orderId
+Lolz:  https://lzt.market/balance/transfer?user_id=4810752&hold=0&amount=15&comment=orderId
 Aaio:  https://aaio.io/merchant/pay?merchant_id=f398c75d-b775-412c-9674-87939692c083&amount=15&order_id=orderId&currency=RUB&sign=6ad5dc2164059a255921ad216c7e5ffd0d2abcaec9af7415636fc12df938582f
 CryptoBot:  https://t.me/CryptoBot?start=IVYOJWPOZh15
 CrystalPay:  https://pay.crystalpay.io/?i=715297022_MxRoixNnSrMSBD
 ------------------------------------------
 RuKassa:
 Сумма:  50
 Статус:  WAIT
```

### Comparing `AsyncPayments-1.4.1/AsyncPayments.egg-info/SOURCES.txt` & `AsyncPayments-1.4.2/AsyncPayments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AsyncPayments-1.4.1/LICENSE` & `AsyncPayments-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `AsyncPayments-1.4.1/PKG-INFO` & `AsyncPayments-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AsyncPayments
-Version: 1.4.1
+Version: 1.4.2
 Summary: Add payment acceptance to your projects.
 Author: ToSa
 Maintainer: ToSa
 License: MIT License
 Project-URL: Homepage, https://github.com/I-ToSa-I/AsyncPayments
 Project-URL: Repository, https://github.com/I-ToSa-I/AsyncPayments
 Project-URL: Issues, https://github.com/I-ToSa-I/AsyncPayments/issues
@@ -26,27 +26,27 @@
 Requires-Dist: aiohttp
 
 # AsyncPayments
 > Add payment acceptance to your projects.
 ## Installing
     pip install AsyncPayments
 ## Version
-    v1.4.1
+    v1.4.2
 ## Code example
 ```python
 import asyncio
 
 from AsyncPayments.ruKassa import AsyncRuKassa
 from AsyncPayments.lolz import AsyncLolzteamMarketPayment
 from AsyncPayments.aaio import AsyncAaio
 from AsyncPayments.cryptoBot import AsyncCryptoBot
 from AsyncPayments.crystalPay import AsyncCrystalPay
 
 ruKassa = AsyncRuKassa("Api-Token", 1, "Email", "Password") # 1 - ShopID
-lolz = AsyncLolzteamMarketPayment("Token", 1, "UserNickname") # 1 - UserID
+lolz = AsyncLolzteamMarketPayment("Token")
 aaio = AsyncAaio("ApiKey", "ShopId", "SecretKey")
 cryptoBot = AsyncCryptoBot("Token")
 crystalPay = AsyncCrystalPay("Login", "Secret", "Salt")
 
 async def main():
     balance_rukassa = await ruKassa.get_balance()
     balance_lolz = await lolz.get_me()
@@ -175,15 +175,15 @@
 Доступно USDCTRC: 0.0  USDC
 Доступно USDTBANKER: 0.0  RUB
 Доступно USDTCHATEX: 0.0  RUB
 Доступно USDTCRYPTOBOT: 0.144637  USDT
 Доступно USDTTRC: 0.0  USDT
 ------------------------------------------
 RuKassa:  https://pay.ruks.pro/?hash=435fc3cee737f9dac2b34c9ba9311eae
-Lolz:  https://lzt.market/balance/transfer?username=ToSa&hold=0&amount=15&comment=orderId
+Lolz:  https://lzt.market/balance/transfer?user_id=4810752&hold=0&amount=15&comment=orderId
 Aaio:  https://aaio.io/merchant/pay?merchant_id=f398c75d-b775-412c-9674-87939692c083&amount=15&order_id=orderId&currency=RUB&sign=6ad5dc2164059a255921ad216c7e5ffd0d2abcaec9af7415636fc12df938582f
 CryptoBot:  https://t.me/CryptoBot?start=IVYOJWPOZh15
 CrystalPay:  https://pay.crystalpay.io/?i=715297022_MxRoixNnSrMSBD
 ------------------------------------------
 RuKassa:
 Сумма:  50
 Статус:  WAIT
```

### Comparing `AsyncPayments-1.4.1/README.md` & `AsyncPayments-1.4.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,192 +1,192 @@
-# AsyncPayments
-> Add payment acceptance to your projects.
-## Installing
-    pip install AsyncPayments
-## Version
-    v1.4.1
-## Code example
-```python
-import asyncio
-
-from AsyncPayments.ruKassa import AsyncRuKassa
-from AsyncPayments.lolz import AsyncLolzteamMarketPayment
-from AsyncPayments.aaio import AsyncAaio
-from AsyncPayments.cryptoBot import AsyncCryptoBot
-from AsyncPayments.crystalPay import AsyncCrystalPay
-
-ruKassa = AsyncRuKassa("Api-Token", 1, "Email", "Password") # 1 - ShopID
-lolz = AsyncLolzteamMarketPayment("Token", 1, "UserNickname") # 1 - UserID
-aaio = AsyncAaio("ApiKey", "ShopId", "SecretKey")
-cryptoBot = AsyncCryptoBot("Token")
-crystalPay = AsyncCrystalPay("Login", "Secret", "Salt")
-
-async def main():
-    balance_rukassa = await ruKassa.get_balance()
-    balance_lolz = await lolz.get_me()
-    balance_aaio = await aaio.get_balance()
-    balance_crypto_bot = await cryptoBot.get_balance()
-    balance_crystal_pay = await crystalPay.get_balance()
-    
-    print("RuKassa:")
-    print("RUB: ", balance_rukassa.balance_rub)
-    print("USD: ", balance_rukassa.balance_usd)
-    print('--------------')
-    print("Lolz:")
-    print('ID: ', balance_lolz.user_id)
-    print('Никнейм: ', balance_lolz.username)
-    print('Доступно: ', balance_lolz.balance)
-    print('В холде: ', balance_lolz.hold)
-    print('--------------')
-    print("Aaio:")
-    print('Доступно: ', balance_aaio.balance)
-    print('В холде: ', balance_aaio.hold)
-    print('Реферальный: ', balance_aaio.referral)
-    print('--------------')
-    print("CryptoBot:")
-    for balance in balance_crypto_bot:
-        print(f"Доступно {balance.currency_code}: ", balance.available, f" (В холде: {balance.onhold})")
-    print('--------------')
-    print("CrystalPay:")
-    for currency, balance in balance_crystal_pay:
-        print(f"Доступно {currency}:", balance.amount, f" {balance.currency}")
-    
-    print('------------------------------------------')
-    
-    order_ruKassa = await ruKassa.create_payment(15)
-    order_lolz = lolz.get_payment_link(15, comment="orderId")
-    order_aaio = await aaio.create_payment_url(15, "orderId")
-    order_crypto_bot = await cryptoBot.create_invoice(15, currency_type="crypto", asset="USDT")
-    order_crystal_pay = await crystalPay.create_payment(15)
-    
-    print("RuKassa: ", order_ruKassa.url)
-    print('Lolz: ', order_lolz)
-    print('Aaio: ', order_aaio)
-    print('CryptoBot: ', order_crypto_bot.pay_url)
-    print('CrystalPay: ', order_crystal_pay.url)
-    
-    print('------------------------------------------')
-    
-    info_ruKassa = await ruKassa.get_info_payment("orderId")
-    info_lolz = await lolz.check_status_payment(50, "orderId")
-    info_aaio = await aaio.get_order_info("orderId")
-    info_crypto_bot = await cryptoBot.get_invoices(
-        invoice_ids=["orderId"], count=1
-    )
-    info_crystal_pay = await crystalPay.get_payment_info("orderId")
-    
-    print('RuKassa:')
-    print("Сумма: ", info_ruKassa.amount)
-    print("Статус: ", info_ruKassa.status)
-    print('--------------')
-    print("Lolz:")
-    print("Сумма: ", 15)
-    print("Статус: ", info_lolz)
-    print('--------------')
-    print("Aaio:")
-    print("Сумма: ", info_aaio.amount)
-    print("Статус: ", info_aaio.status)
-    print('--------------')
-    print("CryptoBot:")
-    print("Сумма: ", info_crypto_bot.amount)
-    print("Статус: ", info_crypto_bot.status)
-    print('--------------')
-    print("CrystalPay:")
-    print("Сумма: ", info_crystal_pay.amount)
-    print("Статус:", info_crystal_pay.state)
-    
-
-asyncio.run(main())
-```
-## Output
-```Python
-RuKassa:
-RUB:  34.0
-USD:  234.1
---------------
-Lolz:
-ID:  4810752
-Никнейм:  ToSa
-Доступно:  5233.0
-В холде:  234.0
---------------
-Aaio:
-Доступно:  1235.0
-В холде:  0.0
-Реферальный:  0.0
---------------
-CryptoBot:
-Доступно USDT:  15.0  (В холде: 0.0)
-Доступно TON:  0.0  (В холде: 0.0)
-Доступно BTC:  0.00000023  (В холде: 0.0)
-Доступно LTC:  0.0  (В холде: 0.0)
-Доступно ETH:  0.0  (В холде: 0.0)
-Доступно BNB:  0.0  (В холде: 0.0)
-Доступно TRX:  0.0  (В холде: 0.0)
-Доступно USDC:  0.0  (В холде: 0.0)
---------------
-CrystalPay:
-Доступно BITCOIN: 0.0  BTC
-Доступно BITCOINCASH: 0.0  BCH
-Доступно BNBCRYPTOBOT: 0.0  BNB
-Доступно BNBSMARTCHAIN: 0.0  BNB
-Доступно BTCBANKER: 0.0  RUB
-Доступно BTCCHATEX: 0.0  RUB
-Доступно BTCCRYPTOBOT: 0.0  BTC
-Доступно CARDRUBP2P: 0.0  RUB
-Доступно CARDTRYP2P: 0.0  TRY
-Доступно DASH: 0.0  DASH
-Доступно DOGECOIN: 0.0  DOGE
-Доступно ETHBANKER: 0.0  RUB
-Доступно ETHCRYPTOBOT: 0.0  ETH
-Доступно ETHEREUM: 0.0  ETH
-Доступно LITECOIN: 0.0  LTC
-Доступно LTCBANKER: 0.0  RUB
-Доступно LZTMARKET: 184.0  RUB
-Доступно POLYGON: 0.0  MATIC
-Доступно TONCRYPTOBOT: 0.09825723  TON
-Доступно TRON: 0.0  TRX
-Доступно USDCTRC: 0.0  USDC
-Доступно USDTBANKER: 0.0  RUB
-Доступно USDTCHATEX: 0.0  RUB
-Доступно USDTCRYPTOBOT: 0.144637  USDT
-Доступно USDTTRC: 0.0  USDT
-------------------------------------------
-RuKassa:  https://pay.ruks.pro/?hash=435fc3cee737f9dac2b34c9ba9311eae
-Lolz:  https://lzt.market/balance/transfer?username=ToSa&hold=0&amount=15&comment=orderId
-Aaio:  https://aaio.io/merchant/pay?merchant_id=f398c75d-b775-412c-9674-87939692c083&amount=15&order_id=orderId&currency=RUB&sign=6ad5dc2164059a255921ad216c7e5ffd0d2abcaec9af7415636fc12df938582f
-CryptoBot:  https://t.me/CryptoBot?start=IVYOJWPOZh15
-CrystalPay:  https://pay.crystalpay.io/?i=715297022_MxRoixNnSrMSBD
-------------------------------------------
-RuKassa:
-Сумма:  50
-Статус:  WAIT
---------------
-Lolz:
-Сумма:  15
-Статус:  False
---------------
-Aaio:
-Сумма:  299.0
-Статус:  in_process
---------------
-CryptoBot:
-Сумма:  15
-Статус:  active
---------------
-CrystalPay:
-Сумма:  15.0
-Статус: notpayed
-
-```
-
-## Docs
-> Lolzteam Market: https://lzt-market.readme.io/reference/ <br>
-> Aaio: https://wiki.aaio.io <br>
-> CryptoBot: https://help.crypt.bot/crypto-pay-api <br>
-> CrystalPay: https://docs.crystalpay.io <br>
-> RuKassa: https://lk.rukassa.is/api/v1 <br>
-
-## Developer Links
-> Zelenka (Lolzteam): https://zelenka.guru/tosa <br>
-> GitHub: https://github.com/I-ToSa-I <br>
-> Telegram: https://t.me/ToSa_LZT
+# AsyncPayments
+> Add payment acceptance to your projects.
+## Installing
+    pip install AsyncPayments
+## Version
+    v1.4.2
+## Code example
+```python
+import asyncio
+
+from AsyncPayments.ruKassa import AsyncRuKassa
+from AsyncPayments.lolz import AsyncLolzteamMarketPayment
+from AsyncPayments.aaio import AsyncAaio
+from AsyncPayments.cryptoBot import AsyncCryptoBot
+from AsyncPayments.crystalPay import AsyncCrystalPay
+
+ruKassa = AsyncRuKassa("Api-Token", 1, "Email", "Password") # 1 - ShopID
+lolz = AsyncLolzteamMarketPayment("Token")
+aaio = AsyncAaio("ApiKey", "ShopId", "SecretKey")
+cryptoBot = AsyncCryptoBot("Token")
+crystalPay = AsyncCrystalPay("Login", "Secret", "Salt")
+
+async def main():
+    balance_rukassa = await ruKassa.get_balance()
+    balance_lolz = await lolz.get_me()
+    balance_aaio = await aaio.get_balance()
+    balance_crypto_bot = await cryptoBot.get_balance()
+    balance_crystal_pay = await crystalPay.get_balance()
+    
+    print("RuKassa:")
+    print("RUB: ", balance_rukassa.balance_rub)
+    print("USD: ", balance_rukassa.balance_usd)
+    print('--------------')
+    print("Lolz:")
+    print('ID: ', balance_lolz.user_id)
+    print('Никнейм: ', balance_lolz.username)
+    print('Доступно: ', balance_lolz.balance)
+    print('В холде: ', balance_lolz.hold)
+    print('--------------')
+    print("Aaio:")
+    print('Доступно: ', balance_aaio.balance)
+    print('В холде: ', balance_aaio.hold)
+    print('Реферальный: ', balance_aaio.referral)
+    print('--------------')
+    print("CryptoBot:")
+    for balance in balance_crypto_bot:
+        print(f"Доступно {balance.currency_code}: ", balance.available, f" (В холде: {balance.onhold})")
+    print('--------------')
+    print("CrystalPay:")
+    for currency, balance in balance_crystal_pay:
+        print(f"Доступно {currency}:", balance.amount, f" {balance.currency}")
+    
+    print('------------------------------------------')
+    
+    order_ruKassa = await ruKassa.create_payment(15)
+    order_lolz = lolz.get_payment_link(15, comment="orderId")
+    order_aaio = await aaio.create_payment_url(15, "orderId")
+    order_crypto_bot = await cryptoBot.create_invoice(15, currency_type="crypto", asset="USDT")
+    order_crystal_pay = await crystalPay.create_payment(15)
+    
+    print("RuKassa: ", order_ruKassa.url)
+    print('Lolz: ', order_lolz)
+    print('Aaio: ', order_aaio)
+    print('CryptoBot: ', order_crypto_bot.pay_url)
+    print('CrystalPay: ', order_crystal_pay.url)
+    
+    print('------------------------------------------')
+    
+    info_ruKassa = await ruKassa.get_info_payment("orderId")
+    info_lolz = await lolz.check_status_payment(50, "orderId")
+    info_aaio = await aaio.get_order_info("orderId")
+    info_crypto_bot = await cryptoBot.get_invoices(
+        invoice_ids=["orderId"], count=1
+    )
+    info_crystal_pay = await crystalPay.get_payment_info("orderId")
+    
+    print('RuKassa:')
+    print("Сумма: ", info_ruKassa.amount)
+    print("Статус: ", info_ruKassa.status)
+    print('--------------')
+    print("Lolz:")
+    print("Сумма: ", 15)
+    print("Статус: ", info_lolz)
+    print('--------------')
+    print("Aaio:")
+    print("Сумма: ", info_aaio.amount)
+    print("Статус: ", info_aaio.status)
+    print('--------------')
+    print("CryptoBot:")
+    print("Сумма: ", info_crypto_bot.amount)
+    print("Статус: ", info_crypto_bot.status)
+    print('--------------')
+    print("CrystalPay:")
+    print("Сумма: ", info_crystal_pay.amount)
+    print("Статус:", info_crystal_pay.state)
+    
+
+asyncio.run(main())
+```
+## Output
+```Python
+RuKassa:
+RUB:  34.0
+USD:  234.1
+--------------
+Lolz:
+ID:  4810752
+Никнейм:  ToSa
+Доступно:  5233.0
+В холде:  234.0
+--------------
+Aaio:
+Доступно:  1235.0
+В холде:  0.0
+Реферальный:  0.0
+--------------
+CryptoBot:
+Доступно USDT:  15.0  (В холде: 0.0)
+Доступно TON:  0.0  (В холде: 0.0)
+Доступно BTC:  0.00000023  (В холде: 0.0)
+Доступно LTC:  0.0  (В холде: 0.0)
+Доступно ETH:  0.0  (В холде: 0.0)
+Доступно BNB:  0.0  (В холде: 0.0)
+Доступно TRX:  0.0  (В холде: 0.0)
+Доступно USDC:  0.0  (В холде: 0.0)
+--------------
+CrystalPay:
+Доступно BITCOIN: 0.0  BTC
+Доступно BITCOINCASH: 0.0  BCH
+Доступно BNBCRYPTOBOT: 0.0  BNB
+Доступно BNBSMARTCHAIN: 0.0  BNB
+Доступно BTCBANKER: 0.0  RUB
+Доступно BTCCHATEX: 0.0  RUB
+Доступно BTCCRYPTOBOT: 0.0  BTC
+Доступно CARDRUBP2P: 0.0  RUB
+Доступно CARDTRYP2P: 0.0  TRY
+Доступно DASH: 0.0  DASH
+Доступно DOGECOIN: 0.0  DOGE
+Доступно ETHBANKER: 0.0  RUB
+Доступно ETHCRYPTOBOT: 0.0  ETH
+Доступно ETHEREUM: 0.0  ETH
+Доступно LITECOIN: 0.0  LTC
+Доступно LTCBANKER: 0.0  RUB
+Доступно LZTMARKET: 184.0  RUB
+Доступно POLYGON: 0.0  MATIC
+Доступно TONCRYPTOBOT: 0.09825723  TON
+Доступно TRON: 0.0  TRX
+Доступно USDCTRC: 0.0  USDC
+Доступно USDTBANKER: 0.0  RUB
+Доступно USDTCHATEX: 0.0  RUB
+Доступно USDTCRYPTOBOT: 0.144637  USDT
+Доступно USDTTRC: 0.0  USDT
+------------------------------------------
+RuKassa:  https://pay.ruks.pro/?hash=435fc3cee737f9dac2b34c9ba9311eae
+Lolz:  https://lzt.market/balance/transfer?user_id=4810752&hold=0&amount=15&comment=orderId
+Aaio:  https://aaio.io/merchant/pay?merchant_id=f398c75d-b775-412c-9674-87939692c083&amount=15&order_id=orderId&currency=RUB&sign=6ad5dc2164059a255921ad216c7e5ffd0d2abcaec9af7415636fc12df938582f
+CryptoBot:  https://t.me/CryptoBot?start=IVYOJWPOZh15
+CrystalPay:  https://pay.crystalpay.io/?i=715297022_MxRoixNnSrMSBD
+------------------------------------------
+RuKassa:
+Сумма:  50
+Статус:  WAIT
+--------------
+Lolz:
+Сумма:  15
+Статус:  False
+--------------
+Aaio:
+Сумма:  299.0
+Статус:  in_process
+--------------
+CryptoBot:
+Сумма:  15
+Статус:  active
+--------------
+CrystalPay:
+Сумма:  15.0
+Статус: notpayed
+
+```
+
+## Docs
+> Lolzteam Market: https://lzt-market.readme.io/reference/ <br>
+> Aaio: https://wiki.aaio.io <br>
+> CryptoBot: https://help.crypt.bot/crypto-pay-api <br>
+> CrystalPay: https://docs.crystalpay.io <br>
+> RuKassa: https://lk.rukassa.is/api/v1 <br>
+
+## Developer Links
+> Zelenka (Lolzteam): https://zelenka.guru/tosa <br>
+> GitHub: https://github.com/I-ToSa-I <br>
+> Telegram: https://t.me/ToSa_LZT
```

### Comparing `AsyncPayments-1.4.1/pyproject.toml` & `AsyncPayments-1.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "AsyncPayments"
-version = "1.4.1"
+version = "1.4.2"
 dependencies = [
     "aiohttp"
 ]
 requires-python = ">= 3.9"
 authors = [
   { name = "ToSa" },
 ]
```

