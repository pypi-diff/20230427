# Comparing `tmp/robotframework_robosapiens-1.1.6-py3-none-any.whl.zip` & `tmp/robotframework_robosapiens-1.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 403748 bytes, number of entries: 17
--rw-rw-rw-  2.0 fat    32251 b- defN 23-Apr-26 11:46 RoboSAPiens/__init__.py
--rw-rw-rw-  2.0 fat     3487 b- defN 23-Apr-26 11:42 RoboSAPiens/client.py
--rw-rw-rw-  2.0 fat    36002 b- defN 23-Apr-26 11:46 RoboSAPiens/DE/__init__.py
+Zip file size: 404053 bytes, number of entries: 17
+-rw-rw-rw-  2.0 fat    32308 b- defN 23-Apr-27 19:06 RoboSAPiens/__init__.py
+-rw-rw-rw-  2.0 fat     3850 b- defN 23-Apr-27 19:04 RoboSAPiens/client.py
+-rw-rw-rw-  2.0 fat    36059 b- defN 23-Apr-27 19:06 RoboSAPiens/DE/__init__.py
 -rw-rw-rw-  2.0 fat   187392 b- defN 21-Nov-23 21:13 RoboSAPiens/lib/CsvHelper.dll
 -rw-rw-rw-  2.0 fat    49664 b- defN 19-Feb-01 18:19 RoboSAPiens/lib/Horizon.XmlRpc.Core.dll
 -rw-rw-rw-  2.0 fat    19456 b- defN 19-Feb-01 18:19 RoboSAPiens/lib/Horizon.XmlRpc.Server.dll
--rw-rw-rw-  2.0 fat     3181 b- defN 23-Apr-26 11:46 RoboSAPiens/lib/RoboSAPiens.deps.json
--rw-rw-rw-  2.0 fat   266752 b- defN 23-Apr-26 11:46 RoboSAPiens/lib/RoboSAPiens.dll
--rw-rw-rw-  2.0 fat   118784 b- defN 23-Apr-26 11:46 RoboSAPiens/lib/RoboSAPiens.exe
--rw-rw-rw-  2.0 fat      253 b- defN 23-Apr-26 11:46 RoboSAPiens/lib/RoboSAPiens.runtimeconfig.json
+-rw-rw-rw-  2.0 fat     3181 b- defN 23-Apr-27 19:05 RoboSAPiens/lib/RoboSAPiens.deps.json
+-rw-rw-rw-  2.0 fat   266752 b- defN 23-Apr-27 19:05 RoboSAPiens/lib/RoboSAPiens.dll
+-rw-rw-rw-  2.0 fat   118784 b- defN 23-Apr-27 19:05 RoboSAPiens/lib/RoboSAPiens.exe
+-rw-rw-rw-  2.0 fat      253 b- defN 23-Apr-27 19:05 RoboSAPiens/lib/RoboSAPiens.runtimeconfig.json
 -rw-rw-rw-  2.0 fat    21128 b- defN 19-Feb-01 18:19 RoboSAPiens/lib/System.ComponentModel.Composition.dll
 -rw-rw-rw-  2.0 fat   388096 b- defN 22-Oct-28 02:14 RoboSAPiens/lib/sapfewse.dll
 -rw-rw-rw-  2.0 fat     4096 b- defN 22-Oct-28 02:14 RoboSAPiens/lib/saprotwr.net.dll
--rw-rw-rw-  2.0 fat     2145 b- defN 23-Apr-26 11:46 robotframework_robosapiens-1.1.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-26 11:46 robotframework_robosapiens-1.1.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Apr-26 11:46 robotframework_robosapiens-1.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1564 b- defN 23-Apr-26 11:46 robotframework_robosapiens-1.1.6.dist-info/RECORD
-17 files, 1134355 bytes uncompressed, 401152 bytes compressed:  64.6%
+-rw-rw-rw-  2.0 fat     2171 b- defN 23-Apr-27 19:06 robotframework_robosapiens-1.1.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-27 19:06 robotframework_robosapiens-1.1.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Apr-27 19:06 robotframework_robosapiens-1.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1564 b- defN 23-Apr-27 19:06 robotframework_robosapiens-1.1.7.dist-info/RECORD
+17 files, 1134858 bytes uncompressed, 401457 bytes compressed:  64.6%
```

## zipnote {}

```diff
@@ -33,20 +33,20 @@
 
 Filename: RoboSAPiens/lib/sapfewse.dll
 Comment: 
 
 Filename: RoboSAPiens/lib/saprotwr.net.dll
 Comment: 
 
-Filename: robotframework_robosapiens-1.1.6.dist-info/METADATA
+Filename: robotframework_robosapiens-1.1.7.dist-info/METADATA
 Comment: 
 
-Filename: robotframework_robosapiens-1.1.6.dist-info/WHEEL
+Filename: robotframework_robosapiens-1.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: robotframework_robosapiens-1.1.6.dist-info/top_level.txt
+Filename: robotframework_robosapiens-1.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: robotframework_robosapiens-1.1.6.dist-info/RECORD
+Filename: robotframework_robosapiens-1.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## RoboSAPiens/__init__.py

