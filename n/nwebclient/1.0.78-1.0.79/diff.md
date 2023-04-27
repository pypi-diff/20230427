# Comparing `tmp/nwebclient-1.0.78.tar.gz` & `tmp/nwebclient-1.0.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nwebclient-1.0.78.tar", last modified: Tue Apr 25 10:38:41 2023, max compression
+gzip compressed data, was "dist/nwebclient-1.0.79.tar", last modified: Thu Apr 27 11:54:57 2023, max compression
```

## Comparing `nwebclient-1.0.78.tar` & `nwebclient-1.0.79.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-25 10:38:41.439799 nwebclient-1.0.78/
--rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.78/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-04-25 10:38:41.439799 nwebclient-1.0.78/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.78/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-25 10:38:41.439799 nwebclient-1.0.78/nwebclient/
--rw-r--r--   0 pi        (1000) pi        (1000)     4704 2023-03-17 18:34:02.000000 nwebclient-1.0.78/nwebclient/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.78/nwebclient/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3104 2023-03-29 20:50:31.000000 nwebclient-1.0.78/nwebclient/crypt.py
--rw-r--r--   0 pi        (1000) pi        (1000)     9793 2023-04-25 09:31:04.000000 nwebclient-1.0.78/nwebclient/sd.py
--rw-r--r--   0 pi        (1000) pi        (1000)     5582 2023-03-29 09:33:58.000000 nwebclient-1.0.78/nwebclient/sdb.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3218 2023-03-27 16:42:32.000000 nwebclient-1.0.78/nwebclient/ticker.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-25 10:38:41.439799 nwebclient-1.0.78/nwebclient.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-04-25 10:38:41.000000 nwebclient-1.0.78/nwebclient.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-04-25 10:38:41.000000 nwebclient-1.0.78/nwebclient.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-04-25 10:38:41.000000 nwebclient-1.0.78/nwebclient.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       84 2023-04-25 10:38:41.000000 nwebclient-1.0.78/nwebclient.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-04-25 10:38:41.000000 nwebclient-1.0.78/nwebclient.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-04-25 10:38:41.000000 nwebclient-1.0.78/nwebclient.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-04-25 10:38:41.439799 nwebclient-1.0.78/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      829 2023-04-25 10:38:38.000000 nwebclient-1.0.78/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-27 11:54:57.555689 nwebclient-1.0.79/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.79/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-04-27 11:54:57.555689 nwebclient-1.0.79/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.79/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-27 11:54:57.545689 nwebclient-1.0.79/nwebclient/
+-rw-r--r--   0 pi        (1000) pi        (1000)     4704 2023-03-17 18:34:02.000000 nwebclient-1.0.79/nwebclient/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.79/nwebclient/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3274 2023-04-26 10:42:29.000000 nwebclient-1.0.79/nwebclient/crypt.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    10590 2023-04-27 10:43:05.000000 nwebclient-1.0.79/nwebclient/sd.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     5625 2023-04-26 11:35:41.000000 nwebclient-1.0.79/nwebclient/sdb.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.79/nwebclient/ticker.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-27 11:54:57.555689 nwebclient-1.0.79/nwebclient.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-04-27 11:54:57.000000 nwebclient-1.0.79/nwebclient.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-04-27 11:54:57.000000 nwebclient-1.0.79/nwebclient.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-04-27 11:54:57.000000 nwebclient-1.0.79/nwebclient.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-04-27 11:54:57.000000 nwebclient-1.0.79/nwebclient.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-04-27 11:54:57.000000 nwebclient-1.0.79/nwebclient.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-04-27 11:54:57.000000 nwebclient-1.0.79/nwebclient.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-04-27 11:54:57.555689 nwebclient-1.0.79/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-04-27 11:54:52.000000 nwebclient-1.0.79/setup.py
```

### Comparing `nwebclient-1.0.78/LICENSE` & `nwebclient-1.0.79/LICENSE`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.78/PKG-INFO` & `nwebclient-1.0.79/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.78
+Version: 1.0.79
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.78/README.md` & `nwebclient-1.0.79/README.md`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.78/nwebclient/__init__.py` & `nwebclient-1.0.79/nwebclient/__init__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.78/nwebclient/__main__.py` & `nwebclient-1.0.79/nwebclient/__main__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.78/nwebclient/crypt.py` & `nwebclient-1.0.79/nwebclient/crypt.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,19 +24,25 @@
     if save_to_file:
         with open('public_key.pem', 'wb') as f:
             f.write(pem)
     result['public_key'] = pem
     return result
 
 def encrypt(message):
