# Comparing `tmp/art-daq-1.1.0.tar.gz` & `tmp/art-daq-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "art-daq-1.1.0.tar", last modified: Mon Mar 27 22:05:41 2023, max compression
+gzip compressed data, was "art-daq-1.1.2.tar", last modified: Thu Apr 27 09:29:41 2023, max compression
```

## Comparing `art-daq-1.1.0.tar` & `art-daq-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 22:05:41.630234 art-daq-1.1.0/
--rw-rw-rw-   0        0        0     1087 2023-03-18 07:37:39.000000 art-daq-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      714 2023-03-27 22:05:41.629232 art-daq-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      495 2023-03-20 19:46:13.000000 art-daq-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-27 22:05:41.620215 art-daq-1.1.0/art_daq/
--rw-rw-rw-   0        0        0     8583 2023-03-27 22:03:16.000000 art-daq-1.1.0/art_daq/MIN.py
--rw-rw-rw-   0        0        0     2167 2023-03-27 22:04:47.000000 art-daq-1.1.0/art_daq/__init__.py
--rw-rw-rw-   0        0        0    15517 2023-03-27 07:01:34.000000 art-daq-1.1.0/art_daq/daq.py
-drwxrwxrwx   0        0        0        0 2023-03-27 22:05:41.628232 art-daq-1.1.0/art_daq.egg-info/
--rw-rw-rw-   0        0        0      714 2023-03-27 22:05:41.000000 art-daq-1.1.0/art_daq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-03-27 22:05:41.000000 art-daq-1.1.0/art_daq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 22:05:41.000000 art-daq-1.1.0/art_daq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-03-27 22:05:41.000000 art-daq-1.1.0/art_daq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-27 22:05:41.000000 art-daq-1.1.0/art_daq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-27 22:05:41.630234 art-daq-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      937 2023-03-27 22:04:40.000000 art-daq-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 09:29:41.280942 art-daq-1.1.2/
+-rw-rw-rw-   0        0        0     1087 2023-03-18 07:37:39.000000 art-daq-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0      714 2023-04-27 09:29:41.279943 art-daq-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4330 2023-04-23 12:57:02.000000 art-daq-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 09:29:41.270937 art-daq-1.1.2/art_daq/
+-rw-rw-rw-   0        0        0     9272 2023-04-23 12:56:06.000000 art-daq-1.1.2/art_daq/MIN.py
+-rw-rw-rw-   0        0        0     2167 2023-04-23 12:56:13.000000 art-daq-1.1.2/art_daq/__init__.py
+-rw-rw-rw-   0        0        0    15663 2023-04-23 12:55:54.000000 art-daq-1.1.2/art_daq/daq.py
+drwxrwxrwx   0        0        0        0 2023-04-27 09:29:41.277937 art-daq-1.1.2/art_daq.egg-info/
+-rw-rw-rw-   0        0        0      714 2023-04-27 09:29:41.000000 art-daq-1.1.2/art_daq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-04-27 09:29:41.000000 art-daq-1.1.2/art_daq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 09:29:41.000000 art-daq-1.1.2/art_daq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-04-27 09:29:41.000000 art-daq-1.1.2/art_daq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-27 09:29:41.000000 art-daq-1.1.2/art_daq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 09:29:41.280942 art-daq-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      937 2023-04-23 12:55:41.000000 art-daq-1.1.2/setup.py
```

### Comparing `art-daq-1.1.0/LICENSE` & `art-daq-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `art-daq-1.1.0/PKG-INFO` & `art-daq-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: art-daq
-Version: 1.1.0
+Version: 1.1.2
 Summary: Paquete para usar la tarjeta de NI, USB-6001
 Home-page: https://github.com/Julumisan/art-daq
 Author: Juan Luis
 Author-email: julumisan@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `art-daq-1.1.0/art_daq/MIN.py` & `art-daq-1.1.2/art_daq/MIN.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,71 +3,72 @@
 Created on Fri Mar 24 22:34:59 2023
 
 @author: Julu
 
 Clase de testeo de la DAQ con iface gráfica para poder comprobar
 de manera sencilla y clara cómo está la tarjeta.
 