```diff
@@ -35,15 +35,15 @@
             'presenter_mode': presenter_mode,
         }
         
         super().__init__(args)
     
 
     @keyword('Select Tab') # type: ignore
-    def ActivateTab(self, tabname: str): # type: ignore
+    def activate_tab(self, tabname: str): # type: ignore
         """
         Select the tab with the name provided.
         
         | ``Select Tab    tabname``
         """
         
         args = {
@@ -57,15 +57,15 @@
             "Pass": "The tab {0} was selected",
             "Exception": "The tab could not be selected. {0}\nFor more details run 'robot --loglevel DEBUG test.robot' and consult the file log.html"
         }
         return super()._run_keyword('ActivateTab', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Open SAP') # type: ignore
-    def OpenSAP(self, path: str): # type: ignore
+    def open_s_a_p(self, path: str): # type: ignore
         """
         Open the SAP GUI. The standard path is\n\n| ``C:\\Program Files (x86)\\SAP\\FrontEnd\\SAPgui\\saplogon.exe``
         """
         
         args = {
             'Pfad': path,
         }
@@ -75,15 +75,15 @@
             "SAPNotStarted": "The SAP GUI could not be opened. Verify that the path is correct.",
             "Exception": "The SAP GUI could not be opened. {0}\nFor more details run 'robot --loglevel DEBUG test.robot' and consult the file log.html"
         }
         return super()._run_keyword('OpenSAP', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Disconnect from Server') # type: ignore
-    def CloseConnection(self, ): # type: ignore
+    def close_connection(self, ): # type: ignore
         """
         Terminate the connection to the SAP server.
         """
         
         args = {
         }
         
@@ -95,15 +95,15 @@
             "Pass": "Disconnected from the server.",
             "Exception": "Could not disconnect from the server. {0}\nFor more details run 'robot --loglevel DEBUG test.robot' and consult the file log.html"
         }
         return super()._run_keyword('CloseConnection', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Close SAP') # type: ignore
-    def CloseSAP(self, ): # type: ignore
+    def close_s_a_p(self, ): # type: ignore
         """
         Close the SAP GUI
         """
         
         args = {
         }
         
@@ -111,15 +111,15 @@
             "NoSapGui": "No open SAP GUI found. Call the keyword \"Open SAP\" first.",
             "Pass": "The SAP GUI was closed."
         }
         return super()._run_keyword('CloseSAP', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Export Function Tree') # type: ignore
-    def ExportTree(self, filepath: str): # type: ignore
+    def export_tree(self, filepath: str): # type: ignore
         """
         Export the function tree in JSON format to the file provided.
         
         | ``Export Function Tree     filepath``
         """
         
         args = {
@@ -132,15 +132,15 @@
             "Pass": "The function tree was exported to {0}",
             "Exception": "The function tree could not be exported. {0}\nFor more details run 'robot --loglevel DEBUG test.robot' and consult the file log.html"
         }
         return super()._run_keyword('ExportTree', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Connect to Running SAP') # type: ignore
-    def AttachToRunningSAP(self, ): # type: ignore
+    def attach_to_running_s_a_p(self, ): # type: ignore
         """
         Connect to a running SAP instance and take control of it.
         """
         
         args = {
         }
         
@@ -152,15 +152,15 @@
             "Pass": "Connected to a running SAP instance.",
             "Exception": "Could not connect to a running SAP instance. {0}\nFor more details run 'robot --loglevel DEBUG test.robot' and consult the file log.html"
         }
         return super()._run_keyword('AttachToRunningSAP', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Connect to Server') # type: ignore
-    def ConnectToServer(self, servername: str): # type: ignore
+    def connect_to_server(self, servername: str): # type: ignore
         """
         Connect to the SAP Server provided.
         
         | ``Connect to Server    servername``
         """
         
         args = {
@@ -175,15 +175,15 @@
             "NoServerScripting": "Scripting is not activated on the server side. Please consult the documentation of RoboSAPiens.",
             "Exception": "Could not establish the connection. {0}\nFor more details run 'robot --loglevel DEBUG test.robot' and consult the file log.html"
         }
         return super()._run_keyword('ConnectToServer', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Double-click Cell') # type: ignore
-    def DoubleClickCell(self, row_number_or_cell_content: str, column: str): # type: ignore
+    def double_click_cell(self, row_number_or_cell_content: str, column: str): # type: ignore
         """
         Double-click the cell at the intersection of the row and the column provided.
         
         | ``Double-click Cell     row_locator     column``
         row_locator: either the row number or the content of a cell in the row.
         """
         
@@ -198,15 +198,15 @@
             "Pass": "The cell with the locator '{0}, {1}' was double-clicked.",
             "Exception": "The cell could not be double-clicked. {0}\nFor more details run 'robot --loglevel DEBUG test.robot' and consult the file log.html"
         }
         return super()._run_keyword('DoubleClickCell', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Double-click Text Field') # type: ignore
-    def DoubleClickTextField(self, content: str): # type: ignore
+    def double_click_text_field(self, content: str): # type: ignore
         """
         Double click the text field with the content provided.
         
         | ``Double-click Text Field     Content``
         """
         
         args = {
@@ -219,15 +219,15 @@
             "Pass": "The text field with the content '{0}' was double-clicked.",
             "Exception": "The text field could not be double-clicked. {0}\nFor more details run 'robot --loglevel DEBUG test.robot' and consult the file log.html"
         }
         return super()._run_keyword('DoubleClickTextField', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Execute Transaction') # type: ignore
-    def ExecuteTransaction(self, T_Code: str): # type: ignore
+    def execute_transaction(self, T_Code: str): # type: ignore
         """
         Execute the transaction with the given T-Code.
         
         | ``Execute Transaction    T_Code``
         """
         
         args = {
@@ -239,15 +239,15 @@
             "Pass": "The transaction with T-Code {0} was executed.",
             "Exception": "The transaction could not be executed. {0}\nFor more details run 'robot --loglevel DEBUG test.robot' and consult the file log.html"
         }
         return super()._run_keyword('ExecuteTransaction', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Export Dynpro') # type: ignore
-    def ExportForm(self, name: str, directory: str): # type: ignore
+    def export_form(self, name: str, directory: str): # type: ignore
         """
         Write all texts in the Dynpro to a CSV file. Also a screenshot will be saved in PNG format.
         
         | ``Export Dynpro     name     directory``
         directory: Absolute path to the directory where the files will be saved.
         """
         
@@ -261,15 +261,15 @@
             "Pass": "The Dynpro was exported to the CSV file {0} and the PNG image {1}",
             "Exception": "The Dynpro could not be exported. {0}\nFor more details run 'robot --loglevel DEBUG test.robot' and consult the file log.html"
         }
         return super()._run_keyword('ExportForm', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Fill Cell') # type: ignore
-    def FillTableCell(self, row_number_or_content: str, column_equals_content: str): # type: ignore
+    def fill_table_cell(self, row_number_or_content: str, column_equals_content: str): # type: ignore
         """
         Fill the cell at the intersection of the row and the column specified with the content provided.
         
         | ``Fill Cell     row     column = content``
         row: either the row number or the contents of a cell in the row.
         
         *Hint*: Some cells can be filled using the keyword 'Fill Text Field' providing as locator the description obtained by selecting the cell and pressing F1.
@@ -288,15 +288,15 @@
             "Pass": "The cell with the locator '{0}, {1}' was filled.",
             "Exception": "The cell could not be filled. {0}\nFor more details run 'robot --loglevel DEBUG test.robot' and consult the file log.html"
         }
         return super()._run_keyword('FillTableCell', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Fill Text Field') # type: ignore
-    def FillTextField(self, locator: str, content: str): # type: ignore
+    def fill_text_field(self, locator: str, content: str): # type: ignore
         """
         Fill the text Field specified by the locator with the content provided.
         
         *Text field with a label to its left*
         | ``Fill Text Field    label    content``
         *Text field with a label above*
         | ``Fill Text Field    @ label    content``
@@ -325,15 +325,15 @@
             "Pass": "The text field with the locator '{0}' was filled.",
             "Exception": "The text field could not be filled. {0}\nFor more details run 'robot --loglevel DEBUG test.robot' and consult the file log.html"
         }
         return super()._run_keyword('FillTextField', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Push Button') # type: ignore
-    def PushButton(self, name_or_tooltip: str): # type: ignore
+    def push_button(self, name_or_tooltip: str): # type: ignore
         """
         Push the button with the given name or tooltip.
         
         | ``Push Button    name or tooltip``
         """
         
         args = {
@@ -347,15 +347,15 @@
             "Pass": "The button '{0}' was pushed.",
             "Exception": "The button could not be pushed. {0}\nFor more details run 'robot --loglevel DEBUG test.robot' and consult the file log.html"
         }
         return super()._run_keyword('PushButton', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Push Button Cell') # type: ignore
-    def PushButtonCell(self, row_index_label_tooltip: str, column: str): # type: ignore
+    def push_button_cell(self, row_index_label_tooltip: str, column: str): # type: ignore
         """
         Push the button cell located at the intersection of the row and column provided.
         
         | ``Push Button Cell     row_locator     column``
         row_locator: Row number, label or tooltip.
         """
         
@@ -370,15 +370,15 @@
             "Pass": "The button cell with the locator '{0}' was pushed.",
             "Exception": "The button cell could not be pushed. {0}\nFor more details run 'robot --loglevel DEBUG test.robot' and consult the file log.html"
         }
         return super()._run_keyword('PushButtonCell', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Read Text Field') # type: ignore
-    def ReadTextField(self, locator: str): # type: ignore
+    def read_text_field(self, locator: str): # type: ignore
         """
         Read the contents of the text field specified by the locator.
         
         *Text field with a label to its left*
         | ``Read Text Field    label``
         *Text field with a label above it*
         | ``Read Text Field    @ label``
@@ -398,15 +398,15 @@
             "Pass": "The text field with the locator '{0}' was read.",
             "Exception": "The text field could not be read. {0}\nFor more details run 'robot --loglevel DEBUG test.robot' and consult the file log.html"
         }
         return super()._run_keyword('ReadTextField', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Read Text') # type: ignore
-    def ReadText(self, content: str): # type: ignore
+    def read_text(self, content: str): # type: ignore
         """
         Read the text specified by the locator.
         
         *Text starting with a given substring*
         | ``Read Text    = substring``
         *Text following a label*
         | ``Read Text    Label``
@@ -422,15 +422,15 @@
             "Pass": "A text with the locator '{0}' was read.",
             "Exception": "The text could not be read. {0}\nFor more details run 'robot --loglevel DEBUG test.robot' and consult the file log.html"
         }
         return super()._run_keyword('ReadText', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Read Cell') # type: ignore
-    def ReadTableCell(self, row_number_or_content: str, column: str): # type: ignore
+    def read_table_cell(self, row_number_or_content: str, column: str): # type: ignore
         """
         Read the contents of the cell at the intersection of the row and column provided.
         
         | ``Read Cell     row_locator     column``
         row_locator: either the row number or the contents of a cell in the row.
         """
         
@@ -445,15 +445,15 @@
             "Pass": "The cell with the locator '{0}, {1}' was read.",
             "Exception": "The cell could not be read. {0}\nFor more details run 'robot --loglevel DEBUG test.robot' and consult the file log.html"
         }
         return super()._run_keyword('ReadTableCell', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Save Screenshot') # type: ignore
-    def SaveScreenshot(self, filepath: str): # type: ignore
+    def save_screenshot(self, filepath: str): # type: ignore
         """
         Save a screenshot of the current window in the file provided.
         
         | ``Save Screenshot     filepath``
         filepath: Absolute path to a .png file.
         """
         
@@ -469,15 +469,15 @@
             "Pass": "The screenshot was saved in {0}.",
             "Exception": "The screenshot could not be saved. {0}\nFor more details run 'robot --loglevel DEBUG test.robot' and consult the file log.html"
         }
         return super()._run_keyword('SaveScreenshot', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Select Cell') # type: ignore
-    def SelectCell(self, row_number_or_content: str, column: str): # type: ignore
+    def select_cell(self, row_number_or_content: str, column: str): # type: ignore
         """
         Select the cell at the intersection of the row and column provided.
         
         | ``Select Cell     row_locator     column``
         row_locator: either the row number or the contents of a cell in the row.
         """
         
@@ -492,15 +492,15 @@
             "Pass": "The cell with the locator '{0}, {1}' was selected.",
             "Exception": "The cell could not be selected. {0}\nFor more details run 'robot --loglevel DEBUG test.robot' and consult the file log.html"
         }
         return super()._run_keyword('SelectCell', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Select Dropdown Menu Entry') # type: ignore
-    def SelectComboBoxEntry(self, dropdown_menu: str, entry: str): # type: ignore
+    def select_combo_box_entry(self, dropdown_menu: str, entry: str): # type: ignore
         """
         Select the specified entry from the dropdown menu provided.
         
         | ``Select Dropdown Menu Entry   dropdown menu    entry``
         """
         
         args = {
@@ -515,15 +515,15 @@
             "Pass": "In the dropdown menu '{0}' the entry '{1}' was selected.",
             "Exception": "The entry could not be selected. {0}\nFor more details run 'robot --loglevel DEBUG test.robot' and consult the file log.html"
         }
         return super()._run_keyword('SelectComboBoxEntry', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Select Radio Button') # type: ignore
-    def SelectRadioButton(self, locator: str): # type: ignore
+    def select_radio_button(self, locator: str): # type: ignore
         """
         Select the radio button specified by the locator.
         
         *Radio button with a label to its left or its right*
         | ``Select Radio Button    label``
         *Radio button with a label above it*
         | ``Select Radio Button    @ label``
@@ -541,15 +541,15 @@
             "Pass": "The radio button with locator '{0}' was selected.",
             "Exception": "The radio button could not be selected. {0}\nFor more details run 'robot --loglevel DEBUG test.robot' and consult the file log.html"
         }
         return super()._run_keyword('SelectRadioButton', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Select Text Field') # type: ignore
-    def SelectTextField(self, locator: str): # type: ignore
+    def select_text_field(self, locator: str): # type: ignore
         """
         Select the text field specified by the locator.
         
         *Text field with a label to its left*
         | ``Select Text Field    label``
         *Text field with a label above it*
         | ``Select Text Field    @ label``
@@ -569,15 +569,15 @@
             "Pass": "The text field with the locator '{0}' was selected.",
             "Exception": "The text field could not be selected. {0}\nFor more details run 'robot --loglevel DEBUG test.robot' and consult the file log.html"
         }
         return super()._run_keyword('SelectTextField', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Select Text Line') # type: ignore
-    def SelectTextLine(self, content: str): # type: ignore
+    def select_text_line(self, content: str): # type: ignore
         """
         Select the text line starting with the given content.
         | ``Select Text Line    content``
         """
         
         args = {
             'Inhalt': content,
@@ -589,15 +589,15 @@
             "Pass": "The text line starting with '{0}' was selected.",
             "Exception": "The text line could not be selected. {0}\nFor more details run 'robot --loglevel DEBUG test.robot' and consult the file log.html"
         }
         return super()._run_keyword('SelectTextLine', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Tick Checkbox') # type: ignore
-    def TickCheckBox(self, locator: str): # type: ignore
+    def tick_check_box(self, locator: str): # type: ignore
         """
         Tick the checkbox specified by the locator.
         
         *Checkbox with a label to its left or its right*
         | ``Tick Checkbox    label``
         *Checkbox with a label above it*
         | ``Tick Checkbox    @ label``
@@ -615,15 +615,15 @@
             "Pass": "The checkbox with the locator '{0}' was ticked.",
             "Exception": "The checkbox could not be ticked. {0}\nFor more details run 'robot --loglevel DEBUG test.robot' and consult the file log.html"
         }
         return super()._run_keyword('TickCheckBox', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Untick Checkbox') # type: ignore
-    def UntickCheckBox(self, locator: str): # type: ignore
+    def untick_check_box(self, locator: str): # type: ignore
         """
         Untick the checkbox specified by the locator.
         
         *Checkbox with a label to its left or its right*
         | ``Untick Checkbox    label``
         *Checkbox with a label above it*
         | ``Untick Checkbox    @ label``
@@ -641,15 +641,15 @@
             "Pass": "The checkbox with the locator '{0}' was unticked.",
             "Exception": "The checkbox could not be unticked. {0}\nFor more details run 'robot --loglevel DEBUG test.robot' and consult the file log.html"
         }
         return super()._run_keyword('UntickCheckBox', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Tick Checkbox Cell') # type: ignore
-    def TickCheckBoxCell(self, row_number: str, column: str): # type: ignore
+    def tick_check_box_cell(self, row_number: str, column: str): # type: ignore
         """
         Tick the checkbox cell at the intersection of the row and the column provided.
         
         | ``Tick Checkbox Cell     row number     column``
         """
         
         args = {
@@ -663,15 +663,15 @@
             "Pass": "The checkbox cell with the locator '{0}' was ticked.",
             "Exception": "The checkbox cell could not be ticked. {0}\nFor more details run 'robot --loglevel DEBUG test.robot' and consult the file log.html"
         }
         return super()._run_keyword('TickCheckBoxCell', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Get Window Title') # type: ignore
-    def GetWindowTitle(self, ): # type: ignore
+    def get_window_title(self, ): # type: ignore
         """
         Get the title of the window in the foreground.
         
         | ``${Title}    Get Window Title``
         """
         
         args = {
@@ -681,15 +681,15 @@
             "NoSession": "No existing SAP-Session. Call the keyword \"Connect To Server\" first.",
             "Pass": "The title of the window was obtained."
         }
         return super()._run_keyword('GetWindowTitle', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Get Window Text') # type: ignore
-    def GetWindowText(self, ): # type: ignore
+    def get_window_text(self, ): # type: ignore
         """
         Get the text message of the window in the foreground.
         
         | ``${Text}    Get Window Text``
         """
         
         args = {
@@ -698,8 +698,8 @@
         result = {
             "NoSession": "No existing SAP-Session. Call the keyword \"Connect To Server\" first.",
             "Pass": "The text message of the window was obtained."
         }
         return super()._run_keyword('GetWindowText', list(args.values()), dict(), result) # type: ignore
     
     ROBOT_LIBRARY_SCOPE = 'GLOBAL'
-    ROBOT_LIBRARY_VERSION = '1.1.6'
+    ROBOT_LIBRARY_VERSION = '1.1.7'
```