+    """
+      256-Byte Limit
+    """
     with open("public_key.pem", "rb") as key_file:
         public_key = serialization.load_pem_public_key(key_file.read(), backend=default_backend())
     return public_key.encrypt(message,padding.OAEP(mgf=padding.MGF1(algorithm=hashes.SHA256()),algorithm=hashes.SHA256(), label=None))
 
 def encryptFile(in_file, out_file):
+    """
+      Erwartet einen public_key.pem und legt den Schuessel fuer die Datei in {out_file}.key per RSA verschuesselt ab
+    """
     key = Fernet.generate_key()
     ekey = encrypt(key)
     hexlify = codecs.getencoder('hex')
     hkey=hexlify(ekey)[0]
     fernet = Fernet(key)
     with open(in_file, 'rb') as file:
         original = file.read()
```

### Comparing `nwebclient-1.0.78/nwebclient/sd.py` & `nwebclient-1.0.79/nwebclient/sd.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,23 +23,23 @@
       negative_prompt = negative_prompt,
       ).images
     for i in range(len(images)):
         #  images[i].save(prefix+str(i)+".jpg")
         sdb.sdb_write_pil(images[i], prompt, negative_prompt, guidance_scale, prefix, dbfile)
 
 
-"""
-  from nwebclient import sd
-  ig = sd.ImageGen()
-  ig.prompt = "photo"
-  ig.loop(5)
-  
-  ig.executeFromUrl('https://...')
-"""
 class ImageGen:
+    """
+    from nwebclient import sd
+    ig = sd.ImageGen()
+    ig.prompt = "photo"
+    ig.loop(5)
+  
+    ig.executeFromUrl('https://...')
+    """
     generator = 'diffusers' # diffusers or automatic1111 dummy cn_pose_1111 diffcn
     # scheduler
     pipe = None
     prompt = "photo"
     negative_prompt = "text, cartoon, anime, drawing, meme, postcard, painting, ((fuzzy)), ((blurred)), ((low resolution)), ((b&w)), ((monochrome)), ambiguous, ((deformed)), oversaturated, ((out of shot)), ((incoherent)), (((glitched))), (((3d render))), cgi, ((incorrect anatomy)), bad hands, lowres, long body, ((blurry)), double, ((duplicate body parts)), (disfigured), (extra limbs), fused fingers, extra fingers, malformed hands, ((((mutated hands and fingers)))), conjoined, ((missing limbs)), logo, signature, mutated, jpeg artifacts, low quality, bad eyes, oversized, disproportionate, (((incorrect proportions))), exaggerated, (((aliasing)))"
     guidance_scale = 7.5
     num_inference_steps=25
@@ -54,15 +54,15 @@
     gen_count = 0
     api = None
     cn_image = None
     diff_cn = None
     def __init__(self, model_id="XpucT/Deliberate"):
         self.model_id = model_id
     def load(self):
-        if self.loaded_model == self.model_id:
+        if self.loaded_model == self.model_id or self.generator == 'automatic1111':
             return
         self.scheduler = DPMSolverMultistepScheduler.from_pretrained(self.model_id, subfolder="scheduler")
         device = "cuda"
         model_revision = None
         if self.scheduler is None:
            self.pipe = StableDiffusionPipeline.from_pretrained(self.model_id, torch_dtype=torch.float16, revision=model_revision)
         else:
@@ -106,14 +106,16 @@
     def genCnPose1111(self, loop_number=1):
         self.initA1111();
         result = self.api.txt2img(prompt=self.prompt,negative_prompt=self.negative_prompt, height=self.height, width=self.width, controlnet_units=[self.cn_image],cfg_scale=7)
         self.save_image(result.image, 0,loop_number)
         self.gen_count = self.gen_count + 1
     def genA1111(self, loop_number=1):  
         self.initA1111();
