# Comparing `tmp/insta-tweet-2.1.1.tar.gz` & `tmp/insta-tweet-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insta-tweet-2.1.1.tar", last modified: Wed Oct 12 04:57:16 2022, max compression
+gzip compressed data, was "insta-tweet-2.1.2.tar", last modified: Thu Apr 27 10:10:31 2023, max compression
```

## Comparing `insta-tweet-2.1.1.tar` & `insta-tweet-2.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-10-12 04:57:16.750115 insta-tweet-2.1.1/
-drwxrwxrwx   0        0        0        0 2022-10-12 04:57:16.734491 insta-tweet-2.1.1/InstaTweet/
--rw-rw-rw-   0        0        0      349 2022-09-05 10:22:33.000000 insta-tweet-2.1.1/InstaTweet/__init__.py
--rw-rw-rw-   0        0        0     5062 2022-09-03 02:22:55.000000 insta-tweet-2.1.1/InstaTweet/db.py
--rw-rw-rw-   0        0        0     4535 2022-10-12 04:08:29.000000 insta-tweet-2.1.1/InstaTweet/instaclient.py
--rw-rw-rw-   0        0        0     4528 2022-10-12 04:08:29.000000 insta-tweet-2.1.1/InstaTweet/instapost.py
--rw-rw-rw-   0        0        0     5831 2022-10-12 04:08:29.000000 insta-tweet-2.1.1/InstaTweet/instatweet.py
--rw-rw-rw-   0        0        0     2833 2022-10-12 04:08:29.000000 insta-tweet-2.1.1/InstaTweet/instauser.py
--rw-rw-rw-   0        0        0    17213 2022-09-05 10:22:33.000000 insta-tweet-2.1.1/InstaTweet/profile.py
--rw-rw-rw-   0        0        0     7104 2022-10-12 04:08:29.000000 insta-tweet-2.1.1/InstaTweet/tweetclient.py
--rw-rw-rw-   0        0        0     1695 2022-09-03 02:22:55.000000 insta-tweet-2.1.1/InstaTweet/utils.py
--rw-rw-rw-   0        0        0     1083 2022-01-16 08:08:16.000000 insta-tweet-2.1.1/LICENSE
--rw-rw-rw-   0        0        0     5719 2022-10-12 04:57:16.750115 insta-tweet-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5295 2022-10-12 04:54:20.000000 insta-tweet-2.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2022-10-12 04:57:16.750115 insta-tweet-2.1.1/insta_tweet.egg-info/
--rw-rw-rw-   0        0        0     5719 2022-10-12 04:57:16.000000 insta-tweet-2.1.1/insta_tweet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      408 2022-10-12 04:57:16.000000 insta-tweet-2.1.1/insta_tweet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-12 04:57:16.000000 insta-tweet-2.1.1/insta_tweet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2022-10-12 04:57:16.000000 insta-tweet-2.1.1/insta_tweet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-10-12 04:57:16.000000 insta-tweet-2.1.1/insta_tweet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-12 04:57:16.750115 insta-tweet-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1470 2022-10-12 04:55:24.000000 insta-tweet-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 10:10:31.131460 insta-tweet-2.1.2/
+drwxrwxrwx   0        0        0        0 2023-04-27 10:10:31.115838 insta-tweet-2.1.2/InstaTweet/
+-rw-rw-rw-   0        0        0      349 2023-04-27 09:44:14.000000 insta-tweet-2.1.2/InstaTweet/__init__.py
+-rw-rw-rw-   0        0        0     5070 2023-04-27 09:44:14.000000 insta-tweet-2.1.2/InstaTweet/db.py
+-rw-rw-rw-   0        0        0     4516 2023-04-27 09:44:14.000000 insta-tweet-2.1.2/InstaTweet/instaclient.py
+-rw-rw-rw-   0        0        0     4494 2023-04-27 09:44:14.000000 insta-tweet-2.1.2/InstaTweet/instapost.py
+-rw-rw-rw-   0        0        0     5831 2023-04-27 09:44:14.000000 insta-tweet-2.1.2/InstaTweet/instatweet.py
+-rw-rw-rw-   0        0        0     2833 2023-04-27 09:44:14.000000 insta-tweet-2.1.2/InstaTweet/instauser.py
+-rw-rw-rw-   0        0        0    17255 2023-04-27 09:44:14.000000 insta-tweet-2.1.2/InstaTweet/profile.py
+-rw-rw-rw-   0        0        0     7454 2023-04-27 09:44:14.000000 insta-tweet-2.1.2/InstaTweet/tweetclient.py
+-rw-rw-rw-   0        0        0     1695 2023-04-27 09:44:14.000000 insta-tweet-2.1.2/InstaTweet/utils.py
+-rw-rw-rw-   0        0        0     1084 2023-04-27 09:24:17.000000 insta-tweet-2.1.2/LICENSE
+-rw-rw-rw-   0        0        0     7529 2023-04-27 10:10:31.131460 insta-tweet-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6547 2023-04-27 09:44:14.000000 insta-tweet-2.1.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-27 10:10:31.131460 insta-tweet-2.1.2/insta_tweet.egg-info/
+-rw-rw-rw-   0        0        0     7529 2023-04-27 10:10:30.000000 insta-tweet-2.1.2/insta_tweet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2023-04-27 10:10:30.000000 insta-tweet-2.1.2/insta_tweet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 10:10:30.000000 insta-tweet-2.1.2/insta_tweet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-04-27 10:10:30.000000 insta-tweet-2.1.2/insta_tweet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-27 10:10:30.000000 insta-tweet-2.1.2/insta_tweet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 10:10:31.131460 insta-tweet-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1480 2023-04-27 10:08:39.000000 insta-tweet-2.1.2/setup.py
```

### Comparing `insta-tweet-2.1.1/InstaTweet/db.py` & `insta-tweet-2.1.2/InstaTweet/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
         :param profile: the :class:`~.Profile` to save
         :param alert: if ``True``, will print a message upon successfully saving
         """
         if (db_profile := self.query_profile(profile.name)).first():
             if profile.local:  # Would only happen if saved directly through this class [not recommended]
                 raise ResourceWarning(  # Save through the Profile itself to avoid this
-                    f"Database profile with the name {name} already exists")
+                    f"Database profile with the name {profile.name} already exists")
             db_profile.update({'config': profile.to_pickle()})
         else:
             new_profile = Profiles(name=profile.name, config=profile.to_pickle())
             self.SESSION.add(new_profile)
 
         self.SESSION.commit()
```

### Comparing `insta-tweet-2.1.1/InstaTweet/instaclient.py` & `insta-tweet-2.1.2/InstaTweet/instaclient.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import os
 import requests
 from json.decoder import JSONDecodeError
 from . import InstaUser, InstaPost
 
 
 USER_AGENT = "Mozilla/5.0 (Linux; Android 9; GM1903 Build/PKQ1.190110.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/75.0.3770.143 Mobile Safari/537.36 Instagram 103.1.0.15.119 Android (28/9; 420dpi; 1080x2260; OnePlus; GM1903; OnePlus7; qcom; sv_SE; 164094539)"
-"""Hardcoded user agent proven to work with the :meth:`~.InstaClient.get_user` endpoint introduced in v2.0.0b13"""
+"""Hardcoded user agent proven to work with the :meth:`~.InstaClient.get_user` endpoint
+ 
+ :Version Added: ``v2.0.0b13``
+ """
 
 
 class InstaClient:
 
     """Minimalistic class for scraping/downloading Instagram user/media data"""
 
     DOWNLOAD_DIR = os.path.abspath('downloads')  #: [*Optional*] -- Directory to temporarily download media to
@@ -75,15 +78,15 @@
 
         :param post: the :class:`~.InstaPost` of the post to download
         :param filepath: the path to save the downloaded media; if ``None``, saves to the :attr:`~DOWNLOAD_DIR`
         """
         if post.is_carousel:
             for child in post.children:
                 self.download_post(child)
-            return all(child.is_downloaded for child in post.children)
+            return post.is_downloaded
 
         response = self.request(post.media_url)
         if not response.ok:
             print(f'Failed to download post {post.permalink} by {post.owner["username"]}')
             return False
 
         filepath = filepath if filepath else os.path.join(self.DOWNLOAD_DIR, post.filename)
```

### Comparing `insta-tweet-2.1.1/InstaTweet/instapost.py` & `insta-tweet-2.1.2/InstaTweet/instapost.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 import os
-from typing import Union
+from functools import cached_property
+from typing import Union, List
 from datetime import datetime
 from tweepy.models import Status
 
 
 class InstaPost:
 
     """Minimalistic API response wrapper for an Instagram post"""
 
     def __init__(self, post_data: dict):
         """Initialize an :class:`~InstaPost`
 
         :param post_data: the JSON response data of a single Instagram post, found within the :attr:`~.InstaUser.user_data`
         """
+        #: Source data from API response
         self.json = post_data
-        self.id = post_data['id']  #: The post id
-        self.is_video = post_data.get('is_video', False)  #: Indicates if the post is a video or photo
+        #: The post id
+        self.id = post_data['id']
+        self.dimensions: dict = post_data.get('dimensions', {})
+        self.is_video: bool = post_data.get('is_video', False)
         self.video_url = post_data.get('video_url', '')
-        self.dimensions = post_data.get('dimensions', {})
-        # Attributes set by other classes
-        self.filepath = ''      #:``str``: Path of downloaded media, set by :meth:`~.InstaClient.download_post`
-        self.tweet_data = {}    #:``dict``: Limited data from a successful tweet based off this post, set by :meth:`~.TweetClient.send_tweet`
-        self._children = []
+        #: Path of downloaded media, set by :meth:`~.InstaClient.download_post`
+        self.filepath: str = ''
+        #: Limited data from a successful tweet based off this post, set by :meth:`~.TweetClient.send_tweet`
+        self.tweet_data: dict = {}
 
     def __str__(self):
         return f'Post {self.id} by @{self.owner["username"]} on {self.timestamp}'
 
-    @property
-    def children(self) -> list:
+    @cached_property
+    def children(self) -> List["InstaPost"]:
         """If the post is a carousel, returns a list of child :class:`InstaPost`'s"""
-        if self.is_carousel and not self._children:
+        if self.is_carousel:
             edges = self.json['edge_sidecar_to_children']['edges']
-            self._children = [InstaPost(edge['node']) for edge in edges]
-        return self._children
+            return [InstaPost(edge['node']) for edge in edges]
+        return []
 
     @property
     def permalink(self) -> str:
         return f'https://www.instagram.com/p/{self.shortcode}'
 
     @property
     def shortcode(self) -> str:
@@ -75,18 +78,18 @@
     def is_carousel(self) -> bool:
         return 'edge_sidecar_to_children' in self.json
 
     @property
     def filename(self) -> str:
         """Concatenates :attr:`~id` + :attr:`~filetype` to create the default filename, for use when saving the post
 
-        :For Example:::
+        **For Example**::
 
-           >> print(post.filename)
-           "2868062811604347946.mp4"
+         >> print(post.filename)
+         "2868062811604347946.mp4"
 
         """
         return self.id + self.filetype
 
     @property
     def filetype(self) -> str:
         """Filetype of the post, based on the value of :attr:`~is_video`"""
```

### Comparing `insta-tweet-2.1.1/InstaTweet/instatweet.py` & `insta-tweet-2.1.2/InstaTweet/instatweet.py`

 * *Files identical despite different names*

### Comparing `insta-tweet-2.1.1/InstaTweet/instauser.py` & `insta-tweet-2.1.2/InstaTweet/instauser.py`

 * *Files identical despite different names*

### Comparing `insta-tweet-2.1.1/InstaTweet/profile.py` & `insta-tweet-2.1.2/InstaTweet/profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import os
 import copy
 import json
 import pickle
-
+from pathlib import Path
 from typing import Iterable
 from . import TweetClient, DBConnection, USER_AGENT
 
 
 class Profile:
 
     """The :class:`Profile` is a configuration class used extensively throughout the package
@@ -63,15 +63,15 @@
 
        * InstaTweet uses ``SQLAlchemy`` to create a :class:`~.DBConnection` -- any db it supports is compatible
        * See the :mod:`~.db` module for more information
 
     """
 
     USER_MAPPING = {'hashtags': [], 'scraped': [], 'tweets': []}  #: Template for an entry in the ``user_map``
-    LOCAL_DIR = os.path.abspath('profiles')  #: Directory where local profiles are saved
+    LOCAL_DIR = Path(__file__).parent.parent.joinpath("profiles") #: Directory where local profiles are saved
 
     def __init__(self, name: str = 'default', local: bool = True, **kwargs):
         """Create a new :class:`Profile`
 
         .. note:: :class:`Profile` creation is mandatory to use the ``InstaTweet`` package
 
            * Required as a parameter to initialize an :class:`~.InstaTweet` object
@@ -350,15 +350,15 @@
             :meth:`~profile_exists` with that name before actually updating it
 
             * This ensures that you don't accidentally overwrite a different Profile's save data
 
         ...
 
         :raises FileExistsError: if :attr:`~local` ``==True`` and a save is found in the :attr:`~LOCAL_DIR`
-        :raises ResourceWarning: if :attr:`~local` ``==False`` and a database row is found by :meth:`~.db.query_profile`
+        :raises ResourceWarning: if :attr:`~local` ``==False`` and a database row is found by :meth:`~.query_profile`
         """
         return self._name
 
     @name.setter
     def name(self, profile_name):
         """Sets the profile name, if a profile with that name doesn't already exist locally/remotely"""
         if profile_name != 'default' and self.profile_exists(profile_name, local=self.local):
```

### Comparing `insta-tweet-2.1.1/InstaTweet/tweetclient.py` & `insta-tweet-2.1.2/InstaTweet/tweetclient.py`

 * *Files 9% similar despite different names*

```diff
@@ -60,28 +60,23 @@
             access_token=api_keys['Access Token'],
             access_token_secret=api_keys['Token Secret']
         )
 
     def send_tweet(self, post: InstaPost, hashtags: Optional[list[str]] = None) -> bool:
         """Composes and sends a Tweet using an already-downloaded Instagram post
 
-        :param post: the post to tweet
-        :param hashtags: a list of hashtags to randomly chose from and include in the tweet
-
-        .. admonition:: How Tweets are Composed and Sent
+        .. admonition:: How Tweets are Sent
            :class: instatweet
 
            The :attr:`.InstaPost.filepath` -- set by :meth:`~.download_post` -- is used as the media source
 
-           The body of the tweet is then generated by :meth:`~build_tweet` as folows:
-
-             - The :attr:`InstaPost.caption` is used as a starting point
-             - If you've :meth:`~.add_hashtags` for the user, will randomly :meth:`~pick_hashtags` to include
-             - Lastly, the :attr:`InstaPost.permalink` is added to the end
+           The body of the tweet is then generated by :meth:`~build_tweet`
 
+        :param post: the post to tweet
+        :param hashtags: a list of hashtags to randomly chose from and include in the tweet
         """
         if not post.is_downloaded:
             raise FileNotFoundError('Post must be downloaded first')
 
         media_ids = self.upload_media(post)
         if not isinstance(media_ids, list):
             return False