-TO DO: Comentar mejor antes de que se me olvide qué he hecho.
-
+v1.1.2
 """
 
 import tkinter as tk
-import matplotlib.pyplot as plt
 import numpy as np
 from tkinter import ttk
 from art_daq import daq
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 from matplotlib.figure import Figure
+from tkinter import messagebox
 
 class MIN:
 
     def __init__(self):
+        """
+        Inicializa la aplicación y configura la interfaz gráfica de usuario, los gráficos y la comunicación con el hardware.
+        """
         try:
             self.previous_channel = None  # Para poder cambiar la gráfica si cambio el canal
             self.setup_gui()
         finally:
             daq.safe_state(self.device_name)
-
-
-
-    # Configura la interfaz gráfica de usuario
+    
     def setup_gui(self):
-        # Configurar la ventana principal y el marco
+        """
+        Configura la interfaz gráfica de usuario.
+        """
         self.root = tk.Tk()
         self.root.title("DAQ Control")
         frame = ttk.Frame(self.root, padding="10")
         frame.grid(row=0, column=0, sticky=(tk.W, tk.E, tk.N, tk.S))
 
         # Configurar los widgets
         self.voltage_label = ttk.Label(frame, text="Voltage: -- V")
         self.voltage_label.grid(row=0, column=0, padx=5, pady=5, sticky=tk.W)
 
         input_channel_label = ttk.Label(frame, text="Select input channel:")
         input_channel_label.grid(row=1, column=0, padx=5, pady=5, sticky=tk.W)
 
-        self.input_channel_combobox = ttk.Combobox(frame, values=list(range(0, 9)), state="readonly", width=3)
+        self.input_channel_combobox = ttk.Combobox(frame, values=list(range(0, 8)), state="readonly", width=3)
         self.input_channel_combobox.set("0")
         self.input_channel_combobox.grid(row=1, column=1, padx=5, pady=5, sticky=tk.W)
 
         spinbox_label = ttk.Label(frame, text="Output voltage (0-5V):")
         spinbox_label.grid(row=2, column=0, padx=5, pady=5, sticky=tk.W)
 
         self.spinbox = ttk.Spinbox(frame, from_=0, to=5, increment=0.01, width=10)
         self.spinbox.grid(row=2, column=1, padx=5, pady=5, sticky=tk.W)
 
-        output_channel_label = ttk.Label(frame, text="Select output channel:")
+        output_channel_label = ttk.Label(frame, text="Select analog output channel:")
         output_channel_label.grid(row=4, column=0, padx=5, pady=5, sticky=tk.W)
 
         # Salida analógica
         self.output_channel_combobox = ttk.Combobox(frame, values=list(range(0,2)), state="readonly", width=3)
         self.output_channel_combobox.set("0")
         self.output_channel_combobox.grid(row=4, column=1, padx=5, pady=5, sticky=tk.W)
 
-        set_voltage_button = ttk.Button(frame, text="Set Voltage", command=self.set_output_voltage)
+        set_voltage_button = ttk.Button(frame, text="Set Analog Voltage", command=self.set_output_voltage)
         set_voltage_button.grid(row=3, column=1, padx=5, pady=5, sticky=tk.W)
 
         # Configurar el gráfico y el canvas
         self.setup_plot()
         self.canvas = FigureCanvasTkAgg(self.fig, master=self.root)
         self.canvas.get_tk_widget().grid(row=0, column=1, padx=10, pady=10, rowspan=6)
 
@@ -79,130 +80,141 @@
 
         self.digital_output_combobox = ttk.Combobox(frame, values=digital_output_options, state="readonly", width=15)
         self.digital_output_combobox.set("port0/line0")  # Establecer el valor predeterminado en "port0/line0"
         self.digital_output_combobox.grid(row=5, column=1, padx=5, pady=5, sticky=tk.W)
         self.digital_output_combobox.bind("<<ComboboxSelected>>", self.update_digital_output_label)
 
         self.digital_output_value = tk.BooleanVar()
-        self.digital_output_checkbutton = tk.Checkbutton(frame, text="Output value (True/False)", variable=self.digital_output_value)
+        self.digital_output_checkbutton = tk.Checkbutton(frame, text="Digital output value (True/False)", variable=self.digital_output_value)
         self.digital_output_checkbutton.grid(row=6, column=0, padx=5, pady=5, sticky=tk.W)
 
         set_digital_output_button = ttk.Button(frame, text="Set Digital Output", command=self.set_digital_output)
         set_digital_output_button.grid(row=6, column=1, padx=5, pady=5, sticky=tk.W)
-
+        
+        exit_button = ttk.Button(frame, text="Exit", command=self.confirm_exit, style="Red.TButton")
+        exit_button.grid(row=7, column=1, padx=5, pady=5, sticky=tk.W)
+        
+        style = ttk.Style()
+        style.configure("Red.TButton", foreground="red")
+    
         self.update_digital_output_label()
         
         # Iniciar la actualización de la etiqueta de voltaje y el bucle principal
         self.root.after(1000, self.update_voltage_label)
         self.root.mainloop()
-
-
         
-    # Configura el gráfico
     def setup_plot(self):
-        # Configurar el gráfico y los ejes
+        """
+        Configura el gráfico y los ejes.
+        """
         self.fig = Figure(figsize=(5, 4))
         self.ax = self.fig.add_subplot(111)
         self.ax.set_title("Analog Input")
         self.ax.set_xlabel("Time (s)")
         self.ax.set_ylabel("Voltage (V)")
         self.ax.grid()
         self.plot_data = self.ax.plot([], [], 'r-')[0]
         self.plot_x = np.array([])
         self.plot_y = np.array([])
         self.time_counter = 0
-        
-
-
-    # Actualizar la gráfica
+    
     def update_plot(self, voltage):
-        # Agregar nuevos datos al gráfico y actualizar
+        """
+        Agrega nuevos datos al gráfico y lo actualiza.
+        
+        Args:
+            voltage (float): Voltaje a cambiar.
+        """
         self.plot_x = np.append(self.plot_x, self.time_counter)
         self.plot_y = np.append(self.plot_y, voltage)
         self.time_counter += 0.1
-    
+        
         self.plot_data.set_data(self.plot_x, self.plot_y)
         
         # Si el tiempo actual es mayor a 10 segundos
         if self.time_counter > 10:
             x_min = self.time_counter - 10  # Ajusta el límite inferior del eje x
         else:
             x_min = 0
         
         self.ax.set_xlim(x_min, self.time_counter)
         self.ax.relim()  # Recalcular los límites de los datos en el eje y
         self.ax.autoscale_view(True, True, True)  # Autoajustar el eje y
         self.canvas.draw()
-        
-        
-        
-    # Reiniciar la gráfica
+    
     def reset_plot(self):
+        """
+        Reinicia el gráfico.
+        """
         self.plot_x = np.array([])
         self.plot_y = np.array([])
         self.time_counter = 0
         self.plot_data.set_data(self.plot_x, self.plot_y)
         self.ax.set_xlim(0, self.time_counter)
         self.canvas.draw()
-
-
-
-    # Actualiza la etiqueta de voltaje
+    
     def update_voltage_label(self):
+        """
+        Actualiza la etiqueta de voltaje.
+        """
         self.device_name = daq.get_connected_device()
         if self.device_name:
-            selected_channel = self.input_channel_combobox.get()
-            
-            # Comdaq si el canal seleccionado ha cambiado
-            if self.previous_channel != selected_channel:
-                self.reset_plot()  # Reinicia la gráfica si el canal cambia
-                self.previous_channel = selected_channel
-            
-            chan_a = self.device_name + "/ai{}".format(selected_channel)
-            voltage = daq.get_voltage_analogic(chan_a)
-            self.voltage_label.config(text="Voltage: {:.6f} V".format(voltage))
-            self.update_plot(voltage)
+           selected_channel = self.input_channel_combobox.get()
+           
+           # Comdaq si el canal seleccionado ha cambiado
+           if self.previous_channel != selected_channel:
+               self.reset_plot()  # Reinicia la gráfica si el canal cambia
+               self.previous_channel = selected_channel
+           
+           chan_a = self.device_name + "/ai{}".format(selected_channel)
+           voltage = daq.get_voltage_analogic(chan_a)
+           self.voltage_label.config(text="Voltage: {:.6f} V".format(voltage))
+           self.update_plot(voltage)
         else:
-            self.voltage_label.config(text="No hay dispositivos conectados")
+           self.voltage_label.config(text="No hay dispositivos conectados")
         self.root.after(100, self.update_voltage_label)
-        
-        
-        
-    # Establece el voltaje de salida
+    
     def set_output_voltage(self):
+        """
+        Establece el voltaje de salida.
+        """
         device_name = daq.get_connected_device()
         if device_name:
             # Leer el canal de salida seleccionado
             selected_channel = self.output_channel_combobox.get()
             chan_a = device_name + "/ao{}".format(selected_channel)
             voltage = float(self.spinbox.get())
             daq.set_voltage_analogic(chan_a, voltage)
-
-
-
-    # Establecer la salida digital
+    
     def set_digital_output(self):
+        """
+        Establece la salida digital.
+        """
         device_name = daq.get_connected_device()
         if device_name:
             selected_channel = self.digital_output_combobox.get()
             chan_d = device_name + "/" + selected_channel  # Actualizar el formato del canal
             state = self.digital_output_value.get()
             daq.set_voltage_digital(chan_d, state)
             self.update_digital_output_label()
-
-
-
-    # Actualizar la etiqueta de salida digital
+    
     def update_digital_output_label(self, event=None):
+        """
+        Actualiza la etiqueta de salida digital.
+        """
         device_name = daq.get_connected_device()
         if device_name:
             selected_channel = self.digital_output_combobox.get()
             chan_d = device_name + "/" + selected_channel  # Actualizar el formato del canal
             state = daq.get_state_digital(chan_d)
             self.digital_output_value.set(state)
             self.digital_output_checkbutton.config(text="Output value (True/False): {}".format(state))
         else:
             self.digital_output_checkbutton.config(text="Output value (True/False): --")
             
-
+            
+    def confirm_exit(self):
+        if messagebox.askyesno("Exit", "Are you sure you want to exit?"):
+            self.root.destroy()        
+            
 if __name__ == "__main__":
     min_app = MIN()
```

### Comparing `art-daq-1.1.0/art_daq/__init__.py` & `art-daq-1.1.2/art_daq/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sat Mar 18 16:05:36 2023
 
 @author: Julu
-@version: 1.1.0
+@version: 1.1.2
 
 El archivo init.py es necesario para que Python reconozca que este es un paquete. Debe estar vacío para evitar una dependencia cíclica.
 
 Para utilizar la librería, se debe importar de la siguiente manera: "from art_daq import daq"
 
 La siguiente es una lista de las funciones que se encuentran en este paquete:
```

### Comparing `art-daq-1.1.0/art_daq/daq.py` & `art-daq-1.1.2/art_daq/daq.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     -Temporizador.
     -Posibilidad de elección automática de tarjeta con get_connected_device
     -Generación de ondas cuadradas/triangulares/sinusoidales
 
 
 @author: Julu
 
-@version: v1.0.0
+@version: v1.1.2
 
 Esta nueva versión cuenta con todas las funcionalidades previstas, comentarios
 aclaratorios acerca del uso de las funciones, tanto de su función como de 
 qué parámetros se usan y su formato.
 
 """
 