+        if self.model_id.endwith('.safetensors') and self.model_id != self.loaded_model:
+             self.a1111setModel(self.model_id)
         result = self.api.txt2img(prompt=self.prompt,negative_prompt=self.negative_prompt, height=self.height, width=self.width, cfg_scale=7)
         self.save_image(result.image, 0,loop_number)
         self.gen_count = self.gen_count + 1
     def genDiffusers(self, loop_number=1):
         if self.pipe is None:
             self.load()
         images = self.pipe(self.prompt,
@@ -146,14 +148,16 @@
             self.prefix = data['prefix']
         if "guidance_scale" in data:
             self.guidance_scale = float(data['guidance_scale'])
         if "height" in data:
             self.height = int(data['height'])
         if "width" in data:
             self.width = int(data['width'])
+        if "generator" in data:
+            self.generator = int(data['generator'])
         if "model" in data:
             self.model_id = data['model']
             self.load()
         count = 10
         if "count" in data:
             count = int(data['count'])
         self.loop(count)
@@ -185,28 +189,38 @@
         self.info("End: "+time.strftime("%Y-%m-%d, %H:%M:%S", time.localtime()))
         return i
     def executeFromUrl(self, url, askForMore= True):
         res = requests.get(url)
         data = json.loads(res.text)
         i = self.executeJobs(data)
         if i > 0 and askForMore:
+            self.info('Asking for more Work')
             i = i + self.executeFromUrl(url, True)
         return i
     def info(self, message):
         print("[INFO] " + message)
     def a1111models(self):
         self.initA1111();
         result = self.api.util_get_model_names()
         return result
     def a1111setModel(self,model):
         self.initA1111();
         options = {}
         options['sd_model_checkpoint'] = model # 'model.ckpt [7460a6fa]'
+        self.loaded_model = model
         self.api.set_options(options)
+    def __str__(self):
+        return f'ImageGen {self.generator} {self.model_id} {self.prefix}'
+    def __repr__(self):
+        return f'ImageGen(generator=\'{self.generator}\', model_id=\'{self.model_id}\', prefix=\'{self.prefix}\')'
+    def toSdJob(count:50):
+        return {prefix:self.prefix, prompt:self.prompt, count:count, height: self.height, self.width: width}
             
         
 class ImageGenProcess(ticker.FileExtObserver):
     ext = ".sdjob"
-    def __init__(self, generator):
+    def __init__(self, generator=None):
+        if generator is None:
+            generator = ImageGen()
         self.generator = generator
     def processFile(self, filename):
         self.generator.executeJsonFile(filename)
```

### Comparing `nwebclient-1.0.78/nwebclient/sdb.py` & `nwebclient-1.0.79/nwebclient/sdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,9 +155,9 @@
         elif op =='from':
             print("Extract from id:"+str(sys.argv[2]))
         else:
             print("Error: Unknown Operation")
     else:
         show()
    
-if __name__ == '__main__':
+if __name__ == '__main__': # nx-sdb vom python-package bereitgestellt
     main()
```

### Comparing `nwebclient-1.0.78/nwebclient/ticker.py` & `nwebclient-1.0.79/nwebclient/ticker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import time
 import os
 import os.path
+import sys
 
 class Process:
     name = 'process'
     cpu = None
     def __init__(self, name='Process'):
         self.name = name
     def tick(self):
         pass
+    def configure(self, arg):
+        pass
     def cmd(self, args):
         return False
 
 class CmdEcho(Process):
+    """
+       nwebclient.ticker.CmdEcho
+    """
     def __init__(self):
         super().__init__('CmdEcho')
     def cmd(self, args):
         print("CMD: " + ' '.join(args))
         return False
 
 class Ticker(Process):
@@ -103,8 +109,40 @@
             p.cmd(args)
     def loop(self):
         while True:
             self.tick()
     def runTicks(self, count=100) :
         for i in range(count):
              self.tick()
+    def __str__(self):
+        s = "Cpu("
+        for p in self.processes:
+            s = s + ' ' + str(p)
+        return s
 
+def load_class(cl):
+    d = cl.rfind(".")
+    classname = cl[d+1:len(cl)]
+    m = __import__(cl[0:d], globals(), locals(), [classname])
+    return getattr(m, classname)
+
+def load_from_arg(cpu, arg):
+    a = arg.split(':')
+    a.append('')
+    cls = load_class(a[0])
+    c = cls()
+    c.configure(''.join(a[1:]))
+    cpu.add(c)
+                
+def main():
+    print("npy-ticker")
+    print("npy-ticker namespace.Proc:cfg ...")
+    cpu = Cpu()
+    for arg in sys.argv[1:]:
+        print("Loading: " + arg)   
+        load_from_arg(cpu, arg)
+    print(str(cpu))
+    #cpu.loop()
+    
+# 
+if __name__ == '__main__': # npy-ticker vom python-package bereitgestellt
+    main()
```

### Comparing `nwebclient-1.0.78/nwebclient.egg-info/PKG-INFO` & `nwebclient-1.0.79/nwebclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.78
+Version: 1.0.79
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.78/setup.py` & `nwebclient-1.0.79/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nwebclient",
-    version="1.0.78",
+    version="1.0.79",
     author="Bjoern Salgert",
     author_email="bjoern.salgert@hs-duesseldorf.de",
     description="NWebClient via HTTP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bsnx.net/4.0/group/pynwebclient",
     packages=setuptools.find_packages(),
     entry_points={
         'console_scripts': [
             'nx-sdb = nwebclient.sdb:main',
-            'nx-sdb-count =  nwebclient.sdb:count'
+            'nx-sdb-count =  nwebclient.sdb:count',
+            'npy-ticker = nwebclient.ticker:main'
         ]
     },
     classifiers=[
         "Programming Language :: Python :: 2",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