## RoboSAPiens/client.py

```diff
@@ -32,45 +32,56 @@
     ).decode()
 
     return any(line.startswith(cmd) for line in process_list.splitlines())
 
 
 class RoboSAPiensClient(object):
     def __init__(self, args: Mapping[str, Any]):
-        uri = f"http://127.0.0.1:{args['port']}"
-        server_cmd = Path(realpath(__file__)).parent / "lib" / "RoboSAPiens.exe"
-
-        self.server = self._start_server(server_cmd, _cli_args(list(args.items())))
-        self.client = XmlRpcRemoteClient(uri)
+        self.args = list(args.items())
+        self.server_cmd = Path(realpath(__file__)).parent / "lib" / "RoboSAPiens.exe"
+        self.uri = f"http://127.0.0.1:{args['port']}"
+
+        self._server = self.server
+        self._client = self.client
+
+    @property
+    def server(self):
+        return self._start_server(self.server_cmd, _cli_args(self.args))
+
+    @property
+    def client(self):
+        return XmlRpcRemoteClient(self.uri)
 
     def _start_server(self, server: Path, args: List[str]):
         if _is_running(server.name):
             return
 
+        asyncio.set_event_loop_policy(asyncio.WindowsProactorEventLoopPolicy())
         loop = asyncio.get_event_loop()
-        return loop.run_until_complete(self.start_cmd(server, args))
+        return loop.run_until_complete(self._start_cmd(server, args))
 
-    async def start_cmd(self, cmd: Path, args: List[str]):
+    async def _start_cmd(self, cmd: Path, args: List[str]):
         proc = await asyncio.create_subprocess_exec(
             str(cmd), *args, 
             stdout=asyncio.subprocess.PIPE, stderr=asyncio.subprocess.PIPE
         )
 
         try:
             _, stderr = await asyncio.wait_for(proc.communicate(), timeout=0.5)
 
             if proc.returncode and proc.returncode > 0:
                 raise RemoteError(stderr.decode())
         except asyncio.TimeoutError:
             return proc
 
     def __del__(self):
-        if self.server:
-            self.server.terminate()
+        if self._server:
+            self._server.terminate()
 
+    # All methods have to be private so that they are not interpreted as keywords by RF
     def _run_keyword(self, name: str, args: List[Any], kwargs: Dict[str, Any], result: Dict[str, Any]): # type: ignore
         coercer = ArgumentCoercer()
         args = coercer.coerce(args) # type: ignore
         kwargs = coercer.coerce(kwargs) # type: ignore
 
         try:
             rf_result = RemoteResult(self.client.run_keyword(name, args, kwargs)) # type: ignore
```