@@ -28,254 +28,261 @@
 import time
 import math
 
 
 
 def measure_frequency(counter_channel: str, input_terminal: str, duration: float) -> float:
     """
-    Esta función mide la frecuencia de una señal utilizando el contador.
-    La función configura el contador para medir la frecuencia y conecta el
+    Mide la frecuencia de una señal utilizando el contador.
+
+    Esta función configura el contador para medir la frecuencia y conecta el
     terminal de entrada especificado a la señal que se desea medir. Después
     de medir la frecuencia durante la duración especificada, la función
     devuelve la frecuencia medida.
-    
-    @param counter_channel: el número del canal del contador a utilizar.
-    @param input_terminal: el nombre del terminal de entrada al que está conectada la señal que se desea medir.
-    @param duration: la duración de la medición de la frecuencia en segundos.
-    
-    @return: la frecuencia medida en Hz.
-    
+
+    Args:
+        counter_channel (str): El número del canal del contador a utilizar.
+        input_terminal (str): El nombre del terminal de entrada al que está conectada la señal que se desea medir.
+        duration (float): La duración de la medición de la frecuencia en segundos.
+
+    Returns:
+        float: La frecuencia medida en Hz.
     """
     with nidaqmx.Task() as task:
-        # Configurar la medida de frecuencia
+        # Configura la medida de frecuencia
         task.ci_channels.add_ci_freq_meas_chan(counter_channel,
                                                '',
                                                min_val=1.0,
                                                max_val=10000.0,
                                                edge=nidaqmx.constants.Edge.RISING,
                                                meas_method=nidaqmx.constants.AcquisitionType.FINITE,
                                                meas_time=duration,
                                                timeout=10000.0,
-                                               units=nidaqmx.constantsTimeUnits.SECONDS,
+                                               units=nidaqmx.constants.TimeUnits.SECONDS,
                                                custom_scale_name='',
                                                divisor=4
                                                )
         