@@ -128,15 +123,33 @@
 
         print(f'Successfully uploaded media to Twitter for {post}')
         return media_ids
 
     def build_tweet(self, post: InstaPost, hashtags: Optional[list[str]] = None) -> str:
         """Uses an :class:`~.InstaPost` to build the body text of a tweet
 
-        :param post: the post that's being tweeted; the caption and link are used
+        .. admonition:: How Tweets are Composed
+           :class: instatweet
+
+           - The :attr:`~.InstaPost.caption` is used as a starting point
+           - If you :meth:`~.add_hashtags` for the user, it will randomly :meth:`~pick_hashtags` to include
+           - Lastly, the post's :attr:`~.InstaPost.permalink` is added to the end
+
+        **Example**::
+
+         >> post = instatweet.insta.get_user("dailykittenig").posts[0]
+         >> tweet = instatweet.twitter.build_tweet(post)
+         >> print(tweet)
+
+         carousel support yuh
+         #kitten #kittycat #catlover #petstagram #animals
+
+         https://www.instagram.com/p/Cjl3UWBOd8k
+
+        :param post: the post being tweeted
         :param hashtags: optional list of hashtags to randomly pick from and include
         :return: the text to use for the tweet
         """
         tags = self.pick_hashtags(hashtags)
         caption = post.caption.strip().replace('@', '@/')  # Avoid tagging randos on Twitter
         characters = 280 - len(tags) - len(post.permalink) - 2
         tweet = "{text}\n{hashtags}\n{link}".format(
```

### Comparing `insta-tweet-2.1.1/InstaTweet/utils.py` & `insta-tweet-2.1.2/InstaTweet/utils.py`

 * *Files identical despite different names*

### Comparing `insta-tweet-2.1.1/LICENSE` & `insta-tweet-2.1.2/LICENSE`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `insta-tweet-2.1.1/PKG-INFO` & `insta-tweet-2.1.2/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,358 +1,410 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310d 0a4e 616d 653a 2069 6e73  : 2.1..Name: ins
-00000020: 7461 2d74 7765 6574 0d0a 5665 7273 696f  ta-tweet..Versio
-00000030: 6e3a 2032 2e31 2e31 0d0a 5375 6d6d 6172  n: 2.1.1..Summar
-00000040: 793a 2041 7574 6f6d 6174 6963 616c 6c79  y: Automatically
-00000050: 2052 6570 6f73 7420 436f 6e74 656e 7420   Repost Content 
-00000060: 4672 6f6d 2049 6e73 7461 6772 616d 2074  From Instagram t
-00000070: 6f20 5477 6974 7465 720d 0a48 6f6d 652d  o Twitter..Home-
-00000080: 7061 6765 3a20 6874 7470 733a 2f2f 7777  page: https://ww
-00000090: 772e 6769 7468 7562 2e63 6f6d 2f54 444b  w.github.com/TDK
-000000a0: 6f72 6e2f 696e 7374 612d 7477 6565 742f  orn/insta-tweet/
-000000b0: 0d0a 4175 7468 6f72 3a20 4164 616d 204b  ..Author: Adam K
-000000c0: 6f72 6e0d 0a41 7574 686f 722d 656d 6169  orn..Author-emai
-000000d0: 6c3a 2068 656c 6c6f 4064 6169 6c79 6b69  l: hello@dailyki
-000000e0: 7474 656e 2e6e 6574 0d0a 4c69 6365 6e73  tten.net..Licens
-000000f0: 653a 204d 4954 0d0a 446f 776e 6c6f 6164  e: MIT..Download
-00000100: 2d55 524c 3a20 6874 7470 733a 2f2f 6769  -URL: https://gi
-00000110: 7468 7562 2e63 6f6d 2f54 444b 6f72 6e2f  thub.com/TDKorn/
-00000120: 696e 7374 612d 7477 6565 742f 7461 7262  insta-tweet/tarb
-00000130: 616c 6c2f 322e 302e 302f 0d0a 4b65 7977  all/2.0.0/..Keyw
-00000140: 6f72 6473 3a20 696e 7374 6167 7261 6d2c  ords: instagram,
-00000150: 7477 6974 7465 722c 7265 706f 7374 2c72  twitter,repost,r
-00000160: 6570 6f73 7465 722c 696e 7374 6173 6372  eposter,instascr
-00000170: 6170 652c 696e 7374 6167 7261 6d2d 7265  ape,instagram-re
-00000180: 706f 7374 0d0a 506c 6174 666f 726d 3a20  post..Platform: 
-00000190: 554e 4b4e 4f57 4e0d 0a44 6573 6372 6970  UNKNOWN..Descrip
-000001a0: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
-000001b0: 653a 2074 6578 742f 782d 7273 743b 2063  e: text/x-rst; c
-000001c0: 6861 7273 6574 3d55 5446 2d38 0d0a 4c69  harset=UTF-8..Li
-000001d0: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
-000001e0: 4e53 450d 0a0d 0a2e 2e20 5f61 626f 7574  NSE...... _about
-000001f0: 2d69 6e73 7461 2d74 7765 6574 3a0d 0a0d  -insta-tweet:...
-00000200: 0ae2 9ca8 f09f 90a5 2049 6e73 7461 5477  ........ InstaTw
-00000210: 6565 7420 f09f 90a4 e29c a80d 0a2d 2d2d  eet .........---
-00000220: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000230: 2d2d 2d2d 0d0a 0d0a 2e2e 2069 6d61 6765  ----...... image
-00000240: 3a3a 2068 7474 7073 3a2f 2f69 6d67 2e73  :: https://img.s
-00000250: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
-00000260: 2f69 6e73 7461 2d74 7765 6574 0d0a 2020  /insta-tweet..  
-00000270: 203a 7461 7267 6574 3a20 6874 7470 733a   :target: https:
-00000280: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-00000290: 6374 2f69 6e73 7461 2d74 7765 6574 2f0d  ct/insta-tweet/.
-000002a0: 0a20 2020 3a61 6c74 3a20 5079 5049 2056  .   :alt: PyPI V
-000002b0: 6572 7369 6f6e 0d0a 0d0a 2e2e 2069 6d61  ersion...... ima
-000002c0: 6765 3a3a 2068 7474 7073 3a2f 2f72 6561  ge:: https://rea
-000002d0: 6474 6865 646f 6373 2e6f 7267 2f70 726f  dthedocs.org/pro
-000002e0: 6a65 6374 732f 696e 7374 6174 7765 6574  jects/instatweet
-000002f0: 2f62 6164 6765 2f3f 7665 7273 696f 6e3d  /badge/?version=
-00000300: 6c61 7465 7374 0d0a 2020 2020 3a74 6172  latest..    :tar
-00000310: 6765 743a 2068 7474 7073 3a2f 2f69 6e73  get: https://ins
-00000320: 7461 7477 6565 742e 7265 6164 7468 6564  tatweet.readthed
-00000330: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-00000340: 2f3f 6261 6467 653d 6c61 7465 7374 0d0a  /?badge=latest..
-00000350: 2020 2020 3a61 6c74 3a20 446f 6375 6d65      :alt: Docume
-00000360: 6e74 6174 696f 6e20 5374 6174 7573 0d0a  ntation Status..
-00000370: 0d0a 2e2e 2069 6d61 6765 3a3a 2068 7474  .... image:: htt
-00000380: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000390: 2e69 6f2f 6769 7468 7562 2f63 6f6d 6d69  .io/github/commi
-000003a0: 742d 6163 7469 7669 7479 2f6d 2f74 646b  t-activity/m/tdk
-000003b0: 6f72 6e2f 696e 7374 612d 7477 6565 740d  orn/insta-tweet.
-000003c0: 0a20 2020 203a 7461 7267 6574 3a20 6874  .    :target: ht
-000003d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000003e0: 2f74 646b 6f72 6e2f 696e 7374 612d 7477  /tdkorn/insta-tw
-000003f0: 6565 742f 7075 6c73 650d 0a20 2020 203a  eet/pulse..    :
-00000400: 616c 743a 2041 6374 6976 6974 790d 0a0d  alt: Activity...
-00000410: 0a0d 0a41 7574 6f6d 6174 6963 616c 6c79  ...Automatically
-00000420: 2052 6570 6f73 7420 436f 6e74 656e 7420   Repost Content 
-00000430: 4672 6f6d 2049 6e73 7461 6772 616d 2074  From Instagram t
-00000440: 6f20 5477 6974 7465 720d 0a7e 7e7e 7e7e  o Twitter..~~~~~
-00000450: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00000460: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00000470: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00000480: 7e7e 7e7e 7e7e 7e0d 0a0d 0a45 7665 7220  ~~~~~~~....Ever 
-00000490: 7472 6965 6420 7368 6172 696e 6720 616e  tried sharing an
-000004a0: 2049 6e73 7461 6772 616d 2070 6f73 7420   Instagram post 
-000004b0: 746f 2054 7769 7474 6572 2c20 6f6e 6c79  to Twitter, only
-000004c0: 2074 6f20 6669 6e64 206f 7574 2074 6861   to find out tha
-000004d0: 7420 616c 6c20 796f 7520 7477 6565 7465  t all you tweete
-000004e0: 6420 7761 7320 6120 6c69 6e6b 2c20 616e  d was a link, an
-000004f0: 6420 6e6f 7420 7468 6520 6163 7475 616c  d not the actual
-00000500: 2070 686f 746f 2f76 6964 656f 3f0d 0a0d   photo/video?...
-00000510: 0a2e 2e20 696d 6167 653a 3a20 6874 7470  ... image:: http
-00000520: 733a 2f2f 696e 7374 6174 7765 6574 2e72  s://instatweet.r
-00000530: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00000540: 2f6c 6174 6573 742f 5f69 6d61 6765 732f  /latest/_images/
-00000550: 7368 6172 655f 7769 7468 5f69 6e73 7461  share_with_insta
-00000560: 6772 616d 2e70 6e67 0d0a 2020 2020 3a61  gram.png..    :a
-00000570: 6c74 3a20 5368 6172 696e 6720 616e 2049  lt: Sharing an I
-00000580: 6e73 7461 6772 616d 2070 6f73 7420 746f  nstagram post to
-00000590: 2054 7769 7474 6572 2064 6972 6563 746c   Twitter directl
-000005a0: 7920 6672 6f6d 2074 6865 2049 6e73 7461  y from the Insta
-000005b0: 6772 616d 2061 7070 2e20 4f6e 6c79 2061  gram app. Only a
-000005c0: 206c 696e 6b20 6170 7065 6172 732e 0d0a   link appears...
-000005d0: 2020 2020 2020 2020 4974 2063 6f75 6c64          It could
-000005e0: 2062 6520 6c69 7465 7261 6c6c 7920 616e   be literally an
-000005f0: 7974 6869 6e67 2c20 6e6f 626f 6479 2077  ything, nobody w
-00000600: 696c 6c20 636c 6963 6b20 6974 2e0d 0a0d  ill click it....
-00000610: 0a0d 0a2e 2e20 6164 6d6f 6e69 7469 6f6e  ..... admonition
-00000620: 3a3a 202a 2a48 756d 696c 6961 7469 6e67  :: **Humiliating
-00000630: 20f0 9fa4 ae2a 2a0d 0a20 2020 3a63 6c61   ....**..   :cla
-00000640: 7373 3a20 696d 706f 7274 616e 742d 6166  ss: important-af
-00000650: 0d0a 0d0a 2020 2054 6861 7420 636f 756c  ....   That coul
-00000660: 6420 6265 206c 6974 6572 616c 6c79 2061  d be literally a
-00000670: 6e79 7468 696e 672e 204e 6f62 6f64 7920  nything. Nobody 
-00000680: 7769 6c6c 2063 6c69 636b 2069 742e 0d0a  will click it...
-00000690: 0d0a 7c0d 0a0d 0a0d 0a60 496e 7374 6154  ..|......`InstaT
-000006a0: 7765 6574 203c 6874 7470 733a 2f2f 6769  weet <https://gi
-000006b0: 7468 7562 2e63 6f6d 2f74 646b 6f72 6e2f  thub.com/tdkorn/
-000006c0: 696e 7374 612d 7477 6565 742f 626c 6f62  insta-tweet/blob
-000006d0: 2f76 322e 312e 312f 496e 7374 6154 7765  /v2.1.1/InstaTwe
-000006e0: 6574 2f69 6e73 7461 7477 6565 742e 7079  et/instatweet.py
-000006f0: 234c 352d 4c31 3432 3e60 5f20 2a2a 7368  #L5-L142>`_ **sh
-00000700: 6172 6573 2074 6865 2a2a 202a 6163 7475  ares the** *actu
-00000710: 616c 2a20 2a2a 636f 6e74 656e 7420 6f66  al* **content of
-00000720: 2074 6865 2070 6f73 742e 204e 6f74 206a   the post. Not j
-00000730: 7573 7420 6120 6c69 6e6b 2074 6f20 6974  ust a link to it
-00000740: 2e2a 2a0d 0a0d 0a0d 0a0d 0a2e 2e20 696d  .**.......... im
-00000750: 6167 653a 3a20 6874 7470 733a 2f2f 696e  age:: https://in
-00000760: 7374 6174 7765 6574 2e72 6561 6474 6865  statweet.readthe
-00000770: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-00000780: 742f 5f69 6d61 6765 732f 7368 6172 655f  t/_images/share_
-00000790: 7769 7468 5f69 6e73 7461 7477 6565 742e  with_instatweet.
-000007a0: 706e 670d 0a20 2020 203a 616c 743a 2053  png..    :alt: S
-000007b0: 6861 7269 6e67 2061 6e20 496e 7374 6167  haring an Instag
-000007c0: 7261 6d20 706f 7374 2074 6f20 5477 6974  ram post to Twit
-000007d0: 7465 7220 7573 696e 6720 496e 7374 6154  ter using InstaT
-000007e0: 7765 6574 2e20 5468 6520 6163 7475 616c  weet. The actual
-000007f0: 2070 686f 746f 206f 7220 7669 6465 6f20   photo or video 
-00000800: 6170 7065 6172 7320 696e 2074 6865 2074  appears in the t
-00000810: 7765 6574 2e0d 0a20 2020 2020 2020 2049  weet...        I
-00000820: 7427 7320 6120 7468 6963 6320 6361 742c  t's a thicc cat,
-00000830: 2076 6572 7920 6861 6e64 736f 6d65 2e20   very handsome. 
-00000840: 4e6f 626f 6479 2077 696c 6c20 636c 6963  Nobody will clic
-00000850: 6b20 7468 6520 6c69 6e6b 2c20 6275 7420  k the link, but 
-00000860: 7468 6579 276c 6c20 6465 6669 6e69 7465  they'll definite
-00000870: 6c79 2073 6565 2074 6869 7320 6261 6420  ly see this bad 
-00000880: 626f 792e 0d0a 0d0a 0d0a 5769 7468 2060  boy.......With `
-00000890: 6049 6e73 7461 5477 6565 7460 602c 2079  `InstaTweet``, y
-000008a0: 6f75 2063 616e 2072 6573 7420 6561 7379  ou can rest easy
-000008b0: 206b 6e6f 7769 6e67 2074 6861 742c 0d0a   knowing that,..
-000008c0: 616c 7468 6f75 6768 206e 6f62 6f64 7920  although nobody 
-000008d0: 7769 6c6c 2063 6c69 636b 2074 6865 206c  will click the l
-000008e0: 696e 6b2c 2074 6865 7927 6c6c 2061 7420  ink, they'll at 
-000008f0: 6c65 6173 7420 7365 6520 7768 6174 2079  least see what y
-00000900: 6f75 2070 6f73 7465 642e 0d0a 0d0a 0d0a  ou posted.......
-00000910: 0d0a 5768 6174 2773 2049 6e73 7461 5477  ..What's InstaTw
-00000920: 6565 743f 0d0a 7e7e 7e7e 7e7e 7e7e 7e7e  eet?..~~~~~~~~~~
-00000930: 7e7e 7e7e 7e7e 7e7e 7e7e 7e0d 0a0d 0a60  ~~~~~~~~~~~....`
-00000940: 496e 7374 6154 7765 6574 203c 6874 7470  InstaTweet <http
-00000950: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
-00000960: 646b 6f72 6e2f 696e 7374 612d 7477 6565  dkorn/insta-twee
-00000970: 742f 626c 6f62 2f76 322e 312e 312f 496e  t/blob/v2.1.1/In
-00000980: 7374 6154 7765 6574 2f69 6e73 7461 7477  staTweet/instatw
-00000990: 6565 742e 7079 234c 352d 4c31 3432 3e60  eet.py#L5-L142>`
-000009a0: 5f20 6973 2061 2063 7573 746f 6d69 7a61  _ is a customiza
-000009b0: 626c 6520 746f 6f6c 2074 6f20 6175 746f  ble tool to auto
-000009c0: 6d61 7469 6361 6c6c 7920 7265 706f 7374  matically repost
-000009d0: 2063 6f6e 7465 6e74 2066 726f 6d20 496e   content from In
-000009e0: 7374 6167 7261 6d20 746f 2054 7769 7474  stagram to Twitt
-000009f0: 6572 2e0d 0a0d 0a53 696d 706c 7920 6372  er.....Simply cr
-00000a00: 6561 7465 2061 2060 5072 6f66 696c 6520  eate a `Profile 
-00000a10: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
-00000a20: 636f 6d2f 7464 6b6f 726e 2f69 6e73 7461  com/tdkorn/insta
-00000a30: 2d74 7765 6574 2f62 6c6f 622f 7632 2e31  -tweet/blob/v2.1
-00000a40: 2e31 2f49 6e73 7461 5477 6565 742f 7072  .1/InstaTweet/pr
-00000a50: 6f66 696c 652e 7079 234c 3132 2d4c 3431  ofile.py#L12-L41
-00000a60: 363e 605f 2c0d 0a63 6f6e 6669 6775 7265  6>`_,..configure
-00000a70: 2074 6865 2060 6d61 6e64 6174 6f72 792d   the `mandatory-
-00000a80: 7365 7474 696e 6773 203c 6874 7470 733a  settings <https:
-00000a90: 2f2f 696e 7374 6174 7765 6574 2e72 6561  //instatweet.rea
-00000aa0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00000ab0: 6174 6573 742f 5f72 6561 646d 652f 6765  atest/_readme/ge
-00000ac0: 7474 696e 672d 7374 6172 7465 642e 6874  tting-started.ht
-00000ad0: 6d6c 236d 616e 6461 746f 7279 2d73 6574  ml#mandatory-set
-00000ae0: 7469 6e67 733e 605f 2c0d 0a61 6e64 2060  tings>`_,..and `
-00000af0: 6164 645f 7573 6572 7328 2920 3c68 7474  add_users() <htt
-00000b00: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000b10: 7464 6b6f 726e 2f69 6e73 7461 2d74 7765  tdkorn/insta-twe
-00000b20: 6574 2f62 6c6f 622f 7632 2e31 2e31 2f49  et/blob/v2.1.1/I
-00000b30: 6e73 7461 5477 6565 742f 7072 6f66 696c  nstaTweet/profil
-00000b40: 652e 7079 234c 3136 372d 4c31 3937 3e60  e.py#L167-L197>`
-00000b50: 5f20 746f 2072 6570 6f73 7420 6672 6f6d  _ to repost from
-00000b60: 0d0a 0d0a 2e2e 2063 6f64 652d 626c 6f63  ...... code-bloc
-00000b70: 6b3a 3a20 7079 7468 6f6e 0d0a 0d0a 2020  k:: python....  
-00000b80: 2020 6672 6f6d 2049 6e73 7461 5477 6565    from InstaTwee
-00000b90: 7420 696d 706f 7274 2050 726f 6669 6c65  t import Profile
-00000ba0: 0d0a 0d0a 2020 2020 2320 4372 6561 7465  ....    # Create
-00000bb0: 2061 206e 6577 2028 6c6f 6361 6c29 2050   a new (local) P
-00000bc0: 726f 6669 6c65 0d0a 2020 2020 3e3e 3e20  rofile..    >>> 
-00000bd0: 7072 6f66 696c 6520 3d20 5072 6f66 696c  profile = Profil
-00000be0: 6528 276d 7950 726f 6669 6c65 2729 0d0a  e('myProfile')..
-00000bf0: 0d0a 2020 2020 2320 436f 6e66 6967 7572  ..    # Configur
-00000c00: 6520 7468 6520 7265 7175 6972 6564 2073  e the required s
-00000c10: 6574 7469 6e67 7320 2861 7420 6d69 6e69  ettings (at mini
-00000c20: 6d75 6d29 0d0a 2020 2020 3e3e 3e20 7072  mum)..    >>> pr
-00000c30: 6f66 696c 652e 7477 6974 7465 725f 6b65  ofile.twitter_ke
-00000c40: 7973 203d 2074 7769 7474 6572 5f61 7069  ys = twitter_api
-00000c50: 5f6b 6579 730d 0a20 2020 203e 3e3e 2070  _keys..    >>> p
-00000c60: 726f 6669 6c65 2e73 6573 7369 6f6e 5f69  rofile.session_i
-00000c70: 6420 3d20 2736 3031 3139 3931 4127 0d0a  d = '6011991A'..
-00000c80: 0d0a 2020 2020 2320 4164 6420 6174 206c  ..    # Add at l
-00000c90: 6561 7374 206f 6e65 2049 6e73 7461 6772  east one Instagr
-00000ca0: 616d 2061 6363 6f75 6e74 2074 6f20 7265  am account to re
-00000cb0: 706f 7374 2066 726f 6d0d 0a20 2020 203e  post from..    >
-00000cc0: 3e3e 2070 726f 6669 6c65 2e61 6464 5f75  >> profile.add_u
-00000cd0: 7365 7273 2827 7468 652e 6461 696c 796b  sers('the.dailyk
-00000ce0: 6974 7465 6e27 290d 0a0d 0a0d 0a4f 6e63  itten')......Onc
-00000cf0: 6520 636f 6e66 6967 7572 6564 2c20 7468  e configured, th
-00000d00: 6520 6050 726f 6669 6c65 203c 6874 7470  e `Profile <http
-00000d10: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
-00000d20: 646b 6f72 6e2f 696e 7374 612d 7477 6565  dkorn/insta-twee
-00000d30: 742f 626c 6f62 2f76 322e 312e 312f 496e  t/blob/v2.1.1/In
-00000d40: 7374 6154 7765 6574 2f70 726f 6669 6c65  staTweet/profile
-00000d50: 2e70 7923 4c31 322d 4c34 3136 3e60 5f20  .py#L12-L416>`_ 
-00000d60: 6361 6e20 6265 2075 7365 6420 746f 2069  can be used to i
-00000d70: 6e69 7469 616c 697a 6520 616e 640d 0a60  nitialize and..`
-00000d80: 7374 6172 7428 2920 3c68 7474 7073 3a2f  start() <https:/
-00000d90: 2f67 6974 6875 622e 636f 6d2f 7464 6b6f  /github.com/tdko
-00000da0: 726e 2f69 6e73 7461 2d74 7765 6574 2f62  rn/insta-tweet/b
-00000db0: 6c6f 622f 7632 2e31 2e31 2f49 6e73 7461  lob/v2.1.1/Insta
-00000dc0: 5477 6565 742f 696e 7374 6174 7765 6574  Tweet/instatweet
-00000dd0: 2e70 7923 4c37 322d 4c31 3137 3e60 5f20  .py#L72-L117>`_ 
-00000de0: 616e 2060 496e 7374 6154 7765 6574 203c  an `InstaTweet <
-00000df0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000e00: 6f6d 2f74 646b 6f72 6e2f 696e 7374 612d  om/tdkorn/insta-
-00000e10: 7477 6565 742f 626c 6f62 2f76 322e 312e  tweet/blob/v2.1.
-00000e20: 312f 496e 7374 6154 7765 6574 2f69 6e73  1/InstaTweet/ins
-00000e30: 7461 7477 6565 742e 7079 234c 352d 4c31  tatweet.py#L5-L1
-00000e40: 3432 3e60 5f20 6f62 6a65 6374 0d0a 0d0a  42>`_ object....
-00000e50: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
-00000e60: 7079 7468 6f6e 0d0a 0d0a 2020 2020 6672  python....    fr
-00000e70: 6f6d 2049 6e73 7461 5477 6565 7420 696d  om InstaTweet im
-00000e80: 706f 7274 2049 6e73 7461 5477 6565 740d  port InstaTweet.
-00000e90: 0a0d 0a20 2020 2023 2044 6972 6563 746c  ...    # Directl
-00000ea0: 7920 696e 6974 6961 6c69 7a65 2077 6974  y initialize wit
-00000eb0: 6820 7468 6520 5072 6f66 696c 6520 6672  h the Profile fr
-00000ec0: 6f6d 2061 626f 7665 0d0a 2020 2020 3e3e  om above..    >>
-00000ed0: 3e20 696e 7374 615f 7477 6565 7420 3d20  > insta_tweet = 
-00000ee0: 496e 7374 6154 7765 6574 2870 726f 6669  InstaTweet(profi
-00000ef0: 6c65 290d 0a0d 0a20 2020 2023 204f 722c  le)....    # Or,
-00000f00: 2073 6176 6520 7468 6520 5072 6f66 696c   save the Profil
-00000f10: 652e 2e2e 0d0a 2020 2020 3e3e 3e20 7072  e.....    >>> pr
-00000f20: 6f66 696c 652e 7361 7665 2829 0d0a 0d0a  ofile.save()....
-00000f30: 2020 2020 5361 7665 6420 4c6f 6361 6c20      Saved Local 
-00000f40: 5072 6f66 696c 6520 6d79 5072 6f66 696c  Profile myProfil
-00000f50: 650d 0a0d 0a20 2020 2023 202e 2e2e 7468  e....    # ...th
-00000f60: 656e 2049 6e73 7461 5477 6565 742e 6c6f  en InstaTweet.lo
-00000f70: 6164 2829 2074 6865 2073 6574 7469 6e67  ad() the setting
-00000f80: 7320 696e 2028 6279 2050 726f 6669 6c65  s in (by Profile
-00000f90: 206e 616d 6529 0d0a 2020 2020 3e3e 3e20   name)..    >>> 
-00000fa0: 696e 7374 615f 7477 6565 7420 3d20 496e  insta_tweet = In
-00000fb0: 7374 6154 7765 6574 2e6c 6f61 6428 7072  staTweet.load(pr
-00000fc0: 6f66 696c 655f 6e61 6d65 3d22 6d79 5072  ofile_name="myPr
-00000fd0: 6f66 696c 6522 290d 0a0d 0a20 2020 2023  ofile")....    #
-00000fe0: 2052 756e 2049 6e73 7461 5477 6565 7420   Run InstaTweet 
-00000ff0: 6279 2063 616c 6c69 6e67 2073 7461 7274  by calling start
-00001000: 2829 0d0a 2020 2020 3e3e 3e20 696e 7374  ()..    >>> inst
-00001010: 615f 7477 6565 742e 7374 6172 7428 290d  a_tweet.start().
-00001020: 0a0d 0a0d 0a2e 2e20 696d 6167 653a 3a20  ....... image:: 
-00001030: 6874 7470 733a 2f2f 7573 6572 2d69 6d61  https://user-ima
-00001040: 6765 732e 6769 7468 7562 7573 6572 636f  ges.githubuserco
-00001050: 6e74 656e 742e 636f 6d2f 3936 3339 3436  ntent.com/963946
-00001060: 3532 2f31 3837 3135 3836 3137 2d66 3435  52/187158617-f45
-00001070: 3736 3161 622d 3361 6139 2d34 3732 662d  761ab-3aa9-472f-
-00001080: 6136 6662 2d61 3939 6364 3063 6539 3030  a6fb-a99cd0ce900
-00001090: 632e 706e 670d 0a0d 0a0d 0a41 7320 6060  c.png......As ``
-000010a0: 496e 7374 6154 7765 6574 6060 2072 756e  InstaTweet`` run
-000010b0: 732c 2069 7473 2070 726f 6772 6573 7320  s, its progress 
-000010c0: 7769 6c6c 2062 6520 6c6f 6767 6564 2074  will be logged t
-000010d0: 6f20 636f 6e73 6f6c 653a 0d0a 0d0a 2e2e  o console:......
-000010e0: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-000010f0: 7468 6f6e 0d0a 0d0a 2020 2020 5374 6172  thon....    Star
-00001100: 7469 6e67 2049 6e73 7461 5477 6565 7420  ting InstaTweet 
-00001110: 666f 7220 5072 6f66 696c 653a 206d 7950  for Profile: myP
-00001120: 726f 6669 6c65 0d0a 2020 2020 4368 6563  rofile..    Chec
-00001130: 6b69 6e67 2070 6f73 7473 2066 726f 6d20  king posts from 
-00001140: 4074 6865 2e64 6169 6c79 6b69 7474 656e  @the.dailykitten
-00001150: 0d0a 2020 2020 2e2e 2e0d 0a20 2020 2046  ..    .....    F
-00001160: 696e 6973 6865 6420 696e 7374 612d 7477  inished insta-tw
-00001170: 6565 7469 6e67 2066 6f72 2040 7468 652e  eeting for @the.
-00001180: 6461 696c 796b 6974 7465 6e0d 0a20 2020  dailykitten..   
-00001190: 2041 6c6c 2075 7365 7273 2068 6176 6520   All users have 
-000011a0: 6265 656e 2069 6e73 7461 2d74 7765 6574  been insta-tweet
-000011b0: 6564 0d0a 0d0a 0d0a 4f6b 6179 2e2e 2e20  ed......Okay... 
-000011c0: 4275 7420 5768 793f 20f0 9f98 9f0d 0a7e  But Why? ......~
-000011d0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-000011e0: 7e7e 7e7e 7e7e 0d0a 0d0a 2e2e 2061 646d  ~~~~~~...... adm
-000011f0: 6f6e 6974 696f 6e3a 3a20 4275 7420 5768  onition:: But Wh
-00001200: 793f 20f0 9fa4 a80d 0a20 2020 3a63 6c61  y? ......   :cla
-00001210: 7373 3a20 696e 7374 6174 7765 6574 0d0a  ss: instatweet..
-00001220: 0d0a 2020 202a 2a49 6e73 7461 5477 6565  ..   **InstaTwee
-00001230: 7420 6861 7320 7477 6f20 6d61 696e 2075  t has two main u
-00001240: 7365 2063 6173 6573 3a2a 2a0d 0a0d 0a20  se cases:**.... 
-00001250: 2020 2a20 546f 2061 7574 6f6d 6174 6963    * To automatic
-00001260: 616c 6c79 2073 6861 7265 2079 6f75 7220  ally share your 
-00001270: 6f77 6e20 496e 7374 6167 7261 6d20 706f  own Instagram po
-00001280: 7374 7320 746f 2054 7769 7474 6572 0d0a  sts to Twitter..
-00001290: 2020 202a 2054 6f20 6175 746f 6d61 7469     * To automati
-000012a0: 6361 6c6c 7920 7477 6565 7420 6e65 7720  cally tweet new 
-000012b0: 636f 6e74 656e 7420 6672 6f6d 206f 7468  content from oth
-000012c0: 6572 2049 6e73 7461 6772 616d 2075 7365  er Instagram use
-000012d0: 7273 0d0a 0d0a 2020 2052 6567 6172 646c  rs....   Regardl
-000012e0: 6573 7320 6f66 2079 6f75 7220 696e 7465  ess of your inte
-000012f0: 6e74 696f 6e2c 2049 6e73 7461 5477 6565  ntion, InstaTwee
-00001300: 7420 7769 6c6c 2064 6574 6563 7420 6e65  t will detect ne
-00001310: 7720 706f 7374 7320 6672 6f6d 2074 6865  w posts from the
-00001320: 2075 7365 7273 2079 6f75 2073 7065 6369   users you speci
-00001330: 6679 2c20 646f 776e 6c6f 6164 2074 6865  fy, download the
-00001340: 6d2c 2061 6e64 2072 6570 6f73 740d 0a20  m, and repost.. 
-00001350: 2020 7468 656d 2074 6f20 5477 6974 7465    them to Twitte
-00001360: 722e 0d0a 0d0a 0d0a 446f 6375 6d65 6e74  r.......Document
-00001370: 6174 696f 6e0d 0a7e 7e7e 7e7e 7e7e 7e7e  ation..~~~~~~~~~
-00001380: 7e7e 7e7e 7e7e 7e7e 0d0a 0d0a 5468 6520  ~~~~~~~~....The 
-00001390: 7265 7374 206f 6620 7468 6973 2060 5245  rest of this `RE
-000013a0: 4144 4d45 203c 6874 7470 733a 2f2f 696e  ADME <https://in
-000013b0: 7374 6174 7765 6574 2e72 6561 6474 6865  statweet.readthe
-000013c0: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-000013d0: 742f 5f72 6561 646d 652f 6162 6f75 742d  t/_readme/about-
-000013e0: 696e 7374 6174 7765 6574 2e68 746d 6c3e  instatweet.html>
-000013f0: 605f 2c0d 0a74 6865 2060 4150 4920 646f  `_,..the `API do
-00001400: 6375 6d65 6e74 6174 696f 6e20 3c68 7474  cumentation <htt
-00001410: 7073 3a2f 2f69 6e73 7461 7477 6565 742e  ps://instatweet.
-00001420: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-00001430: 6e2f 6c61 7465 7374 2f6d 6f64 756c 6573  n/latest/modules
-00001440: 2e68 746d 6c3e 605f 2c20 616e 640d 0a60  .html>`_, and..`
-00001450: 736e 6970 7065 7473 203c 6874 7470 733a  snippets <https:
-00001460: 2f2f 696e 7374 6174 7765 6574 2e72 6561  //instatweet.rea
-00001470: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00001480: 6174 6573 742f 736e 6970 7065 7473 2e68  atest/snippets.h
-00001490: 746d 6c3e 605f 0d0a 6361 6e20 616c 6c20  tml>`_..can all 
-000014a0: 6265 2066 6f75 6e64 206f 6e20 6052 6561  be found on `Rea
-000014b0: 6420 7468 6520 446f 6373 203c 6874 7470  d the Docs <http
-000014c0: 733a 2f2f 696e 7374 6174 7765 6574 2e72  s://instatweet.r
-000014d0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-000014e0: 2f6c 6174 6573 742f 696e 6465 782e 6874  /latest/index.ht
-000014f0: 6d6c 3e60 5f0d 0a0d 0a49 2070 7574 2061  ml>`_....I put a
-00001500: 206c 6f74 206f 6620 7469 6d65 2069 6e74   lot of time int
-00001510: 6f20 6372 6561 7469 6e67 2074 6865 2064  o creating the d
-00001520: 6f63 756d 656e 7461 7469 6f6e 2066 6f72  ocumentation for
-00001530: 2074 6869 7320 7061 636b 6167 652c 2069   this package, i
-00001540: 7420 7761 7320 6120 7374 7275 6767 6c65  t was a struggle
-00001550: 2c0d 0a73 6f20 6974 2764 206d 6561 6e20  ,..so it'd mean 
-00001560: 6120 6c6f 7420 746f 206d 6520 6966 2079  a lot to me if y
-00001570: 6f75 2063 6f75 6c64 2070 6c65 6173 6520  ou could please 
-00001580: 636f 6e74 696e 7565 2072 6561 6469 6e67  continue reading
-00001590: 2074 6865 7265 2120 f09f a5b0 0d0a 0d0a   there! ........
-000015a0: 0d0a 0d0a 496e 7374 616c 6c61 7469 6f6e  ....Installation
-000015b0: 0d0a 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ..~~~~~~~~~~~~~~
-000015c0: 0d0a 0d0a 546f 2069 6e73 7461 6c6c 2075  ....To install u
-000015d0: 7369 6e67 2070 6970 3a0d 0a0d 0a2e 2e20  sing pip:...... 
-000015e0: 636f 6465 2d62 6c6f 636b 3a3a 2073 6865  code-block:: she
-000015f0: 6c6c 0d0a 0d0a 2020 2020 7069 7020 696e  ll....    pip in
-00001600: 7374 616c 6c20 696e 7374 612d 7477 6565  stall insta-twee
-00001610: 740d 0a0d 0a0d 0a50 6c65 6173 6520 6e6f  t......Please no
-00001620: 7465 2074 6861 7420 6060 496e 7374 6154  te that ``InstaT
-00001630: 7765 6574 6060 2072 6571 7569 7265 7320  weet`` requires 
-00001640: 6060 5079 7468 6f6e 203e 3d20 332e 3860  ``Python >= 3.8`
-00001650: 600d 0a0d 0a0d 0a                        `......
+00000000: 2e2e 206d 6574 613a 3a0d 0a20 2020 3a74  .. meta::..   :t
+00000010: 6974 6c65 3a20 496e 7374 6154 7765 6574  itle: InstaTweet
+00000020: 202d 2041 7574 6f6d 6174 6963 616c 6c79   - Automatically
+00000030: 2052 6570 6f73 7420 436f 6e74 656e 7420   Repost Content 
+00000040: 4672 6f6d 2049 6e73 7461 6772 616d 2074  From Instagram t
+00000050: 6f20 5477 6974 7465 720d 0a20 2020 3a64  o Twitter..   :d
+00000060: 6573 6372 6970 7469 6f6e 3a20 4120 5079  escription: A Py
+00000070: 7468 6f6e 2070 6163 6b61 6765 2074 6f20  thon package to 
+00000080: 6175 746f 6d61 7469 6361 6c6c 7920 7265  automatically re
+00000090: 706f 7374 2063 6f6e 7465 6e74 2066 726f  post content fro
+000000a0: 6d20 496e 7374 6167 7261 6d20 746f 2054  m Instagram to T
+000000b0: 7769 7474 6572 0d0a 0d0a 2e2e 207c 2e49  witter...... |.I
+000000c0: 6e73 7461 5477 6565 747c 2072 6570 6c61  nstaTweet| repla
+000000d0: 6365 3a3a 2060 6049 6e73 7461 5477 6565  ce:: ``InstaTwee
+000000e0: 7460 600d 0a2e 2e20 5f2e 496e 7374 6154  t``.... _.InstaT
+000000f0: 7765 6574 3a20 6874 7470 733a 2f2f 6769  weet: https://gi
+00000100: 7468 7562 2e63 6f6d 2f74 646b 6f72 6e2f  thub.com/tdkorn/
+00000110: 696e 7374 612d 7477 6565 742f 626c 6f62  insta-tweet/blob
+00000120: 2f6d 6173 7465 722f 496e 7374 6154 7765  /master/InstaTwe
+00000130: 6574 2f69 6e73 7461 7477 6565 742e 7079  et/instatweet.py
+00000140: 234c 352d 4c31 3432 0d0a 2e2e 207c 2e61  #L5-L142.... |.a
+00000150: 6464 5f75 7365 7273 7c20 7265 706c 6163  dd_users| replac
+00000160: 653a 3a20 6060 6164 645f 7573 6572 7328  e:: ``add_users(
+00000170: 2960 600d 0a2e 2e20 5f2e 6164 645f 7573  )``.... _.add_us
+00000180: 6572 733a 2068 7474 7073 3a2f 2f67 6974  ers: https://git
+00000190: 6875 622e 636f 6d2f 7464 6b6f 726e 2f69  hub.com/tdkorn/i
+000001a0: 6e73 7461 2d74 7765 6574 2f62 6c6f 622f  nsta-tweet/blob/
+000001b0: 6d61 7374 6572 2f49 6e73 7461 5477 6565  master/InstaTwee
+000001c0: 742f 7072 6f66 696c 652e 7079 234c 3136  t/profile.py#L16
+000001d0: 372d 4c31 3937 0d0a 2e2e 207c 2e50 726f  7-L197.... |.Pro
+000001e0: 6669 6c65 7c20 7265 706c 6163 653a 3a20  file| replace:: 
+000001f0: 6060 5072 6f66 696c 6560 600d 0a2e 2e20  ``Profile``.... 
+00000200: 5f2e 5072 6f66 696c 653a 2068 7474 7073  _.Profile: https
+00000210: 3a2f 2f67 6974 6875 622e 636f 6d2f 7464  ://github.com/td
+00000220: 6b6f 726e 2f69 6e73 7461 2d74 7765 6574  korn/insta-tweet
+00000230: 2f62 6c6f 622f 6d61 7374 6572 2f49 6e73  /blob/master/Ins
+00000240: 7461 5477 6565 742f 7072 6f66 696c 652e  taTweet/profile.
+00000250: 7079 234c 3132 2d4c 3431 360d 0a2e 2e20  py#L12-L416.... 
+00000260: 7c2e 7374 6172 747c 2072 6570 6c61 6365  |.start| replace
+00000270: 3a3a 2060 6073 7461 7274 2829 6060 0d0a  :: ``start()``..
+00000280: 2e2e 205f 2e73 7461 7274 3a20 6874 7470  .. _.start: http
+00000290: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
+000002a0: 646b 6f72 6e2f 696e 7374 612d 7477 6565  dkorn/insta-twee
+000002b0: 742f 626c 6f62 2f6d 6173 7465 722f 496e  t/blob/master/In
+000002c0: 7374 6154 7765 6574 2f69 6e73 7461 7477  staTweet/instatw
+000002d0: 6565 742e 7079 234c 3732 2d4c 3131 370d  eet.py#L72-L117.
+000002e0: 0a2e 2e20 7c2e 496e 7374 6143 6c69 656e  ... |.InstaClien
+000002f0: 747c 2072 6570 6c61 6365 3a3a 2060 6049  t| replace:: ``I
+00000300: 6e73 7461 436c 6965 6e74 6060 0d0a 2e2e  nstaClient``....
+00000310: 205f 2e49 6e73 7461 436c 6965 6e74 3a20   _.InstaClient: 
+00000320: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000330: 6f6d 2f74 646b 6f72 6e2f 696e 7374 612d  om/tdkorn/insta-
+00000340: 7477 6565 742f 626c 6f62 2f6d 6173 7465  tweet/blob/maste
+00000350: 722f 496e 7374 6154 7765 6574 2f69 6e73  r/InstaTweet/ins
+00000360: 7461 636c 6965 6e74 2e70 7923 4c31 342d  taclient.py#L14-
+00000370: 4c31 3038 0d0a 2e2e 207c 6d61 6e64 6174  L108.... |mandat
+00000380: 6f72 792d 7365 7474 696e 6773 7c20 7265  ory-settings| re
+00000390: 706c 6163 653a 3a20 6d61 6e64 6174 6f72  place:: mandator
+000003a0: 7920 7365 7474 696e 6773 0d0a 2e2e 205f  y settings.... _
+000003b0: 6d61 6e64 6174 6f72 792d 7365 7474 696e  mandatory-settin
+000003c0: 6773 3a20 6874 7470 733a 2f2f 696e 7374  gs: https://inst
+000003d0: 6174 7765 6574 2e72 6561 6474 6865 646f  atweet.readthedo
+000003e0: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+000003f0: 5f72 6561 646d 652f 6765 7474 696e 672d  _readme/getting-
+00000400: 7374 6172 7465 642e 6874 6d6c 236d 616e  started.html#man
+00000410: 6461 746f 7279 2d73 6574 7469 6e67 730d  datory-settings.
+00000420: 0a0d 0a2e 2e20 5f61 626f 7574 2d69 6e73  ..... _about-ins
+00000430: 7461 2d74 7765 6574 3a0d 0a0d 0ae2 9ca8  ta-tweet:.......
+00000440: f09f 90a5 2049 6e73 7461 5477 6565 7420  .... InstaTweet 
+00000450: f09f 90a4 e29c a80d 0a2d 2d2d 2d2d 2d2d  .........-------
+00000460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000470: 0d0a 0d0a 2e2e 2069 6d61 6765 3a3a 2068  ...... image:: h
+00000480: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000490: 6473 2e69 6f2f 7079 7069 2f76 2f69 6e73  ds.io/pypi/v/ins
+000004a0: 7461 2d74 7765 6574 0d0a 2020 203a 7461  ta-tweet..   :ta
+000004b0: 7267 6574 3a20 6874 7470 733a 2f2f 7079  rget: https://py
+000004c0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f69  pi.org/project/i
+000004d0: 6e73 7461 2d74 7765 6574 2f0d 0a20 2020  nsta-tweet/..   
+000004e0: 3a61 6c74 3a20 5079 5049 2056 6572 7369  :alt: PyPI Versi
+000004f0: 6f6e 0d0a 0d0a 2e2e 2069 6d61 6765 3a3a  on...... image::
+00000500: 2068 7474 7073 3a2f 2f69 6d67 2e73 6869   https://img.shi
+00000510: 656c 6473 2e69 6f2f 6261 6467 652f 4769  elds.io/badge/Gi
+00000520: 7448 7562 2d69 6e73 7461 2d2d 7477 6565  tHub-insta--twee
+00000530: 742d 3466 3161 6263 0d0a 2020 203a 7461  t-4f1abc..   :ta
+00000540: 7267 6574 3a20 6874 7470 733a 2f2f 6769  rget: https://gi
+00000550: 7468 7562 2e63 6f6d 2f74 646b 6f72 6e2f  thub.com/tdkorn/
+00000560: 696e 7374 612d 7477 6565 740d 0a20 2020  insta-tweet..   
+00000570: 3a61 6c74 3a20 4769 7448 7562 2052 6570  :alt: GitHub Rep
+00000580: 6f73 6974 6f72 790d 0a0d 0a2e 2e20 696d  ository...... im
+00000590: 6167 653a 3a20 6874 7470 733a 2f2f 7374  age:: https://st
+000005a0: 6174 6963 2e70 6570 792e 7465 6368 2f70  atic.pepy.tech/p
+000005b0: 6572 736f 6e61 6c69 7a65 642d 6261 6467  ersonalized-badg
+000005c0: 652f 696e 7374 612d 7477 6565 743f 7065  e/insta-tweet?pe
+000005d0: 7269 6f64 3d74 6f74 616c 2675 6e69 7473  riod=total&units
+000005e0: 3d6e 6f6e 6526 6c65 6674 5f63 6f6c 6f72  =none&left_color
+000005f0: 3d67 7265 7926 7269 6768 745f 636f 6c6f  =grey&right_colo
+00000600: 723d 626c 7565 266c 6566 745f 7465 7874  r=blue&left_text
+00000610: 3d44 6f77 6e6c 6f61 6473 0d0a 2020 2020  =Downloads..    
+00000620: 3a74 6172 6765 743a 2068 7474 7073 3a2f  :target: https:/
+00000630: 2f70 6570 792e 7465 6368 2f70 726f 6a65  /pepy.tech/proje
+00000640: 6374 2f69 6e73 7461 2d74 7765 6574 0d0a  ct/insta-tweet..
+00000650: 0d0a 2e2e 2069 6d61 6765 3a3a 2068 7474  .... image:: htt
+00000660: 7073 3a2f 2f72 6561 6474 6865 646f 6373  ps://readthedocs
+00000670: 2e6f 7267 2f70 726f 6a65 6374 732f 696e  .org/projects/in
+00000680: 7374 6174 7765 6574 2f62 6164 6765 2f3f  statweet/badge/?
+00000690: 7665 7273 696f 6e3d 6c61 7465 7374 0d0a  version=latest..
+000006a0: 2020 2020 3a74 6172 6765 743a 2068 7474      :target: htt
+000006b0: 7073 3a2f 2f69 6e73 7461 7477 6565 742e  ps://instatweet.
+000006c0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+000006d0: 6e2f 6c61 7465 7374 2f3f 6261 6467 653d  n/latest/?badge=
+000006e0: 6c61 7465 7374 0d0a 2020 2020 3a61 6c74  latest..    :alt
+000006f0: 3a20 446f 6375 6d65 6e74 6174 696f 6e20  : Documentation 
+00000700: 5374 6174 7573 0d0a 0d0a 0d0a 4175 746f  Status......Auto
+00000710: 6d61 7469 6361 6c6c 7920 5265 706f 7374  matically Repost
+00000720: 2043 6f6e 7465 6e74 2046 726f 6d20 496e   Content From In
+00000730: 7374 6167 7261 6d20 746f 2054 7769 7474  stagram to Twitt
+00000740: 6572 0d0a 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  er..~~~~~~~~~~~~
+00000750: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+00000760: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+00000770: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+00000780: 0d0a 0d0a 4576 6572 2074 7269 6564 2073  ....Ever tried s
+00000790: 6861 7269 6e67 2061 6e20 496e 7374 6167  haring an Instag
+000007a0: 7261 6d20 706f 7374 2074 6f20 5477 6974  ram post to Twit
+000007b0: 7465 722c 206f 6e6c 7920 746f 2066 696e  ter, only to fin
+000007c0: 6420 6f75 7420 7468 6174 2061 6c6c 2079  d out that all y
+000007d0: 6f75 2074 7765 6574 6564 2077 6173 2061  ou tweeted was a
+000007e0: 206c 696e 6b2c 2061 6e64 206e 6f74 2074   link, and not t
+000007f0: 6865 2061 6374 7561 6c20 7068 6f74 6f2f  he actual photo/
+00000800: 7669 6465 6f3f 0d0a 0d0a 2e2e 2069 6d61  video?...... ima
+00000810: 6765 3a3a 2068 7474 7073 3a2f 2f69 6e73  ge:: https://ins
+00000820: 7461 7477 6565 742e 7265 6164 7468 6564  tatweet.readthed
+00000830: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00000840: 2f5f 696d 6167 6573 2f73 6861 7265 5f77  /_images/share_w
+00000850: 6974 685f 696e 7374 6167 7261 6d2e 706e  ith_instagram.pn
+00000860: 670d 0a20 2020 203a 616c 743a 2053 6861  g..    :alt: Sha
+00000870: 7269 6e67 2061 6e20 496e 7374 6167 7261  ring an Instagra
+00000880: 6d20 706f 7374 2074 6f20 5477 6974 7465  m post to Twitte
+00000890: 7220 6469 7265 6374 6c79 2066 726f 6d20  r directly from 
+000008a0: 7468 6520 496e 7374 6167 7261 6d20 6170  the Instagram ap
+000008b0: 702e 204f 6e6c 7920 6120 6c69 6e6b 2061  p. Only a link a
+000008c0: 7070 6561 7273 2e0d 0a20 2020 2020 2020  ppears...       
+000008d0: 2049 7420 636f 756c 6420 6265 206c 6974   It could be lit
+000008e0: 6572 616c 6c79 2061 6e79 7468 696e 672c  erally anything,
+000008f0: 206e 6f62 6f64 7920 7769 6c6c 2063 6c69   nobody will cli
+00000900: 636b 2069 742e 0d0a 0d0a 0d0a 2e2e 2072  ck it......... r
+00000910: 6177 3a3a 2068 746d 6c0d 0a0d 0a20 2020  aw:: html....   
+00000920: 3c74 6162 6c65 3e0d 0a20 2020 2020 203c  <table>..      <
+00000930: 7472 2061 6c69 676e 3d22 6c65 6674 223e  tr align="left">
+00000940: 0d0a 2020 2020 2020 2020 203c 7468 3ee2  ..         <th>.
+00000950: 9aa0 2048 756d 696c 6961 7469 6e67 20f0  .. Humiliating .
+00000960: 9fa4 ae3c 2f74 683e 0d0a 2020 2020 2020  ...</th>..      
+00000970: 3c2f 7472 3e0d 0a20 2020 2020 203c 7472  </tr>..      <tr
+00000980: 3e0d 0a20 2020 2020 2020 2020 3c74 643e  >..         <td>
+00000990: 0d0a 0d0a 0d0a 5468 6174 2063 6f75 6c64  ......That could
+000009a0: 2062 6520 6c69 7465 7261 6c6c 7920 616e   be literally an
+000009b0: 7974 6869 6e67 2e20 4e6f 626f 6479 2077  ything. Nobody w
+000009c0: 696c 6c20 636c 6963 6b20 6974 2e0d 0a0d  ill click it....
+000009d0: 0a2e 2e20 7261 773a 3a20 6874 6d6c 0d0a  ... raw:: html..
+000009e0: 0d0a 2020 203c 2f74 643e 3c2f 7472 3e0d  ..   </td></tr>.
+000009f0: 0a20 2020 3c2f 7461 626c 653e 0d0a 0d0a  .   </table>....
+00000a00: 7c0d 0a0d 0a7c 2e49 6e73 7461 5477 6565  |....|.InstaTwee
+00000a10: 747c 5f20 2a2a 7368 6172 6573 2074 6865  t|_ **shares the
+00000a20: 2a2a 202a 6163 7475 616c 2a20 2a2a 636f  ** *actual* **co
+00000a30: 6e74 656e 7420 6f66 2074 6865 2070 6f73  ntent of the pos
+00000a40: 742e 204e 6f74 206a 7573 7420 6120 6c69  t. Not just a li
+00000a50: 6e6b 2074 6f20 6974 2e2a 2a0d 0a0d 0a7c  nk to it.**....|
+00000a60: 0d0a 0d0a 2e2e 2069 6d61 6765 3a3a 2068  ...... image:: h
+00000a70: 7474 7073 3a2f 2f69 6e73 7461 7477 6565  ttps://instatwee
+00000a80: 742e 7265 6164 7468 6564 6f63 732e 696f  t.readthedocs.io
+00000a90: 2f65 6e2f 6c61 7465 7374 2f5f 696d 6167  /en/latest/_imag
+00000aa0: 6573 2f73 6861 7265 5f77 6974 685f 696e  es/share_with_in
+00000ab0: 7374 6174 7765 6574 2e70 6e67 0d0a 2020  statweet.png..  
+00000ac0: 2020 3a61 6c74 3a20 5368 6172 696e 6720    :alt: Sharing 
+00000ad0: 616e 2049 6e73 7461 6772 616d 2070 6f73  an Instagram pos
+00000ae0: 7420 746f 2054 7769 7474 6572 2075 7369  t to Twitter usi
+00000af0: 6e67 2049 6e73 7461 5477 6565 742e 2054  ng InstaTweet. T
+00000b00: 6865 2061 6374 7561 6c20 7068 6f74 6f20  he actual photo 
+00000b10: 6f72 2076 6964 656f 2061 7070 6561 7273  or video appears
+00000b20: 2069 6e20 7468 6520 7477 6565 742e 0d0a   in the tweet...
+00000b30: 2020 2020 2020 2020 4974 2773 2061 2074          It's a t
+00000b40: 6869 6363 2063 6174 2c20 7665 7279 2068  hicc cat, very h
+00000b50: 616e 6473 6f6d 652e 204e 6f62 6f64 7920  andsome. Nobody 
+00000b60: 7769 6c6c 2063 6c69 636b 2074 6865 206c  will click the l
+00000b70: 696e 6b2c 2062 7574 2074 6865 7927 6c6c  ink, but they'll
+00000b80: 2064 6566 696e 6974 656c 7920 7365 6520   definitely see 
+00000b90: 7468 6973 2062 6164 2062 6f79 2e0d 0a0d  this bad boy....
+00000ba0: 0a0d 0a57 6974 6820 6060 496e 7374 6154  ...With ``InstaT
+00000bb0: 7765 6574 6060 2c20 796f 7520 6361 6e20  weet``, you can 
+00000bc0: 7265 7374 2065 6173 7920 6b6e 6f77 696e  rest easy knowin
+00000bd0: 6720 7468 6174 2c20 616c 7468 6f75 6768  g that, although
+00000be0: 206e 6f62 6f64 7920 7769 6c6c 2063 6c69   nobody will cli
+00000bf0: 636b 2074 6865 206c 696e 6b2c 0d0a 7468  ck the link,..th
+00000c00: 6579 276c 6c20 6174 206c 6561 7374 2073  ey'll at least s
+00000c10: 6565 2077 6861 7420 796f 7520 706f 7374  ee what you post
+00000c20: 6564 2e0d 0a0d 0a2e 2e2e 0d0a 0d0a 5768  ed............Wh
+00000c30: 6174 2773 2049 6e73 7461 5477 6565 743f  at's InstaTweet?
+00000c40: 0d0a 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ..~~~~~~~~~~~~~~
+00000c50: 7e7e 7e7e 7e7e 7e0d 0a0d 0a7c 2e49 6e73  ~~~~~~~....|.Ins
+00000c60: 7461 5477 6565 747c 5f20 6973 2061 2063  taTweet|_ is a c
+00000c70: 7573 746f 6d69 7a61 626c 6520 746f 6f6c  ustomizable tool
+00000c80: 2074 6f20 6175 746f 6d61 7469 6361 6c6c   to automaticall
+00000c90: 7920 7265 706f 7374 2063 6f6e 7465 6e74  y repost content
+00000ca0: 2066 726f 6d20 496e 7374 6167 7261 6d20   from Instagram 
+00000cb0: 746f 2054 7769 7474 6572 2e0d 0a0d 0a0d  to Twitter......
+00000cc0: 0a0d 0a53 696d 706c 7920 6372 6561 7465  ...Simply create
+00000cd0: 2061 207c 2e50 726f 6669 6c65 7c5f 2c20   a |.Profile|_, 
+00000ce0: 636f 6e66 6967 7572 6520 7468 6520 7c6d  configure the |m
+00000cf0: 616e 6461 746f 7279 2d73 6574 7469 6e67  andatory-setting
+00000d00: 737c 5f2c 2061 6e64 207c 2e61 6464 5f75  s|_, and |.add_u
+00000d10: 7365 7273 7c5f 2074 6f20 7265 706f 7374  sers|_ to repost
+00000d20: 2066 726f 6d0d 0a0d 0a0d 0a2e 2e20 636f   from........ co
+00000d30: 6465 2d62 6c6f 636b 3a3a 2070 7974 686f  de-block:: pytho
+00000d40: 6e0d 0a0d 0a20 2020 2066 726f 6d20 496e  n....    from In
+00000d50: 7374 6154 7765 6574 2069 6d70 6f72 7420  staTweet import 
+00000d60: 5072 6f66 696c 650d 0a0d 0a20 2020 2023  Profile....    #
+00000d70: 2043 7265 6174 6520 6120 6e65 7720 286c   Create a new (l
+00000d80: 6f63 616c 2920 5072 6f66 696c 650d 0a20  ocal) Profile.. 
+00000d90: 2020 203e 3e3e 2070 726f 6669 6c65 203d     >>> profile =
+00000da0: 2050 726f 6669 6c65 2827 6d79 5072 6f66   Profile('myProf
+00000db0: 696c 6527 290d 0a0d 0a20 2020 2023 2043  ile')....    # C
+00000dc0: 6f6e 6669 6775 7265 2074 6865 206d 616e  onfigure the man
+00000dd0: 6461 746f 7279 2073 6574 7469 6e67 7320  datory settings 
+00000de0: 2861 7420 6d69 6e69 6d75 6d29 0d0a 2020  (at minimum)..  
+00000df0: 2020 3e3e 3e20 7072 6f66 696c 652e 7477    >>> profile.tw
+00000e00: 6974 7465 725f 6b65 7973 203d 2074 7769  itter_keys = twi
+00000e10: 7474 6572 5f61 7069 5f6b 6579 730d 0a20  tter_api_keys.. 
+00000e20: 2020 203e 3e3e 2070 726f 6669 6c65 2e73     >>> profile.s
+00000e30: 6573 7369 6f6e 5f69 6420 3d20 2736 3031  ession_id = '601
+00000e40: 3139 3931 4127 0d0a 0d0a 2020 2020 2320  1991A'....    # 
+00000e50: 4164 6420 6174 206c 6561 7374 206f 6e65  Add at least one
+00000e60: 2049 6e73 7461 6772 616d 2061 6363 6f75   Instagram accou
+00000e70: 6e74 2074 6f20 7265 706f 7374 2066 726f  nt to repost fro
+00000e80: 6d0d 0a20 2020 203e 3e3e 2070 726f 6669  m..    >>> profi
+00000e90: 6c65 2e61 6464 5f75 7365 7273 2827 7468  le.add_users('th
+00000ea0: 652e 6461 696c 796b 6974 7465 6e27 290d  e.dailykitten').
+00000eb0: 0a0d 0a20 2020 2023 2053 6176 6520 7468  ...    # Save th
+00000ec0: 6520 5072 6f66 696c 6520 5b6f 7074 696f  e Profile [optio
+00000ed0: 6e61 6c5d 0d0a 2020 2020 3e3e 3e20 7072  nal]..    >>> pr
+00000ee0: 6f66 696c 652e 7361 7665 2829 0d0a 0d0a  ofile.save()....
+00000ef0: 2020 2020 5361 7665 6420 4c6f 6361 6c20      Saved Local 
+00000f00: 5072 6f66 696c 6520 6d79 5072 6f66 696c  Profile myProfil
+00000f10: 650d 0a0d 0a0d 0a4f 6e63 6520 636f 6e66  e......Once conf
+00000f20: 6967 7572 6564 2c20 7468 6520 7c2e 5072  igured, the |.Pr
+00000f30: 6f66 696c 657c 5f20 6361 6e20 6265 2075  ofile|_ can be u
+00000f40: 7365 6420 746f 2069 6e69 7469 616c 697a  sed to initializ
+00000f50: 6520 616e 6420 7c2e 7374 6172 747c 5f20  e and |.start|_ 
+00000f60: 496e 7374 6154 7765 6574 3a0d 0a0d 0a2e  InstaTweet:.....
+00000f70: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2070  . code-block:: p
+00000f80: 7974 686f 6e0d 0a0d 0a20 2020 2066 726f  ython....    fro
+00000f90: 6d20 496e 7374 6154 7765 6574 2069 6d70  m InstaTweet imp
+00000fa0: 6f72 7420 496e 7374 6154 7765 6574 0d0a  ort InstaTweet..
+00000fb0: 0d0a 2020 2020 2320 4469 7265 6374 6c79  ..    # Directly
+00000fc0: 2069 6e69 7469 616c 697a 6520 7769 7468   initialize with
+00000fd0: 2061 2050 726f 6669 6c65 206f 626a 6563   a Profile objec
+00000fe0: 740d 0a20 2020 203e 3e3e 2069 6e73 7461  t..    >>> insta
+00000ff0: 5f74 7765 6574 203d 2049 6e73 7461 5477  _tweet = InstaTw
+00001000: 6565 7428 7072 6f66 696c 6529 0d0a 0d0a  eet(profile)....
+00001010: 2020 2020 2320 4f72 206c 6f61 6420 6120      # Or load a 
+00001020: 7361 7665 6420 5072 6f66 696c 6520 6279  saved Profile by
+00001030: 206e 616d 650d 0a20 2020 203e 3e3e 2069   name..    >>> i
+00001040: 6e73 7461 5f74 7765 6574 203d 2049 6e73  nsta_tweet = Ins
+00001050: 7461 5477 6565 742e 6c6f 6164 2822 6d79  taTweet.load("my
+00001060: 5072 6f66 696c 6522 290d 0a0d 0a20 2020  Profile")....   
+00001070: 2023 2052 756e 2049 6e73 7461 5477 6565   # Run InstaTwee
+00001080: 7420 6279 2063 616c 6c69 6e67 2073 7461  t by calling sta
+00001090: 7274 2829 0d0a 2020 2020 3e3e 3e20 696e  rt()..    >>> in
+000010a0: 7374 615f 7477 6565 742e 7374 6172 7428  sta_tweet.start(
+000010b0: 290d 0a0d 0a0d 0a7c 0d0a 0d0a 2e2e 2069  )......|...... i
+000010c0: 6d61 6765 3a3a 2068 7474 7073 3a2f 2f75  mage:: https://u
+000010d0: 7365 722d 696d 6167 6573 2e67 6974 6875  ser-images.githu
+000010e0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+000010f0: 2f39 3633 3934 3635 322f 3233 3232 3734  /96394652/232274
+00001100: 3736 362d 3731 6538 3766 6232 2d66 3430  766-71e87fb2-f40
+00001110: 322d 3436 3664 2d39 3632 342d 6637 3735  2-466d-9624-f775
+00001120: 6438 6539 3835 6163 2e70 6e67 0d0a 0d0a  d8e985ac.png....
+00001130: 7c0d 0a0d 0a41 7320 6060 496e 7374 6154  |....As ``InstaT
+00001140: 7765 6574 6060 2072 756e 732c 2069 7473  weet`` runs, its
+00001150: 2070 726f 6772 6573 7320 7769 6c6c 2062   progress will b
+00001160: 6520 6c6f 6767 6564 2074 6f20 636f 6e73  e logged to cons
+00001170: 6f6c 653a 0d0a 0d0a 2e2e 2063 6f64 652d  ole:...... code-
+00001180: 626c 6f63 6b3a 3a20 7079 7468 6f6e 0d0a  block:: python..
+00001190: 0d0a 2020 2020 5374 6172 7469 6e67 2049  ..    Starting I
+000011a0: 6e73 7461 5477 6565 7420 666f 7220 5072  nstaTweet for Pr
+000011b0: 6f66 696c 653a 206d 7950 726f 6669 6c65  ofile: myProfile
+000011c0: 0d0a 2020 2020 4368 6563 6b69 6e67 2070  ..    Checking p
+000011d0: 6f73 7473 2066 726f 6d20 4074 6865 2e64  osts from @the.d
+000011e0: 6169 6c79 6b69 7474 656e 0d0a 2020 2020  ailykitten..    
+000011f0: 0d0a 2020 2020 4669 6e69 7368 6564 2069  ..    Finished i
+00001200: 6e73 7461 2d74 7765 6574 696e 6720 666f  nsta-tweeting fo
+00001210: 7220 4074 6865 2e64 6169 6c79 6b69 7474  r @the.dailykitt
+00001220: 656e 0d0a 2020 2020 416c 6c20 7573 6572  en..    All user
+00001230: 7320 6861 7665 2062 6565 6e20 696e 7374  s have been inst
+00001240: 612d 7477 6565 7465 640d 0a0d 0a2e 2e2e  a-tweeted.......
+00001250: 0d0a 0d0a 4f6b 6179 2e2e 2e20 4275 7420  ....Okay... But 
+00001260: 5768 793f 20f0 9f98 9f0d 0a7e 7e7e 7e7e  Why? ......~~~~~
+00001270: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+00001280: 7e7e 0d0a 0d0a 2e2e 2072 6177 3a3a 2068  ~~...... raw:: h
+00001290: 746d 6c0d 0a0d 0a20 2020 3c74 6162 6c65  tml....   <table
+000012a0: 3e0d 0a20 2020 2020 203c 7472 2061 6c69  >..      <tr ali
+000012b0: 676e 3d22 6c65 6674 223e 0d0a 2020 2020  gn="left">..    
+000012c0: 2020 2020 203c 7468 3ef0 9f90 a520 4275       <th>.... Bu
+000012d0: 7420 5768 793f 20f0 9fa4 a83c 2f74 683e  t Why? ....</th>
+000012e0: 0d0a 2020 2020 2020 3c2f 7472 3e0d 0a20  ..      </tr>.. 
+000012f0: 2020 2020 203c 7472 3e0d 0a20 2020 2020       <tr>..     
+00001300: 2020 2020 3c74 643e 0d0a 0d0a 2a2a 496e      <td>....**In
+00001310: 7374 6154 7765 6574 2068 6173 2074 776f  staTweet has two
+00001320: 206d 6169 6e20 7573 6520 6361 7365 733a   main use cases:
+00001330: 2a2a 0d0a 0d0a 2a20 546f 2061 7574 6f6d  **....* To autom
+00001340: 6174 6963 616c 6c79 2073 6861 7265 2079  atically share y
+00001350: 6f75 7220 6f77 6e20 496e 7374 6167 7261  our own Instagra
+00001360: 6d20 706f 7374 7320 746f 2054 7769 7474  m posts to Twitt
+00001370: 6572 0d0a 2a20 546f 2061 7574 6f6d 6174  er..* To automat
+00001380: 6963 616c 6c79 2074 7765 6574 206e 6577  ically tweet new
+00001390: 2063 6f6e 7465 6e74 2066 726f 6d20 6f74   content from ot
+000013a0: 6865 7220 496e 7374 6167 7261 6d20 7573  her Instagram us
+000013b0: 6572 730d 0a0d 0a52 6567 6172 646c 6573  ers....Regardles
+000013c0: 7320 6f66 2079 6f75 7220 696e 7465 6e74  s of your intent
+000013d0: 696f 6e2c 2049 6e73 7461 5477 6565 7420  ion, InstaTweet 
+000013e0: 7769 6c6c 2064 6574 6563 7420 6e65 7720  will detect new 
+000013f0: 706f 7374 7320 6672 6f6d 2074 6865 2075  posts from the u
+00001400: 7365 7273 2079 6f75 2073 7065 6369 6679  sers you specify
+00001410: 2c0d 0a64 6f77 6e6c 6f61 6420 7468 656d  ,..download them
+00001420: 2c20 616e 6420 7265 706f 7374 2074 6865  , and repost the
+00001430: 6d20 746f 2054 7769 7474 6572 2e0d 0a0d  m to Twitter....
+00001440: 0a2e 2e20 7261 773a 3a20 6874 6d6c 0d0a  ... raw:: html..
+00001450: 0d0a 2020 203c 2f74 643e 3c2f 7472 3e0d  ..   </td></tr>.
+00001460: 0a20 2020 3c2f 7461 626c 653e 0d0a 0d0a  .   </table>....
+00001470: 0d0a 2e2e 2e0d 0a0d 0a0d 0a4f 7468 6572  ...........Other
+00001480: 2055 7365 2043 6173 653a 2054 6865 207c   Use Case: The |
+00001490: 2e49 6e73 7461 436c 6965 6e74 7c5f 0d0a  .InstaClient|_..
+000014a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000014b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000014c0: 3d3d 3d3d 3d3d 0d0a 0d0a 5468 6520 7061  ======....The pa
+000014d0: 636b 6167 6527 7320 6375 7374 6f6d 207c  ckage's custom |
+000014e0: 2e49 6e73 7461 436c 6965 6e74 7c5f 2063  .InstaClient|_ c
+000014f0: 616e 2061 6c73 6f20 6265 2075 7365 6420  an also be used 
+00001500: 6173 2061 2073 7461 6e64 616c 6f6e 6520  as a standalone 
+00001510: 496e 7374 6167 7261 6d20 7363 7261 7065  Instagram scrape
+00001520: 720d 0a0d 0a2e 2e20 636f 6465 2d62 6c6f  r...... code-blo
+00001530: 636b 3a3a 2070 7974 686f 6e0d 0a0d 0a20  ck:: python.... 
+00001540: 2020 6672 6f6d 2049 6e73 7461 5477 6565    from InstaTwee
+00001550: 7420 696d 706f 7274 2049 6e73 7461 436c  t import InstaCl
+00001560: 6965 6e74 0d0a 0d0a 2020 203e 3e3e 2069  ient....   >>> i
+00001570: 6720 3d20 496e 7374 6143 6c69 656e 7428  g = InstaClient(
+00001580: 7365 7373 696f 6e5f 6964 3d22 6b6a 6664  session_id="kjfd
+00001590: 6e33 3039 7772 6564 7366 6c22 290d 0a20  n309wredsfl").. 
+000015a0: 2020 3e3e 3e20 7573 6572 203d 2069 672e    >>> user = ig.
+000015b0: 6765 745f 7573 6572 2827 6461 696c 796b  get_user('dailyk
+000015c0: 6974 7465 6e69 6727 290d 0a20 2020 3e3e  ittenig')..   >>
+000015d0: 3e20 7072 696e 7428 7573 6572 290d 0a0d  > print(user)...
+000015e0: 0a20 2020 3c49 6e73 7461 5477 6565 742e  .   <InstaTweet.
+000015f0: 696e 7374 6175 7365 722e 496e 7374 6155  instauser.InstaU
+00001600: 7365 7220 6f62 6a65 6374 2061 7420 3078  ser object at 0x
+00001610: 3030 3030 3032 4239 4131 3130 3133 3330  000002B9A1101330
+00001620: 3e0d 0a0d 0a20 2020 3e3e 3e20 7072 696e  >....   >>> prin
+00001630: 7428 7573 6572 2e70 6f73 7473 290d 0a20  t(user.posts).. 
+00001640: 2020 3e3e 3e20 6967 2e64 6f77 6e6c 6f61    >>> ig.downloa
+00001650: 645f 706f 7374 2875 7365 722e 706f 7374  d_post(user.post
+00001660: 735b 305d 290d 0a0d 0a20 2020 5b3c 496e  s[0])....   [<In
+00001670: 7374 6154 7765 6574 2e69 6e73 7461 706f  staTweet.instapo
+00001680: 7374 2e49 6e73 7461 506f 7374 206f 626a  st.InstaPost obj
+00001690: 6563 7420 6174 2030 7830 3030 3030 3242  ect at 0x000002B
+000016a0: 3941 3235 3046 3545 303e 2c20 2e2e 2e5d  9A250F5E0>, ...]
+000016b0: 0d0a 2020 2044 6f77 6e6c 6f61 6465 6420  ..   Downloaded 
+000016c0: 706f 7374 2068 7474 7073 3a2f 2f77 7777  post https://www
+000016d0: 2e69 6e73 7461 6772 616d 2e63 6f6d 2f70  .instagram.com/p
+000016e0: 2f43 6c68 7434 4e52 7271 524f 2062 7920  /Clht4NRrqRO by 
+000016f0: 6461 696c 796b 6974 7465 6e69 6720 746f  dailykittenig to
+00001700: 2043 3a5c 5c70 6174 685c 5c74 6f5c 5c69   C:\\path\\to\\i
+00001710: 6e73 7461 2d74 7765 6574 5c5c 646f 776e  nsta-tweet\\down
+00001720: 6c6f 6164 735c 5c32 3938 3138 3636 3230  loads\\298186620
+00001730: 3239 3334 3937 3736 3134 2e6d 7034 0d0a  2934977614.mp4..
+00001740: 0d0a 2e2e 2e0d 0a0d 0a49 6e73 7461 6c6c  .........Install
+00001750: 6174 696f 6e0d 0a7e 7e7e 7e7e 7e7e 7e7e  ation..~~~~~~~~~
+00001760: 7e7e 7e7e 7e0d 0a0d 0a54 6f20 696e 7374  ~~~~~....To inst
+00001770: 616c 6c20 7573 696e 6720 7069 703a 0d0a  all using pip:..
+00001780: 0d0a 2e2e 2063 6f64 652d 626c 6f63 6b3a  .... code-block:
+00001790: 3a20 7368 656c 6c0d 0a0d 0a20 2020 2070  : shell....    p
+000017a0: 6970 2069 6e73 7461 6c6c 2069 6e73 7461  ip install insta
+000017b0: 2d74 7765 6574 0d0a 0d0a 0d0a 506c 6561  -tweet......Plea
+000017c0: 7365 206e 6f74 6520 7468 6174 2060 6049  se note that ``I
+000017d0: 6e73 7461 5477 6565 7460 6020 7265 7175  nstaTweet`` requ
+000017e0: 6972 6573 2060 6050 7974 686f 6e20 3e3d  ires ``Python >=
+000017f0: 2033 2e38 6060 0d0a 0d0a 2e2e 2e0d 0a0d   3.8``..........
+00001800: 0a44 6f63 756d 656e 7461 7469 6f6e 0d0a  .Documentation..
+00001810: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+00001820: 7e0d 0a0d 0a54 6865 2072 6573 7420 6f66  ~....The rest of
+00001830: 2074 6869 7320 6052 4541 444d 4520 3c68   this `README <h
+00001840: 7474 7073 3a2f 2f69 6e73 7461 7477 6565  ttps://instatwee
+00001850: 742e 7265 6164 7468 6564 6f63 732e 696f  t.readthedocs.io
+00001860: 2f65 6e2f 6c61 7465 7374 2f5f 7265 6164  /en/latest/_read
+00001870: 6d65 2f67 6574 7469 6e67 2d73 7461 7274  me/getting-start
+00001880: 6564 2e68 746d 6c3e 605f 2c0d 0a74 6865  ed.html>`_,..the
+00001890: 2060 4150 4920 646f 6375 6d65 6e74 6174   `API documentat
+000018a0: 696f 6e20 3c68 7474 7073 3a2f 2f69 6e73  ion <https://ins
+000018b0: 7461 7477 6565 742e 7265 6164 7468 6564  tatweet.readthed
+000018c0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+000018d0: 2f6d 6f64 756c 6573 2e68 746d 6c3e 605f  /modules.html>`_
+000018e0: 2c20 616e 640d 0a60 736e 6970 7065 7473  , and..`snippets
+000018f0: 203c 6874 7470 733a 2f2f 696e 7374 6174   <https://instat
+00001900: 7765 6574 2e72 6561 6474 6865 646f 6373  weet.readthedocs
+00001910: 2e69 6f2f 656e 2f6c 6174 6573 742f 736e  .io/en/latest/sn
+00001920: 6970 7065 7473 2e68 746d 6c3e 605f 0d0a  ippets.html>`_..
+00001930: 6361 6e20 616c 6c20 6265 2066 6f75 6e64  can all be found
+00001940: 206f 6e20 6052 6561 6420 7468 6520 446f   on `Read the Do
+00001950: 6373 203c 6874 7470 733a 2f2f 696e 7374  cs <https://inst
+00001960: 6174 7765 6574 2e72 6561 6474 6865 646f  atweet.readthedo
+00001970: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00001980: 696e 6465 782e 6874 6d6c 3e60 5f0d 0a0d  index.html>`_...
+00001990: 0a0d 0a                                  ...
```

### Comparing `insta-tweet-2.1.1/README.rst` & `insta-tweet-2.1.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,152 +1,220 @@
+Metadata-Version: 2.1
+Name: insta-tweet
+Version: 2.1.2
+Summary: Automatically Repost Content From Instagram to Twitter
+Home-page: https://www.github.com/TDKorn/insta-tweet/
+Author: Adam Korn
+Author-email: hello@dailykitten.net
+License: MIT
+Download-URL: https://github.com/TDKorn/insta-tweet/tarball/master/
+Keywords: instagram,twitter,api,instagram api,twitter api,repost,instagram repost,reposter
+Platform: UNKNOWN
+Description-Content-Type: text/x-rst; charset=UTF-8
+License-File: LICENSE
+
+.. meta::
+   :title: InstaTweet - Automatically Repost Content From Instagram to Twitter
+   :description: A Python package to automatically repost content from Instagram to Twitter
+
+.. |.InstaTweet| replace:: ``InstaTweet``
+.. _.InstaTweet: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/instatweet.py#L5-L142
+.. |.add_users| replace:: ``add_users()``
+.. _.add_users: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/profile.py#L167-L197
+.. |.Profile| replace:: ``Profile``
+.. _.Profile: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/profile.py#L12-L416
+.. |.start| replace:: ``start()``
+.. _.start: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/instatweet.py#L72-L117
+.. |.InstaClient| replace:: ``InstaClient``
+.. _.InstaClient: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/instaclient.py#L14-L108
+.. |mandatory-settings| replace:: mandatory settings
+.. _mandatory-settings: https://instatweet.readthedocs.io/en/latest/_readme/getting-started.html#mandatory-settings
+
 .. _about-insta-tweet:
 
 ✨🐥 InstaTweet 🐤✨
 -----------------------
 
 .. image:: https://img.shields.io/pypi/v/insta-tweet
    :target: https://pypi.org/project/insta-tweet/
    :alt: PyPI Version
 
+.. image:: https://img.shields.io/badge/GitHub-insta--tweet-4f1abc
+   :target: https://github.com/tdkorn/insta-tweet
+   :alt: GitHub Repository
+
+.. image:: https://static.pepy.tech/personalized-badge/insta-tweet?period=total&units=none&left_color=grey&right_color=blue&left_text=Downloads
+    :target: https://pepy.tech/project/insta-tweet
+
 .. image:: https://readthedocs.org/projects/instatweet/badge/?version=latest
     :target: https://instatweet.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/github/commit-activity/m/tdkorn/insta-tweet
-    :target: https://github.com/tdkorn/insta-tweet/pulse
-    :alt: Activity
-
 
 Automatically Repost Content From Instagram to Twitter
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Ever tried sharing an Instagram post to Twitter, only to find out that all you tweeted was a link, and not the actual photo/video?
 
 .. image:: https://instatweet.readthedocs.io/en/latest/_images/share_with_instagram.png
     :alt: Sharing an Instagram post to Twitter directly from the Instagram app. Only a link appears.
         It could be literally anything, nobody will click it.
 
 
-.. admonition:: **Humiliating 🤮**
-   :class: important-af
++-------------------------------------------------------------+
+| ⚠ Humiliating 🤮                                            |
++=============================================================+
+|  That could be literally anything. Nobody will click it.    |
++-------------------------------------------------------------+
 
-   That could be literally anything. Nobody will click it.
 
 |
 
+|.InstaTweet|_ **shares the** *actual* **content of the post. Not just a link to it.**
 
-`InstaTweet <https://github.com/tdkorn/insta-tweet/blob/v2.1.1/InstaTweet/instatweet.py#L5-L142>`_ **shares the** *actual* **content of the post. Not just a link to it.**
-
-
+|
 
 .. image:: https://instatweet.readthedocs.io/en/latest/_images/share_with_instatweet.png
     :alt: Sharing an Instagram post to Twitter using InstaTweet. The actual photo or video appears in the tweet.
         It's a thicc cat, very handsome. Nobody will click the link, but they'll definitely see this bad boy.
 
 
-With ``InstaTweet``, you can rest easy knowing that,
-although nobody will click the link, they'll at least see what you posted.
-
+With ``InstaTweet``, you can rest easy knowing that, although nobody will click the link,
+they'll at least see what you posted.
 
+...
 
 What's InstaTweet?
 ~~~~~~~~~~~~~~~~~~~~~
 
-`InstaTweet <https://github.com/tdkorn/insta-tweet/blob/v2.1.1/InstaTweet/instatweet.py#L5-L142>`_ is a customizable tool to automatically repost content from Instagram to Twitter.
+|.InstaTweet|_ is a customizable tool to automatically repost content from Instagram to Twitter.
+
+
+
+Simply create a |.Profile|_, configure the |mandatory-settings|_, and |.add_users|_ to repost from
 
-Simply create a `Profile <https://github.com/tdkorn/insta-tweet/blob/v2.1.1/InstaTweet/profile.py#L12-L416>`_,
-configure the `mandatory-settings <https://instatweet.readthedocs.io/en/latest/_readme/getting-started.html#mandatory-settings>`_,
-and `add_users() <https://github.com/tdkorn/insta-tweet/blob/v2.1.1/InstaTweet/profile.py#L167-L197>`_ to repost from
 
 .. code-block:: python
 
     from InstaTweet import Profile
 
     # Create a new (local) Profile
     >>> profile = Profile('myProfile')
 
-    # Configure the required settings (at minimum)
+    # Configure the mandatory settings (at minimum)
     >>> profile.twitter_keys = twitter_api_keys
     >>> profile.session_id = '6011991A'
 
     # Add at least one Instagram account to repost from
     >>> profile.add_users('the.dailykitten')
 
+    # Save the Profile [optional]
+    >>> profile.save()
+
+    Saved Local Profile myProfile
+
 
-Once configured, the `Profile <https://github.com/tdkorn/insta-tweet/blob/v2.1.1/InstaTweet/profile.py#L12-L416>`_ can be used to initialize and
-`start() <https://github.com/tdkorn/insta-tweet/blob/v2.1.1/InstaTweet/instatweet.py#L72-L117>`_ an `InstaTweet <https://github.com/tdkorn/insta-tweet/blob/v2.1.1/InstaTweet/instatweet.py#L5-L142>`_ object
+Once configured, the |.Profile|_ can be used to initialize and |.start|_ InstaTweet:
 
 .. code-block:: python
 
     from InstaTweet import InstaTweet
 
-    # Directly initialize with the Profile from above
+    # Directly initialize with a Profile object
     >>> insta_tweet = InstaTweet(profile)
 
-    # Or, save the Profile...
-    >>> profile.save()
-
-    Saved Local Profile myProfile
-
-    # ...then InstaTweet.load() the settings in (by Profile name)
-    >>> insta_tweet = InstaTweet.load(profile_name="myProfile")
+    # Or load a saved Profile by name
+    >>> insta_tweet = InstaTweet.load("myProfile")
 
     # Run InstaTweet by calling start()
     >>> insta_tweet.start()
 
 
-.. admonition:: From the Docs...
-    :class: docs
-    
-    https://github.com/TDKorn/insta-tweet/blob/cec73930d28db24e6fd492f5860d3edf0c2afbbe/InstaTweet/instatweet.py#L72-L117
+|
 
+.. image:: https://user-images.githubusercontent.com/96394652/232274766-71e87fb2-f402-466d-9624-f775d8e985ac.png
+
+|
 
 As ``InstaTweet`` runs, its progress will be logged to console:
 
 .. code-block:: python
 
     Starting InstaTweet for Profile: myProfile
     Checking posts from @the.dailykitten
-    ...
+    
     Finished insta-tweeting for @the.dailykitten
     All users have been insta-tweeted
 
+...
 
 Okay... But Why? 😟
 ~~~~~~~~~~~~~~~~~~~~~~~
 
-.. admonition:: But Why? 🤨
-   :class: instatweet
 
-   **InstaTweet has two main use cases:**
+.. |why| replace:: 🐥 But Why? 🤨
 
-   * To automatically share your own Instagram posts to Twitter
-   * To automatically tweet new content from other Instagram users
++-----------------------------------------------------------------+
+| |why|                                                           |
++=================================================================+
+| **InstaTweet has two main use cases:**                          |
+|                                                                 |
+| * To automatically share your own Instagram posts to Twitter    |
+| * To automatically tweet new content from other Instagram users |
+|                                                                 |
+| Regardless of your intention, InstaTweet will detect new posts  |
+| from the users you specify, download them, and repost them to   |
+| Twitter.                                                        |
++-----------------------------------------------------------------+
 
-   Regardless of your intention, InstaTweet will detect new posts from the users you specify, download them, and repost
-   them to Twitter.
 
+...
 
-Documentation
-~~~~~~~~~~~~~~~~~
 
-The rest of this `README <https://instatweet.readthedocs.io/en/latest/_readme/about-instatweet.html>`_,
-the `API documentation <https://instatweet.readthedocs.io/en/latest/modules.html>`_, and
-`snippets <https://instatweet.readthedocs.io/en/latest/snippets.html>`_
-can all be found on `Read the Docs <https://instatweet.readthedocs.io/en/latest/index.html>`_
+Other Use Case: The |.InstaClient|_
+======================================
+
+The package's custom |.InstaClient|_ can also be used as a standalone Instagram scraper
 
-I put a lot of time into creating the documentation for this package, it was a struggle,
-so it'd mean a lot to me if you could please continue reading there! 🥰
+.. code-block:: python
+
+   from InstaTweet import InstaClient
+
+   >>> ig = InstaClient(session_id="kjfdn309wredsfl")
+   >>> user = ig.get_user('dailykittenig')
+   >>> print(user)
 
+   <InstaTweet.instauser.InstaUser object at 0x000002B9A1101330>
 
+   >>> print(user.posts)
+   >>> ig.download_post(user.posts[0])
+
+   [<InstaTweet.instapost.InstaPost object at 0x000002B9A250F5E0>, ...]
+   Downloaded post https://www.instagram.com/p/Clht4NRrqRO by dailykittenig to C:\\path\\to\\insta-tweet\\downloads\\2981866202934977614.mp4
+
+...
 
 Installation
 ~~~~~~~~~~~~~~
 
 To install using pip:
 
 .. code-block:: shell
 
     pip install insta-tweet
 
 
 Please note that ``InstaTweet`` requires ``Python >= 3.8``
+
+...
+
+Documentation
+~~~~~~~~~~~~~~~~~
+
+The rest of this `README <https://instatweet.readthedocs.io/en/latest/_readme/getting-started.html>`_,
+the `API documentation <https://instatweet.readthedocs.io/en/latest/modules.html>`_, and
+`snippets <https://instatweet.readthedocs.io/en/latest/snippets.html>`_
+can all be found on `Read the Docs <https://instatweet.readthedocs.io/en/latest/index.html>`_
+
+
+
+
```

### Comparing `insta-tweet-2.1.1/insta_tweet.egg-info/PKG-INFO` & `insta-tweet-2.1.2/insta_tweet.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,165 +1,220 @@
 Metadata-Version: 2.1
 Name: insta-tweet
-Version: 2.1.1
+Version: 2.1.2
 Summary: Automatically Repost Content From Instagram to Twitter
 Home-page: https://www.github.com/TDKorn/insta-tweet/
 Author: Adam Korn
 Author-email: hello@dailykitten.net
 License: MIT
-Download-URL: https://github.com/TDKorn/insta-tweet/tarball/2.0.0/
-Keywords: instagram,twitter,repost,reposter,instascrape,instagram-repost
+Download-URL: https://github.com/TDKorn/insta-tweet/tarball/master/
+Keywords: instagram,twitter,api,instagram api,twitter api,repost,instagram repost,reposter
 Platform: UNKNOWN
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 
+.. meta::
+   :title: InstaTweet - Automatically Repost Content From Instagram to Twitter
+   :description: A Python package to automatically repost content from Instagram to Twitter
+
+.. |.InstaTweet| replace:: ``InstaTweet``
+.. _.InstaTweet: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/instatweet.py#L5-L142
+.. |.add_users| replace:: ``add_users()``
+.. _.add_users: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/profile.py#L167-L197
+.. |.Profile| replace:: ``Profile``
+.. _.Profile: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/profile.py#L12-L416
+.. |.start| replace:: ``start()``
+.. _.start: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/instatweet.py#L72-L117
+.. |.InstaClient| replace:: ``InstaClient``
+.. _.InstaClient: https://github.com/tdkorn/insta-tweet/blob/master/InstaTweet/instaclient.py#L14-L108
+.. |mandatory-settings| replace:: mandatory settings
+.. _mandatory-settings: https://instatweet.readthedocs.io/en/latest/_readme/getting-started.html#mandatory-settings
+
 .. _about-insta-tweet:
 
 ✨🐥 InstaTweet 🐤✨
 -----------------------
 
 .. image:: https://img.shields.io/pypi/v/insta-tweet
    :target: https://pypi.org/project/insta-tweet/
    :alt: PyPI Version
 
+.. image:: https://img.shields.io/badge/GitHub-insta--tweet-4f1abc
+   :target: https://github.com/tdkorn/insta-tweet
+   :alt: GitHub Repository
+
+.. image:: https://static.pepy.tech/personalized-badge/insta-tweet?period=total&units=none&left_color=grey&right_color=blue&left_text=Downloads
+    :target: https://pepy.tech/project/insta-tweet
+
 .. image:: https://readthedocs.org/projects/instatweet/badge/?version=latest
     :target: https://instatweet.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. image:: https://img.shields.io/github/commit-activity/m/tdkorn/insta-tweet
-    :target: https://github.com/tdkorn/insta-tweet/pulse
-    :alt: Activity
-
 
 Automatically Repost Content From Instagram to Twitter
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Ever tried sharing an Instagram post to Twitter, only to find out that all you tweeted was a link, and not the actual photo/video?
 
 .. image:: https://instatweet.readthedocs.io/en/latest/_images/share_with_instagram.png
     :alt: Sharing an Instagram post to Twitter directly from the Instagram app. Only a link appears.
         It could be literally anything, nobody will click it.
 
 
-.. admonition:: **Humiliating 🤮**
-   :class: important-af
++-------------------------------------------------------------+
+| ⚠ Humiliating 🤮                                            |
++=============================================================+
+|  That could be literally anything. Nobody will click it.    |
++-------------------------------------------------------------+
 
-   That could be literally anything. Nobody will click it.
 
 |
 
+|.InstaTweet|_ **shares the** *actual* **content of the post. Not just a link to it.**
 
-`InstaTweet <https://github.com/tdkorn/insta-tweet/blob/v2.1.1/InstaTweet/instatweet.py#L5-L142>`_ **shares the** *actual* **content of the post. Not just a link to it.**
-
-
+|
 
 .. image:: https://instatweet.readthedocs.io/en/latest/_images/share_with_instatweet.png
     :alt: Sharing an Instagram post to Twitter using InstaTweet. The actual photo or video appears in the tweet.
         It's a thicc cat, very handsome. Nobody will click the link, but they'll definitely see this bad boy.
 
 
-With ``InstaTweet``, you can rest easy knowing that,
-although nobody will click the link, they'll at least see what you posted.
-
+With ``InstaTweet``, you can rest easy knowing that, although nobody will click the link,
+they'll at least see what you posted.
 
+...
 
 What's InstaTweet?
 ~~~~~~~~~~~~~~~~~~~~~
 
-`InstaTweet <https://github.com/tdkorn/insta-tweet/blob/v2.1.1/InstaTweet/instatweet.py#L5-L142>`_ is a customizable tool to automatically repost content from Instagram to Twitter.
+|.InstaTweet|_ is a customizable tool to automatically repost content from Instagram to Twitter.
+
+
+
+Simply create a |.Profile|_, configure the |mandatory-settings|_, and |.add_users|_ to repost from
 
-Simply create a `Profile <https://github.com/tdkorn/insta-tweet/blob/v2.1.1/InstaTweet/profile.py#L12-L416>`_,
-configure the `mandatory-settings <https://instatweet.readthedocs.io/en/latest/_readme/getting-started.html#mandatory-settings>`_,
-and `add_users() <https://github.com/tdkorn/insta-tweet/blob/v2.1.1/InstaTweet/profile.py#L167-L197>`_ to repost from
 
 .. code-block:: python
 
     from InstaTweet import Profile
 
     # Create a new (local) Profile
     >>> profile = Profile('myProfile')
 
-    # Configure the required settings (at minimum)
+    # Configure the mandatory settings (at minimum)
     >>> profile.twitter_keys = twitter_api_keys
     >>> profile.session_id = '6011991A'
 
     # Add at least one Instagram account to repost from
     >>> profile.add_users('the.dailykitten')
 
+    # Save the Profile [optional]
+    >>> profile.save()
+
+    Saved Local Profile myProfile
 
-Once configured, the `Profile <https://github.com/tdkorn/insta-tweet/blob/v2.1.1/InstaTweet/profile.py#L12-L416>`_ can be used to initialize and
-`start() <https://github.com/tdkorn/insta-tweet/blob/v2.1.1/InstaTweet/instatweet.py#L72-L117>`_ an `InstaTweet <https://github.com/tdkorn/insta-tweet/blob/v2.1.1/InstaTweet/instatweet.py#L5-L142>`_ object
+
+Once configured, the |.Profile|_ can be used to initialize and |.start|_ InstaTweet:
 
 .. code-block:: python
 
     from InstaTweet import InstaTweet
 
-    # Directly initialize with the Profile from above
+    # Directly initialize with a Profile object
     >>> insta_tweet = InstaTweet(profile)
 
-    # Or, save the Profile...
-    >>> profile.save()
-
-    Saved Local Profile myProfile
-
-    # ...then InstaTweet.load() the settings in (by Profile name)
-    >>> insta_tweet = InstaTweet.load(profile_name="myProfile")
+    # Or load a saved Profile by name
+    >>> insta_tweet = InstaTweet.load("myProfile")
 
     # Run InstaTweet by calling start()
     >>> insta_tweet.start()
 
 
-.. image:: https://user-images.githubusercontent.com/96394652/187158617-f45761ab-3aa9-472f-a6fb-a99cd0ce900c.png
+|
 
+.. image:: https://user-images.githubusercontent.com/96394652/232274766-71e87fb2-f402-466d-9624-f775d8e985ac.png
+
+|
 
 As ``InstaTweet`` runs, its progress will be logged to console:
 
 .. code-block:: python
 
     Starting InstaTweet for Profile: myProfile
     Checking posts from @the.dailykitten
-    ...
+    
     Finished insta-tweeting for @the.dailykitten
     All users have been insta-tweeted
 
+...
 
 Okay... But Why? 😟
 ~~~~~~~~~~~~~~~~~~~~~~~
 
-.. admonition:: But Why? 🤨
-   :class: instatweet
 
-   **InstaTweet has two main use cases:**
+.. |why| replace:: 🐥 But Why? 🤨
 
-   * To automatically share your own Instagram posts to Twitter
-   * To automatically tweet new content from other Instagram users
++-----------------------------------------------------------------+
+| |why|                                                           |
++=================================================================+
+| **InstaTweet has two main use cases:**                          |
+|                                                                 |
+| * To automatically share your own Instagram posts to Twitter    |
+| * To automatically tweet new content from other Instagram users |
+|                                                                 |
+| Regardless of your intention, InstaTweet will detect new posts  |
+| from the users you specify, download them, and repost them to   |
+| Twitter.                                                        |
++-----------------------------------------------------------------+
 
-   Regardless of your intention, InstaTweet will detect new posts from the users you specify, download them, and repost
-   them to Twitter.
 
+...
 
-Documentation
-~~~~~~~~~~~~~~~~~
 
-The rest of this `README <https://instatweet.readthedocs.io/en/latest/_readme/about-instatweet.html>`_,
-the `API documentation <https://instatweet.readthedocs.io/en/latest/modules.html>`_, and
-`snippets <https://instatweet.readthedocs.io/en/latest/snippets.html>`_
-can all be found on `Read the Docs <https://instatweet.readthedocs.io/en/latest/index.html>`_
+Other Use Case: The |.InstaClient|_
+======================================
+
+The package's custom |.InstaClient|_ can also be used as a standalone Instagram scraper
+
+.. code-block:: python
+
+   from InstaTweet import InstaClient
+
+   >>> ig = InstaClient(session_id="kjfdn309wredsfl")
+   >>> user = ig.get_user('dailykittenig')
+   >>> print(user)
+
+   <InstaTweet.instauser.InstaUser object at 0x000002B9A1101330>
 
-I put a lot of time into creating the documentation for this package, it was a struggle,
-so it'd mean a lot to me if you could please continue reading there! 🥰
+   >>> print(user.posts)
+   >>> ig.download_post(user.posts[0])
 
+   [<InstaTweet.instapost.InstaPost object at 0x000002B9A250F5E0>, ...]
+   Downloaded post https://www.instagram.com/p/Clht4NRrqRO by dailykittenig to C:\\path\\to\\insta-tweet\\downloads\\2981866202934977614.mp4
 
+...
 
 Installation
 ~~~~~~~~~~~~~~
 
 To install using pip:
 
 .. code-block:: shell
 
     pip install insta-tweet
 
 
 Please note that ``InstaTweet`` requires ``Python >= 3.8``
 
+...
+
+Documentation
+~~~~~~~~~~~~~~~~~
+
+The rest of this `README <https://instatweet.readthedocs.io/en/latest/_readme/getting-started.html>`_,
+the `API documentation <https://instatweet.readthedocs.io/en/latest/modules.html>`_, and
+`snippets <https://instatweet.readthedocs.io/en/latest/snippets.html>`_
+can all be found on `Read the Docs <https://instatweet.readthedocs.io/en/latest/index.html>`_
+
+
+
```

### Comparing `insta-tweet-2.1.1/setup.py` & `insta-tweet-2.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import re
 from setuptools import setup
 
 
-LONG_DESCRIPTION_SRC = 'README.rst'
+LONG_DESCRIPTION_SRC = 'README_PyPi.rst'
 
 
 def read(file):
     with open(os.path.abspath(file), 'r', encoding='utf-8') as f:
         return f.read()
 
 
@@ -24,24 +24,23 @@
         string=rst
     )
 
 
 setup(
     name='insta-tweet',
     packages=['InstaTweet'],
-    version='2.1.1',
+    version='2.1.2',
     license='MIT',
     description='Automatically Repost Content From Instagram to Twitter',
     long_description=get_pypi_desc(LONG_DESCRIPTION_SRC),
     long_description_content_type="text/x-rst; charset=UTF-8",
     author='Adam Korn',
     author_email='hello@dailykitten.net',
     url='https://www.github.com/TDKorn/insta-tweet/',
-    download_url="https://github.com/TDKorn/insta-tweet/tarball/2.0.0/",
-    keywords=['instagram', 'twitter', 'repost', 'reposter', 'instascrape', 'instagram-repost'],
+    download_url=f"https://github.com/TDKorn/insta-tweet/tarball/master/",
+    keywords=['instagram', 'twitter', 'api', 'instagram api', 'twitter api', 'repost', 'instagram repost', 'reposter'],
     install_requires=[
         "requests",
         "tweepy",
-        "psycopg2",
         "sqlalchemy",
     ],
 )
```

