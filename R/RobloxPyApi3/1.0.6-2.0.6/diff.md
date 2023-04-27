# Comparing `tmp/RobloxPyApi3-1.0.6.tar.gz` & `tmp/RobloxPyApi3-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\RobloxPyApi3-1.0.6.tar", last modified: Sat Jul 30 18:09:23 2022, max compression
+gzip compressed data, was "RobloxPyApi3-2.0.6.tar", last modified: Thu Apr 27 13:36:45 2023, max compression
```

## Comparing `RobloxPyApi3-1.0.6.tar` & `RobloxPyApi3-2.0.6.tar`

### file list

```diff
@@ -1,20 +1,40 @@
-drwxrwxrwx   0        0        0        0 2022-07-30 18:09:23.484416 RobloxPyApi3-1.0.6/
--rw-rw-rw-   0        0        0      577 2022-07-30 18:09:23.484416 RobloxPyApi3-1.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-07-30 18:09:23.437616 RobloxPyApi3-1.0.6/RobloxPyApi3/
--rw-rw-rw-   0        0        0    21907 2022-07-23 16:10:01.000000 RobloxPyApi3-1.0.6/RobloxPyApi3/Avatar.py
--rw-rw-rw-   0        0        0    36813 2022-07-18 18:28:08.000000 RobloxPyApi3-1.0.6/RobloxPyApi3/Catalog.py
--rw-rw-rw-   0        0        0    17955 2022-07-24 13:30:53.000000 RobloxPyApi3-1.0.6/RobloxPyApi3/Client.py
--rw-rw-rw-   0        0        0     1601 2022-07-19 18:56:15.000000 RobloxPyApi3-1.0.6/RobloxPyApi3/Errors.py
--rw-rw-rw-   0        0        0     1032 2022-07-18 17:49:18.000000 RobloxPyApi3-1.0.6/RobloxPyApi3/JoinGame.py
--rw-rw-rw-   0        0        0      449 2022-07-19 17:36:39.000000 RobloxPyApi3-1.0.6/RobloxPyApi3/LeaveGame.py
--rw-rw-rw-   0        0        0      596 2022-07-24 13:26:52.000000 RobloxPyApi3-1.0.6/RobloxPyApi3/Version.py
--rw-rw-rw-   0        0        0      752 2022-07-30 13:00:24.000000 RobloxPyApi3-1.0.6/RobloxPyApi3/__Changes__.py
--rw-rw-rw-   0        0        0    52911 2022-07-30 18:08:57.000000 RobloxPyApi3-1.0.6/RobloxPyApi3/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-30 18:09:23.468816 RobloxPyApi3-1.0.6/RobloxPyApi3.egg-info/
--rw-rw-rw-   0        0        0      577 2022-07-30 18:09:22.000000 RobloxPyApi3-1.0.6/RobloxPyApi3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      408 2022-07-30 18:09:23.000000 RobloxPyApi3-1.0.6/RobloxPyApi3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-30 18:09:22.000000 RobloxPyApi3-1.0.6/RobloxPyApi3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2022-07-30 18:09:22.000000 RobloxPyApi3-1.0.6/RobloxPyApi3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-07-30 18:09:22.000000 RobloxPyApi3-1.0.6/RobloxPyApi3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-07-30 18:09:23.484416 RobloxPyApi3-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      843 2022-07-30 18:08:57.000000 RobloxPyApi3-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:36:45.915984 RobloxPyApi3-2.0.6/
+-rw-rw-rw-   0        0        0       61 2023-04-27 12:20:20.000000 RobloxPyApi3-2.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2225 2023-04-27 13:36:45.915984 RobloxPyApi3-2.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-27 13:36:45.907474 RobloxPyApi3-2.0.6/RobloxPyApi3/
+-rw-rw-rw-   0        0        0    19220 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/AccountInformation.py
+-rw-rw-rw-   0        0        0    15233 2023-04-09 12:42:10.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/Auth.py
+-rw-rw-rw-   0        0        0    21919 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/Avatar.py
+-rw-rw-rw-   0        0        0    16576 2023-04-27 13:25:52.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/Captcha.py
+-rw-rw-rw-   0        0        0    36825 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/Catalog.py
+-rw-rw-rw-   0        0        0     2739 2023-04-08 19:22:28.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/Check.png
+-rw-rw-rw-   0        0        0    18452 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/Client.py
+-rw-rw-rw-   0        0        0     1557 2023-04-12 19:25:10.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/Enums.py
+-rw-rw-rw-   0        0        0     2213 2023-04-09 08:16:10.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/Errors.py
+-rw-rw-rw-   0        0        0    14748 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/FriendsAPI.py
+-rw-rw-rw-   0        0        0     5938 2023-04-27 12:30:26.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/JoinGame.py
+-rw-rw-rw-   0        0        0      461 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/LeaveGame.py
+-rw-rw-rw-   0        0        0     9939 2023-04-27 12:47:06.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/MultiAccount.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:36:45.915008 RobloxPyApi3-2.0.6/RobloxPyApi3/Place/
+-rw-rw-rw-   0        0        0     1977 2023-03-30 08:25:08.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/Place/CallMethods.py
+-rw-rw-rw-   0        0        0     3312 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/Place/Instructions.py
+-rw-rw-rw-   0        0        0    26394 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/Place/Place.py
+-rw-rw-rw-   0        0        0      122 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/Place/__init__.py
+-rw-rw-rw-   0        0        0     9691 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/Place/rbxLua2py.py
+-rw-rw-rw-   0        0        0     5550 2023-03-03 16:26:02.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/Place.py
+-rw-rw-rw-   0        0        0        0 2023-03-03 14:18:04.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/PlacePropTypes.py
+-rw-rw-rw-   0        0        0      505 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/SessionUtilities.py
+-rw-rw-rw-   0        0        0       50 2023-04-15 15:18:22.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/Test.py
+-rw-rw-rw-   0        0        0     2762 2023-04-27 12:24:10.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/Utilities.py
+-rw-rw-rw-   0        0        0     1594 2023-04-27 13:25:52.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/Version.py
+-rw-rw-rw-   0        0        0     2498 2023-04-27 13:25:52.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/__Changes__.py
+-rw-rw-rw-   0        0        0    50881 2023-04-27 12:22:44.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/__init__.py
+-rw-rw-rw-   0        0        0     4637 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.6/RobloxPyApi3/friends.py
+drwxrwxrwx   0        0        0        0 2023-04-27 13:36:45.912086 RobloxPyApi3-2.0.6/RobloxPyApi3.egg-info/
+-rw-rw-rw-   0        0        0     2225 2023-04-27 13:36:45.000000 RobloxPyApi3-2.0.6/RobloxPyApi3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-04-27 13:36:45.000000 RobloxPyApi3-2.0.6/RobloxPyApi3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 13:36:45.000000 RobloxPyApi3-2.0.6/RobloxPyApi3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-27 13:36:45.000000 RobloxPyApi3-2.0.6/RobloxPyApi3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-27 13:36:45.000000 RobloxPyApi3-2.0.6/RobloxPyApi3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 13:36:45.915984 RobloxPyApi3-2.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     2706 2023-04-27 13:34:38.000000 RobloxPyApi3-2.0.6/setup.py
```

### Comparing `RobloxPyApi3-1.0.6/RobloxPyApi3/Avatar.py` & `RobloxPyApi3-2.0.6/RobloxPyApi3/Avatar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import requests
-from .Errors import APIConnectFailed,APIError,GetAvatarMetadataFailed,GetAvatarRulesFailed,InvalidUserId
+from RobloxPyApi3.Errors import APIConnectFailed,APIError,GetAvatarMetadataFailed,GetAvatarRulesFailed,InvalidUserId
 import socket
 class RigTypes:
     R6 = "R6"
     R15 = "R15"
     def __init__(self):
         self.R15 = "R15"
         self.R6 = "R6"