-        # Conectar el terminal de entrada a la señal que se desea medir
+        # Conecta el terminal de entrada a la señal que se desea medir
         task.ci_channels.all.connect_terms(input_terminal, '')
 
-        # Leer y retornar la frecuencia medida
+        # Lee y retorna la frecuencia medida
         frequency = task.read()
         return frequency
 
 
-
 def daq_timer(chan_a: str, duration: float) -> None:
     """
-    Esta función configura una tarea de adquisición de datos que espera durante
-    una cantidad de tiempo determinada.
-    
-    
-    @param chan_a: el nombre del canal de entrada analógica.
-    @param duration: la duración de la adquisición de datos en segundos.
+    Configura una tarea de adquisición de datos que espera durante una cantidad de tiempo determinada.
+
+    Args:
+        chan_a (str): El nombre del canal de entrada analógica.
+        duration (float): La duración de la adquisición de datos en segundos.
     """
     with nidaqmx.Task() as task:
         # Se agrega un canal de entrada analógica al objeto de tarea. "Dev/aiX"
         # es el identificador del canal de entrada.
         ai_channel = task.ai_channels.add_ai_voltage_chan(chan_a)
-        
+
         # Se configura el temporizador de la tarea para utilizar el reloj interno
         # del dispositivo. El temporizador espera durante la duración especificada
         # (en segundos), adquiriendo muestras a una tasa de 1000 muestras por segundo.
         # El modo de muestra es FINITE, lo que significa que la tarea se detendrá
         # automáticamente después de adquirir un número específico de muestras.
         task.timing.cfg_samp_clk_timing(
-            rate=1000, 
-            sample_mode=nidaqmx.constants.AcquisitionType.FINITE, 
-            samps_per_chan=duration*1000, 
+            rate=1000,
+            sample_mode=nidaqmx.constants.AcquisitionType.FINITE,
+            samps_per_chan=duration*1000,
             source="OnboardClock"
         )
