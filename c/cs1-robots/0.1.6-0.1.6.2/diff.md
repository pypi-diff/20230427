# Comparing `tmp/cs1-robots-0.1.6.tar.gz` & `tmp/cs1-robots-0.1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs1-robots-0.1.6.tar", last modified: Fri Mar 31 05:26:51 2023, max compression
+gzip compressed data, was "cs1-robots-0.1.6.2.tar", last modified: Thu Apr 27 04:35:44 2023, max compression
```

## Comparing `cs1-robots-0.1.6.tar` & `cs1-robots-0.1.6.2.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 05:26:51.521356 cs1-robots-0.1.6/
--rw-rw-rw-   0        0        0      157 2023-03-31 05:26:51.521356 cs1-robots-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-03-31 04:40:58.000000 cs1-robots-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-03-31 05:26:51.523351 cs1-robots-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      339 2023-03-31 05:26:47.000000 cs1-robots-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-31 05:26:51.447325 cs1-robots-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-03-31 05:26:51.503383 cs1-robots-0.1.6/src/cs1_robots.egg-info/
--rw-rw-rw-   0        0        0      157 2023-03-31 05:26:51.000000 cs1-robots-0.1.6/src/cs1_robots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2023-03-31 05:26:51.000000 cs1-robots-0.1.6/src/cs1_robots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 05:26:51.000000 cs1-robots-0.1.6/src/cs1_robots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-03-31 05:26:51.000000 cs1-robots-0.1.6/src/cs1_robots.egg-info/requires.txt
--rw-rw-rw-   0        0        0       56 2023-03-31 05:26:51.000000 cs1-robots-0.1.6/src/cs1_robots.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-31 05:26:51.505364 cs1-robots-0.1.6/src/cs1graphics/
--rw-rw-rw-   0        0        0   207300 2023-03-31 04:58:34.000000 cs1-robots-0.1.6/src/cs1graphics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-31 05:26:51.510359 cs1-robots-0.1.6/src/cs1media/
--rw-rw-rw-   0        0        0    14580 2023-03-31 03:48:17.000000 cs1-robots-0.1.6/src/cs1media/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-31 05:26:51.512358 cs1-robots-0.1.6/src/cs1robots/
--rw-rw-rw-   0        0        0    17026 2023-03-31 03:48:17.000000 cs1-robots-0.1.6/src/cs1robots/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-31 05:26:51.515356 cs1-robots-0.1.6/src/cs1robots_images/
--rw-rw-rw-   0        0        0    32873 2023-03-31 03:48:17.000000 cs1-robots-0.1.6/src/cs1robots_images/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-31 05:26:51.518353 cs1-robots-0.1.6/src/easygui/
--rw-rw-rw-   0        0        0    55849 2023-03-31 03:48:16.000000 cs1-robots-0.1.6/src/easygui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 04:35:44.553293 cs1-robots-0.1.6.2/
+-rw-rw-rw-   0        0        0      619 2023-04-27 04:35:44.553293 cs1-robots-0.1.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2023-04-27 04:29:12.000000 cs1-robots-0.1.6.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-27 04:35:44.556230 cs1-robots-0.1.6.2/setup.cfg
+-rw-rw-rw-   0        0        0      524 2023-04-27 04:32:04.000000 cs1-robots-0.1.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 04:35:43.410206 cs1-robots-0.1.6.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-27 04:35:43.789985 cs1-robots-0.1.6.2/src/cs1_robots.egg-info/
+-rw-rw-rw-   0        0        0      619 2023-04-27 04:35:42.000000 cs1-robots-0.1.6.2/src/cs1_robots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-04-27 04:35:42.000000 cs1-robots-0.1.6.2/src/cs1_robots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 04:35:42.000000 cs1-robots-0.1.6.2/src/cs1_robots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-27 04:35:42.000000 cs1-robots-0.1.6.2/src/cs1_robots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       65 2023-04-27 04:35:42.000000 cs1-robots-0.1.6.2/src/cs1_robots.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 04:35:43.793979 cs1-robots-0.1.6.2/src/cs1elice/
+-rw-rw-rw-   0        0        0      856 2023-04-27 04:02:40.000000 cs1-robots-0.1.6.2/src/cs1elice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 04:35:43.865347 cs1-robots-0.1.6.2/src/cs1graphics/
+-rw-rw-rw-   0        0        0   229446 2023-04-27 04:02:04.000000 cs1-robots-0.1.6.2/src/cs1graphics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 04:35:44.125750 cs1-robots-0.1.6.2/src/cs1media/
+-rw-rw-rw-   0        0        0    15024 2023-04-22 05:54:52.000000 cs1-robots-0.1.6.2/src/cs1media/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 04:35:44.300613 cs1-robots-0.1.6.2/src/cs1robots/
+-rw-rw-rw-   0        0        0    17566 2023-04-22 05:54:52.000000 cs1-robots-0.1.6.2/src/cs1robots/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 04:35:44.472709 cs1-robots-0.1.6.2/src/cs1robots_images/
+-rw-rw-rw-   0        0        0    37116 2023-04-27 04:00:38.000000 cs1-robots-0.1.6.2/src/cs1robots_images/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 04:35:44.521999 cs1-robots-0.1.6.2/src/easygui/
+-rw-rw-rw-   0        0        0    55849 2023-04-22 05:54:52.000000 cs1-robots-0.1.6.2/src/easygui/__init__.py
```

### Comparing `cs1-robots-0.1.6/src/cs1media/__init__.py` & `cs1-robots-0.1.6.2/src/cs1media/__init__.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,444 +1,444 @@
-#
-# cs1media.py
-#
-# Environment for manipulating Images 
-#
-# 2010/03/24 Otfried Cheong
-# 2010/09/02: Convert image to RGB on loading
-#
-# Inspired and using some code from picture.py by Mark Guzdial.
-#
-# On Linux, need packages python-tk, python-imaging-tk
-#
-
-import sys as _sys
-import PIL.Image as _Image
-import PIL.ImageTk as _ImageTk
-import easygui as _easygui
-import tkinter.colorchooser as _tkColorChooser
-import tkinter.font as _tkFont
-import tkinter as _Tk
-
-# --------------------------------------------------------------------
-
-class Picture(object):
-  """A digital image."""
-
-  def __init__(self, surf):
-    """Create a Picture from an Image object."""
-    self._title = ""
-    self._reset(surf)
-
-  def _reset(self, surf):
-    self._surf = surf
-    self._pixels = surf.load()
-
-  def size(self):
-    """Return size of the image as a tuple (width, height)."""
-    return self._surf.size
-
-  def show1(self):
-    """Display the image."""
-    self._surf.show()
-
-  def show(self):
-    """Display the image and wait until user closes the image window."""
-    tool = PictureTool(self)
-    tool.run_tool()
-
-  def set_pixels(self, color = (0,0,0)):
-    """Set all pixels of the image to the given color."""
-    surf = _Image.new("RGB", self._surf.size, color)
-    self._reset(surf)
-
-  def set_title(self, title):
-    """Set title of image."""
-    self._title = title
-
-  def title(self):
-    """Return title of image."""
-    return self._title
-
-  def get(self, x, y):
-    """Return pixel at x, y."""
-    return self._pixels[x, y]
-
-  def set(self, x, y, color):
-    """Set pixel at x, y to color."""
-    self._pixels[x, y] = color
-
-  def save_as(self, filename = None):
-    """Save image as filename.
-    If no filename is given, open file-chooser."""
-    if not filename:
-      filename = _easygui.filesavebox("Save image as", _sys.argv[0], 
-                                      "unnamed.png",
-                                      [ [ "*.jpg", "*.png", "*.bmp",
-                                          "Image files" ] ])
-      if not filename: 
-        raise RuntimeError("No file name provided for saving.")
-    self._surf.save(filename)
-
-# --------------------------------------------------------------------
-
-def create_picture(width, height, color = (0,0,0)):
-  """Create an image of size width x height, and fill with color."""
-  if width < 0 or height < 0:
-    raise ValueError("Invalid image dimensions: " + str(width) + ", " 
-                     + str(height))
-  p = Picture(_Image.new("RGB", (width, height), color))
-  return p
-
-def load_picture(filename = None):
-  """Create an image by loading file filename.
-  Opens file-chooser if no file name given."""
-  if not filename:
-    filename = _easygui.fileopenbox("Select an image", 
-                                    _sys.argv[0], '*', 
-                                    [ [ "*.jpg", "*.png", "*.bmp", "*.gif",
-                                        "Image files" ] ])
-    if not filename: 
-      raise RuntimeError("No image file selected.")
-  img = _Image.open(filename)
-  if img.mode != "RGB":
-    img = img.convert("RGB")
-  p = Picture(img)
-  p.set_title(filename)
-  return p
-
-def choose_color():
-  color = _tkColorChooser.askcolor()
-  new_color = (color[0][0], color[0][1], color[0][2])
-  return new_color
-
-# --------------------------------------------------------------------
-
-##
-## Color Constants
-##
-
-class Color(object):
-  """Definitions for many beautiful colors."""
-
-  aliceblue = (240, 248, 255)
-  antiquewhite = (250, 235, 215)
-  aqua = (0, 255, 255)
-  aquamarine = (127, 255, 212)
-  azure = (240, 255, 255)
-  beige = (245, 245, 220)
-  bisque = (255, 228, 196)
-  black = (0, 0, 0)
-  blanchedalmond = (255, 235, 205)
-  blue = (0, 0, 255)
-  blueviolet = (138, 43, 226)
-  brown = (165, 42, 42)
-  burlywood = (222, 184, 135)
-  cadetblue = (95, 158, 160)
-  chartreuse = (127, 255, 0)
-  chocolate = (210, 105, 30)
-  coral = (255, 127, 80)
-  cornflowerblue = (100, 149, 237)
-  cornsilk = (255, 248, 220)
-  crimson = (220, 20, 60)
-  cyan = (0, 255, 255)
-  darkblue = (0, 0, 139)
-  darkcyan = (0, 139, 139)
-  darkgoldenrod = (184, 134, 11)
-  darkgray = (169, 169, 169)
-  darkgreen = (0, 100, 0)
-  darkkhaki = (189, 183, 107)
-  darkmagenta = (139, 0, 139)
-  darkolivegreen = (85, 107, 47)
-  darkorange = (255, 140, 0)
-  darkorchid = (153, 50, 204)
-  darkred = (139, 0, 0)
-  darksalmon = (233, 150, 122)
-  darkseagreen = (143, 188, 143)
-  darkslateblue = (72, 61, 139)
-  darkslategray = (47, 79, 79)
-  darkturquoise = (0, 206, 209)
-  darkviolet = (148, 0, 211)
-  deeppink = (255, 20, 147)
-  deepskyblue = (0, 191, 255)
-  dimgray = (105, 105, 105)
-  dodgerblue = (30, 144, 255)
-  firebrick = (178, 34, 34)
-  floralwhite = (255, 250, 240)
-  forestgreen = (34, 139, 34)
-  fuchsia = (255, 0, 255)
-  gainsboro = (220, 220, 220)
-  ghostwhite = (248, 248, 255)
-  gold = (255, 215, 0)
-  goldenrod = (218, 165, 32)
-  gray = (128, 128, 128)
-  green = (0, 128, 0)
-  greenyellow = (173, 255, 47)
-  honeydew = (240, 255, 240)
-  hotpink = (255, 105, 180)
-  indianred = (205, 92, 92)
-  indigo = (75, 0, 130)
-  ivory = (255, 255, 240)
-  khaki = (240, 230, 140)
-  lavender = (230, 230, 250)
-  lavenderblush = (255, 240, 245)
-  lawngreen = (124, 252, 0)
-  lemonchiffon = (255, 250, 205)
-  lightblue = (173, 216, 230)
-  lightcoral = (240, 128, 128)
-  lightcyan = (224, 255, 255)
-  lightgoldenrodyellow = (250, 250, 210)
-  lightgreen = (144, 238, 144)
-  lightgrey = (211, 211, 211)
-  lightpink = (255, 182, 193)
-  lightsalmon = (255, 160, 122)
-  lightseagreen = (32, 178, 170)
-  lightskyblue = (135, 206, 250)
-  lightslategray = (119, 136, 153)
-  lightsteelblue = (176, 196, 222)
-  lightyellow = (255, 255, 224)
-  lime = (0, 255, 0)
-  limegreen = (50, 205, 50)
-  linen = (250, 240, 230)
-  magenta = (255, 0, 255)
-  maroon = (128, 0, 0)
-  mediumaquamarine = (102, 205, 170)
-  mediumblue = (0, 0, 205)
-  mediumorchid = (186, 85, 211)
-  mediumpurple = (147, 112, 219)
-  mediumseagreen = (60, 179, 113)
-  mediumslateblue = (123, 104, 238)
-  mediumspringgreen = (0, 250, 154)
-  mediumturquoise = (72, 209, 204)
-  mediumvioletred = (199, 21, 133)
-  midnightblue = (25, 25, 112)
-  mintcream = (245, 255, 250)
-  mistyrose = (255, 228, 225)
-  moccasin = (255, 228, 181)
-  navajowhite = (255, 222, 173)
-  navy = (0, 0, 128)
-  oldlace = (253, 245, 230)
-  olive = (128, 128, 0)
-  olivedrab = (107, 142, 35)
-  orange = (255, 165, 0)
-  orangered = (255, 69, 0)
-  orchid = (218, 112, 214)
-  palegoldenrod = (238, 232, 170)
-  palegreen = (152, 251, 152)
-  paleturquoise = (175, 238, 238)
-  palevioletred = (219, 112, 147)
-  papayawhip = (255, 239, 213)
-  peachpuff = (255, 218, 185)
-  peru = (205, 133, 63)
-  pink = (255, 192, 203)
-  plum = (221, 160, 221)
-  powderblue = (176, 224, 230)
-  purple = (128, 0, 128)
-  red = (255, 0, 0)
-  rosybrown = (188, 143, 143)
-  royalblue = (65, 105, 225)
-  saddlebrown = (139, 69, 19)
-  salmon = (250, 128, 114)
-  sandybrown = (244, 164, 96)
-  seagreen = (46, 139, 87)
-  seashell = (255, 245, 238)
-  sienna = (160, 82, 45)
-  silver = (192, 192, 192)
-  skyblue = (135, 206, 235)
-  slateblue = (106, 90, 205)
-  slategray = (112, 128, 144)
-  snow = (255, 250, 250)
-  springgreen = (0, 255, 127)
-  steelblue = (70, 130, 180)
-  tan = (210, 180, 140)
-  teal = (0, 128, 128)
-  thistle = (216, 191, 216)
-  tomato = (255, 99, 71)
-  turquoise = (64, 224, 208)
-  violet = (238, 130, 238)
-  wheat = (245, 222, 179)
-  white = (255, 255, 255)
-  whitesmoke = (245, 245, 245)
-  yellow = (255, 255, 0)
-  yellowgreen = (154, 205, 50)
-  
-# --------------------------------------------------------------------
-
-class PictureTool:
-
-  def __init__(self, pict):
-    self.pict = pict
-    
-  def run_tool(self):
-    self.root = _Tk.Tk()
-    
-    self.top = _Tk.Menu(self.root, bd=2)
-    self.root.config(menu=self.top)
-    
-    self.zoom = _Tk.Menu(self.top, tearoff=0)
-    self.zoom.add_command(label='25%', command=lambda : self.zoomf(0.25),
-                          underline=0)
-    self.zoom.add_command(label='50%', command=lambda : self.zoomf(0.5),
-                          underline=0)
-    self.zoom.add_command(label='75%', command=lambda : self.zoomf(0.75),
-                          underline=0)
-    self.zoom.add_command(label='100%', command=lambda : self.zoomf(1.0),
-                          underline=0)
-    self.zoom.add_command(label='150%', command=lambda : self.zoomf(1.5),
-                          underline=0)
-    self.zoom.add_command(label='200%', command=lambda : self.zoomf(2.0),
-                          underline=0)
-    self.zoom.add_command(label='400%', command=lambda : self.zoomf(4.0),
-                          underline=0)
-    self.zoom.add_command(label='800%', command=lambda : self.zoomf(8.0),
-                          underline=0)
-    
-    self.top.add_cascade(label='Zoom', menu=self.zoom, underline=0)
-    
-    # create a frame and pack it
-    self.frame1 = _Tk.Frame(self.root)
-    self.frame1.pack(side=_Tk.BOTTOM, fill=_Tk.X)
-    
-    self.root.im = self.pict._surf
-    self.root.zoomMult = 1.0
-    
-    self.root.photo1 = _ImageTk.PhotoImage(image=self.root.im)
-    
-    self.root.title(self.pict.title())
-    
-    # Canvas for the Image, with scroll bars
-    
-    self.canvas1 = _Tk.Canvas(self.frame1, width=self.root.photo1.width() -
-                              1, height=self.root.photo1.height() - 1,
-                              cursor="crosshair", borderwidth=0)
-    self.root.vbar = _Tk.Scrollbar(self.frame1)
-    self.root.hbar = _Tk.Scrollbar(self.frame1, orient='horizontal')
-    self.root.vbar.pack(side=_Tk.RIGHT, fill=_Tk.Y)
-    self.root.hbar.pack(side=_Tk.BOTTOM, fill=_Tk.X)
-    
-    self.canvas1.pack(side=_Tk.BOTTOM, padx=0, pady=0, anchor=_Tk.NW, 
-                      fill=_Tk.BOTH, expand=_Tk.YES)
-
-    # call on scroll move
-    self.root.vbar.config(command=self.canvas1.yview)  
-    self.root.hbar.config(command=self.canvas1.xview)
-    # call on canvas move
-    self.canvas1.config(yscrollcommand=self.root.vbar.set)  
-    self.canvas1.config(xscrollcommand=self.root.hbar.set)
-    self.draw_image(self.root.im)
-    self.canvas1.bind('<Button-1>', self.canvClick)
-    
-    self.v = _Tk.StringVar()
-    self.v.set("R:      G:      B:     ")
-    self.xy = _Tk.StringVar()
-    self.xy.set("X:      Y:      ")
-    row = _Tk.Frame(self.root)
-    font = _tkFont.Font(size=10)
-    xyLabel = _Tk.Label(row, textvariable=self.xy, font=font)
-    colorLabel = _Tk.Label(row, textvariable=self.v, font=font)
-    self.canvas2 = _Tk.Canvas(row, width=35, bd=2, relief=_Tk.RIDGE, height=30)
-    xyLabel.pack(side=_Tk.LEFT)
-    colorLabel.pack(side=_Tk.LEFT, padx=100, pady=1)
-    self.canvas2.pack(side=_Tk.LEFT, padx=2, pady=1)
-    row.pack(side=_Tk.TOP, fill=_Tk.X)  # pack row on top
-
-    # start the event loop
-    self.root.mainloop()
-      
-  def zoomf(self, factor):
-    # zoom in or out
-    self.root.zoomMult = factor
-    (wide, high) = self.root.im.size
-    new = self.root.im.resize((int(wide * factor), int(high * factor)))
-    self.draw_image(new)
-
-  def draw_image(self, imgpil):
-    self.root.photo1 = _ImageTk.PhotoImage(image=imgpil)  # not file=imgpath
-    (scrwide, scrhigh) = self.root.maxsize()  # wm screen size x,y
-    scrhigh -= 200  # leave room for top display/button at max photo size
-    imgwide = self.root.photo1.width()  # size in pixels
-    imghigh = self.root.photo1.height()  # same as imgpil.size
-    
-    fullsize = (0, 0, imgwide, imghigh)  # scrollable
-    viewwide = min(imgwide, scrwide)  # viewable
-    viewhigh = min(imghigh, scrhigh)
-    
-    self.canvas1.delete('all')  # clear prior photo
-    self.canvas1.config(height=viewhigh, width=viewwide)  # viewable window size
-    self.canvas1.config(scrollregion=fullsize)  # scrollable area size
-    
-    self.root.img = self.canvas1.create_image(0, 0, image=self.root.photo1,
-                                              anchor=_Tk.NW)
-    
-    if imgwide <= scrwide and imghigh <= scrhigh:  # too big for display?
-      self.root.state('normal')  # no: win size per img
-    elif (_sys.platform)[:3] == 'win':
-      # do windows fullscreen
-      self.root.state('zoomed')  # others use geometry( )
-
-  def canvClick(self, event):
-    try:
-      x = int(self.canvas1.canvasx(event.x) / self.root.zoomMult)
-      y = int(self.canvas1.canvasy(event.y) / self.root.zoomMult)
-      w, h = self.root.im.size
-      if 0 <= x < w and 0 <= y < h:
-        tk_rgb = "#%02x%02x%02x" % self.root.im.getpixel((x, y))
-        self.canvas2.config(bg=tk_rgb)
-        rgb = "R: %d; G: %d; B: %d;" % self.root.im.getpixel((x, y))
-        self.v.set(rgb)
-        xy = "X: %d; Y: %d;" % (x, y)
-        self.xy.set(xy)
-      else:
-        rgb = "X,Y Out of Range"
-        self.v.set(rgb)
-    except ValueError:
-      pass
-    
-def picture_tool(filename = None):
-  """Allows you to find information about digital images.
-
-  The PictureTool's Toolbar:
-
-  Once you have opened an image, you can view information about its
-  individual pixels by looking at the toolbar. To select a pixel drag
-  (click and hold down) the mouse to the position you want and then
-  release it to hold that position's information in the toolbar.
-
-  The following information in the toolbar changes to reflect the
-  properties of the pixel you selected:
-
-  X = the x coordinate of the pixel (starting with 0, counting from the left) 
-  Y = the y coordinate of the pixel (starting with 0, counting from the top)
-  R = the Red value of the pixel (0 to 255)
-  G = the Green value of the pixel (0 to 255)
-  B = the Blue value of the pixel (0 to 255)
-
-  In addition, the box at the far right displays the color of the pixel.
-
-  Zooming in/out:
-  To Zoom, select the amount of zoom you want from the zoom menu.
-  Less than 100% zooms out and more than 100% zooms in. 
-  The 100% zoom level will always return you to your orginal picture.
-  
-  filename: a string representing the location and name of picture.
-  If no filename is given, a file-chooser opens."""
-
-  if not filename:
-    filename = _easygui.fileopenbox("Select an image", 
-                                    _sys.argv[0], '*', 
-                                    [ [ "*.jpg", "*.png", "*.bmp", "*.gif",
-                                        "Image files" ] ])
-    if not filename: 
-      raise RuntimeError("No image file selected.")
-  img = load_picture(filename)
-  tool = PictureTool(img)
-  tool.run_tool()
-
-# --------------------------------------------------------------------
-  
-if __name__ == "__main__":
-  if len(_sys.argv > 1):
-    picture_tool(_sys.argv[1])
-  else:
-    picture_tool()
-
-# --------------------------------------------------------------------
+#
+# cs1media.py
+#
+# Environment for manipulating Images 
+#
+# 2010/03/24 Otfried Cheong
+# 2010/09/02: Convert image to RGB on loading
+#
+# Inspired and using some code from picture.py by Mark Guzdial.
+#
+# On Linux, need packages python-tk, python-imaging-tk
+#
+
+import sys as _sys
+import PIL.Image as _Image
+import PIL.ImageTk as _ImageTk
+import easygui as _easygui
+import tkinter.colorchooser as _tkColorChooser
+import tkinter.font as _tkFont
+import tkinter as _Tk
+
+# --------------------------------------------------------------------
+
+class Picture(object):
+  """A digital image."""
+
+  def __init__(self, surf):
+    """Create a Picture from an Image object."""
+    self._title = ""
+    self._reset(surf)
+
+  def _reset(self, surf):
+    self._surf = surf
+    self._pixels = surf.load()
+
+  def size(self):
+    """Return size of the image as a tuple (width, height)."""
+    return self._surf.size
+
+  def show1(self):
+    """Display the image."""
+    self._surf.show()
+
+  def show(self):
+    """Display the image and wait until user closes the image window."""
+    tool = PictureTool(self)
+    tool.run_tool()
+
+  def set_pixels(self, color = (0,0,0)):
+    """Set all pixels of the image to the given color."""
+    surf = _Image.new("RGB", self._surf.size, color)
+    self._reset(surf)
+
+  def set_title(self, title):
+    """Set title of image."""
+    self._title = title
+
+  def title(self):
+    """Return title of image."""
+    return self._title
+
+  def get(self, x, y):
+    """Return pixel at x, y."""
+    return self._pixels[x, y]
+
+  def set(self, x, y, color):
+    """Set pixel at x, y to color."""
+    self._pixels[x, y] = color
+
+  def save_as(self, filename = None):
+    """Save image as filename.
+    If no filename is given, open file-chooser."""
+    if not filename:
+      filename = _easygui.filesavebox("Save image as", _sys.argv[0], 
+                                      "unnamed.png",
+                                      [ [ "*.jpg", "*.png", "*.bmp",
+                                          "Image files" ] ])
+      if not filename: 
+        raise RuntimeError("No file name provided for saving.")
+    self._surf.save(filename)
+
+# --------------------------------------------------------------------
+
+def create_picture(width, height, color = (0,0,0)):
+  """Create an image of size width x height, and fill with color."""
+  if width < 0 or height < 0:
+    raise ValueError("Invalid image dimensions: " + str(width) + ", " 
+                     + str(height))
+  p = Picture(_Image.new("RGB", (width, height), color))
+  return p
+
+def load_picture(filename = None):
+  """Create an image by loading file filename.
+  Opens file-chooser if no file name given."""
+  if not filename:
+    filename = _easygui.fileopenbox("Select an image", 
+                                    _sys.argv[0], '*', 
+                                    [ [ "*.jpg", "*.png", "*.bmp", "*.gif",
+                                        "Image files" ] ])
+    if not filename: 
+      raise RuntimeError("No image file selected.")
+  img = _Image.open(filename)
+  if img.mode != "RGB":
+    img = img.convert("RGB")
+  p = Picture(img)
+  p.set_title(filename)
+  return p
+
+def choose_color():
+  color = _tkColorChooser.askcolor()
+  new_color = (color[0][0], color[0][1], color[0][2])
+  return new_color
+
+# --------------------------------------------------------------------
+
+##
+## Color Constants
+##
+
+class Color(object):
+  """Definitions for many beautiful colors."""
+
+  aliceblue = (240, 248, 255)
+  antiquewhite = (250, 235, 215)
+  aqua = (0, 255, 255)
+  aquamarine = (127, 255, 212)
+  azure = (240, 255, 255)
+  beige = (245, 245, 220)
+  bisque = (255, 228, 196)
+  black = (0, 0, 0)
+  blanchedalmond = (255, 235, 205)
+  blue = (0, 0, 255)
+  blueviolet = (138, 43, 226)
+  brown = (165, 42, 42)
+  burlywood = (222, 184, 135)
+  cadetblue = (95, 158, 160)
+  chartreuse = (127, 255, 0)
+  chocolate = (210, 105, 30)
+  coral = (255, 127, 80)
+  cornflowerblue = (100, 149, 237)
+  cornsilk = (255, 248, 220)
+  crimson = (220, 20, 60)
+  cyan = (0, 255, 255)
+  darkblue = (0, 0, 139)
+  darkcyan = (0, 139, 139)
+  darkgoldenrod = (184, 134, 11)
+  darkgray = (169, 169, 169)
+  darkgreen = (0, 100, 0)
+  darkkhaki = (189, 183, 107)
+  darkmagenta = (139, 0, 139)
+  darkolivegreen = (85, 107, 47)
+  darkorange = (255, 140, 0)
+  darkorchid = (153, 50, 204)
+  darkred = (139, 0, 0)
+  darksalmon = (233, 150, 122)
+  darkseagreen = (143, 188, 143)
+  darkslateblue = (72, 61, 139)
+  darkslategray = (47, 79, 79)
+  darkturquoise = (0, 206, 209)
+  darkviolet = (148, 0, 211)
+  deeppink = (255, 20, 147)
+  deepskyblue = (0, 191, 255)
+  dimgray = (105, 105, 105)
+  dodgerblue = (30, 144, 255)
+  firebrick = (178, 34, 34)
+  floralwhite = (255, 250, 240)
+  forestgreen = (34, 139, 34)
+  fuchsia = (255, 0, 255)
+  gainsboro = (220, 220, 220)
+  ghostwhite = (248, 248, 255)
+  gold = (255, 215, 0)
+  goldenrod = (218, 165, 32)
+  gray = (128, 128, 128)
+  green = (0, 128, 0)
+  greenyellow = (173, 255, 47)
+  honeydew = (240, 255, 240)
+  hotpink = (255, 105, 180)
+  indianred = (205, 92, 92)
+  indigo = (75, 0, 130)
+  ivory = (255, 255, 240)
+  khaki = (240, 230, 140)
+  lavender = (230, 230, 250)
+  lavenderblush = (255, 240, 245)
+  lawngreen = (124, 252, 0)
+  lemonchiffon = (255, 250, 205)
+  lightblue = (173, 216, 230)
+  lightcoral = (240, 128, 128)
+  lightcyan = (224, 255, 255)
+  lightgoldenrodyellow = (250, 250, 210)
+  lightgreen = (144, 238, 144)
+  lightgrey = (211, 211, 211)
+  lightpink = (255, 182, 193)
+  lightsalmon = (255, 160, 122)
+  lightseagreen = (32, 178, 170)
+  lightskyblue = (135, 206, 250)
+  lightslategray = (119, 136, 153)
+  lightsteelblue = (176, 196, 222)
+  lightyellow = (255, 255, 224)
+  lime = (0, 255, 0)
+  limegreen = (50, 205, 50)
+  linen = (250, 240, 230)
+  magenta = (255, 0, 255)
+  maroon = (128, 0, 0)
+  mediumaquamarine = (102, 205, 170)
+  mediumblue = (0, 0, 205)
+  mediumorchid = (186, 85, 211)
+  mediumpurple = (147, 112, 219)
+  mediumseagreen = (60, 179, 113)
+  mediumslateblue = (123, 104, 238)
+  mediumspringgreen = (0, 250, 154)
+  mediumturquoise = (72, 209, 204)
+  mediumvioletred = (199, 21, 133)
+  midnightblue = (25, 25, 112)
+  mintcream = (245, 255, 250)
+  mistyrose = (255, 228, 225)
+  moccasin = (255, 228, 181)
+  navajowhite = (255, 222, 173)
+  navy = (0, 0, 128)
+  oldlace = (253, 245, 230)
+  olive = (128, 128, 0)
+  olivedrab = (107, 142, 35)
+  orange = (255, 165, 0)
+  orangered = (255, 69, 0)
+  orchid = (218, 112, 214)
+  palegoldenrod = (238, 232, 170)
+  palegreen = (152, 251, 152)
+  paleturquoise = (175, 238, 238)
+  palevioletred = (219, 112, 147)
+  papayawhip = (255, 239, 213)
+  peachpuff = (255, 218, 185)
+  peru = (205, 133, 63)
+  pink = (255, 192, 203)
+  plum = (221, 160, 221)
+  powderblue = (176, 224, 230)
+  purple = (128, 0, 128)
+  red = (255, 0, 0)
+  rosybrown = (188, 143, 143)
+  royalblue = (65, 105, 225)
+  saddlebrown = (139, 69, 19)
+  salmon = (250, 128, 114)
+  sandybrown = (244, 164, 96)
+  seagreen = (46, 139, 87)
+  seashell = (255, 245, 238)
+  sienna = (160, 82, 45)
+  silver = (192, 192, 192)
+  skyblue = (135, 206, 235)
+  slateblue = (106, 90, 205)
+  slategray = (112, 128, 144)
+  snow = (255, 250, 250)
+  springgreen = (0, 255, 127)
+  steelblue = (70, 130, 180)
+  tan = (210, 180, 140)
+  teal = (0, 128, 128)
+  thistle = (216, 191, 216)
+  tomato = (255, 99, 71)
+  turquoise = (64, 224, 208)
+  violet = (238, 130, 238)
+  wheat = (245, 222, 179)
+  white = (255, 255, 255)
+  whitesmoke = (245, 245, 245)
+  yellow = (255, 255, 0)
+  yellowgreen = (154, 205, 50)
+  
+# --------------------------------------------------------------------
+
+class PictureTool:
+
+  def __init__(self, pict):
+    self.pict = pict
+    
+  def run_tool(self):
+    self.root = _Tk.Tk()
+    
+    self.top = _Tk.Menu(self.root, bd=2)
+    self.root.config(menu=self.top)
+    
+    self.zoom = _Tk.Menu(self.top, tearoff=0)
+    self.zoom.add_command(label='25%', command=lambda : self.zoomf(0.25),
+                          underline=0)
+    self.zoom.add_command(label='50%', command=lambda : self.zoomf(0.5),
+                          underline=0)
+    self.zoom.add_command(label='75%', command=lambda : self.zoomf(0.75),
+                          underline=0)
+    self.zoom.add_command(label='100%', command=lambda : self.zoomf(1.0),
+                          underline=0)
+    self.zoom.add_command(label='150%', command=lambda : self.zoomf(1.5),
+                          underline=0)
+    self.zoom.add_command(label='200%', command=lambda : self.zoomf(2.0),
+                          underline=0)
+    self.zoom.add_command(label='400%', command=lambda : self.zoomf(4.0),
+                          underline=0)
+    self.zoom.add_command(label='800%', command=lambda : self.zoomf(8.0),
+                          underline=0)
+    
+    self.top.add_cascade(label='Zoom', menu=self.zoom, underline=0)
+    
+    # create a frame and pack it
+    self.frame1 = _Tk.Frame(self.root)
+    self.frame1.pack(side=_Tk.BOTTOM, fill=_Tk.X)
+    
+    self.root.im = self.pict._surf
+    self.root.zoomMult = 1.0
+    
+    self.root.photo1 = _ImageTk.PhotoImage(image=self.root.im)
+    
+    self.root.title(self.pict.title())
+    
+    # Canvas for the Image, with scroll bars
+    
+    self.canvas1 = _Tk.Canvas(self.frame1, width=self.root.photo1.width() -
+                              1, height=self.root.photo1.height() - 1,
+                              cursor="crosshair", borderwidth=0)
+    self.root.vbar = _Tk.Scrollbar(self.frame1)
+    self.root.hbar = _Tk.Scrollbar(self.frame1, orient='horizontal')
+    self.root.vbar.pack(side=_Tk.RIGHT, fill=_Tk.Y)
+    self.root.hbar.pack(side=_Tk.BOTTOM, fill=_Tk.X)
+    
+    self.canvas1.pack(side=_Tk.BOTTOM, padx=0, pady=0, anchor=_Tk.NW, 
+                      fill=_Tk.BOTH, expand=_Tk.YES)
+
+    # call on scroll move
+    self.root.vbar.config(command=self.canvas1.yview)  
+    self.root.hbar.config(command=self.canvas1.xview)
+    # call on canvas move
+    self.canvas1.config(yscrollcommand=self.root.vbar.set)  
+    self.canvas1.config(xscrollcommand=self.root.hbar.set)
+    self.draw_image(self.root.im)
+    self.canvas1.bind('<Button-1>', self.canvClick)
+    
+    self.v = _Tk.StringVar()
+    self.v.set("R:      G:      B:     ")
+    self.xy = _Tk.StringVar()
+    self.xy.set("X:      Y:      ")
+    row = _Tk.Frame(self.root)
+    font = _tkFont.Font(size=10)
+    xyLabel = _Tk.Label(row, textvariable=self.xy, font=font)
+    colorLabel = _Tk.Label(row, textvariable=self.v, font=font)
+    self.canvas2 = _Tk.Canvas(row, width=35, bd=2, relief=_Tk.RIDGE, height=30)
+    xyLabel.pack(side=_Tk.LEFT)
+    colorLabel.pack(side=_Tk.LEFT, padx=100, pady=1)
+    self.canvas2.pack(side=_Tk.LEFT, padx=2, pady=1)
+    row.pack(side=_Tk.TOP, fill=_Tk.X)  # pack row on top
+
+    # start the event loop
+    self.root.mainloop()
+      
+  def zoomf(self, factor):
+    # zoom in or out
+    self.root.zoomMult = factor
+    (wide, high) = self.root.im.size
+    new = self.root.im.resize((int(wide * factor), int(high * factor)))
+    self.draw_image(new)
+
+  def draw_image(self, imgpil):
+    self.root.photo1 = _ImageTk.PhotoImage(image=imgpil)  # not file=imgpath
+    (scrwide, scrhigh) = self.root.maxsize()  # wm screen size x,y
+    scrhigh -= 200  # leave room for top display/button at max photo size
+    imgwide = self.root.photo1.width()  # size in pixels
+    imghigh = self.root.photo1.height()  # same as imgpil.size
+    
+    fullsize = (0, 0, imgwide, imghigh)  # scrollable
+    viewwide = min(imgwide, scrwide)  # viewable
+    viewhigh = min(imghigh, scrhigh)
+    
+    self.canvas1.delete('all')  # clear prior photo
+    self.canvas1.config(height=viewhigh, width=viewwide)  # viewable window size
+    self.canvas1.config(scrollregion=fullsize)  # scrollable area size
+    
+    self.root.img = self.canvas1.create_image(0, 0, image=self.root.photo1,
+                                              anchor=_Tk.NW)
+    
+    if imgwide <= scrwide and imghigh <= scrhigh:  # too big for display?
+      self.root.state('normal')  # no: win size per img
+    elif (_sys.platform)[:3] == 'win':
+      # do windows fullscreen
+      self.root.state('zoomed')  # others use geometry( )
+
+  def canvClick(self, event):
+    try:
+      x = int(self.canvas1.canvasx(event.x) / self.root.zoomMult)
+      y = int(self.canvas1.canvasy(event.y) / self.root.zoomMult)
+      w, h = self.root.im.size
+      if 0 <= x < w and 0 <= y < h:
+        tk_rgb = "#%02x%02x%02x" % self.root.im.getpixel((x, y))
+        self.canvas2.config(bg=tk_rgb)
+        rgb = "R: %d; G: %d; B: %d;" % self.root.im.getpixel((x, y))
+        self.v.set(rgb)
+        xy = "X: %d; Y: %d;" % (x, y)
+        self.xy.set(xy)
+      else:
+        rgb = "X,Y Out of Range"
+        self.v.set(rgb)
+    except ValueError:
+      pass
+    
+def picture_tool(filename = None):
+  """Allows you to find information about digital images.
+
+  The PictureTool's Toolbar:
+
+  Once you have opened an image, you can view information about its
+  individual pixels by looking at the toolbar. To select a pixel drag
+  (click and hold down) the mouse to the position you want and then
+  release it to hold that position's information in the toolbar.
+
+  The following information in the toolbar changes to reflect the
+  properties of the pixel you selected:
+
+  X = the x coordinate of the pixel (starting with 0, counting from the left) 
+  Y = the y coordinate of the pixel (starting with 0, counting from the top)
+  R = the Red value of the pixel (0 to 255)
+  G = the Green value of the pixel (0 to 255)
+  B = the Blue value of the pixel (0 to 255)
+
+  In addition, the box at the far right displays the color of the pixel.
+
+  Zooming in/out:
+  To Zoom, select the amount of zoom you want from the zoom menu.
+  Less than 100% zooms out and more than 100% zooms in. 
+  The 100% zoom level will always return you to your orginal picture.
+  
+  filename: a string representing the location and name of picture.
+  If no filename is given, a file-chooser opens."""
+
+  if not filename:
+    filename = _easygui.fileopenbox("Select an image", 
+                                    _sys.argv[0], '*', 
+                                    [ [ "*.jpg", "*.png", "*.bmp", "*.gif",
+                                        "Image files" ] ])
+    if not filename: 
+      raise RuntimeError("No image file selected.")
+  img = load_picture(filename)
+  tool = PictureTool(img)
+  tool.run_tool()
+
+# --------------------------------------------------------------------
+  
+if __name__ == "__main__":
+  if len(_sys.argv > 1):
+    picture_tool(_sys.argv[1])
+  else:
+    picture_tool()
+
+# --------------------------------------------------------------------
```

### Comparing `cs1-robots-0.1.6/src/cs1robots/__init__.py` & `cs1-robots-0.1.6.2/src/cs1robots/__init__.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,540 +1,540 @@
-#
-# cs1robots.py
-#
-# Environment for steering a robot through a grid world
-# for learning to program in Python
-#
-# Inspired by and using code from RUR-PLE by Andre Roberge
-#
-# 2010/01/14 Otfried Cheong
-# 2010/02/23: Changed to refresh only once after every move
-# 2010/02/24: Fixed refresh in world editing.
-# 2010/08/12: Improved handling of beepers to speed up.
-#
-# On Linux, need packages python-tk, python-imaging-tk
-#
-
-import sys as _sys
-import cs1graphics as _g
-import easygui as _easygui
-import re as _re
-import time as _time
-
-from cs1robots_images import _robot_images
-
-# PIL isn't actually used in cs1robots, but is needed to use
-# cs1graphics properly.  So we make sure it is there, as otherwise
-# users get a confusing error message.
-import PIL.Image as _Image
-import PIL.ImageDraw as _ImageDraw
-import PIL.ImageTk as _ImageTk
-
-#_g._debug = 2
-
-_scene = None
-_world = None
-
-_directions = [ (0, 1), (-1, 0), (0, -1), (1, 0) ]
-_orient_dict = { 'E': 3, 'S': 2, 'W': 1, 'N': 0}
-
-class RobotError(Exception):
-  def __init__(self, str):
-    Exception.__init__(self, str)
-
-def pause(delay = 1.0):
-  """Pause for delay seconds."""
-  _time.sleep(delay)
-
-# --------------------------------------------------------------------
-
-class _Beeper(object):
-  """One ore more beepers at a crossing in the world."""
-  def __init__(self, radius, av, st, num = 1):
-    self.av = av
-    self.st = st
-    self.num = num
-    self.layer = _g.Layer()
-    self.circle = _g.Circle(radius = radius)
-    self.text = _g.Text("%d" % num, 11, _g.Point(0, 0))
-    self.layer.add(self.circle)
-    self.layer.add(self.text)
-    self.circle.setFillColor("yellow")
-    self.circle.setBorderColor("orange")
-    self.circle.setDepth(10)
-    self.text.setDepth(5)
-    self.layer.setDepth(5)
-
-  def set_number(self, num):
-    self.num = num
-    self.text.setMessage("%d" % num)
-    
-class _World(object):
-  """This class defines the world's logic."""
-
-  def __init__(self, avenues = 10, streets = 10, walls = [], beepers = {}):
-    self.av = avenues
-    self.st = streets
-    self.num_cols = 2*avenues + 1
-    self.num_rows = 2*streets + 1
-    self.walls = walls
-    for (col, row) in self.walls:
-      if not (col+row) % 2:
-        raise RuntimeError("Wall in impossible position (%d, %d)." % (col,row))
-    self.beepers = beepers
-    self.borders = []
-    self.beeper_icons = {}
-    self.set_borders()
-
-  def cr2xy(self, col, row):
-    x = self.left + self.ts * col
-    y = self.bottom - self.ts * row
-    return x, y
-
-  def set_borders(self):
-    """The world is surrounded by a continuous wall.  This function
-       sets the corresponding "wall" or "border" based on the world's
-       dimensions."""
-    for col in range(1, self.num_cols-1, 2):
-      if (col, 0) not in self.borders:
-        self.borders.append( (col, 0) )
-      if (col, self.num_rows) not in self.borders:
-        self.borders.append( (col, self.num_rows-1) )
-      for row in range(1, self.num_rows-1, 2):
-        if (0, row) not in self.borders:
-          self.borders.append( (0, row) )
-        if (self.num_cols, row) not in self.borders:
-          self.borders.append( (self.num_cols-1, row) )
-
-  def toggle_wall(self, col, row):
-    """This function is intended for adding or removing a
-       wall from a GUI world editor."""
-    if (col+row) % 2 :  # safety check
-      if (col, row) in self.walls: # toggle value
-        self.walls.remove((col, row))
-      else:
-        self.walls.append((col, row))
-    else:
-      raise RuntimeError("Wall in impossible position (%d, %d)." % (col,row))
-
-  def is_clear(self, col, row):
-    """Returns True if there is no wall or border here."""
-    return not ((col, row) in self.walls or
-                (col, row) in self.borders)
-  
-  def add_beeper(self, av, st):
-    """Add a single beeper."""
-    assert self.layer
-    if (av, st) in self.beepers:
-      self.beepers[(av, st)] += 1
-      bp = self.beeper_icons[(av,st)]
-      bp.set_number(self.beepers[(av, st)])
-    else:
-      self.beepers[(av, st)] = 1
-      self._create_beeper(av, st)
-
-  def remove_beeper(self, av, st):
-    """Remove a beeper (does nothing if no beeper here)."""
-    assert self.layer
-    if (av, st) in self.beepers:
-      self.beepers[(av, st)] -= 1
-      if self.beepers[(av, st)] == 0:
-        del self.beepers[(av, st)]
-        self.layer.remove(self.beeper_icons[(av,st)].layer)
-        del self.beeper_icons[(av,st)]
-      else:
-        bp = self.beeper_icons[(av,st)]
-        bp.set_number(self.beepers[(av, st)])
-
-  def _create_beeper(self, av, st):
-    num = self.beepers[(av, st)]
-    bp = _Beeper(0.6 * self.ts, av, st, num)
-    x, y = self.cr2xy(2 * av - 1, 2 * st - 1)
-    bp.layer.moveTo(x, y)
-    self.beeper_icons[(av, st)] = bp
-    self.layer.add(bp.layer)
-
-  def create_layer(self):
-    # compute tilesize and border coordinates
-    w, h = _scene.getWidth(), _scene.getHeight()
-    tsx =  w / (self.num_cols + 2)
-    tsy =  h / (self.num_rows + 2)
-    self.ts = min(tsx, tsy)
-    self.left = 2 * self.ts
-    self.right = self.left + 2 * self.ts * self.av
-    self.bottom = h - 2 * self.ts
-    self.top = self.bottom - 2 * self.ts * self.st
-    self.layer = _g.Layer()
-    # Create avenues
-    for av in range(self.av):
-      x = self.left + self.ts * (2 * av + 1) 
-      l = _g.Path([_g.Point(x, self.top), _g.Point(x, self.bottom)])
-      l.setBorderColor("light gray")
-      self.layer.add(l)
-      self.layer.add(_g.Text("%d" % (av + 1), 10, 
-                             _g.Point(x, self.bottom + self.ts)))
-    # Create streets
-    for st in range(self.st):
-      y = self.bottom - self.ts * (2 * st + 1) 
-      l = _g.Path([_g.Point(self.left, y), _g.Point(self.right, y)])
-      l.setBorderColor("light gray")
-      self.layer.add(l)
-      self.layer.add(_g.Text("%d" % (st + 1), 10, 
-                             _g.Point(self.left - self.ts, y)))
-    # Create border
-    border = _g.Polygon(_g.Point(self.left, self.bottom),
-                        _g.Point(self.right, self.bottom),
-                        _g.Point(self.right, self.top),
-                        _g.Point(self.left, self.top))
-    border.setBorderWidth(5)
-    border.setBorderColor("dark red")
-    border.setDepth(10)
-    self.layer.add(border)
-    # Create walls
-    for (col, row) in self.walls:
-      if col % 2 == 0:  # vertical wall
-        x1, y1 = self.cr2xy(col, row - 1)
-        x2, y2 = self.cr2xy(col, row + 1)
-      else: # horizontal wall
-        x1, y1 = self.cr2xy(col - 1, row)
-        x2, y2 = self.cr2xy(col + 1, row)
-      w = _g.Path([_g.Point(x1,y1), _g.Point(x2,y2)])
-      w.setBorderWidth(5)
-      w.setBorderColor("dark red")
-      w.setDepth(10)
-      self.layer.add(w)
-    # Create beepers
-    for (av, st) in self.beepers:
-      self._create_beeper(av, st)
-    # Layer finished
-    _scene.add(self.layer)
-    
-  def update_layer(self):
-    _scene.remove(self.layer)
-    self.beeper_icons = {}
-    self.create_layer()
-
-  def save(self, out):
-    av_string = "avenues = " + str(self.av) + '\n'
-    st_string = "streets = " + str(self.st) + '\n'
-    if len(self.walls) > 0:
-      wall_string = "walls = [\n"
-      for item in self.walls:
-        wall_string += ("    " + str(item) + ', \n')
-      wall_string = wall_string[:-3] + '\n]\n'
-    else:
-      wall_string = "walls = []\n"
-    if len(self.beepers) > 0:
-      beeper_string = "beepers = {\n"
-      for key in self.beepers:
-        beeper_string += ("    " + str(key) + ': ' +
-                          str(self.beepers[key]) + ', \n')
-      beeper_string = beeper_string[:-3] + '\n}\n'
-    else:
-      beeper_string = "beepers = {}\n"
-    out.write(av_string + st_string + wall_string + beeper_string)
-    
-# --------------------------------------------------------------------
-
-def create_world(avenues = 10, streets = 10):
-  """Create an empty robot world."""
-  global _scene, _world
-  if _scene:
-    raise RuntimeError("A robot world already exists!")
-  _scene = _g.Canvas()
-  _scene.setWidth(50 * avenues)
-  _scene.setHeight(50 * streets)
-  _scene.setTitle("Robot World")
-  _world = _World(avenues, streets)
-  _world.create_layer()
-  _scene.setAutoRefresh(False)
-
-def _check_world(contents):
-  # safety check
-  safe = contents[:]
-    # only allow known keywords
-  keywords = ["avenues", "streets", "walls", "beepers", "robot",
-              "'s'", "'S'", '"s"', '"S"',
-              "'e'", "'E'", '"e"', '"E"',
-              "'w'", "'W'", '"w"', '"W"',
-              "'n'", "'N'", '"n"', '"N"', ]
-  for word in keywords:
-    safe = safe.replace(word, '')
-  safe = list(safe)
-  for char in safe:
-    if char.isalpha():
-      raise ValueError("Invalid word or character in world file")
-    
-def load_world(filename = None):
-  """Loads a robot world from filename.
-  Opens file-chooser if no filename is given."""
-  global _scene, _world
-  if _scene:
-    raise RuntimeError("A robot world already exists!")
-  if not filename:
-    filename = _easygui.fileopenbox("Select a Robot world", 
-                                    "Robot World", '*', [ "*.wld" ])
-    if not filename: 
-      raise RuntimeError("No world file selected.")
-  txt = open(filename, 'rb').read()
-  txt = _re.sub('\r\n', '\n', txt) # Windows
-  txt = _re.sub('\r', '\n', txt)  # Mac
-  _check_world(txt)
-  wd = {}
-  # extracts avenues, streets, walls and beepers
-  try:
-    exec (txt in wd)
-    w = _World(wd['avenues'], wd['streets'], wd['walls'], wd['beepers'])
-  except:
-    raise ValueError("Error interpreting world file.")
-  _world = w
-  _scene = _g.Canvas()
-  _scene.setWidth(50 * w.av)
-  _scene.setHeight(50 * w.st)
-  i = filename.rfind("/")
-  if i >= 0: filename = filename[i+1:]
-  _scene.setTitle("Robot World: " + filename)
-  _world.create_layer()
-  _scene.setAutoRefresh(False)
-
-def save_world(filename = None):
-  """Save a robot world to filename.
-  Opens file-chooser if no filename is given."""
-  if not filename:
-    filename = _easygui.filesavebox("Select a Robot world", 
-                                    "Robot World", '*', [ "*.wld" ])
-    if not filename: 
-      raise RuntimeError("No world file selected.")
-  out = open(filename, "w")
-  _world.save(out)
-  out.close()
-
-def edit_world():
-  """Edit the current robot world.
-  You can add and remove walls by clicking at the wall position.
-  Add a beeper by clicking with the left button at an intersection.
-  Remove a beeper with the right mouse button."""
-  while True:
-    e = _scene.wait()
-    d = e.getDescription()
-    if d == "canvas close":
-      _sys.exit(1)
-    if d == "keyboard" and e.getKey() in [ '\r', '\n' ]:
-      return
-    if d == "mouse click":
-      x = int(e.getMouseLocation().getX())
-      y = int(e.getMouseLocation().getY())
-      print ("Mouse button", e.getButton(), "at", (x, y))
-      col = (x - _world.left + _world.ts / 2) / _world.ts
-      row = (_world.bottom - y + _world.ts / 2) / _world.ts
-      if (col % 2) == 1 and (row % 2) == 1:
-        print ("corner")
-        # corner
-        av = (col + 1) / 2
-        st = (row + 1) / 2
-        if av < 1 or av > _world.av or st < 1 or st > _world.st:
-          continue
-        if e.getButton() == 1:
-          print ("add beeper")
-          _world.add_beeper(av, st)
-          _scene.refresh()
-        elif e.getButton() == 3:
-          print ("remove beeper")
-          _world.remove_beeper(av, st)
-          _scene.refresh()
-      elif ((col + row) % 2) == 1:
-        # wall position
-        print ("wall position")
-        if (col < 1 or col >= _world.num_cols - 1 or
-            row < 1 or row >= _world.num_rows - 1):
-          continue
-        _world.toggle_wall(col, row)
-        _world.update_layer()
-        _scene.refresh()
-  
-# --------------------------------------------------------------------
-
-class Robot(object):
-
-  def __init__(self, color = "gray", orientation = 'E', beepers = 0,
-               avenue = 1, street = 1):
-    """Create a new robot."""
-    if not color in _robot_images:
-      raise TypeError('color must be a color name')
-    self._image = [ None, None, None, None ]
-    for i in range(4):
-      self._image[i] = _g.Image("base64:" + _robot_images[color][i])
-      self._image[i].moveTo(-100, -100)
-      self._image[i].setDepth(0)
-      _scene.add(self._image[i])
-    self._dir = _orient_dict[orientation]
-    self._x = avenue
-    self._y = street
-    self._beeper_bag = beepers
-    self._trace = None
-    self._delay = 0
-    self._steps = 0
-    self._update_pos()
-    _scene.refresh()
-
-  def _update_pos(self):
-    x, y  = _world.cr2xy(2 * self._x - 1, 2 * self._y - 1)
-    self._image[self._dir].moveTo(x, y)
-
-  def _trace_pos(self):
-    x, y  = _world.cr2xy(2 * self._x - 1, 2 * self._y - 1)
-    xr, yr =  _directions[(self._dir - 1) % 4]
-    xb, yb =  _directions[(self._dir - 2) % 4]
-    return x + 5 * (xr + xb), y - 5 * (yr + yb)
-
-  def _update_trace(self):
-    if self._trace:
-      x, y = self._trace_pos()
-      self._trace.addPoint(_g.Point(x, y))
-
-  def _refresh(self):
-    _scene.refresh()
-      
-  def __del__(self):
-    if _scene:
-      for i in range(4):
-        _scene.remove(self._image[i])
-
-# --------------------------------------------------------------------
-
-  def set_trace(self, color = None):
-    """Without color argument, turn off tracing.
-With color argument, start a new trace in that color."""
-    if not color:
-      if self._trace:
-        _scene.remove(self._trace)
-      self._trace = None
-    else:
-      x, y  = self._trace_pos()
-      self._trace = _g.Path([_g.Point(x, y)])
-      self._trace.setBorderColor(color)
-      _scene.add(self._trace)
-
-  def set_pause(self, delay = 0):
-    """Set a pause to be made after each move."""
-    self._delay = delay
-
-# --------------------------------------------------------------------
-
-  def get_pos(self):
-    """Returns current robot position."""
-    return self._x, self._y
-
-  def turn_left(self):
-    """Rotate left by 90 degrees."""
-    self._image[self._dir].moveTo(-100, -100)
-    self._dir = (self._dir + 1) % 4
-    self._update_pos()
-    self._update_trace()
-    self._refresh()
-
-  def move(self):
-    """Move one street/avenue in direction where robot is facing."""
-    if self.front_is_clear():
-      xx, yy = _directions[self._dir]
-      self._x += xx
-      self._y += yy
-    else:
-      raise RobotError("That move really hurt!\n Please, make sure that " + 
-                       "there is no wall in front of me!""")
-    self._update_pos()
-    self._update_trace()
-    self._refresh()
-    if self._delay > 0:
-      _time.sleep(self._delay)
-    
-  def front_is_clear(self):
-    """Returns True if no wall or border in front of robot."""
-    col = 2 * self._x - 1
-    row = 2 * self._y - 1
-    xx, yy = _directions[self._dir]
-    return _world.is_clear(col + xx, row + yy)
-
-  def left_is_clear(self):
-    """Returns True if no walls or borders are to the immediate left
-    of the robot."""
-    col = 2 * self._x - 1
-    row = 2 * self._y - 1
-    xx, yy = _directions[(self._dir + 1) % 4]
-    return _world.is_clear(col + xx, row + yy)
-
-  def right_is_clear(self):
-    """Returns True if no walls or borders are to the immediate right
-    of the robot."""
-    col = 2 * self._x - 1
-    row = 2 * self._y - 1
-    xx, yy = _directions[(self._dir - 1) % 4]
-    return _world.is_clear(col + xx, row + yy)
-
-  def facing_north(self):
-    """Returns True if Robot is facing north."""
-    return (self._dir == 0)
-
-  def carries_beepers(self):
-    """Returns True if some beepers are left in Robot's bag."""
-    return (self._beeper_bag > 0)
-
-  def on_beeper(self):
-    """Returns True if beepers are present at current robot position."""
-    return ((self._x, self._y) in _world.beepers)
-
-  def pick_beeper(self):
-    """Robot picks one beeper up at current location."""
-    if self.on_beeper():
-      _world.remove_beeper(self._x, self._y)
-      self._refresh()
-      self._beeper_bag += 1
-    else:
-      raise RobotError("I must be on a beeper to pick it up.")
-
-  def drop_beeper(self):
-    """Robot drops one beeper down at current location."""
-    if self.carries_beepers():
-      self._beeper_bag -= 1
-      _world.add_beeper(self._x, self._y)
-      self._refresh()
-    else:
-      raise RobotError("I am not carrying any beepers.")
-
-# --------------------------------------------------------------------
-
-if __name__ == "__main__":
-  if len(_sys.argv) > 1:
-    load_world(_sys.argv[1])
-  else:
-    create_world(24, 14)
-  edit_world()
-  r = Robot("yellow")
-  r.set_trace("blue")
-  while True:
-    try:
-      e = _scene.wait()
-      d = e.getDescription()
-      if d == "canvas close":
-        break
-      if d == "keyboard":
-        k = e.getKey()
-        if k == "q":
-          _scene.close()
-          break
-        elif k == " ":
-          try:
-            r.move()
-          except:
-            _easygui.msgbox("OUCH!")
-        elif k == "t":
-          r.turn_left()
-        elif k == "w":
-          load_world()
-        elif k == "p":
-          r.pick_beeper()
-        elif k == "d":
-          r.drop_beeper()
-    except:
-      _easygui.exceptionbox()
-
-# --------------------------------------------------------------------
+#
+# cs1robots.py
+#
+# Environment for steering a robot through a grid world
+# for learning to program in Python
+#
+# Inspired by and using code from RUR-PLE by Andre Roberge
+#
+# 2010/01/14 Otfried Cheong
+# 2010/02/23: Changed to refresh only once after every move
+# 2010/02/24: Fixed refresh in world editing.
+# 2010/08/12: Improved handling of beepers to speed up.
+#
+# On Linux, need packages python-tk, python-imaging-tk
+#
+
+import sys as _sys
+import cs1graphics as _g
+import easygui as _easygui
+import re as _re
+import time as _time
+
+from cs1robots_images import _robot_images
+
+# PIL isn't actually used in cs1robots, but is needed to use
+# cs1graphics properly.  So we make sure it is there, as otherwise
+# users get a confusing error message.
+import PIL.Image as _Image
+import PIL.ImageDraw as _ImageDraw
+import PIL.ImageTk as _ImageTk
+
+#_g._debug = 2
+
+_scene = None
+_world = None
+
+_directions = [ (0, 1), (-1, 0), (0, -1), (1, 0) ]
+_orient_dict = { 'E': 3, 'S': 2, 'W': 1, 'N': 0}
+
+class RobotError(Exception):
+  def __init__(self, str):
+    Exception.__init__(self, str)
+
+def pause(delay = 1.0):
+  """Pause for delay seconds."""
+  _time.sleep(delay)
+
+# --------------------------------------------------------------------
+
+class _Beeper(object):
+  """One ore more beepers at a crossing in the world."""
+  def __init__(self, radius, av, st, num = 1):
+    self.av = av
+    self.st = st
+    self.num = num
+    self.layer = _g.Layer()
+    self.circle = _g.Circle(radius = radius)
+    self.text = _g.Text("%d" % num, 11, _g.Point(0, 0))
+    self.layer.add(self.circle)
+    self.layer.add(self.text)
+    self.circle.setFillColor("yellow")
+    self.circle.setBorderColor("orange")
+    self.circle.setDepth(10)
+    self.text.setDepth(5)
+    self.layer.setDepth(5)
+
+  def set_number(self, num):
+    self.num = num
+    self.text.setMessage("%d" % num)
+    
+class _World(object):
+  """This class defines the world's logic."""
+
+  def __init__(self, avenues = 10, streets = 10, walls = [], beepers = {}):
+    self.av = avenues
+    self.st = streets
+    self.num_cols = 2*avenues + 1
+    self.num_rows = 2*streets + 1
+    self.walls = walls
+    for (col, row) in self.walls:
+      if not (col+row) % 2:
+        raise RuntimeError("Wall in impossible position (%d, %d)." % (col,row))
+    self.beepers = beepers
+    self.borders = []
+    self.beeper_icons = {}
+    self.set_borders()
+
+  def cr2xy(self, col, row):
+    x = self.left + self.ts * col
+    y = self.bottom - self.ts * row
+    return x, y
+
+  def set_borders(self):
+    """The world is surrounded by a continuous wall.  This function
+       sets the corresponding "wall" or "border" based on the world's
+       dimensions."""
+    for col in range(1, self.num_cols-1, 2):
+      if (col, 0) not in self.borders:
+        self.borders.append( (col, 0) )
+      if (col, self.num_rows) not in self.borders:
+        self.borders.append( (col, self.num_rows-1) )
+      for row in range(1, self.num_rows-1, 2):
+        if (0, row) not in self.borders:
+          self.borders.append( (0, row) )
+        if (self.num_cols, row) not in self.borders:
+          self.borders.append( (self.num_cols-1, row) )
+
+  def toggle_wall(self, col, row):
+    """This function is intended for adding or removing a
+       wall from a GUI world editor."""
+    if (col+row) % 2 :  # safety check
+      if (col, row) in self.walls: # toggle value
+        self.walls.remove((col, row))
+      else:
+        self.walls.append((col, row))
+    else:
+      raise RuntimeError("Wall in impossible position (%d, %d)." % (col,row))
+
+  def is_clear(self, col, row):
+    """Returns True if there is no wall or border here."""
+    return not ((col, row) in self.walls or
+                (col, row) in self.borders)
+  
+  def add_beeper(self, av, st):
+    """Add a single beeper."""
+    assert self.layer
+    if (av, st) in self.beepers:
+      self.beepers[(av, st)] += 1
+      bp = self.beeper_icons[(av,st)]
+      bp.set_number(self.beepers[(av, st)])
+    else:
+      self.beepers[(av, st)] = 1
+      self._create_beeper(av, st)
+
+  def remove_beeper(self, av, st):
+    """Remove a beeper (does nothing if no beeper here)."""
+    assert self.layer
+    if (av, st) in self.beepers:
+      self.beepers[(av, st)] -= 1
+      if self.beepers[(av, st)] == 0:
+        del self.beepers[(av, st)]
+        self.layer.remove(self.beeper_icons[(av,st)].layer)
+        del self.beeper_icons[(av,st)]
+      else:
+        bp = self.beeper_icons[(av,st)]
+        bp.set_number(self.beepers[(av, st)])
+
+  def _create_beeper(self, av, st):
+    num = self.beepers[(av, st)]
+    bp = _Beeper(0.6 * self.ts, av, st, num)
+    x, y = self.cr2xy(2 * av - 1, 2 * st - 1)
+    bp.layer.moveTo(x, y)
+    self.beeper_icons[(av, st)] = bp
+    self.layer.add(bp.layer)
+
+  def create_layer(self):
+    # compute tilesize and border coordinates
+    w, h = _scene.getWidth(), _scene.getHeight()
+    tsx =  w / (self.num_cols + 2)
+    tsy =  h / (self.num_rows + 2)
+    self.ts = min(tsx, tsy)
+    self.left = 2 * self.ts
+    self.right = self.left + 2 * self.ts * self.av
+    self.bottom = h - 2 * self.ts
+    self.top = self.bottom - 2 * self.ts * self.st
+    self.layer = _g.Layer()
+    # Create avenues
+    for av in range(self.av):
+      x = self.left + self.ts * (2 * av + 1) 
+      l = _g.Path([_g.Point(x, self.top), _g.Point(x, self.bottom)])
+      l.setBorderColor("light gray")
+      self.layer.add(l)
+      self.layer.add(_g.Text("%d" % (av + 1), 10, 
+                             _g.Point(x, self.bottom + self.ts)))
+    # Create streets
+    for st in range(self.st):
+      y = self.bottom - self.ts * (2 * st + 1) 
+      l = _g.Path([_g.Point(self.left, y), _g.Point(self.right, y)])
+      l.setBorderColor("light gray")
+      self.layer.add(l)
+      self.layer.add(_g.Text("%d" % (st + 1), 10, 
+                             _g.Point(self.left - self.ts, y)))
+    # Create border
+    border = _g.Polygon(_g.Point(self.left, self.bottom),
+                        _g.Point(self.right, self.bottom),
+                        _g.Point(self.right, self.top),
+                        _g.Point(self.left, self.top))
+    border.setBorderWidth(5)
+    border.setBorderColor("dark red")
+    border.setDepth(10)
+    self.layer.add(border)
+    # Create walls
+    for (col, row) in self.walls:
+      if col % 2 == 0:  # vertical wall
+        x1, y1 = self.cr2xy(col, row - 1)
+        x2, y2 = self.cr2xy(col, row + 1)
+      else: # horizontal wall
+        x1, y1 = self.cr2xy(col - 1, row)
+        x2, y2 = self.cr2xy(col + 1, row)
+      w = _g.Path([_g.Point(x1,y1), _g.Point(x2,y2)])
+      w.setBorderWidth(5)
+      w.setBorderColor("dark red")
+      w.setDepth(10)
+      self.layer.add(w)
+    # Create beepers
+    for (av, st) in self.beepers:
+      self._create_beeper(av, st)
+    # Layer finished
+    _scene.add(self.layer)
+    
+  def update_layer(self):
+    _scene.remove(self.layer)
+    self.beeper_icons = {}
+    self.create_layer()
+
+  def save(self, out):
+    av_string = "avenues = " + str(self.av) + '\n'
+    st_string = "streets = " + str(self.st) + '\n'
+    if len(self.walls) > 0:
+      wall_string = "walls = [\n"
+      for item in self.walls:
+        wall_string += ("    " + str(item) + ', \n')
+      wall_string = wall_string[:-3] + '\n]\n'
+    else:
+      wall_string = "walls = []\n"
+    if len(self.beepers) > 0:
+      beeper_string = "beepers = {\n"
+      for key in self.beepers:
+        beeper_string += ("    " + str(key) + ': ' +
+                          str(self.beepers[key]) + ', \n')
+      beeper_string = beeper_string[:-3] + '\n}\n'
+    else:
+      beeper_string = "beepers = {}\n"
+    out.write(av_string + st_string + wall_string + beeper_string)
+    
+# --------------------------------------------------------------------
+
+def create_world(avenues = 10, streets = 10):
+  """Create an empty robot world."""
+  global _scene, _world
+  if _scene:
+    raise RuntimeError("A robot world already exists!")
+  _scene = _g.Canvas()
+  _scene.setWidth(50 * avenues)
+  _scene.setHeight(50 * streets)
+  _scene.setTitle("Robot World")
+  _world = _World(avenues, streets)
+  _world.create_layer()
+  _scene.setAutoRefresh(False)
+
+def _check_world(contents):
+  # safety check
+  safe = contents[:]
+    # only allow known keywords
+  keywords = ["avenues", "streets", "walls", "beepers", "robot",
+              "'s'", "'S'", '"s"', '"S"',
+              "'e'", "'E'", '"e"', '"E"',
+              "'w'", "'W'", '"w"', '"W"',
+              "'n'", "'N'", '"n"', '"N"', ]
+  for word in keywords:
+    safe = safe.replace(word, '')
+  safe = list(safe)
+  for char in safe:
+    if char.isalpha():
+      raise ValueError("Invalid word or character in world file")
+    
+def load_world(filename = None):
+  """Loads a robot world from filename.
+  Opens file-chooser if no filename is given."""
+  global _scene, _world
+  if _scene:
+    raise RuntimeError("A robot world already exists!")
+  if not filename:
+    filename = _easygui.fileopenbox("Select a Robot world", 
+                                    "Robot World", '*', [ "*.wld" ])
+    if not filename: 
+      raise RuntimeError("No world file selected.")
+  txt = open(filename, 'rb').read()
+  txt = _re.sub('\r\n', '\n', txt) # Windows
+  txt = _re.sub('\r', '\n', txt)  # Mac
+  _check_world(txt)
+  wd = {}
+  # extracts avenues, streets, walls and beepers
+  try:
+    exec (txt in wd)
+    w = _World(wd['avenues'], wd['streets'], wd['walls'], wd['beepers'])
+  except:
+    raise ValueError("Error interpreting world file.")
+  _world = w
+  _scene = _g.Canvas()
+  _scene.setWidth(50 * w.av)
+  _scene.setHeight(50 * w.st)
+  i = filename.rfind("/")
+  if i >= 0: filename = filename[i+1:]
+  _scene.setTitle("Robot World: " + filename)
+  _world.create_layer()
+  _scene.setAutoRefresh(False)
+
+def save_world(filename = None):
+  """Save a robot world to filename.
+  Opens file-chooser if no filename is given."""
+  if not filename:
+    filename = _easygui.filesavebox("Select a Robot world", 
+                                    "Robot World", '*', [ "*.wld" ])
+    if not filename: 
+      raise RuntimeError("No world file selected.")
+  out = open(filename, "w")
+  _world.save(out)
+  out.close()
+
+def edit_world():
+  """Edit the current robot world.
+  You can add and remove walls by clicking at the wall position.
+  Add a beeper by clicking with the left button at an intersection.
+  Remove a beeper with the right mouse button."""
+  while True:
+    e = _scene.wait()
+    d = e.getDescription()
+    if d == "canvas close":
+      _sys.exit(1)
+    if d == "keyboard" and e.getKey() in [ '\r', '\n' ]:
+      return
+    if d == "mouse click":
+      x = int(e.getMouseLocation().getX())
+      y = int(e.getMouseLocation().getY())
+      print ("Mouse button", e.getButton(), "at", (x, y))
+      col = (x - _world.left + _world.ts / 2) / _world.ts
+      row = (_world.bottom - y + _world.ts / 2) / _world.ts
+      if (col % 2) == 1 and (row % 2) == 1:
+        print ("corner")
+        # corner
+        av = (col + 1) / 2
+        st = (row + 1) / 2
+        if av < 1 or av > _world.av or st < 1 or st > _world.st:
+          continue
+        if e.getButton() == 1:
+          print ("add beeper")
+          _world.add_beeper(av, st)
+          _scene.refresh()
+        elif e.getButton() == 3:
+          print ("remove beeper")
+          _world.remove_beeper(av, st)
+          _scene.refresh()
+      elif ((col + row) % 2) == 1:
+        # wall position
+        print ("wall position")
+        if (col < 1 or col >= _world.num_cols - 1 or
+            row < 1 or row >= _world.num_rows - 1):
+          continue
+        _world.toggle_wall(col, row)
+        _world.update_layer()
+        _scene.refresh()
+  
+# --------------------------------------------------------------------
+
+class Robot(object):
+
+  def __init__(self, color = "gray", orientation = 'E', beepers = 0,
+               avenue = 1, street = 1):
+    """Create a new robot."""
+    if not color in _robot_images:
+      raise TypeError('color must be a color name')
+    self._image = [ None, None, None, None ]
+    for i in range(4):
+      self._image[i] = _g.Image("base64:" + _robot_images[color][i])
+      self._image[i].moveTo(-100, -100)
+      self._image[i].setDepth(0)
+      _scene.add(self._image[i])
+    self._dir = _orient_dict[orientation]
+    self._x = avenue
+    self._y = street
+    self._beeper_bag = beepers
+    self._trace = None
+    self._delay = 0
+    self._steps = 0
+    self._update_pos()
+    _scene.refresh()
+
+  def _update_pos(self):
+    x, y  = _world.cr2xy(2 * self._x - 1, 2 * self._y - 1)
+    self._image[self._dir].moveTo(x, y)
+
+  def _trace_pos(self):
+    x, y  = _world.cr2xy(2 * self._x - 1, 2 * self._y - 1)
+    xr, yr =  _directions[(self._dir - 1) % 4]
+    xb, yb =  _directions[(self._dir - 2) % 4]
+    return x + 5 * (xr + xb), y - 5 * (yr + yb)
+
+  def _update_trace(self):
+    if self._trace:
+      x, y = self._trace_pos()
+      self._trace.addPoint(_g.Point(x, y))
+
+  def _refresh(self):
+    _scene.refresh()
+      
+  def __del__(self):
+    if _scene:
+      for i in range(4):
+        _scene.remove(self._image[i])
+
+# --------------------------------------------------------------------
+
+  def set_trace(self, color = None):
+    """Without color argument, turn off tracing.
+With color argument, start a new trace in that color."""
+    if not color:
+      if self._trace:
+        _scene.remove(self._trace)
+      self._trace = None
+    else:
+      x, y  = self._trace_pos()
+      self._trace = _g.Path([_g.Point(x, y)])
+      self._trace.setBorderColor(color)
+      _scene.add(self._trace)
+
+  def set_pause(self, delay = 0):
+    """Set a pause to be made after each move."""
+    self._delay = delay
+
+# --------------------------------------------------------------------
+
+  def get_pos(self):
+    """Returns current robot position."""
+    return self._x, self._y
+
+  def turn_left(self):
+    """Rotate left by 90 degrees."""
+    self._image[self._dir].moveTo(-100, -100)
+    self._dir = (self._dir + 1) % 4
+    self._update_pos()
+    self._update_trace()
+    self._refresh()
+
+  def move(self):
+    """Move one street/avenue in direction where robot is facing."""
+    if self.front_is_clear():
+      xx, yy = _directions[self._dir]
+      self._x += xx
+      self._y += yy
+    else:
+      raise RobotError("That move really hurt!\n Please, make sure that " + 
+                       "there is no wall in front of me!""")
+    self._update_pos()
+    self._update_trace()
+    self._refresh()
+    if self._delay > 0:
+      _time.sleep(self._delay)
+    
+  def front_is_clear(self):
+    """Returns True if no wall or border in front of robot."""
+    col = 2 * self._x - 1
+    row = 2 * self._y - 1
+    xx, yy = _directions[self._dir]
+    return _world.is_clear(col + xx, row + yy)
+
+  def left_is_clear(self):
+    """Returns True if no walls or borders are to the immediate left
+    of the robot."""
+    col = 2 * self._x - 1
+    row = 2 * self._y - 1
+    xx, yy = _directions[(self._dir + 1) % 4]
+    return _world.is_clear(col + xx, row + yy)
+
+  def right_is_clear(self):
+    """Returns True if no walls or borders are to the immediate right
+    of the robot."""
+    col = 2 * self._x - 1
+    row = 2 * self._y - 1
+    xx, yy = _directions[(self._dir - 1) % 4]
+    return _world.is_clear(col + xx, row + yy)
+
+  def facing_north(self):
+    """Returns True if Robot is facing north."""
+    return (self._dir == 0)
+
+  def carries_beepers(self):
+    """Returns True if some beepers are left in Robot's bag."""
+    return (self._beeper_bag > 0)
+
+  def on_beeper(self):
+    """Returns True if beepers are present at current robot position."""
+    return ((self._x, self._y) in _world.beepers)
+
+  def pick_beeper(self):
+    """Robot picks one beeper up at current location."""
+    if self.on_beeper():
+      _world.remove_beeper(self._x, self._y)
+      self._refresh()
+      self._beeper_bag += 1
+    else:
+      raise RobotError("I must be on a beeper to pick it up.")
+
+  def drop_beeper(self):
+    """Robot drops one beeper down at current location."""
+    if self.carries_beepers():
+      self._beeper_bag -= 1
+      _world.add_beeper(self._x, self._y)
+      self._refresh()
+    else:
+      raise RobotError("I am not carrying any beepers.")
+
+# --------------------------------------------------------------------
+
+if __name__ == "__main__":
+  if len(_sys.argv) > 1:
+    load_world(_sys.argv[1])
+  else:
+    create_world(24, 14)
+  edit_world()
+  r = Robot("yellow")
+  r.set_trace("blue")
+  while True:
+    try:
+      e = _scene.wait()
+      d = e.getDescription()
+      if d == "canvas close":
+        break
+      if d == "keyboard":
+        k = e.getKey()
+        if k == "q":
+          _scene.close()
+          break
+        elif k == " ":
+          try:
+            r.move()
+          except:
+            _easygui.msgbox("OUCH!")
+        elif k == "t":
+          r.turn_left()
+        elif k == "w":
+          load_world()
+        elif k == "p":
+          r.pick_beeper()
+        elif k == "d":
+          r.drop_beeper()
+    except:
+      _easygui.exceptionbox()
+
+# --------------------------------------------------------------------
```

### Comparing `cs1-robots-0.1.6/src/cs1robots_images/__init__.py` & `cs1-robots-0.1.6.2/src/cs1robots_images/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,30 @@
-_robot_images = {
-  "gray" : [ "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",  ],
-  "blue" : [ "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",  ],
-  "green" : [ "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",  ],
-  "light_blue" : [ "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",  ],
-  "purple" : [ "iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEURAAJLHjtwQ1+Xa4f//wDFl7XYrMr////XBGfUxJj////UxJPXZEgpBZQBCMsAAIA8CTgAACQAAAGhoaIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5+jxWDYBCMs8CTgAAIDUhLLUhr4BCMsAADkS6CTY57IpBZQBCMspBZQ8CTgAABgAAALaFogAABUS6HzXOZU8CUgpBZS1WqAS6GAS6QG2L+RFNyApBZQAAIAAAAFPyjgS6OS1WqC1VShP0RYAAABPyji1WqAS6OS1RBxP7jPXNnrY5zIAAAAAAAEAAAAAAADUi9kS6NxBx0G1DExCx4VCx43LD8i1DGxFM5sS6NxFM7JFM7oS6XhFM8QS6NwS6VzLD8jLD8i1WqAS6PRCWLYABAEAAADAWqAAAAES6SDUhzQRBWIABAEAAADAWqDLD8i6q80AAAAS6VwS6TjUtqPUhPzUhaQlBV4AAAEWIagWIcgABAAWX8gAAADUtik94ZERBWIS6fAAAAAWX8g94ZwAAAAAAAAABAAAABMAAAAS6fzXBGfUiDD////UiCrUuJsAAADLD8gRBWIABAEAAADAWqB/zwQAAAEAAAAAAAAAAAAAAACKACEABADV8+N/zvB/a8gAAAAAAAQAAaYAAAIABAAAABMWIcgBCMsAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5TiAFjwAAAUAAAXcAqSAGByAGKzcArAArugS6sA97BsWX8gAAAAWIUgAAAQAAAAS6yg95ZgAAAAS6ojUhzQS6oDUtqPUhPzUhaQlBV4AAAEAAAAWX8gWIUglBQES6pTUwr8S6sQ90ZMlBV495ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS6uzUhzQRBWIAAA8AAAAAAAA95Zi6q80AAAAS6yg95ZgS61TUi9n94AAS61TUiFoS6xTUiCoAAA895ZgS7iwAABQAAAEAAAAAAAAAABAAAAApBZQAAAEAAAAAAAAS6wjxbGQS7fzXBGfUiDD////UiCoRAAIRAAJWkx99AAAACHRSTlP/////////AN6DvVkAAACXSURBVHjaxZLhCoQwDIOzbl7f/41vSdsx0RP8dWNg+YhtUoU7LmeySVuzvs5xfAzEzTYqnrifjjDuMF7iH70f8L3BU5yecRhz03Mgw1+X4rEThHaMkMseWr49dDXTKLWixXvERGpTXxNQHeLCF96bCNONra6DTrx8WzUE/SWmXM9ZhfhPGGlQVSxQOJaFyKVPmer6IVf1BTTtCE84csDNAAAAAElFTkSuQmCC",
-  "iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEURAAJIGjlxRWL/AACXa4e8j6vYrMr////XBGfUxJj////UxJPXZEgKBnwBCaoAAICp79AAACQAAAGhoaIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5+jxWDYBCaqp79AAAIDUhLLUhr4BCaoAADkS6CTY57IKBnwBCaoKBnyp79AAABgAAALaFogAABUS6HzXOZWp7+AKBny1WqAS6GAS6QG2L+RFNyAKBnwAAIAAAAFPyjgS6OS1WqC1VShP0RYAAABPyji1WqAS6OS1RBxP7jPXNnrY5zIAAAAAAAEAAAAAAADUi9kS6NxBx0G1DExCx4VCx43LD8i1DGxFM5sS6NxFM7JFM7oS6XhFM8QS6NwS6VzLD8jLD8i1WqAS6PRCWLYABAEAAADBiwAAAAES6SDUhzQRBWIABAEAAADBiwDLD8i6q80AAAAS6VwS6TjUtqPUhPzUhaQlBV4AAAEWIagWIcgABAAWX8gAAADUtik94ZERBWIS6fAAAAAWX8g94ZwAAAAAAAAABAAAABMAAAAS6fzXBGfUiDD////UiCrUuJsAAADLD8gRBWIABAEAAADBiwB/zwQAAAEAAAAAAAAAAAAAAACKACEABADV8+N/zvB/a8gAAAAAAAQAAaYAAAIABAAAABMWIcgBCaoAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5TiAFjwAAAUAAAXcAqSAGByAGKzcArAArugS6sA97BsWX8gAAAAWIUgAAAQAAAAS6yg95ZgAAAAS6ojUhzQS6oDUtqPUhPzUhaQlBV4AAAEAAAAWX8gWIUglBQES6pTUwr8S6sQ90ZMlBV495ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS6uzUhzQRBWIAAA8AAAAAAAA95Zi6q80AAAAS6yg95ZgS61TUi9n94AAS61TUiFoS6xTUiCoAAA895ZgS7iwAABQAAAEAAAAAAAAAABAAAAAKBnwAAAEAAAAAAAAS6wjxbGQS7fzXBGfUiDD////UiCoRAAIRAAIpItfNAAAACHRSTlP/////////AN6DvVkAAAB9SURBVHjardBBDsAgCATABaX8/8dFjBWVHpqUk5kAAlBVbMFGTYm4jhC5mBWlLOqOzlHNN2bIw9Z7ZiNlTpmRZ4cv37h8Yk23zG7ifFwQfsEWVtB2hDfWwLVzlY2tOOV+qiQbJ9PcJfAy3sP+HKn/cv/rZIrTbSx5kzG0xQ39dAqxz8DMUwAAAABJRU5ErkJggg==",
-  "iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEURAAJNIDxxRWL/AACXa4f//wC7jqrYrMr////UxJj////UxJPXZEgYBZYBCpwAAICp61gAACQAAAGhoaIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5+jxWDYBCpyp61gAAIDUhLLUhr4BCpwAADkS6CTY57IYBZYBCpwYBZap61gAABgAAALaFogAABUS6HzXOZWp62gYBZa1WqAS6GAS6QG2L+RFNyAYBZYAAIAAAAFPyjgS6OS1WqC1VShP0RYAAABPyji1WqAS6OS1RBxP7jPXNnrY5zIAAAAAAAEAAAAAAADUi9kS6NxBx0G1DExCx4VCx43LD8i1DGxFM5sS6NxFM7JFM7oS6XhFM8QS6NwS6VzLD8jLD8i1WqAS6PRCWLYABAEAAADBiuwAAAES6SDUhzQRBWIABAEAAADBiuzLD8i6q80AAAAS6VwS6TjUtqPUhPzUhaQlBV4AAAEWIagWIcgABAAWX8gAAADUtik94ZERBWIS6fAAAAAWX8g94ZwAAAAAAAAABAAAABMAAAAS6fzXBGfUiDD////UiCrUuJsAAADLD8gRBWIABAEAAADBiux/zwQAAAEAAAAAAAAAAAAAAACKACEABADV8+N/zvB/a8gAAAAAAAQAAaYAAAIABAAAABMWIcgBCpwAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5TiAFjwAAAUAAAXcAqSAGByAGKzcArAArugS6sA97BsWX8gAAAAWIUgAAAQAAAAS6yg95ZgAAAAS6ojUhzQS6oDUtqPUhPzUhaQlBV4AAAEAAAAWX8gWIUglBQES6pTUwr8S6sQ90ZMlBV495ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS6uzUhzQRBWIAAA8AAAAAAAA95Zi6q80AAAAS6yg95ZgS61TUi9n94AAS61TUiFoS6xTUiCoAAA895ZgS7iwAABQAAAEAAAAAAAAAABAAAAAYBZYAAAEAAAAAAAAS6wjxbGQS7fzXBGfUiDD////UiCoRAAIRAAKVOkYIAAAACXRSTlP//////////wBTT3gSAAAAnklEQVR42sWSSxLEIAhEW0TD/U88fKMp3Q+L2HlFoMFABEcoE7RGvMV8CI6Je09mYj6B9SW5C8e44eb4KGLx7ZhYbjha3jFFr56dN3yOox53PmcMfy5FfCffbNbs5pB4LDq0DNU0Y9F3TCxuR3VAgXhANmwoPnFsbsLJGOlEyjdVQfBEYUv3U1Uk/wkjDboyg7HvvB7kXHZnmV0/5Kt+a7kJ+cUredMAAAAASUVORK5CYII=",
-  "iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEURAAJIGjlxRWL/AACXa4e8j6vYrMr////XBGfUxJj////UxJPXZEgfBbgBCpwAAIA8CTgAACQAAAGhoaIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5+jxWDYBCpw8CTgAAIDUhLLUhr4BCpwAADkS6CTY57IfBbgBCpwfBbg8CTgAABgAAALaFogAABUS6HzXOZU8CUgfBbi1WqAS6GAS6QG2L+RFNyAfBbgAAIAAAAFPyjgS6OS1WqC1VShP0RYAAABPyji1WqAS6OS1RBxP7jPXNnrY5zIAAAAAAAEAAAAAAADUi9kS6NxBx0G1DExCx4VCx43LD8i1DGxFM5sS6NxFM7JFM7oS6XhFM8QS6NwS6VzLD8jLD8i1WqAS6PRCWLYABAEAAADB5pAAAAES6SDUhzQRBWIABAEAAADB5pDLD8i6q80AAAAS6VwS6TjUtqPUhPzUhaQlBV4AAAEWIagWIcgABAAWX8gAAADUtik94ZERBWIS6fAAAAAWX8g94ZwAAAAAAAAABAAAABMAAAAS6fzXBGfUiDD////UiCrUuJsAAADLD8gRBWIABAEAAADB5pB/zwQAAAEAAAAAAAAAAAAAAACKACEABADV8+N/zvB/a8gAAAAAAAQAAaYAAAIABAAAABMWIcgBCpwAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5TiAFjwAAAUAAAXcAqSAGByAGKzcArAArugS6sA97BsWX8gAAAAWIUgAAAQAAAAS6yg95ZgAAAAS6ojUhzQS6oDUtqPUhPzUhaQlBV4AAAEAAAAWX8gWIUglBQES6pTUwr8S6sQ90ZMlBV495ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS6uzUhzQRBWIAAA8AAAAAAAA95Zi6q80AAAAS6yg95ZgS61TUi9n94AAS61TUiFoS6xTUiCoAAA895ZgS7iwAABQAAAEAAAAAAAAAABAAAAAfBbgAAAEAAAAAAAAS6wjxbGQS7fzXBGfUiDD////UiCoRAAIRAAK3In3PAAAACHRSTlP/////////AN6DvVkAAAB4SURBVHjardBBDsAgCARAiij//3FBi6JS00NJ9DAhKwjMsBaLiV6IZJVLURf22jylykSTe0bIEYPrfrIr55hdiGOKQz5wOvK65eFPXn5QL4kH3bMGcGekxhQxQMR6doa92zZanpynM7YZudf/PN70TGN7xxjxPPgN+sEKkg2MzBYAAAAASUVORK5CYII=",  ],
-  "yellow" : [ "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",  ], }
+_robot_images = {
+    "gray": ["iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEUAAAA1NTVZWVn//wCAgICsrKzAwMD////XBGfUxJj////UxJPXZEgLBoIBC/EAAICp+MAAACQAAAGhoaIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5+jxWDYBC/Gp+MAAAIDUhLLUhr4BC/EAADkS6CTY57ILBoIBC/ELBoKp+MAAABgAAALaFogAABUS6HzXOZWp+NALBoK1WqAS6GAS6QG2L+RFNyALBoIAAIAAAAFPyjgS6OS1WqC1VShP0RYAAABPyji1WqAS6OS1RBxP7jPXNnrY5zIAAAAAAAEAAAAAAADUi9kS6NxBx0G1DExCx4VCx43LD8i1DGxFM5sS6NxFM7JFM7oS6XhFM8QS6NwS6VzLD8jLD8i1WqAS6PRCWLYABAEAAADBLUQAAAES6SDUhzQRBWIABAEAAADBLUTLD8i6q80AAAAS6VwS6TjUtqPUhPzUhaQlBV4AAAEWIagWIcgABAAWX8gAAADUtik94ZERBWIS6fAAAAAWX8g94ZwAAAAAAAAABAAAABMAAAAS6fzXBGfUiDD////UiCrUuJsAAADLD8gRBWIABAEAAADBLUR/zwQAAAEAAAAAAAAAAAAAAACKACEABADV8+N/zvB/a8gAAAAAAAQAAaYAAAIABAAAABMWIcgBC/EAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5TiAFjwAAAUAAAXcAqSAGByAGKzcArAArugS6sA97BsWX8gAAAAWIUgAAAQAAAAS6yg95ZgAAAAS6ojUhzQS6oDUtqPUhPzUhaQlBV4AAAEAAAAWX8gWIUglBQES6pTUwr8S6sQ90ZMlBV495ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS6uzUhzQRBWIAAA8AAAAAAAA95Zi6q80AAAAS6yg95ZgS61TUi9n94AAS61TUiFoS6xTUiCoAAA895ZgS7iwAABQAAAEAAAAAAAAAABAAAAALBoIAAAEAAAAAAAAS6wjxbGQS7fzXBGfUiDD////UiCoAAAAAAABePXMrAAAACHRSTlP/////////AN6DvVkAAACXSURBVHjaxZLhCoQwDIOzbl7f/41vSdsx0RP8dWNg+YhtUoU7LmeySVuzsc5xfAzEzTYqnnicjjDuMF7iH70f8L3BU5yRcRhz03Mgw1+X4rEThLb3kMseWr7ddTXTKLWixUfERGpTXxNQHeLCF96bCNONra6dTrx8WzUE/SWmXM9ZhfhPGGlQVSxQOJaFyKVPmer6IVf1BbCqCS9jk1GTAAAAAElFTkSuQmCC",
+             "iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEUAAAAzMzNbW1v/AACAgICkpKTAwMD////XBGfUxJj////UxJPXZEgQCQABCJgAAICpsbAAACQAAAGhoaIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5+jxWDYBCJipsbAAAIDUhLLUhr4BCJgAADkS6CTY57IQCQABCJgQCQCpsbAAABgAAALaFogAABUS6HzXOZWpscAQCQC1WqAS6GAS6QG2L+RFNyAQCQAAAIAAAAFPyjgS6OS1WqC1VShP0RYAAABPyji1WqAS6OS1RBxP7jPXNnrY5zIAAAAAAAEAAAAAAADUi9kS6NxBx0G1DExCx4VCx43LD8i1DGxFM5sS6NxFM7JFM7oS6XhFM8QS6NwS6VzLD8jLD8i1WqAS6PRCWLYABAEAAAC7q7gAAAES6SDUhzQMCQgABAEAAAC7q7jLD8i6q80AAAAS6VwS6TjUtqPUhPzUhaQXAywAAAEWIhgWIjgABAAWYDgAAADUtik94ZEMCQgS6fAAAAAWYDg94ZwAAAAAAAAABAAAABMAAAAS6fzXBGfUiDD////UiCrUuJsAAADLD8gMCQgABAEAAAC7q7h/uXwAAAEAAAAAAAAAAAAAAACKACEABADV8+N/uWh/mfgAAAAAAAQAAaYAAAIABAAAABMWIjgBEtkAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5TiAFjwAAAUAAAUj8qSAGByAGKwj8rAAc0YS6sA97BsWYDgAAAAWIbgAAAQAAAAS6yg95ZgAAAAS6ojUhzQS6oDUtqPUhPzUhaQXAywAAAEAAAAWYDgWIbgXAwES6pTUwr8S6sQ90ZMXAyw95ZgWYDjUiKYAAAAAAAIAAMgAABMWIcAS6uzUhzQMCQgAAA8AAAAAAAA95Zi6q80AAAAS6yg95ZgS61TUi9n98AAS61TUiFoS6xTUiCoAAA895ZgS7iwAABQAAAEAAAAAAAAAABAAAAAQCQAAAAEAAAAAAAAS6wjxbGQS7fzXBGfUiDD////UiCoAAAAAAAAQ6+rlAAAACHRSTlP/////////AN6DvVkAAAB9SURBVHjardBBDsAgCATABaX8/8dFjBWVHpqUk5kAAlBVbMFGTYm4jhC5mBWlLOqOzlHNN2bIw9Z7ZiNlTpmRZ4cv37h8Yk23zG7ifFwQfsEWVtB2hDfWwLVzlY2tOOV+qiQbJ9PcJfAy3sP+HKn/cv/rZIrTbSx5kzG0xQ39dAqxz8DMUwAAAABJRU5ErkJggg==",
+             "iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEUAAAA3NzdbW1v/AAD//wCAgICjo6PAwMD///8S8uhyd1MAAAABELAAADYAAAAAAFAAABkAAAGFBoMAAAkAADYAAAAAAFAAABkAAAAAAAAAABQAABcAAAkAAAQAAAQAAAQAAATxogDxoeQBELAAADkAAAMAABMAABMBDy0AAAAAACYFESAAAAAAACaqAAD///8V5iAV5hgS9XC1WqAS85wBEAG2L+RFNyAAABMAABMBDy1PyjgS9CC1WqC1VShP0RYAAABPyji1WqAS9CC1RBxP7jMAAAIBELAAADkAAAMAABMAABMV5iAS9BhBx0G1DExCx4VCx43LD8i1DGxFM5sS9BhFM7JFM7oS9LRFM8QS9BgS9JjLD8jLD8i1WqAS9DBCWLYABAEAAADA+CAAAAES9FzUhzQRBWIABAEAAADA+CDLD8i6q80AAAAS9JgS9HTUtqPUhPzUhaQlBV4AAAEWIagWIcgABAAWX8gAAADUtik94ZERBWIS9SwAAAAWX8g94ZwAAAAAAAAABAAAABMS9RAS9TjXBGfUiDD////UiCrUuJsAAADLD8gRBWIABAEAAADA+CB/zwQAAAEAAAAAAAAAAAAAAACKACEABADV8+N/zvB/a8gAAAAAAAQAAaYAAAIABAAAABMWIcgBCrEAAAAAAAAAAAAAAAAAAAAAAAAAAAAS8HSAFjwAAAUAAAXcCFSAGByAGKzcCGAArugS9fw97BsWX8gAAAAWIUgAAAQAAAAS9mQ95ZgAAADXIloAAAAS9bzUtqPUhPzUhaQlBV4AAAEAAAAWX8gWIUglBQES9dDUwr8S9gA90ZMlBV495ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS9ijUhzQRBWIAAA8AAAAAAAA95Zi6q80AAAAS9mQ95ZgS9pDUi9n94AAS9pDUiFoS9lDUiCoAAA895ZgS+WgAABQAAAEAAAAAAAAAABAAAAAAAFAAAAEAAAAAAAAS9kTxbGQS+TjXBGfUiDD////UiCoAAAAAAAAJXRdjAAAACXRSTlP//////////wBTT3gSAAAAnklEQVR42sWSSxLEIAhEW0TD/U88fKMp3Q+L2HlFoMFABEcoE7RGY4v5EBzT6D2ZifkE1pfkLhzjhpvjo4jFt2NiueFoeccUvXp23vA5jnrc+Zwx/LkU8Z18s4dmN4c0eFHWMlTT8KLvmFjcjuqAAvGAbNhQfOLY3IQT5nQi5ZuqIMZEYUv3U1Uk/wkjDboyg7HvvB7kXHZnmV0/5Kt+x38Kzw6IUBEAAAAASUVORK5CYII=",
+             "iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEUAAAAzMzNbW1v/AACAgICkpKTAwMD///8AAAAS8uhyd1MAAAABD3UAADYAAAAAAFAAABkAAAGFBJ4AAAkAADYAAAAAAFAAABkAAAAAAAAAABQAABcAAAkAAAQAAAQAAAQAAATxogDxoeQBD3UAADkAAAMAABMAABMBDusAAAAAACYFDpQAAAAAACaqAAD///8V5iAV5hgS9XC1WqAS85wBDwG2L+RFNyAAABMAABMBDutPyjgS9CC1WqC1VShP0RYAAABPyji1WqAS9CC1RBxP7jMAAAIBD3UAADkAAAMAABMAABMV5iAS9BhBx0G1DExCx4VCx43LD8i1DGxFM5sS9BhFM7JFM7oS9LRFM8QS9BgS9JjLD8jLD8i1WqAS9DBCWLYABAEAAAC6Z1AAAAES9FzUhzRTBRAABAEAAAC6Z1DLD8i6q80AAAAS9JgS9HTUtqPUhPzUhaQDBRoAAAEWIagWIcgABAAWX8gAAADUtik94ZFTBRAS9SwAAAAWX8g94ZwAAAAAAAAABAAAABMS9RAS9TjXBGfUiDD////UiCrUuJsAAADLD8hTBRAABAEAAAC6Z1B+cqwAAAEAAAAAAAAAAAAAAACKACEABADV8+N+cph+8XAAAAAAAAQAAaYAAAIABAAAABMWIcgBCJ4AAAAAAAAAAAAAAAAAAAAAAAAAAAAS8HSAFjwAAAUAAAVI2FSAGByAGKxI2GAAb1oS9fw97BsWX8gAAAAWIUgAAAQAAAAS9mQ95ZgAAADXIloAAAAS9bzUtqPUhPzUhaQDBRoAAAEAAAAWX8gWIUgDBQES9dDUwr8S9gA90ZMDBRo95ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS9ijUhzRTBRAAAA8AAAAAAAA95Zi6q80AAAAS9mQ95ZgS9pDUi9n90AAS9pDUiFoS9lDUiCoAAA895ZgS+WgAABQAAAEAAAAAAAAAABAAAAAAAFAAAAEAAAAAAAAS9kTxbGQS+TjXBGfUiDD////UiCoAAAAAAADKTwNHAAAACHRSTlP/////////AN6DvVkAAAB6SURBVHjardCLCsAgCAXQO7P8/z+eyVxWEgzmKNghfEEES5CoqV5E7FFbIzKOao5SjJknj0yoGbt2fnKfOCQJHEt+43Lkdcp8J8bbBmEb7Jemh35cq/07axJjzhjIuJ+dsb/2iZaSc3fO3qO88T+PmpF5TB+YMp4bvwEGcAqR53QgIgAAAABJRU5ErkJggg==", ],
+    "blue": ["iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEUAACMbHUdAQm5qbZX//wCZmsausdr////XBGfUxJj////UxJPXZEgdBeQBCsMAAICpXoAAACQAAAGhoaIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5+jxWDYBCsOpXoAAAIDUhLLUhr4BCsMAADkS6CTY57IdBeQBCsMdBeSpXoAAABgAAALaFogAABUS6HzXOZWpXpAdBeS1WqAS6GAS6QG2L+RFNyAdBeQAAIAAAAFPyjgS6OS1WqC1VShP0RYAAABPyji1WqAS6OS1RBxP7jPXNnrY5zIAAAAAAAEAAAAAAADUi9kS6NxBx0G1DExCx4VCx43LD8i1DGxFM5sS6NxFM7JFM7oS6XhFM8QS6NwS6VzLD8jLD8i1WqAS6PRCWLYABAEAAAC9VJgAAAES6SDUhzQRBWIABAEAAAC9VJjLD8i6q80AAAAS6VwS6TjUtqPUhPzUhaQlBV4AAAEWIagWIcgABAAWX8gAAADUtik94ZERBWIS6fAAAAAWX8g94ZwAAAAAAAAABAAAABMAAAAS6fzXBGfUiDD////UiCrUuJsAAADLD8gRBWIABAEAAAC9VJh/zwQAAAEAAAAAAAAAAAAAAACKACEABADV8+N/zvB/a8gAAAAAAAQAAaYAAAIABAAAABMWIcgBCsMAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5TiAFjwAAAUAAAXcAqSAGByAGKzcArAArugS6sA97BsWX8gAAAAWIUgAAAQAAAAS6yg95ZgAAAAS6ojUhzQS6oDUtqPUhPzUhaQlBV4AAAEAAAAWX8gWIUglBQES6pTUwr8S6sQ90ZMlBV495ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS6uzUhzQRBWIAAA8AAAAAAAA95Zi6q80AAAAS6yg95ZgS61TUi9n94AAS61TUiFoS6xTUiCoAAA895ZgS7iwAABQAAAEAAAAAAAAAABAAAAAdBeQAAAEAAAAAAAAS6wjxbGQS7fzXBGfUiDD////UiCoAACMAACNcr9aKAAAACHRSTlP/////////AN6DvVkAAACXSURBVHjaxZLhCoQwDIOzbl7f/41vSdsx0RP8dWNg+YhtUoU7LmeySVuzvs5xfAzEzTYqnrifjjDuMF7iH70f8L3BU5yecRhz03Mgw1+X4rEThHaMkMseWr49dDXTKLWixXvERGpTXxNQHeLCF96bCNONra6DTrx8WzUE/SWmXM9ZhfhPGGlQVSxQOJaFyKVPmer6IVf1BTTtCE84csDNAAAAAElFTkSuQmCC",
+             "iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEUAACgWGERGSHJtbpn/AACVlr+ys9/////XBGfUxJj////UxJPXZEgNBggBC/EAAICpyvgAACQAAAGhoaIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5+jxWDYBC/GpyvgAAIDUhLLUhr4BC/EAADkS6CTY57INBggBC/ENBgipyvgAABgAAALaFogAABUS6HzXOZWpywgNBgi1WqAS6GAS6QG2L+RFNyANBggAAIAAAAFPyjgS6OS1WqC1VShP0RYAAABPyji1WqAS6OS1RBxP7jPXNnrY5zIAAAAAAAEAAAAAAADUi9kS6NxBx0G1DExCx4VCx43LD8i1DGxFM5sS6NxFM7JFM7oS6XhFM8QS6NwS6VzLD8jLD8i1WqAS6PRCWLYABAEAAAC9jkAAAAES6SDUhzQRBWIABAEAAAC9jkDLD8i6q80AAAAS6VwS6TjUtqPUhPzUhaQlBV4AAAEWIagWIcgABAAWX8gAAADUtik94ZERBWIS6fAAAAAWX8g94ZwAAAAAAAAABAAAABMAAAAS6fzXBGfUiDD////UiCrUuJsAAADLD8gRBWIABAEAAAC9jkB/zwQAAAEAAAAAAAAAAAAAAACKACEABADV8+N/zvB/a8gAAAAAAAQAAaYAAAIABAAAABMWIcgBC/EAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5TiAFjwAAAUAAAXcAqSAGByAGKzcArAArugS6sA97BsWX8gAAAAWIUgAAAQAAAAS6yg95ZgAAAAS6ojUhzQS6oDUtqPUhPzUhaQlBV4AAAEAAAAWX8gWIUglBQES6pTUwr8S6sQ90ZMlBV495ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS6uzUhzQRBWIAAA8AAAAAAAA95Zi6q80AAAAS6yg95ZgS61TUi9n94AAS61TUiFoS6xTUiCoAAA895ZgS7iwAABQAAAEAAAAAAAAAABAAAAANBggAAAEAAAAAAAAS6wjxbGQS7fzXBGfUiDD////UiCoAACgAACiJue8kAAAACHRSTlP/////////AN6DvVkAAAB9SURBVHjardBBDsAgCATABaX8/8dFjBWVHpqUk5kAAlBVbMFGTYm4jBC5mBW1LuqOzlHNN2bIw9Z7ZiNlTpmRZ4cv37h+Yk23zG7ifFwQfsEWVtB2hDfWwKVzkY2tOOV+qiQbJ9PcJfAy3sP+HKn/cv/rZIrTbSx5kzG0xQ3CdAn6/PCEzQAAAABJRU5ErkJggg==",
+             "iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEUAACMcHkhERnJqbZX/AAD//wCQkb2usdr////UxJj////UxJPXZEgqBVgBCaoAAICprGAAACQAAAGhoaIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5+jxWDYBCaqprGAAAIDUhLLUhr4BCaoAADkS6CTY57IqBVgBCaoqBViprGAAABgAAALaFogAABUS6HzXOZWprHAqBVi1WqAS6GAS6QG2L+RFNyAqBVgAAIAAAAFPyjgS6OS1WqC1VShP0RYAAABPyji1WqAS6OS1RBxP7jPXNnrY5zIAAAAAAAEAAAAAAADUi9kS6NxBx0G1DExCx4VCx43LD8i1DGxFM5sS6NxFM7JFM7oS6XhFM8QS6NwS6VzLD8jLD8i1WqAS6PRCWLYABAEAAAC810AAAAES6SDUhzQRBWIABAEAAAC810DLD8i6q80AAAAS6VwS6TjUtqPUhPzUhaQlBV4AAAEWIagWIcgABAAWX8gAAADUtik94ZERBWIS6fAAAAAWX8g94ZwAAAAAAAAABAAAABMAAAAS6fzXBGfUiDD////UiCrUuJsAAADLD8gRBWIABAEAAAC810B/zwQAAAEAAAAAAAAAAAAAAACKACEABADV8+N/zvB/a8gAAAAAAAQAAaYAAAIABAAAABMWIcgBCaoAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5TiAFjwAAAUAAAXcAqSAGByAGKzcArAArugS6sA97BsWX8gAAAAWIUgAAAQAAAAS6yg95ZgAAAAS6ojUhzQS6oDUtqPUhPzUhaQlBV4AAAEAAAAWX8gWIUglBQES6pTUwr8S6sQ90ZMlBV495ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS6uzUhzQRBWIAAA8AAAAAAAA95Zi6q80AAAAS6yg95ZgS61TUi9n94AAS61TUiFoS6xTUiCoAAA895ZgS7iwAABQAAAEAAAAAAAAAABAAAAAqBVgAAAEAAAAAAAAS6wjxbGQS7fzXBGfUiDD////UiCoAACMAACNBU5ZGAAAACXRSTlP//////////wBTT3gSAAAAnklEQVR42sWSSxLEIAhEW1DD/U88fKMp3Q+L2HlFoMFABEcoE7RGvMV8CI6Je09mYj6B9SW5C8e44eb4KGLx7ZhYbjha3jFFr56dN3yOox53PmcMfy5FfCffbNbs5pB4LDq0DNU0Y9F3TCxuR3VAgXhANmwoPnFsbsLJGOlEyjdVQfBEYUv3U1Uk/wkjDboyg7HvvB7kXHZnmV0/5Kt+SqMJOP/C1HgAAAAASUVORK5CYII=",
+             "iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEUAACUCBC46PWlpapP/AACIibX///8S6MjXBGfUxJj////UxJPXZEgdBYYBC8IAAICpkXAAACQAAAGhoaIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5+jxWDYBC8KpkXAAAIDUhLLUhr4BC8IAADkS6CTY57IdBYYBC8IdBYapkXAAABgAAALaFogAABUS6HzXOZWpkYAdBYa1WqAS6GAS6QG2L+RFNyAdBYYAAIAAAAFPyjgS6OS1WqC1VShP0RYAAABPyji1WqAS6OS1RBxP7jPXNnrY5zIAAAAAAAEAAAAAAADUi9kS6NxBx0G1DExCx4VCx43LD8i1DGxFM5sS6NxFM7JFM7oS6XhFM8QS6NwS6VzLD8jLD8i1WqAS6PRCWLYABAEAAAC6kHwAAAES6SDUhzQRBWIABAEAAAC6kHzLD8i6q80AAAAS6VwS6TjUtqPUhPzUhaQlBV4AAAEWIagWIcgABAAWX8gAAADUtik94ZERBWIS6fAAAAAWX8g94ZwAAAAAAAAABAAAABMAAAAS6fzXBGfUiDD////UiCrUuJsAAADLD8gRBWIABAEAAAC6kHx/zwQAAAEAAAAAAAAAAAAAAACKACEABADV8+N/zvB/a8gAAAAAAAQAAaYAAAIABAAAABMWIcgBC8IAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5TiAFjwAAAUAAAXcAqSAGByAGKzcArAArugS6sA97BsWX8gAAAAWIUgAAAQAAAAS6yg95ZgAAAAS6ojUhzQS6oDUtqPUhPzUhaQlBV4AAAEAAAAWX8gWIUglBQES6pTUwr8S6sQ90ZMlBV495ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS6uzUhzQRBWIAAA8AAAAAAAA95Zi6q80AAAAS6yg95ZgS61TUi9n94AAS61TUiFoS6xTUiCoAAA895ZgS7iwAABQAAAEAAAAAAAAAABAAAAAdBYYAAAEAAAAAAAAS6wjxbGQS7fzXBGfUiDD////UiCoAACUAACXp3SOvAAAAB3RSTlP///////8AGksDRgAAAHlJREFUeNqt0IsKwCAIBdCrlf//yUs3l5UEgzkKdghfEMESJN1UidijtEZ0c1Bz1GrMPHlkQsnYVfnJfeKQJHAs+Y3rkdcp850YbxuEbVCvnh7941Ls37knMeaMgYz17Iz9tU+0lJy7c/Ye5Y3/edSMzGP6wJTy1PgF6dUHud5WP/kAAAAASUVORK5CYII=", ],
+    "green": ["iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEUAFgAVQhU7ZztkjmT//wCQvpCl06X////XBGfUxJj////UxJPXZEgQBgABDFwAAICpmGgAACQAAAGhoaIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5+jxWDYBDFypmGgAAIDUhLLUhr4BDFwAADkS6CTY57IQBgABDFwQBgCpmGgAABgAAALaFogAABUS6HzXOZWpmHgQBgC1WqAS6GAS6QG2L+RFNyAQBgAAAIAAAAFPyjgS6OS1WqC1VShP0RYAAABPyji1WqAS6OS1RBxP7jPXNnrY5zIAAAAAAAEAAAAAAADUi9kS6NxBx0G1DExCx4VCx43LD8i1DGxFM5sS6NxFM7JFM7oS6XhFM8QS6NwS6VzLD8jLD8i1WqAS6PRCWLYABAEAAAC+wvQAAAES6SDUhzQRBWIABAEAAAC+wvTLD8i6q80AAAAS6VwS6TjUtqPUhPzUhaQlBV4AAAEWIagWIcgABAAWX8gAAADUtik94ZERBWIS6fAAAAAWX8g94ZwAAAAAAAAABAAAABMAAAAS6fzXBGfUiDD////UiCrUuJsAAADLD8gRBWIABAEAAAC+wvR/zwQAAAEAAAAAAAAAAAAAAACKACEABADV8+N/zvB/a8gAAAAAAAQAAaYAAAIABAAAABMWIcgBDFwAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5TiAFjwAAAUAAAXcAqSAGByAGKzcArAArugS6sA97BsWX8gAAAAWIUgAAAQAAAAS6yg95ZgAAAAS6ojUhzQS6oDUtqPUhPzUhaQlBV4AAAEAAAAWX8gWIUglBQES6pTUwr8S6sQ90ZMlBV495ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS6uzUhzQRBWIAAA8AAAAAAAA95Zi6q80AAAAS6yg95ZgS61TUi9n94AAS61TUiFoS6xTUiCoAAA895ZgS7iwAABQAAAEAAAAAAAAAABAAAAAQBgAAAAEAAAAAAAAS6wjxbGQS7fzXBGfUiDD////UiCoAFgAAFgDgzxyHAAAACHRSTlP/////////AN6DvVkAAACXSURBVHjaxZLhCoQwDIOzbl7f/41vSdsx0RP8dWNg+YhtUoU7LmeySVuzvs5xfAzEzTYqnrifjjDuMF7iH70f8L3BU5yecRhz03Mgw1+X4rEThHaMkMseWr49dDXTKLWixXvERGpTXxNQHeLCF96bCNONra6DTrx8WzUE/SWmXM9ZhfhPGGlQVSxQOJaFyKVPmer6IVf1BTTtCE84csDNAAAAAElFTkSuQmCC",
+              "iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEUAHgARPhE/bD9mkGb/AACLuYup1an////XBGfUxJj////UxJPXZEgkBYIBDMoAAICpoVgAACQAAAGhoaIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5+jxWDYBDMqpoVgAAIDUhLLUhr4BDMoAADkS6CTY57IkBYIBDMokBYKpoVgAABgAAALaFogAABUS6HzXOZWpoWgkBYK1WqAS6GAS6QG2L+RFNyAkBYIAAIAAAAFPyjgS6OS1WqC1VShP0RYAAABPyji1WqAS6OS1RBxP7jPXNnrY5zIAAAAAAAEAAAAAAADUi9kS6NxBx0G1DExCx4VCx43LD8i1DGxFM5sS6NxFM7JFM7oS6XhFM8QS6NwS6VzLD8jLD8i1WqAS6PRCWLYABAEAAAC+TAQAAAES6SDUhzQRBWIABAEAAAC+TATLD8i6q80AAAAS6VwS6TjUtqPUhPzUhaQlBV4AAAEWIagWIcgABAAWX8gAAADUtik94ZERBWIS6fAAAAAWX8g94ZwAAAAAAAAABAAAABMAAAAS6fzXBGfUiDD////UiCrUuJsAAADLD8gRBWIABAEAAAC+TAR/zwQAAAEAAAAAAAAAAAAAAACKACEABADV8+N/zvB/a8gAAAAAAAQAAaYAAAIABAAAABMWIcgBDMoAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5TiAFjwAAAUAAAXcAqSAGByAGKzcArAArugS6sA97BsWX8gAAAAWIUgAAAQAAAAS6yg95ZgAAAAS6ojUhzQS6oDUtqPUhPzUhaQlBV4AAAEAAAAWX8gWIUglBQES6pTUwr8S6sQ90ZMlBV495ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS6uzUhzQRBWIAAA8AAAAAAAA95Zi6q80AAAAS6yg95ZgS61TUi9n94AAS61TUiFoS6xTUiCoAAA895ZgS7iwAABQAAAEAAAAAAAAAABAAAAAkBYIAAAEAAAAAAAAS6wjxbGQS7fzXBGfUiDD////UiCoAHgAAHgDUCIb6AAAACHRSTlP/////////AN6DvVkAAAB9SURBVHjardBBDsAgCATABaX8/8dFjBWVHpqUk5kAAlBVbMFGTYm4jBC5mBW1LuqOzlHNN2bIw9Z7ZiNlTpmRZ4cv37h+Yk23zG7ifFwQfsEWVtB2hDfWwKVzkY2tOOV+qiQbJ9PcJfAy3sP+HKn/cv/rZIrTbSx5kzG0xQ3CdAn6/PCEzQAAAABJRU5ErkJggg==",
+              "iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEUAFgAXQxc8azxkjmT/AAD//wCJs4ml06X////UxJj////UxJPXZEgNBgwBCuIAAICpnOAAACQAAAGhoaIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5+jxWDYBCuKpnOAAAIDUhLLUhr4BCuIAADkS6CTY57INBgwBCuINBgypnOAAABgAAALaFogAABUS6HzXOZWpnPANBgy1WqAS6GAS6QG2L+RFNyANBgwAAIAAAAFPyjgS6OS1WqC1VShP0RYAAABPyji1WqAS6OS1RBxP7jPXNnrY5zIAAAAAAAEAAAAAAADUi9kS6NxBx0G1DExCx4VCx43LD8i1DGxFM5sS6NxFM7JFM7oS6XhFM8QS6NwS6VzLD8jLD8i1WqAS6PRCWLYABAEAAAC+y1gAAAES6SDUhzQRBWIABAEAAAC+y1jLD8i6q80AAAAS6VwS6TjUtqPUhPzUhaQlBV4AAAEWIagWIcgABAAWX8gAAADUtik94ZERBWIS6fAAAAAWX8g94ZwAAAAAAAAABAAAABMAAAAS6fzXBGfUiDD////UiCrUuJsAAADLD8gRBWIABAEAAAC+y1h/zwQAAAEAAAAAAAAAAAAAAACKACEABADV8+N/zvB/a8gAAAAAAAQAAaYAAAIABAAAABMWIcgBCuIAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5TiAFjwAAAUAAAXcAqSAGByAGKzcArAArugS6sA97BsWX8gAAAAWIUgAAAQAAAAS6yg95ZgAAAAS6ojUhzQS6oDUtqPUhPzUhaQlBV4AAAEAAAAWX8gWIUglBQES6pTUwr8S6sQ90ZMlBV495ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS6uzUhzQRBWIAAA8AAAAAAAA95Zi6q80AAAAS6yg95ZgS61TUi9n94AAS61TUiFoS6xTUiCoAAA895ZgS7iwAABQAAAEAAAAAAAAAABAAAAANBgwAAAEAAAAAAAAS6wjxbGQS7fzXBGfUiDD////UiCoAFgAAFgB+RvKCAAAACXRSTlP//////////wBTT3gSAAAAnklEQVR42sWSSxLEIAhEW1DD/U88fKMp3Q+L2HlFoMFABEcoE7RGvMV8CI6Je09mYj6B9SW5C8e44eb4KGLx7ZhYbjha3jFFr56dN3yOox53PmcMfy5FfCffbNbs5pB4LDq0DNU0Y9F3TCxuR3VAgXhANmwoPnFsbsLJGOlEyjdVQfBEYUv3U1Uk/wkjDboyg7HvvB7kXHZnmV0/5Kt+SqMJOP/C1HgAAAAASUVORK5CYII=",
+              "iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEUAGgAAKAA0YTRhjWF/rX//AAD///8S6MjXBGfUxJj////UxJPXZEgMBhIBCrEAAICpvvAAACQAAAGhoaIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5+jxWDYBCrGpvvAAAIDUhLLUhr4BCrEAADkS6CTY57IMBhIBCrEMBhKpvvAAABgAAALaFogAABUS6HzXOZWpvwAMBhK1WqAS6GAS6QG2L+RFNyAMBhIAAIAAAAFPyjgS6OS1WqC1VShP0RYAAABPyji1WqAS6OS1RBxP7jPXNnrY5zIAAAAAAAEAAAAAAADUi9kS6NxBx0G1DExCx4VCx43LD8i1DGxFM5sS6NxFM7JFM7oS6XhFM8QS6NwS6VzLD8jLD8i1WqAS6PRCWLYABAEAAAC9lTQAAAES6SDUhzQRBWIABAEAAAC9lTTLD8i6q80AAAAS6VwS6TjUtqPUhPzUhaQlBV4AAAEWIagWIcgABAAWX8gAAADUtik94ZERBWIS6fAAAAAWX8g94ZwAAAAAAAAABAAAABMAAAAS6fzXBGfUiDD////UiCrUuJsAAADLD8gRBWIABAEAAAC9lTR/zwQAAAEAAAAAAAAAAAAAAACKACEABADV8+N/zvB/a8gAAAAAAAQAAaYAAAIABAAAABMWIcgBCrEAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5TiAFjwAAAUAAAXcAqSAGByAGKzcArAArugS6sA97BsWX8gAAAAWIUgAAAQAAAAS6yg95ZgAAAAS6ojUhzQS6oDUtqPUhPzUhaQlBV4AAAEAAAAWX8gWIUglBQES6pTUwr8S6sQ90ZMlBV495ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS6uzUhzQRBWIAAA8AAAAAAAA95Zi6q80AAAAS6yg95ZgS61TUi9n94AAS61TUiFoS6xTUiCoAAA895ZgS7iwAABQAAAEAAAAAAAAAABAAAAAMBhIAAAEAAAAAAAAS6wjxbGQS7fzXBGfUiDD////UiCoAGgAAGgCKN+QpAAAAB3RSTlP///////8AGksDRgAAAHlJREFUeNqt0IsKwCAIBdCrlf//yTM3l5UEgzkKdghfEMESJGpdidij1Ep0c1BztGbMPHlkQsnYtfOT+8QhSeBY8hu3I69T5jsx3jYI22C/ND3041Ls31mTGHPGQMb97Iz9tU+0lJy7c/Ye5Y3/edSMzGP6wJTy1PgF2VMHsLrJY5kAAAAASUVORK5CYII=", ],
+    "light_blue": ["iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEUAAAAACggIHhsWOjVfqaH/AACQ7uK////I///////////UxJPXZEghBfoBCpwAAIA8CTgAACQAAAGhoaIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5+jxWDYBCpw8CTgAAIDUhLLUhr4BCpwAADkS6CTY57IhBfoBCpwhBfo8CTgAABgAAALaFogAABUS6HzXOZU8CUghBfq1WqAS6GAS6QG2L+RFNyAhBfoAAIAAAAFPyjgS6OS1WqC1VShP0RYAAABPyji1WqAS6OS1RBxP7jPXNnrY5zIAAAAAAAEAAAAAAADUi9kS6NxBx0G1DExCx4VCx43LD8i1DGxFM5sS6NxFM7JFM7oS6XhFM8QS6NwS6VzLD8jLD8i1WqAS6PRCWLYABAEAAADACtAAAAES6SDUhzQRBWIABAEAAADACtDLD8i6q80AAAAS6VwS6TjUtqPUhPzUhaQlBV4AAAEWIagWIcgABAAWX8gAAADUtik94ZERBWIS6fAAAAAWX8g94ZwAAAAAAAAABAAAABMAAAAS6fzXBGfUiDD////UiCrUuJsAAADLD8gRBWIABAEAAADACtB/zwQAAAEAAAAAAAAAAAAAAACKACEABADV8+N/zvB/a8gAAAAAAAQAAaYAAAIABAAAABMWIcgBCpwAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5TiAFjwAAAUAAAXcAqSAGByAGKzcArAArugS6sA97BsWX8gAAAAWIUgAAAQAAAAS6yg95ZgAAAAS6ojUhzQS6oDUtqPUhPzUhaQlBV4AAAEAAAAWX8gWIUglBQES6pTUwr8S6sQ90ZMlBV495ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS6uzUhzQRBWIAAA8AAAAAAAA95Zi6q80AAAAS6yg95ZgS61TUi9n94AAS61TUiFoS6xTUiCoAAA895ZgS7iwAABQAAAEAAAAAAAAAABAAAAAhBfoAAAEAAAAAAAAS6wjxbGQS7fzXBGfUiDD////UiCoAAAAAAAAgZlkZAAAACnRSTlP///////////8AsswszwAAAJ1JREFUeNrFklkOhDAMQ820KeT+F546m+iw/E5VQfUwjhOAKi5rsklb66PWvh8fELd+osYDj2UZxh3Gj7Pjhif1g/cLvg+4FmVFZaOLngXZ/HUo6jOBa0VcbvGwxdti22qynfCVuozBfuaj0IY+KyAdfEMLn00MM00vV2ESzdw9DcF8gSm3+zy5+E8YEdBOPkDDPix4X/YpQ50/ZJ2+ESANEMn5E+sAAAAASUVORK5CYII=",
+                   "iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEUAAAAIHh0WOjVfqaH/AACQ7uK////I///////UxJj////UxJPXZEgtBWYBC8IAAIA8CTgAACQAAAGhoaIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5+jxWDYBC8I8CTgAAIDUhLLUhr4BC8IAADkS6CTY57ItBWYBC8ItBWY8CTgAABgAAALaFogAABUS6HzXOZU8CUgtBWa1WqAS6GAS6QG2L+RFNyAtBWYAAIAAAAFPyjgS6OS1WqC1VShP0RYAAABPyji1WqAS6OS1RBxP7jPXNnrY5zIAAAAAAAEAAAAAAADUi9kS6NxBx0G1DExCx4VCx43LD8i1DGxFM5sS6NxFM7JFM7oS6XhFM8QS6NwS6VzLD8jLD8i1WqAS6PRCWLYABAEAAAC/mJAAAAES6SDUhzQRBWIABAEAAAC/mJDLD8i6q80AAAAS6VwS6TjUtqPUhPzUhaQlBV4AAAEWIagWIcgABAAWX8gAAADUtik94ZERBWIS6fAAAAAWX8g94ZwAAAAAAAAABAAAABMAAAAS6fzXBGfUiDD////UiCrUuJsAAADLD8gRBWIABAEAAAC/mJB/zwQAAAEAAAAAAAAAAAAAAACKACEABADV8+N/zvB/a8gAAAAAAAQAAaYAAAIABAAAABMWIcgBC8IAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5TiAFjwAAAUAAAXcAqSAGByAGKzcArAArugS6sA97BsWX8gAAAAWIUgAAAQAAAAS6yg95ZgAAAAS6ojUhzQS6oDUtqPUhPzUhaQlBV4AAAEAAAAWX8gWIUglBQES6pTUwr8S6sQ90ZMlBV495ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS6uzUhzQRBWIAAA8AAAAAAAA95Zi6q80AAAAS6yg95ZgS61TUi9n94AAS61TUiFoS6xTUiCoAAA895ZgS7iwAABQAAAEAAAAAAAAAABAAAAAtBWYAAAEAAAAAAAAS6wjxbGQS7fzXBGfUiDD////UiCoAAAAAAADuz5NzAAAACXRSTlP//////////wBTT3gSAAAAd0lEQVR42q3QSQ7AIAgAQApK+f+LiyVaRDyYlJOZIBuICMRQaopItQfzrQ6lTGpu7FU9MME1WGuPbIIDJsizXcsdlyOWdMvNTbYXbNE+6DLwFhbHZFw5sH5OWfvl2bAyfrs4nsYb/D576r9svVZGP11gzov0oTUeiGEMnes12xEAAAAASUVORK5CYII=",
+                   "iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEUAAAAACwkIHh0WOjVfqaH/AACQ7uK////I///////////UxJPXZEguBdYBCMsAAIA8CTgAACQAAAGhoaIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5+jxWDYBCMs8CTgAAIDUhLLUhr4BCMsAADkS6CTY57IuBdYBCMsuBdY8CTgAABgAAALaFogAABUS6HzXOZU8CUguBda1WqAS6GAS6QG2L+RFNyAuBdYAAIAAAAFPyjgS6OS1WqC1VShP0RYAAABPyji1WqAS6OS1RBxP7jPXNnrY5zIAAAAAAAEAAAAAAADUi9kS6NxBx0G1DExCx4VCx43LD8i1DGxFM5sS6NxFM7JFM7oS6XhFM8QS6NwS6VzLD8jLD8i1WqAS6PRCWLYABAEAAADAEpAAAAES6SDUhzQRBWIABAEAAADAEpDLD8i6q80AAAAS6VwS6TjUtqPUhPzUhaQlBV4AAAEWIagWIcgABAAWX8gAAADUtik94ZERBWIS6fAAAAAWX8g94ZwAAAAAAAAABAAAABMAAAAS6fzXBGfUiDD////UiCrUuJsAAADLD8gRBWIABAEAAADAEpB/zwQAAAEAAAAAAAAAAAAAAACKACEABADV8+N/zvB/a8gAAAAAAAQAAaYAAAIABAAAABMWIcgBCMsAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5TiAFjwAAAUAAAXcAqSAGByAGKzcArAArugS6sA97BsWX8gAAAAWIUgAAAQAAAAS6yg95ZgAAAAS6ojUhzQS6oDUtqPUhPzUhaQlBV4AAAEAAAAWX8gWIUglBQES6pTUwr8S6sQ90ZMlBV495ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS6uzUhzQRBWIAAA8AAAAAAAA95Zi6q80AAAAS6yg95ZgS61TUi9n94AAS61TUiFoS6xTUiCoAAA895ZgS7iwAABQAAAEAAAAAAAAAABAAAAAuBdYAAAEAAAAAAAAS6wjxbGQS7fzXBGfUiDD////UiCoAAAAAAAD5iCX+AAAACnRSTlP///////////8AsswszwAAAKBJREFUeNrFkkkWwyAMQ5UCdnz/C9cjkOF1Wy+C8p8DkglE8ChlgtYabcXnB4H7GMlM8BlYX5K7cIw3fDim+yZWrRNdzzQzb1h+41G14/4SRz3umDnCP4ciPpNrN2n34bDTWFRTcqs0Y9EZE4vbUiegQDwgGzYUnzg2N31Oz51I+e61IYhR2Np9VRXNf8JIg67MYMw7LxOZy+4su+uHnOoL3NgM+NZhtQcAAAAASUVORK5CYII=",
+                   "iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEUAAAAACAgFGRU2hXtn49L/AACh//+u///////UxJj////UxJPXZEg0BcABCpoAAIA8CTgAACQAAAGhoaIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5+jxWDYBCpo8CTgAAIDUhLLUhr4BCpoAADkS6CTY57I0BcABCpo0BcA8CTgAABgAAALaFogAABUS6HzXOZU8CUg0BcC1WqAS6GAS6QG2L+RFNyA0BcAAAIAAAAFPyjgS6OS1WqC1VShP0RYAAABPyji1WqAS6OS1RBxP7jPXNnrY5zIAAAAAAAEAAAAAAADUi9kS6NxBx0G1DExCx4VCx43LD8i1DGxFM5sS6NxFM7JFM7oS6XhFM8QS6NwS6VzLD8jLD8i1WqAS6PRCWLYABAEAAADB5WwAAAES6SDUhzQRBWIABAEAAADB5WzLD8i6q80AAAAS6VwS6TjUtqPUhPzUhaQlBV4AAAEWIagWIcgABAAWX8gAAADUtik94ZERBWIS6fAAAAAWX8g94ZwAAAAAAAAABAAAABMAAAAS6fzXBGfUiDD////UiCrUuJsAAADLD8gRBWIABAEAAADB5Wx/zwQAAAEAAAAAAAAAAAAAAACKACEABADV8+N/zvB/a8gAAAAAAAQAAaYAAAIABAAAABMWIcgBCpoAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5TiAFjwAAAUAAAXcAqSAGByAGKzcArAArugS6sA97BsWX8gAAAAWIUgAAAQAAAAS6yg95ZgAAAAS6ojUhzQS6oDUtqPUhPzUhaQlBV4AAAEAAAAWX8gWIUglBQES6pTUwr8S6sQ90ZMlBV495ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS6uzUhzQRBWIAAA8AAAAAAAA95Zi6q80AAAAS6yg95ZgS61TUi9n94AAS61TUiFoS6xTUiCoAAA895ZgS7iwAABQAAAEAAAAAAAAAABAAAAA0BcAAAAEAAAAAAAAS6wjxbGQS7fzXBGfUiDD////UiCoAAAAAAADgUEUUAAAACXRSTlP//////////wBTT3gSAAAAfElEQVR42q3QSQ7AIAgFUKgT9z9xkRZFISZNysLFi/kMQARbIbGxXillrdoaorBVcShFOOfFLSPUiFU7v9knNiGGbctvXI68bxnfRNhdEOSC/eF44IWeABrMIcI1Yl404H4Xz+B/60Zby3U6ZZ2RRv3Ps6dlGdFxingd/AaZSgv6pVvhUAAAAABJRU5ErkJggg==", ],
+    "purple": ["iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEURAAJLHjtwQ1+Xa4f//wDFl7XYrMr////XBGfUxJj////UxJPXZEgpBZQBCMsAAIA8CTgAACQAAAGhoaIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5+jxWDYBCMs8CTgAAIDUhLLUhr4BCMsAADkS6CTY57IpBZQBCMspBZQ8CTgAABgAAALaFogAABUS6HzXOZU8CUgpBZS1WqAS6GAS6QG2L+RFNyApBZQAAIAAAAFPyjgS6OS1WqC1VShP0RYAAABPyji1WqAS6OS1RBxP7jPXNnrY5zIAAAAAAAEAAAAAAADUi9kS6NxBx0G1DExCx4VCx43LD8i1DGxFM5sS6NxFM7JFM7oS6XhFM8QS6NwS6VzLD8jLD8i1WqAS6PRCWLYABAEAAADAWqAAAAES6SDUhzQRBWIABAEAAADAWqDLD8i6q80AAAAS6VwS6TjUtqPUhPzUhaQlBV4AAAEWIagWIcgABAAWX8gAAADUtik94ZERBWIS6fAAAAAWX8g94ZwAAAAAAAAABAAAABMAAAAS6fzXBGfUiDD////UiCrUuJsAAADLD8gRBWIABAEAAADAWqB/zwQAAAEAAAAAAAAAAAAAAACKACEABADV8+N/zvB/a8gAAAAAAAQAAaYAAAIABAAAABMWIcgBCMsAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5TiAFjwAAAUAAAXcAqSAGByAGKzcArAArugS6sA97BsWX8gAAAAWIUgAAAQAAAAS6yg95ZgAAAAS6ojUhzQS6oDUtqPUhPzUhaQlBV4AAAEAAAAWX8gWIUglBQES6pTUwr8S6sQ90ZMlBV495ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS6uzUhzQRBWIAAA8AAAAAAAA95Zi6q80AAAAS6yg95ZgS61TUi9n94AAS61TUiFoS6xTUiCoAAA895ZgS7iwAABQAAAEAAAAAAAAAABAAAAApBZQAAAEAAAAAAAAS6wjxbGQS7fzXBGfUiDD////UiCoRAAIRAAJWkx99AAAACHRSTlP/////////AN6DvVkAAACXSURBVHjaxZLhCoQwDIOzbl7f/41vSdsx0RP8dWNg+YhtUoU7LmeySVuzvs5xfAzEzTYqnrifjjDuMF7iH70f8L3BU5yecRhz03Mgw1+X4rEThHaMkMseWr49dDXTKLWixXvERGpTXxNQHeLCF96bCNONra6DTrx8WzUE/SWmXM9ZhfhPGGlQVSxQOJaFyKVPmer6IVf1BTTtCE84csDNAAAAAElFTkSuQmCC",
+               "iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEURAAJIGjlxRWL/AACXa4e8j6vYrMr////XBGfUxJj////UxJPXZEgKBnwBCaoAAICp79AAACQAAAGhoaIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5+jxWDYBCaqp79AAAIDUhLLUhr4BCaoAADkS6CTY57IKBnwBCaoKBnyp79AAABgAAALaFogAABUS6HzXOZWp7+AKBny1WqAS6GAS6QG2L+RFNyAKBnwAAIAAAAFPyjgS6OS1WqC1VShP0RYAAABPyji1WqAS6OS1RBxP7jPXNnrY5zIAAAAAAAEAAAAAAADUi9kS6NxBx0G1DExCx4VCx43LD8i1DGxFM5sS6NxFM7JFM7oS6XhFM8QS6NwS6VzLD8jLD8i1WqAS6PRCWLYABAEAAADBiwAAAAES6SDUhzQRBWIABAEAAADBiwDLD8i6q80AAAAS6VwS6TjUtqPUhPzUhaQlBV4AAAEWIagWIcgABAAWX8gAAADUtik94ZERBWIS6fAAAAAWX8g94ZwAAAAAAAAABAAAABMAAAAS6fzXBGfUiDD////UiCrUuJsAAADLD8gRBWIABAEAAADBiwB/zwQAAAEAAAAAAAAAAAAAAACKACEABADV8+N/zvB/a8gAAAAAAAQAAaYAAAIABAAAABMWIcgBCaoAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5TiAFjwAAAUAAAXcAqSAGByAGKzcArAArugS6sA97BsWX8gAAAAWIUgAAAQAAAAS6yg95ZgAAAAS6ojUhzQS6oDUtqPUhPzUhaQlBV4AAAEAAAAWX8gWIUglBQES6pTUwr8S6sQ90ZMlBV495ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS6uzUhzQRBWIAAA8AAAAAAAA95Zi6q80AAAAS6yg95ZgS61TUi9n94AAS61TUiFoS6xTUiCoAAA895ZgS7iwAABQAAAEAAAAAAAAAABAAAAAKBnwAAAEAAAAAAAAS6wjxbGQS7fzXBGfUiDD////UiCoRAAIRAAIpItfNAAAACHRSTlP/////////AN6DvVkAAAB9SURBVHjardBBDsAgCATABaX8/8dFjBWVHpqUk5kAAlBVbMFGTYm4jhC5mBWlLOqOzlHNN2bIw9Z7ZiNlTpmRZ4cv37h8Yk23zG7ifFwQfsEWVtB2hDfWwLVzlY2tOOV+qiQbJ9PcJfAy3sP+HKn/cv/rZIrTbSx5kzG0xQ39dAqxz8DMUwAAAABJRU5ErkJggg==",
+               "iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEURAAJNIDxxRWL/AACXa4f//wC7jqrYrMr////UxJj////UxJPXZEgYBZYBCpwAAICp61gAACQAAAGhoaIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5+jxWDYBCpyp61gAAIDUhLLUhr4BCpwAADkS6CTY57IYBZYBCpwYBZap61gAABgAAALaFogAABUS6HzXOZWp62gYBZa1WqAS6GAS6QG2L+RFNyAYBZYAAIAAAAFPyjgS6OS1WqC1VShP0RYAAABPyji1WqAS6OS1RBxP7jPXNnrY5zIAAAAAAAEAAAAAAADUi9kS6NxBx0G1DExCx4VCx43LD8i1DGxFM5sS6NxFM7JFM7oS6XhFM8QS6NwS6VzLD8jLD8i1WqAS6PRCWLYABAEAAADBiuwAAAES6SDUhzQRBWIABAEAAADBiuzLD8i6q80AAAAS6VwS6TjUtqPUhPzUhaQlBV4AAAEWIagWIcgABAAWX8gAAADUtik94ZERBWIS6fAAAAAWX8g94ZwAAAAAAAAABAAAABMAAAAS6fzXBGfUiDD////UiCrUuJsAAADLD8gRBWIABAEAAADBiux/zwQAAAEAAAAAAAAAAAAAAACKACEABADV8+N/zvB/a8gAAAAAAAQAAaYAAAIABAAAABMWIcgBCpwAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5TiAFjwAAAUAAAXcAqSAGByAGKzcArAArugS6sA97BsWX8gAAAAWIUgAAAQAAAAS6yg95ZgAAAAS6ojUhzQS6oDUtqPUhPzUhaQlBV4AAAEAAAAWX8gWIUglBQES6pTUwr8S6sQ90ZMlBV495ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS6uzUhzQRBWIAAA8AAAAAAAA95Zi6q80AAAAS6yg95ZgS61TUi9n94AAS61TUiFoS6xTUiCoAAA895ZgS7iwAABQAAAEAAAAAAAAAABAAAAAYBZYAAAEAAAAAAAAS6wjxbGQS7fzXBGfUiDD////UiCoRAAIRAAKVOkYIAAAACXRSTlP//////////wBTT3gSAAAAnklEQVR42sWSSxLEIAhEW0TD/U88fKMp3Q+L2HlFoMFABEcoE7RGvMV8CI6Je09mYj6B9SW5C8e44eb4KGLx7ZhYbjha3jFFr56dN3yOox53PmcMfy5FfCffbNbs5pB4LDq0DNU0Y9F3TCxuR3VAgXhANmwoPnFsbsLJGOlEyjdVQfBEYUv3U1Uk/wkjDboyg7HvvB7kXHZnmV0/5Kt+a7kJ+cUredMAAAAASUVORK5CYII=",
+               "iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEURAAJIGjlxRWL/AACXa4e8j6vYrMr////XBGfUxJj////UxJPXZEgfBbgBCpwAAIA8CTgAACQAAAGhoaIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5+jxWDYBCpw8CTgAAIDUhLLUhr4BCpwAADkS6CTY57IfBbgBCpwfBbg8CTgAABgAAALaFogAABUS6HzXOZU8CUgfBbi1WqAS6GAS6QG2L+RFNyAfBbgAAIAAAAFPyjgS6OS1WqC1VShP0RYAAABPyji1WqAS6OS1RBxP7jPXNnrY5zIAAAAAAAEAAAAAAADUi9kS6NxBx0G1DExCx4VCx43LD8i1DGxFM5sS6NxFM7JFM7oS6XhFM8QS6NwS6VzLD8jLD8i1WqAS6PRCWLYABAEAAADB5pAAAAES6SDUhzQRBWIABAEAAADB5pDLD8i6q80AAAAS6VwS6TjUtqPUhPzUhaQlBV4AAAEWIagWIcgABAAWX8gAAADUtik94ZERBWIS6fAAAAAWX8g94ZwAAAAAAAAABAAAABMAAAAS6fzXBGfUiDD////UiCrUuJsAAADLD8gRBWIABAEAAADB5pB/zwQAAAEAAAAAAAAAAAAAAACKACEABADV8+N/zvB/a8gAAAAAAAQAAaYAAAIABAAAABMWIcgBCpwAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5TiAFjwAAAUAAAXcAqSAGByAGKzcArAArugS6sA97BsWX8gAAAAWIUgAAAQAAAAS6yg95ZgAAAAS6ojUhzQS6oDUtqPUhPzUhaQlBV4AAAEAAAAWX8gWIUglBQES6pTUwr8S6sQ90ZMlBV495ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS6uzUhzQRBWIAAA8AAAAAAAA95Zi6q80AAAAS6yg95ZgS61TUi9n94AAS61TUiFoS6xTUiCoAAA895ZgS7iwAABQAAAEAAAAAAAAAABAAAAAfBbgAAAEAAAAAAAAS6wjxbGQS7fzXBGfUiDD////UiCoRAAIRAAK3In3PAAAACHRSTlP/////////AN6DvVkAAAB4SURBVHjardBBDsAgCARAiij//3FBi6JS00NJ9DAhKwjMsBaLiV6IZJVLURf22jylykSTe0bIEYPrfrIr55hdiGOKQz5wOvK65eFPXn5QL4kH3bMGcGekxhQxQMR6doa92zZanpynM7YZudf/PN70TGN7xxjxPPgN+sEKkg2MzBYAAAAASUVORK5CYII=", ],
+    "yellow": ["iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEUAAAA1NTVZWVmAAACAgEDd3QD//wD//7n//9/////////UxJPXZEg/BcABC54AAICpXoAAACQAAAGhoaIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5+jxWDYBC56pXoAAAIDUhLLUhr4BC54AADkS6CTY57I/BcABC54/BcCpXoAAABgAAALaFogAABUS6HzXOZWpXpA/BcC1WqAS6GAS6QG2L+RFNyA/BcAAAIAAAAFPyjgS6OS1WqC1VShP0RYAAABPyji1WqAS6OS1RBxP7jPXNnrY5zIAAAAAAAEAAAAAAADUi9kS6NxBx0G1DExCx4VCx43LD8i1DGxFM5sS6NxFM7JFM7oS6XhFM8QS6NwS6VzLD8jLD8i1WqAS6PRCWLYABAEAAADACOAAAAES6SDUhzQRBWIABAEAAADACODLD8i6q80AAAAS6VwS6TjUtqPUhPzUhaQlBV4AAAEWIagWIcgABAAWX8gAAADUtik94ZERBWIS6fAAAAAWX8g94ZwAAAAAAAAABAAAABMAAAAS6fzXBGfUiDD////UiCrUuJsAAADLD8gRBWIABAEAAADACOB/zwQAAAEAAAAAAAAAAAAAAACKACEABADV8+N/zvB/a8gAAAAAAAQAAaYAAAIABAAAABMWIcgBC54AAAAAAAAAAAAAAAAAAAAAAAAAAAAS5TiAFjwAAAUAAAXcAqSAGByAGKzcArAArugS6sA97BsWX8gAAAAWIUgAAAQAAAAS6yg95ZgAAAAS6ojUhzQS6oDUtqPUhPzUhaQlBV4AAAEAAAAWX8gWIUglBQES6pTUwr8S6sQ90ZMlBV495ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS6uzUhzQRBWIAAA8AAAAAAAA95Zi6q80AAAAS6yg95ZgS61TUi9n94AAS61TUiFoS6xTUiCoAAA895ZgS7iwAABQAAAEAAAAAAAAAABAAAAA/BcAAAAEAAAAAAAAS6wjxbGQS7fzXBGfUiDD////UiCoAAAAAAADUVPSFAAAACnRSTlP///////////8AsswszwAAAJ1JREFUeNrFklkOhDAMQ82kLeT+F546m+iw/E5VQfUwjhOAKi5rsklb66PWvh8fELd+osYDj2UZxh3Gj7Pjhif1g/cLvg+4FmVFZaOLngXZ/HUo6jOBa0VcbvGwxdti22qynfCVuozBfuaj0IY+KyAdfEMLn00MM00vV2ESzdw9DcF8gSm3+zy5+E8YEdBOPkDDPix4X/YpQ50/ZJ2+M+wNHGvcgAEAAAAASUVORK5CYII=",
+               "iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEUAAABbW1v/AACAgEDd3QD//wD//7n//9/////UxJj////UxJPXZEgdBeYBCgMAAICpsYAAACQAAAGhoaIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5+jxWDYBCgOpsYAAAIDUhLLUhr4BCgMAADkS6CTY57IdBeYBCgMdBeapsYAAABgAAALaFogAABUS6HzXOZWpsZAdBea1WqAS6GAS6QG2L+RFNyAdBeYAAIAAAAFPyjgS6OS1WqC1VShP0RYAAABPyji1WqAS6OS1RBxP7jPXNnrY5zIAAAAAAAEAAAAAAADUi9kS6NxBx0G1DExCx4VCx43LD8i1DGxFM5sS6NxFM7JFM7oS6XhFM8QS6NwS6VzLD8jLD8i1WqAS6PRCWLYABAEAAADAAAwAAAES6SDUhzQRBWIABAEAAADAAAzLD8i6q80AAAAS6VwS6TjUtqPUhPzUhaQlBV4AAAEWIagWIcgABAAWX8gAAADUtik94ZERBWIS6fAAAAAWX8g94ZwAAAAAAAAABAAAABMAAAAS6fzXBGfUiDD////UiCrUuJsAAADLD8gRBWIABAEAAADAAAx/zwQAAAEAAAAAAAAAAAAAAACKACEABADV8+N/zvB/a8gAAAAAAAQAAaYAAAIABAAAABMWIcgBCgMAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5TiAFjwAAAUAAAXcAqSAGByAGKzcArAArugS6sA97BsWX8gAAAAWIUgAAAQAAAAS6yg95ZgAAAAS6ojUhzQS6oDUtqPUhPzUhaQlBV4AAAEAAAAWX8gWIUglBQES6pTUwr8S6sQ90ZMlBV495ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS6uzUhzQRBWIAAA8AAAAAAAA95Zi6q80AAAAS6yg95ZgS61TUi9n94AAS61TUiFoS6xTUiCoAAA895ZgS7iwAABQAAAEAAAAAAAAAABAAAAAdBeYAAAEAAAAAAAAS6wjxbGQS7fzXBGfUiDD////UiCoAAAAAAAAd4/SfAAAACXRSTlP//////////wBTT3gSAAAAd0lEQVR42q3QSQ7AIAgAQCpI+f+LiyVaRDyYlJOZIBuICMRQaopItQfzrQ6lTGpu7FU9MME1WGuPbIIDJsizXcsdlyOWdMvNTbYXbNE+6DLwFhbHZFw5sH5OWfvl2bAyfrs4nsYb/D576r9svVZGP11gzov0oTUevOkMweuql6MAAAAASUVORK5CYII=",
+               "iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEUAAAA3NzdbW1sAAP//AACAgEDd3QD//wD//7n//9/////UxJPXZEgiBdgBCpwAAICprGAAACQAAAGhoaIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5+jxWDYBCpyprGAAAIDUhLLUhr4BCpwAADkS6CTY57IiBdgBCpwiBdiprGAAABgAAALaFogAABUS6HzXOZWprHAiBdi1WqAS6GAS6QG2L+RFNyAiBdgAAIAAAAFPyjgS6OS1WqC1VShP0RYAAABPyji1WqAS6OS1RBxP7jPXNnrY5zIAAAAAAAEAAAAAAADUi9kS6NxBx0G1DExCx4VCx43LD8i1DGxFM5sS6NxFM7JFM7oS6XhFM8QS6NwS6VzLD8jLD8i1WqAS6PRCWLYABAEAAAC+7vgAAAES6SDUhzQRBWIABAEAAAC+7vjLD8i6q80AAAAS6VwS6TjUtqPUhPzUhaQlBV4AAAEWIagWIcgABAAWX8gAAADUtik94ZERBWIS6fAAAAAWX8g94ZwAAAAAAAAABAAAABMAAAAS6fzXBGfUiDD////UiCrUuJsAAADLD8gRBWIABAEAAAC+7vh/zwQAAAEAAAAAAAAAAAAAAACKACEABADV8+N/zvB/a8gAAAAAAAQAAaYAAAIABAAAABMWIcgBCpwAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5TiAFjwAAAUAAAXcAqSAGByAGKzcArAArugS6sA97BsWX8gAAAAWIUgAAAQAAAAS6yg95ZgAAAAS6ojUhzQS6oDUtqPUhPzUhaQlBV4AAAEAAAAWX8gWIUglBQES6pTUwr8S6sQ90ZMlBV495ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS6uzUhzQRBWIAAA8AAAAAAAA95Zi6q80AAAAS6yg95ZgS61TUi9n94AAS61TUiFoS6xTUiCoAAA895ZgS7iwAABQAAAEAAAAAAAAAABAAAAAiBdgAAAEAAAAAAAAS6wjxbGQS7fzXBGfUiDD////UiCoAAAAAAACaAEpEAAAAC3RSTlP/////////////AEpPAfIAAAChSURBVHjaxZJJFoQgDETLZgjm/gfujILK621nAeV/MVQCYMYrhDFaa7TEOD9w3GsNpmKcjuUjuAnD2OHDMD2LaLROdD9Tzeww/8Y1Y8V90454XPEY3vx7KGwzuWeTZB8GO5VJi5Rp2U2Z9GoTk+uWJyCBL+AFK/JfDKsbd1JKOOH03bMgaCCxptsuypP/hBEGTalBn3dcJqIvvbPIzgd5qS8HLg6mYkMgDQAAAABJRU5ErkJggg==",
+               "iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAMAAAAfOR5kAAAACXBIWXMAAA7EAAAOxAGVKw4bAAADAFBMVEUAAABbW1v/AACAgEDd3QD//wD//7n//9/////UxJj////UxJPXZEgUBf4BCocAAICpyvgAACQAAAGhoaIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5+jxWDYBCoepyvgAAIDUhLLUhr4BCocAADkS6CTY57IUBf4BCocUBf6pyvgAABgAAALaFogAABUS6HzXOZWpywgUBf61WqAS6GAS6QG2L+RFNyAUBf4AAIAAAAFPyjgS6OS1WqC1VShP0RYAAABPyji1WqAS6OS1RBxP7jPXNnrY5zIAAAAAAAEAAAAAAADUi9kS6NxBx0G1DExCx4VCx43LD8i1DGxFM5sS6NxFM7JFM7oS6XhFM8QS6NwS6VzLD8jLD8i1WqAS6PRCWLYABAEAAAC+UswAAAES6SDUhzQRBWIABAEAAAC+UszLD8i6q80AAAAS6VwS6TjUtqPUhPzUhaQlBV4AAAEWIagWIcgABAAWX8gAAADUtik94ZERBWIS6fAAAAAWX8g94ZwAAAAAAAAABAAAABMAAAAS6fzXBGfUiDD////UiCrUuJsAAADLD8gRBWIABAEAAAC+Usx/zwQAAAEAAAAAAAAAAAAAAACKACEABADV8+N/zvB/a8gAAAAAAAQAAaYAAAIABAAAABMWIcgBCocAAAAAAAAAAAAAAAAAAAAAAAAAAAAS5TiAFjwAAAUAAAXcAqSAGByAGKzcArAArugS6sA97BsWX8gAAAAWIUgAAAQAAAAS6yg95ZgAAAAS6ojUhzQS6oDUtqPUhPzUhaQlBV4AAAEAAAAWX8gWIUglBQES6pTUwr8S6sQ90ZMlBV495ZgWX8jUiKYAAAAAAAIAAMgAABMWIVAS6uzUhzQRBWIAAA8AAAAAAAA95Zi6q80AAAAS6yg95ZgS61TUi9n94AAS61TUiFoS6xTUiCoAAA895ZgS7iwAABQAAAEAAAAAAAAAABAAAAAUBf4AAAEAAAAAAAAS6wjxbGQS7fzXBGfUiDD////UiCoAAAAAAACiBv84AAAACXRSTlP//////////wBTT3gSAAAAfElEQVR42q3QSQ7AIAgFULAO3P/ERVoUhZg0KQsXL+YzABFshcTGeuVctGpriMJWxSEl4VIWt4xQI1bt/Gaf2IQYti2/cTryvmV8E2F3QZAL9ofjgRd6AmgwhwjXiHnRgPtdPIP/rRttLdfplHVGGvU/z56WZUTHOeJ18BvzgwzNnf4n3QAAAABJRU5ErkJggg==", ],
+    "nubzuk": ["iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAYAAAAo5+5WAAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAAf1JREFUeNq8ls9LAkEUx+fNjmRC4J+gpyA6uIeu4dIhykv+BSl1KDpU1yDKS1ftXrT/QV4qpENS0NUNIujmnyBIEmg7vdkdZVx2XTW3ga+zzrz9zNv59R4hERUIM8iZn0msMp5m666w2JoYjLAUVoeoLVQq4N0mqoq6xEGaI8ESeIYqTPjlJqqkDgAKVMDKqOSU0yqmpojw6gAsoTczWjcBN2HG0AGcRgAVpSzAxQjAx9HNsbIrsljd/nFX5BFaF39ov1U2pFGVKaDinXQfGnjyVi9qZRafP4olFgiLJ3xJve8O6XbapPvVLr2c5s5DjzRCU5zbDXVKqBYjlDHn2e71iP3THZoCAKo/n6wPHWvmBVMW8z193LZdTyglGp1Tu5Jy4Y0hj9cqr9jB3buBOz/lKRfPJABvEmsyqmliJ2SHvOMcPw/G2h2KrXpxbTPQWNZj2kJrA+etMZaf3EZbQOdAvV4zFKjWRBFF+uPBiuVpC5RjC5qOzy2lvYVgyOOCVFF18Vzb053VBY2OJVFq+zpCwXAZDscIDE0bV+98nJl42F32ZbDAmAWuN/c7S74vbl5/jByYBUfDkDgb0v//4LC8IKw/Mo9pZJmQzHSefLKdftHxnrU8+YewbYxIZAwqgZkRg08aUcTRTgmwJeVX6mpUUKKNJbOfII+bvwIMAO/emZE2xkKDAAAAAElFTkSuQmCC",
+               "iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAYAAAAo5+5WAAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAAsRJREFUeNq0lT9sElEcx3/v7ih/JHjqgBrbsDkYGxKTBgZiTbc6lEWNG9FoTFzKoGtr1MUJJ50KJjrDYnADh46mNI0aXcpU24GUgIUCd/f8/d5dQ6304I564b1HLrzP+/J93997AP/pYU5+PJ/9roJhJA1dr396OF2w+600KvRm7kcSdWzi1yznRn4us5oaG4zQLA55bCrn2GOHqrMzTz9EXYMRunzZ10i9nQtAfCpIVOQawkMmSXlXYIRGcFgqvlmG23duQYzAJNlAuGEQOnJtcSXlRnGSulAoBPFYHHaaXeRysxm6UI/P9UETlSFglbobj1/B1bAfCl9r4iVZQWBTNUTcgMWzsd2CjV97AkRQjBx+EKyTaqi7seKvSZz+Ojc3j6BiEYDPbsCFo1ABJuW6RiMtnBs0UR70MvGiGL0YSz5qbm3Wg+FLNDlmQg3KL+jdDnSau2Bo2t0vmXuVkRUrPn+JSWwJRZa2K6uvEVoxN83cOL3TJngVoQVHOZYUj8okBRgTR8la7ee6qiGMyL29BnQauyDJSmTmyftZZwXCeRqrqozkqoicJEV+b1WhiY1sUAKnQJ7wkoBjS3pg3LzquYL39Fk8F/i74v0rucTLIle8foT5RH4NrQeagnZ09tWRwaKMOV/jjKkMTZ5f+bZAIFRvpUEnpbiJmu2ZqwwsYwE9iBlLSsqEGTOGYFxA2++CjO+4rDgCl/vXABOqEFlHW9SDDMse4S8tVnZ0g6AdizgsWJWX1nudqHUeHy5DukXOjH01JZ5/5MELU9aBJsiZ4oPp9NhXU6u2g962hT1WWweHm3fsI85gxqxzWGT8ZMB974Y7KDlglg/ZYCk/GfDR/Z51ZQVekhSxEpMV1eMPQK/dEiVtBnu4FXYeLwXPT6rB8GQ/YVaARwmpHbhK0H+3arTo23n8TO91MzZ3Yc4O/EeAAQA+W0ZCy9plxAAAAABJRU5ErkJggg==",
+               "iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAYAAAAo5+5WAAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAAlxJREFUeNq8ls1rE0EUwN+bndBaoiyePGnqRQgKWUTwJFl6EO3FXurRFj0oBfUsiPbiNdWz0r16spcqwUKDgniRrKCCF4n+AbLYD6pJd3xvs5HJsrObhMaBt7M78+Y3b9+8mTcAYyqYpzDrfbWpqiSa/fWFU8HQYIKVqLpDcoWkZBjbIlkjeUyTtDLBMfABycKQf+6RLOsToAZlWO322aJ9ZPs7/CqegCcftjNppAuaLrtmkeD8FyA06OqZY1P2543nMH91HrimbyOU+xK6vBYvYhaIHpQ/dv7sQ7lcjgZyzd+mkqG7ykykh9IHnD9ehJNHJ+Dbz9/w/ke2KzJ0A9QtPsCyiLqPDwpKC+jpUVFl55PYIwI5KuYI2vgXFVzihmmSlRGgPGa6BzXuvAuP6jU5eehuYeowyMn0kOvs7UJ7dwvaO1vLb+/PPszd0gQtKRU2dZcIqwBCyug97HQg3G/3RwAK5829i33bWibBQhZqaX5WYdi1RAiwxITeZccL7/ZZPLPyjjpU92yIIlrVRlw8DxA/xlhPCsviSKj2WacU/R4OFB2arn5wXZNoyWpCNSBtl/zWHMhOFZIuknGoH68VgcJqkYAmzuulc36izSiRLloOvQdae0BgnKMFWSNp8Hv9phOtLlpiIOFSv+UQFN0uI+K4xtR06eknNYgnXt04ncqQxpyFXWteXi+nDrz87EvmxNKcDXPybE7//wfn3Qvy+sdmsRjbTSi+6Wym3HZ6xaFz1k/cP1i3mXGRcUUMrGRMPmxG4a1dYrAfS1pp6FlByzZ+fPsxWdz6K8AAABzTUg24Cq4AAAAASUVORK5CYII=",
+               "iVBORw0KGgoAAAANSUhEUgAAABYAAAAeCAYAAAAo5+5WAAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAAtxJREFUeNrEVj1s00AUfnc+57dELuJPRUitGCgZUCSEkDpFIIGgiyPE3B8JMbaVQGIB2oG5XRnaFMSAWJpKUMZ6QDChpgPQDkAqBsIAtdqmP2ls894lcVtEGttF4qJnO/b5u+++d+87A/zPdvXx/OC18Q+9ft5h+z28eO+51nLiVFZE47oiVACuGIyxzKveM2YzYL7vQ1WdwpMOjlNnkcbT1+7JxVRg4PODE8OMK2mnBhoPcRi9cgQyx00N/2YPwniAEUcCxug4HIGXL57CyO0bsFH8nELWvb6BkS1NWXMcG+oylLYsSCaTkEgkoPVYG93qCcJYaujYNpAUFF9+bcKSloKB8VnY5FG3T6MmGtwvyGNNBjzImP64DIy5XMwgjPNVXBuqcsBO/NHHF/D7sX5ibJAUcgD5qzf3ajroquizK9umm0BnD2WjOP/WuHDn2XDX/SndFzCxdmwrZ5W33JVBza5YNJsM3ssyzh5SEV0efZP2mrxqpSlCL6+tgIjEQAlHYHu9BGvfl7RyaWUOs9hOieSKoH7tvoDRHzSOHlHZKME6Mt/eLCGIojHONWRsAud5jAL6R84zcNeDqTSWNKjROHpGSDJDM5KDIHgmcfI0AerI3JjpP2t61lgJRTBCoESiIFAGkiLUkoDY0TZItHX0oL5zgBoj+Gx3dkH3DhwOm0o4itVnATGvaQlc4FkInfSVXsJkDHgGNu5eymPSTBGOQdWLdnxjF2DDYtnXjxU1lMPlJJkSCIHbVmUSr1vx8RiNjzGJMeJvuTGG1cVce9xaXYaNnz+evHt0k5I1FHgHeX3rXM6dMsZa8RuUS6ue9jzhfVdkIKvQYxPNcVmgnZ03Z7wjhUziPwPexV2NxsicjAN/V1yf+EQ78nK9p1lYlDo7VqWu9xAONOZfY7Z3X9PaO1025HpmYWG0tp79Jo+ZjaZEvqHGDhUCaTzT15mvVddfqx4LJtPo3d8CDAAtEAR7NIeDUQAAAABJRU5ErkJggg=="]
+}
```

### Comparing `cs1-robots-0.1.6/src/easygui/__init__.py` & `cs1-robots-0.1.6.2/src/easygui/__init__.py`

 * *Files identical despite different names*