```

### Comparing `RobloxPyApi3-1.0.6/RobloxPyApi3/Catalog.py` & `RobloxPyApi3-2.0.6/RobloxPyApi3/Catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import socket
 import requests
-from .Errors import Error,GetCategoriesFailed,APIConnectFailed,InvalidBundleId,ListBundlesFromAssetIdFailed,InvalidAssetId,NoItemFound,FindItemInBundleFailed,GetBundleDetailsFailed,GetBundleRecommendationFailed,InvalidUserId,GetPlayerBundlesFailed,NoContentError,UnpackBundleFailed,GetassetToCategoryFailed,GetassetToSubCategoryFailed
+from RobloxPyApi3.Errors import Error,GetCategoriesFailed,APIConnectFailed,InvalidBundleId,ListBundlesFromAssetIdFailed,InvalidAssetId,NoItemFound,FindItemInBundleFailed,GetBundleDetailsFailed,GetBundleRecommendationFailed,InvalidUserId,GetPlayerBundlesFailed,NoContentError,UnpackBundleFailed,GetassetToCategoryFailed,GetassetToSubCategoryFailed
 def list_bundles_from_assetId(cookie,assetId,showErrors=bool):
     try:
         socket.create_connection(('google.com',80))
     except socket.gaierror:
         if showErrors == True:
             raise APIConnectFailed("No internet connection, check your internet connection and try again.")
         else:
```

### Comparing `RobloxPyApi3-1.0.6/RobloxPyApi3/Client.py` & `RobloxPyApi3-2.0.6/RobloxPyApi3/Client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .Version import *
+from RobloxPyApi3.Version import *
 import RobloxPyApi3
 import socket
 import requests
 def Get_Robux2(cookie,showErrors = bool):
     #try:
         #req.urlopen('http://google.com')
     #except:
@@ -226,8 +226,14 @@
     def GetAvatarScalesFromUser(self,UserId):
         return RobloxPyApi3.GetAvatarScalesFromUser(cookie=self.ROBLOSECURITY, UserId=UserId, showErrors=self.showErrors)
     def GetAvatarBodyColorsFromUser(self,UserId):
         return RobloxPyApi3.GetAvatarBodyColorsFromUser(cookie=self.ROBLOSECURITY, UserId=UserId,showErrors=self.showErrors)
     def GetAvatarRigTypeFromUser(self,UserId):
         return RobloxPyApi3.GetAvatarRigTypeFromUser(cookie=self.ROBLOSECURITY, UserId=UserId,showErrors=self.showErrors)
     def GetAvatarRigTypeEnumFromUser(self,UserId):
-        return RobloxPyApi3.GetAvatarRigTypeEnumFromUser(cookie=self.ROBLOSECURITY, UserId=UserId,showErrors=self.showErrors)
+        return RobloxPyApi3.GetAvatarRigTypeEnumFromUser(cookie=self.ROBLOSECURITY, UserId=UserId,showErrors=self.showErrors)
+    def Accept_Friend_Request(self,UserId):
+        return RobloxPyApi3.Accept_Friend_Request(cookie=self.ROBLOSECURITY,UserId=UserId,showErrors=self.showErrors)
+    def Decline_Friend_Request(self,UserId):
+        return RobloxPyApi3.Decline_Friend_Request(cookie=self.ROBLOSECURITY,UserId=UserId,showErrors=self.showErrors)
+    def Decline_All_Friend_Requests(self):
+        return RobloxPyApi3.Decline_All_Friend_Requests(cookie=self.ROBLOSECURITY,showErrors=self.showErrors)
```

### Comparing `RobloxPyApi3-1.0.6/RobloxPyApi3/Errors.py` & `RobloxPyApi3-2.0.6/RobloxPyApi3/Errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,41 @@
+
 class APIError(Exception):
     pass
 
+
 class GetAvatarMetadataFailed(Exception):
     pass
 
+
 class GetAvatarRulesFailed(Exception):
     pass
 
+
+class GetFriendMetadataFailed(Exception):
+
+    pass
+
+
+class DeclineFriendRequestFailed(Exception):
+    pass
+
+
+class DeclineAllFriendsRequest(Exception):
+    pass
+
+
 class NoRobloxProcessFound(Exception):
     pass
 
 
+class AcceptFriendRequestFailed(Exception):
+    pass
+
+
 class ListBundlesFromAssetIdFailed(Exception):
     pass
 
 
 class JoinGameFailed(Exception):
     pass
 
@@ -114,7 +135,43 @@
 class CheckIsBannedFailed(Exception):
     pass
 
 
 class AccountCheckError(Exception):
 
     pass
+
+
+class ValueNotSet(Exception):
+
+    pass
+
+
+class OpenProjectFail(Exception):
+
+    pass
+
+
+class InvalidVariableUsage(Exception):
+
+    pass
+
+
+class FunctionValueFailure(Exception):
+
+    pass
+
+
+class DataNotSpecified(Exception):
+
+    pass
+
+
+class MakeRequestFailed(Exception):
+
+    pass
+
+
+class UrlNotSpecified(Exception):
+
+    pass
+
```

### Comparing `RobloxPyApi3-1.0.6/RobloxPyApi3/__init__.py` & `RobloxPyApi3-2.0.6/RobloxPyApi3/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # This package made by pyProjects3 for Roblox.
 # Scroll till the end to see more information and QNA!