-        
+
         # Se inicia la tarea.
         task.start()
-        
+
         # Se espera hasta que la tarea haya terminado de adquirir muestras.
         task.wait_until_done()
 
 
 # No he encontrado nada que haga esto de una manera mejor/más optimizada.
 def all_digital_safe(device_name: str) -> None:
     """
-    Función para que todas las líneas de salida estén a 0. 
-    Pensado para ser usado en una función mayor, la cual ponga
-    todas las salidas a un estado seguro y conocido. 
-    
-    
-    @param device_name: el nombre del dispositivo DAQ.
+    Establece todas las líneas de salida de un dispositivo NI en 0. 
+    Pensado para ser usado en una función mayor que establezca todas las salidas en un estado seguro y conocido.
+
+    Args:
+        device_name (str): El nombre del dispositivo DAQ.
     """
     # Dado un device_name se recibe una lista con todas las líneas de salida
     available_channels = nidaqmx.system._collections.physical_channel_collection.DOLinesCollection(device_name)
     # Por cada canal en la lista cambiar el tipo a string para poder dividirlo y conseguir sólo el nombre
     for channel in available_channels:
         channel_name = str(channel).split('=')[1][:-1]
         # Una vez con el nombre de cada canal se ponen a 0 uno a uno
         set_voltage_digital(channel_name, False)
 
 
 
 
 def all_analogic_safe(device_name: str) -> list:
     """
-    Función para que todos los canales analógicos de salida estén a 0. 
-    Pensado para ser usado en una función mayor, la cual ponga
-    todas las salidas a un estado seguro y conocido. 
-    Devuelve un array con los voltajes puestos.
-    
-    
-    @param device_name: el nombre del dispositivo DAQ.
-    @return: un array de los voltajes puestos en los canales analógicos de salida del dispositivo.
+    Establece todos los canales analógicos de salida de un dispositivo NI en 0. 
+    Pensado para ser usado en una función mayor que establezca todas las salidas en un estado seguro y conocido.
+
+    Args:
+        device_name (str): El nombre del dispositivo DAQ.
+
+    Returns:
+        list: Un array de los voltajes establecidos en los canales analógicos de salida del dispositivo.
     """
     voltajes = []
     for i in range(2):
         voltajes.append(set_voltage_analogic((device_name+"/ao{}".format(i)),0))      
     return voltajes
     
 
 
 def get_voltage_analogic(chan_a: str) -> float:
     """
-    Acceso al voltaje del canal analógico de entrada. 
-    chan_a tiene el formato " "Dev/aiX" "
-    
-    
-    @param chan_a: el identificador del canal analógico de entrada, en el formato "Dev/aiX".
-    @return: el voltaje actual en el canal analógico de entrada.
+    Accede al voltaje actual de un canal analógico de entrada especificado en el dispositivo NI.
+
+    Args:
+        chan_a (str): El identificador del canal analógico de entrada, en el formato "Dev/aiX".
+
+    Returns:
+        float: El voltaje actual en el canal analógico de entrada.
     """
     with nidaqmx.Task() as task:
         task.ai_channels.add_ai_voltage_chan(chan_a, terminal_config=nidaqmx.constants.TerminalConfiguration.RSE)
         # Leer el voltaje actual del canal ai0 10 veces
         voltages = task.read(number_of_samples_per_channel=10)
         # Calcular la media de los valores leídos
         mean_voltage = sum(voltages)/len(voltages)