## RoboSAPiens/DE/__init__.py

```diff
@@ -30,15 +30,15 @@
             'presenter_mode': vortragsmodus,
         }
         
         super().__init__(args)
     
 
     @keyword('Reiter auswählen') # type: ignore
-    def ActivateTab(self, Reitername: str): # type: ignore
+    def activate_tab(self, Reitername: str): # type: ignore
         """
         Der Reiter mit dem angegebenen Name wird ausgewählt.
         
         | ``Reiter auswählen    Name``
         """
         
         args = {
@@ -52,15 +52,15 @@
             "Pass": "Der Reiter '{0}' wurde ausgewählt.",
             "Exception": "Der Reiter konnte nicht ausgewählt werden.\n{0}\nFür mehr Infos robot --loglevel DEBUG datei.robot ausführen und die log.html Datei durchsuchen."
         }
         return super()._run_keyword('ActivateTab', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('SAP starten') # type: ignore
-    def OpenSAP(self, Pfad: str): # type: ignore
+    def open_s_a_p(self, Pfad: str): # type: ignore
         """
         Die SAP GUI wird gestartet. Der übliche Pfad ist\n\n| ``C:\\Program Files (x86)\\SAP\\FrontEnd\\SAPgui\\saplogon.exe``
         """
         
         args = {
             'Pfad': Pfad,
         }
@@ -70,15 +70,15 @@
             "SAPNotStarted": "Die SAP GUI konnte nicht gestartet werden. Überprüfe den Pfad '{0}'.",
             "Exception": "Die SAP GUI konnte nicht gestartet werden.\n{0}\nFür mehr Infos robot --loglevel DEBUG datei.robot ausführen und die log.html Datei durchsuchen."
         }
         return super()._run_keyword('OpenSAP', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Verbindung zum Server trennen') # type: ignore
-    def CloseConnection(self, ): # type: ignore
+    def close_connection(self, ): # type: ignore
         """
         Die Verbindung mit dem SAP Server wird beendet.
         """
         
         args = {
         }
         
@@ -90,15 +90,15 @@
             "Pass": "Die Verbindung zum Server wurde getrennt.",
             "Exception": "Die Verbindung zum Server konnte nicht getrennt werden.\n{0}\nFür mehr Infos robot --loglevel DEBUG datei.robot ausführen und die log.html Datei durchsuchen."
         }
         return super()._run_keyword('CloseConnection', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('SAP beenden') # type: ignore
-    def CloseSAP(self, ): # type: ignore
+    def close_s_a_p(self, ): # type: ignore
         """
         Die SAP GUI wird beendet.
         """
         
         args = {
         }
         
@@ -106,15 +106,15 @@
             "NoSapGui": "Keine laufende SAP GUI gefunden. Das Keyword \"SAP starten\" muss zuerst aufgerufen werden.",
             "Pass": "Die SAP GUI wurde beendet"
         }
         return super()._run_keyword('CloseSAP', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Funktionsbaum exportieren') # type: ignore
-    def ExportTree(self, Dateipfad: str): # type: ignore
+    def export_tree(self, Dateipfad: str): # type: ignore
         """
         Der Funktionsbaum wird in der angegebenen Datei gespeichert.
         
         | ``Funktionsbaum exportieren     Dateipfad``
         """
         
         args = {
@@ -127,15 +127,15 @@
             "Pass": "Die Baumstruktur wurde in JSON Format in der Datei '{0}' gespeichert",
             "Exception": "Die Baumstruktur konnte nicht exportiert werden.\n{0}\nFür mehr Infos robot --loglevel DEBUG datei.robot ausführen und die log.html Datei durchsuchen."
         }
         return super()._run_keyword('ExportTree', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Laufende SAP GUI übernehmen') # type: ignore
-    def AttachToRunningSAP(self, ): # type: ignore
+    def attach_to_running_s_a_p(self, ): # type: ignore
         """
         Nach der Ausführung dieses Keywords, kann eine laufende SAP GUI mit RoboSAPiens gesteuert werden.
         """
         
         args = {
         }
         
@@ -147,15 +147,15 @@
             "Pass": "Die laufende SAP GUI wurde erfolgreich übernommen.",
             "Exception": "Die laufende SAP GUI konnte nicht übernommen werden.\n{0}\nFür mehr Infos robot --loglevel DEBUG datei.robot ausführen und die log.html Datei durchsuchen."
         }
         return super()._run_keyword('AttachToRunningSAP', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Verbindung zum Server herstellen') # type: ignore
-    def ConnectToServer(self, Servername: str): # type: ignore
+    def connect_to_server(self, Servername: str): # type: ignore
         """
         Die Verbindung mit dem angegebenen SAP Server wird hergestellt.
         
         | ``Verbindung zum Server herstellen    Servername``
         """
         
         args = {
@@ -170,15 +170,15 @@
             "NoServerScripting": "Das Scripting ist auf dem SAP Server nicht freigeschaltet. Siehe die Dokumentation von RoboSAPiens.",
             "Exception": "Die Verbindung konnte nicht hergestellt werden.\n{0}\nFür mehr Infos robot --loglevel DEBUG datei.robot ausführen und die log.html Datei durchsuchen."
         }
         return super()._run_keyword('ConnectToServer', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Tabellenzelle doppelklicken') # type: ignore
-    def DoubleClickCell(self, Zeilennummer_oder_Zellinhalt: str, Spaltentitel: str): # type: ignore
+    def double_click_cell(self, Zeilennummer_oder_Zellinhalt: str, Spaltentitel: str): # type: ignore
         """
         Die angegebene Tabellenzelle wird doppelgeklickt.
         
         | ``Tabellenzelle doppelklicken     Positionsgeber     Spaltentitel``
         Positionsgeber: entweder die Zeilennummer oder der Inhalt der Zelle.
         """
         
@@ -193,15 +193,15 @@
             "Pass": "Die Zelle mit dem Lokator '{0}, {1}' wurde doppelgeklickt.",
             "Exception": "Die Zelle konnte nicht doppelgeklickt werden.\n{0}\nFür mehr Infos robot --loglevel DEBUG datei.robot ausführen und die log.html Datei durchsuchen."
         }
         return super()._run_keyword('DoubleClickCell', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Textfeld doppelklicken') # type: ignore
-    def DoubleClickTextField(self, Inhalt: str): # type: ignore
+    def double_click_text_field(self, Inhalt: str): # type: ignore
         """
         Das angegebene Textfeld wird doppelgeklickt.
         
         | ``Textfeld doppelklicken     Inhalt``
         
         """
         
@@ -215,15 +215,15 @@
             "Pass": "Das Textfeld mit dem Lokator '{0}' wurde doppelgeklickt.",
             "Exception": "Das Textfeld konnte nicht doppelgeklickt werden.\n{0}\nFür mehr Infos robot --loglevel DEBUG datei.robot ausführen und die log.html Datei durchsuchen."
         }
         return super()._run_keyword('DoubleClickTextField', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Transaktion ausführen') # type: ignore
-    def ExecuteTransaction(self, T_Code: str): # type: ignore
+    def execute_transaction(self, T_Code: str): # type: ignore
         """
         Die Transaktion mit dem angegebenen T-Code wird ausgeführt.
         
         | ``Transaktion ausführen    T-Code``
         """
         
         args = {
@@ -235,15 +235,15 @@
             "Pass": "Die Transaktion mit T-Code '{0}' wurde erfolgreich ausgeführt.",
             "Exception": "Die Transaktion konnte nicht ausgeführt werden.\n{0}\nFür mehr Infos robot --loglevel DEBUG datei.robot ausführen und die log.html Datei durchsuchen."
         }
         return super()._run_keyword('ExecuteTransaction', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Maske exportieren') # type: ignore
-    def ExportForm(self, Name: str, Verzeichnis: str): # type: ignore
+    def export_form(self, Name: str, Verzeichnis: str): # type: ignore
         """
         Alle Texte in der aktuellen Maske werden in einer CSV-Datei gespeichert. Außerdem wird ein Bildschirmfoto in PNG-Format erstellt.
         
         | ``Maske exportieren     Name     Verzeichnis``
         Verzeichnis: Der absolute Pfad des Verzeichnisses, wo die Dateien abgelegt werden.
         """
         
@@ -257,15 +257,15 @@
             "Pass": "Die Maske wurde in den Dateien '{0}' und '{1}' gespeichert",
             "Exception": "Die Maske konnte nicht exportiert werden.\n{0}\nFür mehr Infos robot --loglevel DEBUG datei.robot ausführen und die log.html Datei durchsuchen."
         }
         return super()._run_keyword('ExportForm', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Tabellenzelle ausfüllen') # type: ignore
-    def FillTableCell(self, Zeilennummer_oder_Zellinhalt: str, Spaltentitel_Gleich_Inhalt: str): # type: ignore
+    def fill_table_cell(self, Zeilennummer_oder_Zellinhalt: str, Spaltentitel_Gleich_Inhalt: str): # type: ignore
         """
         Die Zelle am Schnittpunkt der angegebenen Zeile und Spalte wird mit dem angegebenen Inhalt ausgefüllt.
         
         | ``Tabellenzelle ausfüllen     Zeile     Spaltentitel = Inhalt``
         Zeile: entweder eine Zeilennummer oder der Inhalt einer Zelle in der Zeile.
         
         *Hinweis*: Eine Tabellenzelle hat u.U. eine Beschriftung, die man über die Hilfe (Taste F1) herausfinden kann. In diesem Fall kann man die Zelle mit dem Keyword [#Textfeld%20Ausfüllen|Textfeld ausfüllen] ausfüllen.
@@ -284,15 +284,15 @@
             "Pass": "Die Zelle mit dem Lokator '{0}, {1}' wurde ausgefüllt.",
             "Exception": "Die Zelle konnte nicht ausgefüllt werden.\n{0}\nFür mehr Infos robot --loglevel DEBUG datei.robot ausführen und die log.html Datei durchsuchen."
         }
         return super()._run_keyword('FillTableCell', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Textfeld ausfüllen') # type: ignore
-    def FillTextField(self, Beschriftung_oder_Positionsgeber: str, Inhalt: str): # type: ignore
+    def fill_text_field(self, Beschriftung_oder_Positionsgeber: str, Inhalt: str): # type: ignore
         """
         Das angegebene Textfeld wird mit dem angegebenen Inhalt ausgefüllt.
         
         *Textfeld mit einer Beschriftung links*
         | ``Textfeld ausfüllen    Beschriftung    Inhalt``
         *Textfeld mit einer Beschriftung oben*
         | ``Textfeld ausfüllen    @ Beschriftung    Inhalt``
@@ -321,15 +321,15 @@
             "Pass": "Das Textfeld mit dem Lokator '{0}' wurde ausgefüllt.",
             "Exception": "Das Textfeld konnte nicht ausgefüllt werden. Möglicherweise, weil der Inhalt nicht dazu passt.\n{0}\nFür mehr Infos robot --loglevel DEBUG datei.robot ausführen und die log.html Datei durchsuchen."
         }
         return super()._run_keyword('FillTextField', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Knopf drücken') # type: ignore
-    def PushButton(self, Name_oder_Kurzinfo: str): # type: ignore
+    def push_button(self, Name_oder_Kurzinfo: str): # type: ignore
         """
         Der Knopf mit dem angegebenen Namen oder Kurzinfo (Tooltip) wird gedrückt.
         
         | ``Knopf drücken    Name oder Kurzinfo (Tooltip)``
         """
         
         args = {
@@ -343,15 +343,15 @@
             "Pass": "Der Knopf '{0}' wurde gedrückt.",
             "Exception": "Der Knopf konnte nicht gedrückt werden.\n{0}\nFür mehr Infos robot --loglevel DEBUG datei.robot ausführen und die log.html Datei durchsuchen."
         }
         return super()._run_keyword('PushButton', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Tabellenzelle drücken') # type: ignore
-    def PushButtonCell(self, Zeilennummer_oder_Name_oder_Kurzinfo: str, Spaltentitel: str): # type: ignore
+    def push_button_cell(self, Zeilennummer_oder_Name_oder_Kurzinfo: str, Spaltentitel: str): # type: ignore
         """
         Die angegebene Tabellenzelle wird gedrückt.
         
         | ``Tabellenzelle drücken     Positionsgeber     Spaltentitel``
         Positionsgeber: Zeilennummer, Beschriftung oder Kurzinfo (Tooltip).
         """
         
@@ -366,15 +366,15 @@
             "Pass": "Die Zelle mit dem Lokator '{0}, {1}' wurde gedrückt.",
             "Exception": "Die Zelle konnte nicht gedrückt werden.\n{0}\nFür mehr Infos robot --loglevel DEBUG datei.robot ausführen und die log.html Datei durchsuchen."
         }
         return super()._run_keyword('PushButtonCell', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Textfeld auslesen') # type: ignore
-    def ReadTextField(self, Beschriftung_oder_Positionsgeber: str): # type: ignore
+    def read_text_field(self, Beschriftung_oder_Positionsgeber: str): # type: ignore
         """
         Der Inhalt des angegebenen Textfeldes wird zurückgegeben.
         
         *Textfeld mit einer Beschriftung links*
         | ``Textfeld auslesen    Beschriftung``
         *Textfeld mit einer Beschriftung oben*
         | ``Textfeld auslesen    @ Beschriftung``
@@ -394,15 +394,15 @@
             "Pass": "Das Textfeld mit dem Lokator '{0}' wurde ausgelesen.",
             "Exception": "Das Textfeld konnte nicht ausgelesen werden.\n{0}\nFür mehr Infos robot --loglevel DEBUG datei.robot ausführen und die log.html Datei durchsuchen."
         }
         return super()._run_keyword('ReadTextField', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Text auslesen') # type: ignore
-    def ReadText(self, Inhalt: str): # type: ignore
+    def read_text(self, Inhalt: str): # type: ignore
         """
         Der Inhalt des angegebenen Texts wird zurückgegeben.
         
         *Text fängt mit der angegebenen Teilzeichenfolge an*
         | ``Text auslesen    = Teilzeichenfolge``
         *Text folgt einer Beschriftung*
         | ``Text auslesen    Beschriftung``
@@ -418,15 +418,15 @@
             "Pass": "Der Text mit dem Lokator '{0}' wurde ausgelesen.",
             "Exception": "Der Text konnte nicht ausgelesen werden.\n{0}\nFür mehr Infos robot --loglevel DEBUG datei.robot ausführen und die log.html Datei durchsuchen."
         }
         return super()._run_keyword('ReadText', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Tabellenzelle auslesen') # type: ignore
-    def ReadTableCell(self, Zeilennummer_oder_Zellinhalt: str, Spaltentitel: str): # type: ignore
+    def read_table_cell(self, Zeilennummer_oder_Zellinhalt: str, Spaltentitel: str): # type: ignore
         """
         Der Inhalt der angegebenen Tabellenzelle wird zurückgegeben.
         
         | ``Tabellenzelle ablesen     Positionsgeber     Spaltentitel``
         Positionsgeber: Zeilennummer oder Zellinhalt.
         """
         
@@ -441,15 +441,15 @@
             "Pass": "Die Zelle mit dem Lokator '{0}, {1}' wurde ausgelesen.",
             "Exception": "Die Zelle konnte nicht ausgelesen werden.\n{0}\nFür mehr Infos robot --loglevel DEBUG datei.robot ausführen und die log.html Datei durchsuchen."
         }
         return super()._run_keyword('ReadTableCell', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Fenster aufnehmen') # type: ignore
-    def SaveScreenshot(self, Aufnahmenverzeichnis: str): # type: ignore
+    def save_screenshot(self, Aufnahmenverzeichnis: str): # type: ignore
         """
         Eine Bildschirmaufnahme des Fensters wird im eingegebenen Dateipfad gespeichert.
         
         | ``Fenster aufnehmen     Dateipfad``
         Dateifpad: Der absolute Pfad einer .png Datei bzw. eines Verzeichnisses.
         """
         
@@ -465,15 +465,15 @@
             "Pass": "Eine Aufnahme des Fensters wurde in '{0}' gespeichert.",
             "Exception": "Eine Aufnahme des Fensters konnte nicht gespeichert werden.\n{0}\nFür mehr Infos robot --loglevel DEBUG datei.robot ausführen und die log.html Datei durchsuchen."
         }
         return super()._run_keyword('SaveScreenshot', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Tabellenzelle markieren') # type: ignore
-    def SelectCell(self, Zeilennummer_oder_Zellinhalt: str, Spaltentitel: str): # type: ignore
+    def select_cell(self, Zeilennummer_oder_Zellinhalt: str, Spaltentitel: str): # type: ignore
         """
         Die angegebene Tabellenzelle wird markiert.
         
         | ``Tabellenzelle markieren     Positionsgeber     Spaltentitel``
         Positionsgeber: Zeilennummer oder Zellinhalt.
         """
         
@@ -488,15 +488,15 @@
             "Pass": "Die Zelle mit dem Lokator '{0}, {1}' wurde markiert.",
             "Exception": "Die Zelle konnte nicht markiert werden.\n{0}\nFür mehr Infos robot --loglevel DEBUG datei.robot ausführen und die log.html Datei durchsuchen."
         }
         return super()._run_keyword('SelectCell', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Auswahlmenüeintrag auswählen') # type: ignore
-    def SelectComboBoxEntry(self, Name: str, Eintrag: str): # type: ignore
+    def select_combo_box_entry(self, Name: str, Eintrag: str): # type: ignore
         """
         Aus dem angegebenen Auswahlmenü wird der angegebene Eintrag ausgewählt.
         
         | ``Auswahlmenüeintrag auswählen    Auswahlmenü    Eintrag``
         """
         
         args = {
@@ -511,15 +511,15 @@
             "Pass": "Der Eintrag '{1}' wurde ausgewählt.",
             "Exception": "Der Eintrag konnte nicht ausgewählt werden.\n{0}\nFür mehr Infos robot --loglevel DEBUG datei.robot ausführen und die log.html Datei durchsuchen."
         }
         return super()._run_keyword('SelectComboBoxEntry', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Optionsfeld auswählen') # type: ignore
-    def SelectRadioButton(self, Beschriftung_oder_Positionsgeber: str): # type: ignore
+    def select_radio_button(self, Beschriftung_oder_Positionsgeber: str): # type: ignore
         """
         Das angegebene Optionsfeld wird ausgewählt.
         
         *Optionsfeld mit einer Beschriftung links oder rechts*
         | ``Optionsfeld auswählen    Beschriftung``
         *Optionsfeld mit einer Beschriftung oben*
         | ``Optionsfeld auswählen    @ Beschriftung``
@@ -538,15 +538,15 @@
             "Pass": "Das Optionsfeld mit dem Lokator '{0}' wurde ausgewählt.",
             "Exception": "Das Optionsfeld konnte nicht ausgewählt werden.\n{0}\nFür mehr Infos robot --loglevel DEBUG datei.robot ausführen und die log.html Datei durchsuchen."
         }
         return super()._run_keyword('SelectRadioButton', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Textfeld markieren') # type: ignore
-    def SelectTextField(self, Beschriftungen_oder_Inhalt: str): # type: ignore
+    def select_text_field(self, Beschriftungen_oder_Inhalt: str): # type: ignore
         """
         Das angegebene Textfeld wird markiert.
         
         *Textfeld mit einer Beschriftung links*
         | ``Textfeld markieren    Beschriftung``
         *Textfeld mit einer Beschriftung oben*
         | ``Textfeld markieren    @ Beschriftung``
@@ -566,15 +566,15 @@
             "Pass": "Das Textfeld mit dem Lokator '{0}' wurde markiert.",
             "Exception": "Das Textfeld konnte nicht markiert werden.\n{0}\nFür mehr Infos robot --loglevel DEBUG datei.robot ausführen und die log.html Datei durchsuchen."
         }
         return super()._run_keyword('SelectTextField', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Textzeile markieren') # type: ignore
-    def SelectTextLine(self, Inhalt: str): # type: ignore
+    def select_text_line(self, Inhalt: str): # type: ignore
         """
         Die Textzeile mit dem angegebenen Inhalt wird markiert.
         | ``Textzeile markieren    Inhalt``
         """
         
         args = {
             'Inhalt': Inhalt,
@@ -586,15 +586,15 @@
             "Pass": "Die Textzeile mit dem Inhalt '{0}' wurde markiert.",
             "Exception": "Die Textzeile konnte nicht markiert werden.\n{0}\nFür mehr Infos robot --loglevel DEBUG datei.robot ausführen und die log.html Datei durchsuchen."
         }
         return super()._run_keyword('SelectTextLine', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Formularfeld ankreuzen') # type: ignore
-    def TickCheckBox(self, Beschriftung_oder_Positionsgeber: str): # type: ignore
+    def tick_check_box(self, Beschriftung_oder_Positionsgeber: str): # type: ignore
         """
         Das angegebene Formularfeld wird angekreuzt.
         
         *Formularfeld mit einer Beschriftung links oder rechts *
         | ``Formularfeld ankreuzen    Beschriftung``
         *Formularfeld mit einer Beschriftung oben*
         | ``Formularfeld ankreuzen    @ Beschriftung``
@@ -612,15 +612,15 @@
             "Pass": "Das Formularfeld mit dem Lokator '{0}' wurde angekreuzt.",
             "Exception": "Das Formularfeld konnte nicht angekreuzt werden.\n{0}\nFür mehr Infos robot --loglevel DEBUG datei.robot ausführen und die log.html Datei durchsuchen."
         }
         return super()._run_keyword('TickCheckBox', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Formularfeld abwählen') # type: ignore
-    def UntickCheckBox(self, Beschriftung_oder_Positionsgeber: str): # type: ignore
+    def untick_check_box(self, Beschriftung_oder_Positionsgeber: str): # type: ignore
         """
         Das angegebene Formularfeld wird abgewählt.
         
         *Formularfeld mit einer Beschriftung links oder rechts *
         | ``Formularfeld abwählen    Beschriftung``
         *Formularfeld mit einer Beschriftung oben*
         | ``Formularfeld abwählen    @ Beschriftung``
@@ -638,15 +638,15 @@
             "Pass": "Das Formularfeld mit dem Lokator '{0}' wurde abgewählt.",
             "Exception": "Das Formularfeld konnte nicht abgewählt werden.\n{0}\nFür mehr Infos robot --loglevel DEBUG datei.robot ausführen und die log.html Datei durchsuchen."
         }
         return super()._run_keyword('UntickCheckBox', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Tabellenzelle ankreuzen') # type: ignore
-    def TickCheckBoxCell(self, Zeilennummer: str, Spaltentitel: str): # type: ignore
+    def tick_check_box_cell(self, Zeilennummer: str, Spaltentitel: str): # type: ignore
         """
         Die angegebene Tabellenzelle wird angekreuzt.
         
         | ``Tabellenzelle ankreuzen     Zeilennummer     Spaltentitel``
         """
         
         args = {
@@ -660,15 +660,15 @@
             "Pass": "Die Zelle mit dem Lokator '{0}, {1}' wurde angekreuzt.",
             "Exception": "Die Zelle konnte nicht angekreuzt werden.\n{0}\nFür mehr Infos robot --loglevel DEBUG datei.robot ausführen und die log.html Datei durchsuchen."
         }
         return super()._run_keyword('TickCheckBoxCell', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Fenstertitel auslesen') # type: ignore
-    def GetWindowTitle(self, ): # type: ignore
+    def get_window_title(self, ): # type: ignore
         """
         Der Titel des Fensters im Fordergrund wird zurückgegeben.
         
         | ``${Titel}    Fenstertitel auslesen``
         """
         
         args = {
@@ -678,15 +678,15 @@
             "NoSession": "Keine SAP-Session vorhanden. Versuche zuerst das Keyword \"Verbindung zum Server Herstellen\" aufzurufen.",
             "Pass": "Der Fenstertitel wurde ausgelesen"
         }
         return super()._run_keyword('GetWindowTitle', list(args.values()), dict(), result) # type: ignore
     
 
     @keyword('Fenstertext auslesen') # type: ignore
-    def GetWindowText(self, ): # type: ignore
+    def get_window_text(self, ): # type: ignore
         """
         Der Text des Fensters im Fordergrund wird zurückgegeben.
         
         | ``${Text}    Fenstertext auslesen``
         """
         
         args = {
@@ -695,8 +695,8 @@
         result = {
             "NoSession": "Keine SAP-Session vorhanden. Versuche zuerst das Keyword \"Verbindung zum Server Herstellen\" aufzurufen.",
             "Pass": "Der Text des Fensters wurde ausgelesen"
         }
         return super()._run_keyword('GetWindowText', list(args.values()), dict(), result) # type: ignore
     
     ROBOT_LIBRARY_SCOPE = 'GLOBAL'
-    ROBOT_LIBRARY_VERSION = '1.1.6'
+    ROBOT_LIBRARY_VERSION = '1.1.7'
```