-import socket
-from .Version import *
+#import socket
+
+from RobloxPyApi3.Version import *
 from RobloxPyApi3.Avatar import * #list_bundles_from_assetId,Get_Bundle_Details,Get_BundleName_From_BundleId,Get_Items_From_Bundle,CheckIf_Item_In_Bundle,Find_Item_In_Bundle,Get_Bundle_Recommendation,Find_Bundle_in_Bundle_Recommendation,Get_Bundles_Names_owned_by_Player,Get_Bundles_Ids_owned_by_Player,CheckIf_Item_In_Bundle_IsOwned,Asset_To_Subcategory,Get_subcategories,Get_Categories,Get_asset_To_Category,Get_Asset_Favorites_Count,Unpack_Bundle,Favorite_Asset,Favorite_Bundle,Delete_Favorite_Asset,Delete_Favorite_Bundle,Get_Items_Details,Items_Details,Get_Bundle_Favorites_Count,Get_Favorite_Bundle,Get_Favorite_Asset,UnFavorite_Bundle,Create_Favorite_Asset,Create_Favorite_Bundle,UnFavorite_Asset
-from .Errors import * #Error,GetCategoriesFailed,APIConnectFailed,InvalidBundleId,ListBundlesFromAssetIdFailed,InvalidAssetId,NoItemFound,FindItemInBundleFailed,GetBundleDetailsFailed,GetBundleRecommendationFailed,InvalidUserId,GetPlayerBundlesFailed,NoContentError,UnpackBundleFailed,GetassetToCategoryFailed,GetassetToSubCategoryFailed
-from .Client import *
-from .__Changes__ import *
-from .JoinGame import *
-from .LeaveGame import *
+from RobloxPyApi3.Errors import * #Error,GetCategoriesFailed,APIConnectFailed,InvalidBundleId,ListBundlesFromAssetIdFailed,InvalidAssetId,NoItemFound,FindItemInBundleFailed,GetBundleDetailsFailed,GetBundleRecommendationFailed,InvalidUserId,GetPlayerBundlesFailed,NoContentError,UnpackBundleFailed,GetassetToCategoryFailed,GetassetToSubCategoryFailed
+from RobloxPyApi3.Client import *
+from RobloxPyApi3.__Changes__ import *
+from RobloxPyApi3.friends import *
+from RobloxPyApi3.JoinGame import *
+from RobloxPyApi3.LeaveGame import *
 import time
 from RobloxPyApi3Update import *
 from colorama import init,Fore
 from RobloxPyApi3.Catalog import * #RigTypes,GetAvatarBodyColorsIds,GetAvatarDetails
 init(convert=True)
 
 __Author__= Version.__Author__
@@ -142,35 +144,38 @@
     except Exception as RE:
         if showErrors == True:
             raise RobuxCheckFailed(f"Robux check process returned Exception: {RE}")
         else:
             return
 def init(Help=bool,cookie=str,showErrors = bool):
     print("This feature is coming soon, check the change log (__Changes__.py)")