-        return mean_voltage     
+        return mean_voltage 
 
 
 
 def get_state_digital(chan_d: str) -> bool:
     """
-    Acceso al estado del canal digital. 
-    chan_d tiene el formato " "Dev/portX/lineY" "
-    
-    
-    @param chan_d: el identificador del canal digital de salida, en el formato "Dev/portX/lineY".
-    @return: el estado actual del canal digital de salida (True si está activado, False si está desactivado).
+    Accede al estado actual de un canal digital de salida especificado en el dispositivo NI.
+
+    Args:
+        chan_d (str): El identificador del canal digital de salida, en el formato "Dev/portX/lineY".
+
+    Returns:
+        bool: El estado actual del canal digital de salida (True si está activado, False si está desactivado).
     """
     with nidaqmx.Task() as task:
         task.do_channels.add_do_chan(chan_d)
         state = task.read()
         return state
 
 
 
 def set_voltage_analogic(chan_a: str, voltage: float) -> float:
     """
-    Cambios de voltaje de un canal análogico.
-    chan_a tiene el formato " "Dev/aoX" "
-    Al no poder leerse el voltaje (por ser de salida), por si 
-    se necesita saber algún cambio se fuerza a que devuelva el voltaje
-    
-    
-    @param chan_a: el identificador del canal analógico de salida, en el formato "Dev/aoX".
-    @param voltage: el voltaje a establecer en el canal analógico de salida.
-    @return: el voltaje establecido en el canal analógico de salida.
+    Establece el voltaje de un canal analógico de salida especificado en el dispositivo NI.
+
+    Args:
+        chan_a (str): El identificador del canal analógico de salida, en el formato "Dev/aoX".
+        voltage (float): El voltaje a establecer en el canal analógico de salida.
+
+    Returns:
+        float: El voltaje establecido en el canal analógico de salida.
     """
     with nidaqmx.Task() as task:
         task.ao_channels.add_ao_voltage_chan(chan_a) # Especificar la salida analógica chanA del dispositivo DAQ
         task.write(voltage, auto_start=True) # Establecer el voltaje en chanA
         return voltage
 
 
 
 def set_voltage_digital(chan_d: str, voltage: bool) -> None:
     """
     Cambios de voltaje de un canal digital.
     chan_d tiene el formato " "Dev/portX/lineY" "
     
-    
-    @param chan_d: el identificador del canal digital de salida, en el formato "Dev/portX/lineY".
-    @param voltage: el estado a establecer en el canal digital de salida (True para encender, False para apagar).
+    Args:
+        chan_d: el identificador del canal digital de salida, en el formato "Dev/portX/lineY".
+        voltage: el estado a establecer en el canal digital de salida (True para encender, False para apagar).
+    Returns:
+        None
+        
     """   
     with nidaqmx.Task() as task:
         task.do_channels.add_do_chan(chan_d) # Especificar la salida digital X.Y del dispositivo DAQ
         task.write(voltage) # Establecer el voltaje en el canal digital
         
     
         
 def safe_state(device_name: str) -> None:
     """
-    Función que va a servir para establecer un voltaje seguro y conocido en todas las salidas.
-    Recomiendado el uso para iniciar y finalizar el programa.
-    
-    
-    @param device_name: el nombre del dispositivo NI.
+    Establece un voltaje seguro y conocido en todas las salidas de un dispositivo NI. Se recomienda su uso para iniciar y
+    finalizar el programa.
+
+    Args:
+        device_name (str): El nombre del dispositivo NI.
     """
     all_digital_safe(device_name)
     all_analogic_safe(device_name)
   