## RoboSAPiens/lib/RoboSAPiens.deps.json

### Pretty-printed

 * *Similarity: 0.9479166666666665%*

 * *Differences: {"'libraries'": "{'RoboSAPiens/1.1.7': OrderedDict([('type', 'project'), ('serviceable', False), "*

 * *                "('sha512', '')]), delete: ['RoboSAPiens/1.1.6']}",*

 * * "'targets'": "{'.NETCoreApp,Version=v7.0/win-x86': {'RoboSAPiens/1.1.7': "*

 * *              "OrderedDict([('dependencies', OrderedDict([('CsvHelper', '27.2.1'), "*

 * *              "('Horizon.XmlRpc.Server', '2.5.0'), ('SAP.GUI.Scripting.net', '1.0.1')])), "*

 * *              "('runtime', OrderedDict([('RoboSAPiens.dll', OrderedDict())]))]), delete: "*

 * *  […]*

```diff
@@ -18,15 +18,15 @@
         "Horizon.XmlRpc.Server/2.5.0": {
             "hashPath": "horizon.xmlrpc.server.2.5.0.nupkg.sha512",
             "path": "horizon.xmlrpc.server/2.5.0",
             "serviceable": true,
             "sha512": "sha512-A2aGS6CmOngl4w2S2FEH7Eel0mSUPBx1HVw4AjZJdhuOIhNKW7LTq+0Jyg0mgycjccIOp1raI2HPoVV0I0CXJQ==",
             "type": "package"
         },
-        "RoboSAPiens/1.1.6": {
+        "RoboSAPiens/1.1.7": {
             "serviceable": false,
             "sha512": "",
             "type": "project"
         },
         "SAP.GUI.Scripting.net/1.0.1": {
             "hashPath": "sap.gui.scripting.net.1.0.1.nupkg.sha512",
             "path": "sap.gui.scripting.net/1.0.1",
@@ -69,15 +69,15 @@
                 "runtime": {
                     "lib/netstandard2.0/Horizon.XmlRpc.Server.dll": {
                         "assemblyVersion": "1.0.0.0",
                         "fileVersion": "1.0.0.0"
                     }
                 }
             },
-            "RoboSAPiens/1.1.6": {
+            "RoboSAPiens/1.1.7": {
                 "dependencies": {
                     "CsvHelper": "27.2.1",
                     "Horizon.XmlRpc.Server": "2.5.0",
                     "SAP.GUI.Scripting.net": "1.0.1"
                 },
                 "runtime": {
                     "RoboSAPiens.dll": {}
```

## RoboSAPiens/lib/RoboSAPiens.dll

### pedump {}

```diff
@@ -1,12 +1,12 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0x874bbb6e
+	             Time stamp: 0xd875c534
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00e0
 	   	Characteristics: 0x0102
 
 PE Header:
 	         Magic (0x010b): 0x010b
```

## RoboSAPiens/lib/RoboSAPiens.exe

```diff
@@ -7015,15 +7015,15 @@
 0001b660: 0000 0000 8000 0000 0000 0000 0000 0000  ................
 0001b670: 0400 0000 0000 0100 0000 0000 9000 0000  ................
 0001b680: a0e0 0100 d402 0000 e404 0000 0000 0000  ................
 0001b690: 74e3 0100 ea01 0000 e404 0000 0000 0000  t...............
 0001b6a0: d402 3400 0000 5600 5300 5f00 5600 4500  ..4...V.S._.V.E.
 0001b6b0: 5200 5300 4900 4f00 4e00 5f00 4900 4e00  R.S.I.O.N._.I.N.
 0001b6c0: 4600 4f00 0000 0000 bd04 effe 0000 0100  F.O.............
-0001b6d0: 0100 0100 0000 0600 0100 0100 0000 0600  ................
+0001b6d0: 0100 0100 0000 0700 0100 0100 0000 0700  ................
 0001b6e0: 3f00 0000 0000 0000 0400 0000 0100 0000  ?...............
 0001b6f0: 0000 0000 0000 0000 0000 0000 4400 0000  ............D...
 0001b700: 0100 5600 6100 7200 4600 6900 6c00 6500  ..V.a.r.F.i.l.e.
 0001b710: 4900 6e00 6600 6f00 0000 0000 2400 0400  I.n.f.o.....$...
 0001b720: 0000 5400 7200 6100 6e00 7300 6c00 6100  ..T.r.a.n.s.l.a.
 0001b730: 7400 6900 6f00 6e00 0000 0000 0000 b004  t.i.o.n.........
 0001b740: 3402 0000 0100 5300 7400 7200 6900 6e00  4.....S.t.r.i.n.
@@ -7035,15 +7035,15 @@
 0001b7a0: 6200 6f00 5300 4100 5000 6900 6500 6e00  b.o.S.A.P.i.e.n.
 0001b7b0: 7300 0000 4000 0c00 0100 4600 6900 6c00  s...@.....F.i.l.
 0001b7c0: 6500 4400 6500 7300 6300 7200 6900 7000  e.D.e.s.c.r.i.p.
 0001b7d0: 7400 6900 6f00 6e00 0000 0000 5200 6f00  t.i.o.n.....R.o.
 0001b7e0: 6200 6f00 5300 4100 5000 6900 6500 6e00  b.o.S.A.P.i.e.n.
 0001b7f0: 7300 0000 3000 0800 0100 4600 6900 6c00  s...0.....F.i.l.
 0001b800: 6500 5600 6500 7200 7300 6900 6f00 6e00  e.V.e.r.s.i.o.n.
-0001b810: 0000 0000 3100 2e00 3100 2e00 3600 2e00  ....1...1...6...
+0001b810: 0000 0000 3100 2e00 3100 2e00 3700 2e00  ....1...1...7...
 0001b820: 3000 0000 4000 1000 0100 4900 6e00 7400  0...@.....I.n.t.
 0001b830: 6500 7200 6e00 6100 6c00 4e00 6100 6d00  e.r.n.a.l.N.a.m.
 0001b840: 6500 0000 5200 6f00 6200 6f00 5300 4100  e...R.o.b.o.S.A.
 0001b850: 5000 6900 6500 6e00 7300 2e00 6400 6c00  P.i.e.n.s...d.l.
 0001b860: 6c00 0000 2800 0200 0100 4c00 6500 6700  l...(.....L.e.g.
 0001b870: 6100 6c00 4300 6f00 7000 7900 7200 6900  a.l.C.o.p.y.r.i.
 0001b880: 6700 6800 7400 0000 2000 0000 4800 1000  g.h.t... ...H...
@@ -7053,18 +7053,18 @@
 0001b8c0: 5000 6900 6500 6e00 7300 2e00 6400 6c00  P.i.e.n.s...d.l.
 0001b8d0: 6c00 0000 3800 0c00 0100 5000 7200 6f00  l...8.....P.r.o.
 0001b8e0: 6400 7500 6300 7400 4e00 6100 6d00 6500  d.u.c.t.N.a.m.e.
 0001b8f0: 0000 0000 5200 6f00 6200 6f00 5300 4100  ....R.o.b.o.S.A.
 0001b900: 5000 6900 6500 6e00 7300 0000 3000 0600  P.i.e.n.s...0...
 0001b910: 0100 5000 7200 6f00 6400 7500 6300 7400  ..P.r.o.d.u.c.t.
 0001b920: 5600 6500 7200 7300 6900 6f00 6e00 0000  V.e.r.s.i.o.n...
-0001b930: 3100 2e00 3100 2e00 3600 0000 3800 0800  1...1...6...8...
+0001b930: 3100 2e00 3100 2e00 3700 0000 3800 0800  1...1...7...8...
 0001b940: 0100 4100 7300 7300 6500 6d00 6200 6c00  ..A.s.s.e.m.b.l.
 0001b950: 7900 2000 5600 6500 7200 7300 6900 6f00  y. .V.e.r.s.i.o.
-0001b960: 6e00 0000 3100 2e00 3100 2e00 3600 2e00  n...1...1...6...
+0001b960: 6e00 0000 3100 2e00 3100 2e00 3700 2e00  n...1...1...7...
 0001b970: 3000 0000 efbb bf3c 3f78 6d6c 2076 6572  0......<?xml ver
 0001b980: 7369 6f6e 3d22 312e 3022 2065 6e63 6f64  sion="1.0" encod
 0001b990: 696e 673d 2255 5446 2d38 2220 7374 616e  ing="UTF-8" stan
 0001b9a0: 6461 6c6f 6e65 3d22 7965 7322 3f3e 0d0a  dalone="yes"?>..
 0001b9b0: 0d0a 3c61 7373 656d 626c 7920 786d 6c6e  ..<assembly xmln
 0001b9c0: 733d 2275 726e 3a73 6368 656d 6173 2d6d  s="urn:schemas-m
 0001b9d0: 6963 726f 736f 6674 2d63 6f6d 3a61 736d  icrosoft-com:asm
```

## Comparing `robotframework_robosapiens-1.1.6.dist-info/METADATA` & `robotframework_robosapiens-1.1.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robosapiens
-Version: 1.1.6
+Version: 1.1.7
 Summary: Fully localized Robot Framework library for automating the SAP GUI using text selectors.
 Home-page: https://github.com/imbus/robotframework-robosapiens
 Author: imbus Rheinland GmbH
 Maintainer: Marduk Bolaños
 Maintainer-email: marduk.bolanos@imbus.de
 License: Apache 2
 Keywords: robotframework testing test automation sap gui
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.7.9
 Description-Content-Type: text/markdown
 Requires-Dist: robotframework
 
 # RoboSAPiens: SAP GUI Automation for Humans
 
 Fully localized Robot Framework library for automating the SAP GUI using text locators.
```