+
+    """
     try:
         socket.create_connection(('google.com',80))
     except socket.gaierror:
         if showErrors == True:
             raise APIConnectFailed("No internet connection, check your internet connection and try again.")
         else:
             return
     if Help == True:
         print("Return: User Description from cookie, User Id from cookie, Username from cookie, Display name from cookie,\n")
         print("Isbanned from cookie, Robux value from cookie.\n")
-        print(f"""
+        print(f
 Usage: 
     init(Help=false,cookie=your .ROBLOSECURITY cookie)
     {Fore.YELLOW}IMPORTANT: Turn off 'Help' argument.
     {Fore.RED}Output:
         {Fore.BLUE}Description, User Id, Username, Display name, Is banned, robux:
         
         {Fore.LIGHTBLUE_EX}Hi, This is user description, 123456789, Username123, MyDisplayName, False, 0 {Fore.RESET}   
-        """)
+
     elif Help is None:
         return
+"""
 def Get_Authentication_ticket(cookie,gameid,showErrors=bool):
     try:
         socket.create_connection(('google.com',80))
     except socket.gaierror:
         if showErrors == True:
             raise APIConnectFailed("No internet connection, check your internet connection and try again.")
         else:
@@ -195,14 +200,15 @@
         a = requests.get(f"https://users.roblox.com/v1/users/{UID}")
         if a.json()["description"] and a.json()["isBanned"] == False and a.json()["name"] and a.json()["displayName"] and a.json()["id"]:
             return True
         else:
             return False
     except:
         return False
+
 def IsBanned(UID,showErrors=bool):
     try:
         socket.create_connection(('google.com',80))
     except socket.gaierror:
         if showErrors == True:
             raise APIConnectFailed("No internet connection, check your internet connection and try again.")
         else:
@@ -1061,49 +1067,13 @@
         return GetAvatarScalesFromUser(cookie=self.ROBLOSECURITY, UserId=UserId, showErrors=self.showErrors)
     def GetAvatarBodyColorsFromUser(self,UserId):
         return GetAvatarBodyColorsFromUser(cookie=self.ROBLOSECURITY, UserId=UserId,showErrors=self.showErrors)
     def GetAvatarRigTypeFromUser(self,UserId):
         return GetAvatarRigTypeFromUser(cookie=self.ROBLOSECURITY, UserId=UserId,showErrors=self.showErrors)
     def GetAvatarRigTypeEnumFromUser(self,UserId):
         return GetAvatarRigTypeEnumFromUser(cookie=self.ROBLOSECURITY, UserId=UserId,showErrors=self.showErrors)
-#==============================================================================================================================================
-#This package doesnt made to perform DDoS attacks or any illegal actions.
-#This package made for controlling a profile, or basically, controlling a BOT.
-#I hope this package is useful and all my hard work is worth it.
-
-#QNA:
-#Q: Why functions always use cookie ?
-#A: This package needs to use roblox API with your cookie, the cookie helps API to authorize,
-# the user.
-#Q:Does that module beams and steals the  ?
-#A: No, we didn't use discord API (Discord Webhook) to perform process. We didn't use discord.py or any discord links except for those
-# Discord links that direct to my Discord server where you can report bugs or contact me.
-#Q: Where can I contact the owner or report bugs ?
-#A: You can report any issues in my Github or in upcoming Discord server.
-#Q: Is this package easy to use ?
-#A: Yes, it is. if its hard for you to use this package,
-# you can simply use client = RobloxPyApi3.Client(".ROBLOSECURITY cookie here",True) print(client.Get_Robux())
-#or you can use bot = RobloxPyApi3.bot(".ROBLOSECURITY cookie here",True) print(bot.Get_Robux()). So this is not hard.
-#Q: Are RobloxPyApi3.bot and RobloxPyApi3.Client exact same things ?
-#A: Yes they are the same, people will easily understand the classes.
-#Q: Why can't you use multiple cookies ?
-#A: You can't use multiple cookies because Roblox did a Patch on multiple cookies due to
-# scam bots and trump bots accident in Roblox.
-# ---------  Usage Number 1:  ------------
-# import RobloxPyApi3
-# client = RobloxPyApi3.Client("ROBLOSECURITY cookie goes here",showErrors=True) # or False     showErrors Used to debug code for errors, if you dont want program to show errors, set showErrors to False.
-# Robux = client.Get_Robux()
-# print(Robux,client.Robux)
-# ---------  Usage Number 2:  ------------
-# import RobloxPyApi3
-# bot = RobloxPyApi3.bot("ROBLOSECURITY cookie goes here",showErrors=True)
-# Robux = bot.Get_Robux()
-# print(Robux,bot.Robux)
-# ---------  Usage Number 3:  ------------
-# import RobloxPyApi3
-# robux = RobloxPyApi.Get_Robux("ROBLOSECURITY Cookie goes here",showErrors=False)
-# print(robux)
-# ---------  Output/Run/Results: ---------
-#             Your robux amount
-# ----------------------------------------
-#Thats it, thanks for using my package! I really appreciate it.
-#==============================================================================================================================================
+    def Accept_Friend_Request(self,UserId):
+        return Accept_Friend_Request(cookie=self.ROBLOSECURITY,UserId=UserId,showErrors=self.showErrors)
+    def Decline_Friend_Request(self,UserId):
+        return Decline_Friend_Request(cookie=self.ROBLOSECURITY,UserId=UserId,showErrors=self.showErrors)
+    def Decline_All_Friend_Requests(self):
+        return Decline_All_Friend_Requests(cookie=self.ROBLOSECURITY,showErrors=self.showErrors)
```