+    
    
-  
 def get_connected_devices() -> list:
     """
-    Función que crea una instancia de la clase nidaqmx.system.System que representa el
-    sistema local. Luego, recopila los nombres de todos los dispositivos NI conectados
-    en una lista llamada connected_devices y la devuelve.
-    
-    
-    La función no recibe argumentos.
-    @return: una lista de los nombres de todos los dispositivos NI conectados al sistema local.
+    Crea una instancia de la clase nidaqmx.system.System que representa el sistema local. Luego, recopila los nombres de
+    todos los dispositivos NI conectados en una lista llamada connected_devices y la devuelve.
+
+    Returns:
+        list: Una lista de los nombres de todos los dispositivos NI conectados al sistema local.
     """
     system = nidaqmx.system.System.local()
     connected_devices = [dev.name for dev in system.devices]
     return connected_devices
 
 
-
 def get_connected_device() -> str:
     """
-    Función que crea una instancia de la función get_connected_devices() para comprobar
-    que solo haya un device conectado, y, si lo hay, se devuelve. 
-    Utilidad: No necesidad de interacción humana por si cambia el devicename.
+    Crea una instancia de la función get_connected_devices() para comprobar que solo hay un dispositivo conectado.
+    Si hay exactamente un dispositivo conectado, devuelve su nombre.
     
-    
-    La función no recibe argumentos.
+    Utilidad: Permite automatizar la selección del dispositivo, sin necesidad de interacción humana en caso de cambio de 
+    nombre del dispositivo.
 
-    @return: el nombre del único dispositivo NI conectado al sistema local, o None si no se detectó exactamente un 
-         dispositivo.
-    """
-    listDev = get_connected_devices()
-    if len(listDev) == 1:
-        return listDev[0]
+    Returns:
+        str: El nombre del único dispositivo NI conectado al sistema local, o None si no se detectó exactamente un 
+        dispositivo.
+    """
+    list_dev = get_connected_devices()
+    if len(list_dev) == 1:
+        return list_dev[0]
     else:
         print("Se necesita acción programativa")
         
 
 
 def generate_square_wave(device_name: str, ao_channel: int, frequency: float, amplitude: float, duration: float) -> None:
     """
     Genera una onda cuadrada de la frecuencia y amplitud especificadas en el canal analógico de salida especificado en el 
     dispositivo NI especificado durante la duración especificada.
 
-    La función recibe el nombre del dispositivo NI, el número del canal analógico de salida, la frecuencia de la onda 
-    cuadrada, la amplitud de la onda cuadrada y la duración durante la cual se generará la onda cuadrada. No devuelve nada.
+    Args:
+        device_name (str): El nombre del dispositivo NI.
+        ao_channel (int): El número del canal analógico de salida.
+        frequency (float): La frecuencia de la onda cuadrada en Hz.
+        amplitude (float): La amplitud de la onda cuadrada en voltios.
+        duration (float): La duración durante la cual se generará la onda cuadrada en segundos.
+
+    Returns:
+        None
+
+    Notas:
+        Esta función establece el voltaje en la amplitud deseada durante la mitad del periodo de la onda cuadrada y
+        en -amplitud durante la otra mitad. Luego espera la mitad del periodo antes de repetir. La implementación asume
+        que el periodo es mayor que el tiempo de espera.
 
-    @param device_name: el nombre del dispositivo NI.
-    @param ao_channel: el número del canal analógico de salida.
-    @param frequency: la frecuencia de la onda cuadrada en Hz.
-    @param amplitude: la amplitud de la onda cuadrada en voltios.
-    @param duration: la duración durante la cual se generará la onda cuadrada en segundos.
     """
     chan_a = f"{device_name}/ao{ao_channel}"
     
     period = 1 / frequency
     half_period = period / 2
 
     start_time = time.time()
@@ -349,37 +356,41 @@
         
 
 
 def generate_sine_wave(device_name: str, ao_channel: int, frequency: float, amplitude: float, duration: float) -> None:
     """
     Genera una señal sinusoidal en el canal de salida analógica especificado durante la duración especificada.
     El voltaje sinusoidal se calcula en función del tiempo utilizando la frecuencia y la amplitud especificadas.
-    
-    @param device_name: el nombre del dispositivo DAQ.
-    @param ao_channel: el número del canal de salida analógica en el que se generará la señal.
-    @param frequency: la frecuencia de la señal sinusoidal en Hz.
-    @param amplitude: la amplitud máxima de la señal sinusoidal en V.
-    @param duration: la duración de la señal sinusoidal en segundos.
-    """
-    # NI PRECISO, NI ESTABLE. PARA ESTE TIPO DE SEÑALES MEJOR UN DAQ QUE PUEDA HACERLO
-    # CONSUME MUCHA CPU debido a la creación y destrucción de tareas
-    # en cada iteración del bucle.
-    
-    # Construir el nombre del canal de salida analógica
+
+    Args:
+        device_name (str): El nombre del dispositivo DAQ.
+        ao_channel (int): El número del canal de salida analógica en el que se generará la señal.
+        frequency (float): La frecuencia de la señal sinusoidal en Hz.
+        amplitude (float): La amplitud máxima de la señal sinusoidal en V.
+        duration (float): La duración de la señal sinusoidal en segundos.
+
+    Returns:
+        None
+
+    Notas:
+        Esta implementación no es precisa ni estable. Para este tipo de señales, se recomienda usar un DAQ que pueda
+        manejarlas eficientemente. Esta implementación también consume mucha CPU debido a la creación y destrucción de
+        tareas en cada iteración del bucle.
+    """
     chan_a = f"{device_name}/ao{ao_channel}"
-    
+
     start_time = time.time()
     current_time = start_time
 
     while current_time - start_time < duration:
         # Calcular el voltaje sinusoidal en función del tiempo
         elapsed_time = current_time - start_time
         voltage = amplitude * math.sin(2 * math.pi * frequency * elapsed_time)
-        
+
         # Establecer el voltaje en el canal de salida analógica
         with nidaqmx.Task() as task:
             task.ao_channels.add_ao_voltage_chan(chan_a)
             task.write(voltage)
-        
+
         # Esperar un corto período de tiempo antes de actualizar el voltaje nuevamente
         time.sleep(0.001)  # 1 ms
         current_time = time.time()
```

### Comparing `art-daq-1.1.0/art_daq.egg-info/PKG-INFO` & `art-daq-1.1.2/art_daq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: art-daq
-Version: 1.1.0
+Version: 1.1.2
 Summary: Paquete para usar la tarjeta de NI, USB-6001
 Home-page: https://github.com/Julumisan/art-daq
 Author: Juan Luis
 Author-email: julumisan@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `art-daq-1.1.0/setup.py` & `art-daq-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 """
 
 from setuptools import setup
 
 setup(
     name='art-daq',
-    version='1.1.0',
+    version='1.1.2',
     description='Paquete para usar la tarjeta de NI, USB-6001',
     packages=['art_daq'],
     install_requires=[
         'nidaqmx',
         'matplotlib',
         'numpy'
     ],
```

