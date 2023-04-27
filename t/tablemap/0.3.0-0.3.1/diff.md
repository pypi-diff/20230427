# Comparing `tmp/tablemap-0.3.0.tar.gz` & `tmp/tablemap-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablemap-0.3.0.tar", last modified: Wed Dec 28 08:35:12 2022, max compression
+gzip compressed data, was "tablemap-0.3.1.tar", last modified: Thu Apr 27 08:10:02 2023, max compression
```

## Comparing `tablemap-0.3.0.tar` & `tablemap-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-12-28 08:35:12.104378 tablemap-0.3.0/
--rw-rw-rw-   0        0        0     1085 2022-12-13 18:38:10.000000 tablemap-0.3.0/LICENSE
--rw-rw-rw-   0        0        0      229 2022-12-28 08:35:12.104378 tablemap-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    14407 2022-12-28 08:34:36.000000 tablemap-0.3.0/README.md
--rw-rw-rw-   0        0        0       42 2022-12-28 08:35:12.105378 tablemap-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      292 2022-12-28 08:11:26.000000 tablemap-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-28 08:35:12.093377 tablemap-0.3.0/tablemap/
--rw-rw-rw-   0        0        0       34 2022-12-13 18:38:10.000000 tablemap-0.3.0/tablemap/__init__.py
--rw-rw-rw-   0        0        0    42352 2022-12-28 08:11:05.000000 tablemap-0.3.0/tablemap/tablemap.py
-drwxrwxrwx   0        0        0        0 2022-12-28 08:35:12.102377 tablemap-0.3.0/tablemap.egg-info/
--rw-rw-rw-   0        0        0      229 2022-12-28 08:35:11.000000 tablemap-0.3.0/tablemap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2022-12-28 08:35:12.000000 tablemap-0.3.0/tablemap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-28 08:35:11.000000 tablemap-0.3.0/tablemap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-12-28 08:35:11.000000 tablemap-0.3.0/tablemap.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-12-28 08:35:12.103378 tablemap-0.3.0/test/
--rw-rw-rw-   0        0        0    39832 2022-12-28 07:59:15.000000 tablemap-0.3.0/test/test_core.py
+drwxr-xr-x   0 kenjin    (1000) kenjin    (1000)        0 2023-04-27 08:10:02.154815 tablemap-0.3.1/
+-rw-r--r--   0 kenjin    (1000) kenjin    (1000)      237 2023-04-27 08:10:02.154815 tablemap-0.3.1/PKG-INFO
+-rw-r--r--   0 kenjin    (1000) kenjin    (1000)    14157 2023-04-27 08:01:02.000000 tablemap-0.3.1/README.md
+-rw-r--r--   0 kenjin    (1000) kenjin    (1000)       38 2023-04-27 08:10:02.154815 tablemap-0.3.1/setup.cfg
+-rwxr-xr-x   0 kenjin    (1000) kenjin    (1000)      340 2023-04-27 08:04:37.000000 tablemap-0.3.1/setup.py
+drwxr-xr-x   0 kenjin    (1000) kenjin    (1000)        0 2023-04-27 08:10:02.154815 tablemap-0.3.1/tablemap/
+-rwxr-xr-x   0 kenjin    (1000) kenjin    (1000)       34 2023-04-27 08:01:02.000000 tablemap-0.3.1/tablemap/__init__.py
+-rwxr-xr-x   0 kenjin    (1000) kenjin    (1000)    42357 2023-04-27 08:01:02.000000 tablemap-0.3.1/tablemap/tablemap.py
+drwxr-xr-x   0 kenjin    (1000) kenjin    (1000)        0 2023-04-27 08:10:02.154815 tablemap-0.3.1/tablemap.egg-info/
+-rw-r--r--   0 kenjin    (1000) kenjin    (1000)      237 2023-04-27 08:10:02.000000 tablemap-0.3.1/tablemap.egg-info/PKG-INFO
+-rw-r--r--   0 kenjin    (1000) kenjin    (1000)      223 2023-04-27 08:10:02.000000 tablemap-0.3.1/tablemap.egg-info/SOURCES.txt
+-rw-r--r--   0 kenjin    (1000) kenjin    (1000)        1 2023-04-27 08:10:02.000000 tablemap-0.3.1/tablemap.egg-info/dependency_links.txt
+-rw-r--r--   0 kenjin    (1000) kenjin    (1000)       14 2023-04-27 08:10:02.000000 tablemap-0.3.1/tablemap.egg-info/top_level.txt
+drwxr-xr-x   0 kenjin    (1000) kenjin    (1000)        0 2023-04-27 08:10:02.154815 tablemap-0.3.1/test/
+-rw-r--r--   0 kenjin    (1000) kenjin    (1000)        0 2023-04-27 08:01:02.000000 tablemap-0.3.1/test/__init__.py
+-rw-r--r--   0 kenjin    (1000) kenjin    (1000)    38834 2023-04-27 08:01:02.000000 tablemap-0.3.1/test/test_core.py
```

### Comparing `tablemap-0.3.0/README.md` & `tablemap-0.3.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,411 +1,422 @@
-# About
-
-Tablemap is a handy little Python data wrangling tool for whom Pandas or SQL feel clunky when problems
-touch just one small step further than their routine, ordinary circle.
-
-While a table is nothing but a list of dictionaries, oftentimes Pandas looks like a long way around. 
-It can wait for what it's really made.
-
-Some people might be happy if only they can easily chain up some processes they do on tables 
-without worrying too much about memory. Less on stackoverflow.com for arcane Pandas spells. This is for those. 
-
-# Installation
-
-Requires only built-in Python libraries. No dependencies.
-
-```
-pip install -u tablemap
-```
-
-
-# Tutorial
-
-## Saving tables in the database
-
-Let's create a table `t1` in `sample.db`. 
-
-```python
-from tablemap import Conn, Rows
-
-t1 = [
-    {'col1': 'a', 'col2': 4},
-    {'col1': 'a', 'col2': 5},
-    {'col1': 'b', 'col2': 1},
-]
-
-conn = Conn('sample.db')
-conn['t1'] = t1
-```
-
-The right-hand side of the assignment can be a list of dictionaries, an iterator that yields dictionaries, or an object fetched from the connection (`Rows` object, shows up soon), for example, `conn['t1']` on which you can chain up table-manipulating methods such as `map`, `update`, `by`, `chain`, and so on.
-
-Each dictionary represents a row in a table. For instance `{'col1': 'a', 'col2': 4}` is a row with two columns, `col1` and `col2`.
-
-Opening and closing the database is safely handled in the background. 
-
-
-To browse tables in the database,
-
-```python
-rs = conn['t1']
-print(rs)
-
-# to turn it into a familiar data structure,
-print(rs.list())
-
-# to see only part of it 
-rs1 = rs[1:]
-print(rs1)
-
-# rs[1:] creates a new object, rs is not modified.
-print(rs.size(), rs1.size())
-```
-
-If you prefer GUI, you can open up the file `sample.db` with software like [SQLiteStudio](https://sqlitestudio.pl/) or [DB Browser for SQLite](https://sqlitebrowser.org/). 
-
-Once you clean up the table, you may wish to begin the analysis with Pandas.
-
-```python
-import pandas as pd
-
-df = pd.DataFrame(conn['t1'].list())
-conn['t1_copy'] = df.to_dict('records')
-```
-
-## Rows objects
-`conn['t1']` is a `Rows` object. Rows objects can be created in two ways
-
-1. Pass a table name to Conn object, `conn['t1']` 
-2. Directly pass a list of dictionaries or a dictionary yielding iterator to the class `Rows`, for example, `Rows(t1)`
-
-Passing a column name to a `Rows` object returns a list of elements for the column, `Rows(t1)['col1'] == ['a', 'a', 'b']`
-
-A `Rows` object represents a list of dictionaries and they have a few methods to chain up to transform a table.
-
-*** 
-
-## Methods for table manipulation
-
-+ ### `chain`
-
-To concatenate `t1` with itself,  
-
-```python
-conn['t1_double'] = conn['t1'].chain(conn['t1'])
-```
-
-A list of dictionaries or an iterator that yields dictionaries can be passed as an argument as well.
-
-```python
-conn['t1_double'] = conn['t1'].chain(t1)
-
-```
-
-Tables for concatenation must have the same columns. The order of the columns is not important.
-
-
-+ #### A few to brag about. 
-
-    Some of the properties of this module that make data-wrangling easier 
-        
-    1. All the methods in this section create a new `Rows` object.  
-
-        ```python
-        rs = conn['t1']
-        rs1 = rs.chain(t1)
-        ```
-
-        `rs` and `rs1` are different objects, so `rs` is not `chain`ed.
-
-        ```python
-        t1 = Rows(t1)
-        t1_listed =t1.list() 
-        t1_listed[0]['col1'] = 'x'
-        # Invoke another list from t1, and it's a fresh one.
-        t1.list()[0]['col1'] != 'x' 
-        ```
-
-    2. `rs` (or `rs1`) does not contain any data in the table, yet. It simply holds instructions and is executed when it's needed. (when you want it to be saved in the database, to be printed out, to be listed up, or simply to get the size of it)
-
-        So you can easily combine all the methods safely and freely, for example, (`filter` is not covered yet, hopefully, it's self-evident.)
-
-        ```python
-        rs = conn['t1']
-        high = rs.filter(lambda r: r['col2'] > 4)
-        low = rs.filter(lambda r: r['col2'] < 2)
-        rs2 = high.chain(low)
-        ```
-
-        Since `rs2` simply holds instructions without actually performing operations, the above code requires very little computing power unless you want to save it in the database or see the result for yourself.  
-
-    3. Memory requirement is minimal. 
-
-        ```python
-        conn['t1_1'] = rs2
-        ```
-
-        Now it actually works because you are trying to save the rows `rs2` generates in the table `t1_1`. Still, `tablemap` does not load up all of `rs2` on memory. It loads and saves one-by-one. 
-
-    4. Opens and closes the database automatically and safely. Users don't have to worry about it. Even the keyboard interrupts (like ctrl-c) during the table insertion do not corrupt the database.
-
- 
-
-+ ### `filter` and `update`
-Each row is simply a dictionary with column names as keys, so you can access a column value by passing a column name to the row(dictionary). To create new columns or update the existing ones,
-
-```python
-# \ for line-continuation
-conn['t1_1'] = conn['t1']\
-    .filter(lambda r: r['col2'] > 2)\
-    .update(
-        col2=lambda r: r['col2'] + 1,
-        col3=lambda r: r['col1'] + str(r['col2'])
-    )
-```
-
-A lambda expression is a nameless function. In the expression `lambda r: r['col2'] > 2`, the parameter `r` represents a single dictionary and the whole expression returns an evaluated value of `r['col'] > 2` for each iteration.
-
-Columns are updated sequentially, so `col3` has `a5` and `a6`, not `a4` and `a5`.
-
-
-+ ### `by` and `fold`
-
-To sum up `col2` grouped by `col1`,
-
-```python
-conn['t1_col2sum_groupby_col1'] = conn['t1'].by('col1')\
-    .fold(
-        col2_sum=lambda rs: sum(rs['col2']),
-        col2_min=lambda rs: min(rs['col2']),
-        col2_max=lambda rs: max(rs['col2']),
-    )
-```
-
-`by` takes fields as an arguement(list of field names or comma separated field names) for grouping and the next process (`fold` in this case) takes on each group (a `Rows` object).
-
-In the expression `lambda rs: sum(rs['col2'])`, the parameter `rs` represents a `Rows` object. So `rs['col2']` returns a list of elements in the column `col2`. And of course for that reason, you may chain up all the methods in this section.
-
-While `update` works on a dictionary, `fold` does on a `Rows` object. (`fold` folds n rows to one row. So the lambda expression in `fold` must return a single value, like a string or a number.)
-
-`fold` must be preceded by grouping methods such as `by` or `windowed` which shows up soon. `filter` may or may not be preceded by grouping methods. 
-
-+ ### `rename`
-
-To replace old column names with new ones,
-
-```python
-conn['t1_1'].rename(
-    c2min='col2_min',
-    c2max='col2_max'
-)
-```
-
-+ ### `join`
-
-To merge tables,
-
-```python
-conn['t2'] = [
-    {'col1': 'b', 'col3': -1},
-    {'col1': 'c', 'col3': 3},
-    {'col1': 'b', 'col3': ''},
-]
-
-conn['t1_col3'] = conn['t1'].by('col1')\
-    .join(conn['t2'].by('col1'), 'full')
-```
-
-There are 4 join types, 'inner', 'left', 'right', and 'full'. The default is 'inner'. You may want to check [this tutorial](https://www.w3schools.com/sql/sql_join.asp) if you are not familiar with these terms.
-
-Tables must be grouped to be joined.
-
-If the table `t1` and `t2` have columns with the same name, `t1` columns will be updated with `t2` columns.
-
-Empty strings represent missing values.
-
-
-
-
-+ ### `distinct`
-To group the table `t1` by `col1` and to leave only the first row in each group, (removing duplicates) 
-
-```python
-conn['t1_1'] = conn['t1'].distinct('col1')
-```
-You can pass multiple columns to `distinct` as in `by`
-
-+ ### `select` and `deselect` 
-You can pass columns to `select` or `deselect` to pick up or delete specific columns in a table
-
-```python
-conn['t1_1'] = conn['t1'].update(col3=lambda r: r['col2'] + 1)\
-    .deselect('col1, col2')
-```
-
-
-+ ### slicing 
-
-To take the first 2 rows from table `t1`,
-
-```python
-print(conn['t1'][:2])
-```
-
-Negative values are not supported. Of course, you can chain up other methods after slicing. 
-
-Like the other methods, slicing does not execute the operation. `conn['t1'][:2]` holds the instruction to take the first two rows, not the rows themselves. However `print` function enforces taking the first two rows to print out on the screen. So it works as expected.
-
-Grouping methods like `by` or `windowed` may come right before slicing and the rows will be flattened. 
-
-`conn['t1']['col1']` is not slicing, it returns a list of column values, not a `Rows` object. 
-
-+ ### `takewhile` and `dropwhile`
-`takewhile` and `dropwhile` take a predicate (a function that returns a value to be considered `True` or `False`, already seen it in `filter`) as an argument to do what these names suggest. Refer to [itertools.takewhile](https://docs.python.org/3/library/itertools.html#itertools.takewhile) and [itertools.dropwhile](https://docs.python.org/3/library/itertools.html#itertools.dropwhile)
-
-Grouping methods may be preceded right before these methods.
-
-
-+ ### `map`
-
-When `update` or `fold` is not powerful enough, you can deal with a row or `Rows` in a more sophisticated way.
-
-```python
-# Some of you may feel uncomfortable with the naming.
-# This is just a lambda function for 'map'
-# Hard to justify spending time on naming a function used nowhere else.
-def fn4t1(rs):
-    # rs is a Rows object. 
-    # Now you can apply all the methods in this section.
-    # And again, since these methods create a new Rows object instead of modifying the original,
-    # it's safe to build any combinations as you want. 
-    tot = sum(rs['col2'])
-    # you don't always have to pass a function to `update`, same for `fold`
-    return rs[:1].update(col2_sum=tot)
-
-conn['t1_col2sum_groupby_col1'] = conn['t1'].by('col1')\
-    .map(fn4t1)\
-    .deselect('col2')
-```
-
-The argument for `map` is a function that returns a `Rows` object or a single dictionary, or None. It takes a single dictionary as an argument or a `Rows` object in case the previous process is `by`(`group`) or `windowed`.
-
-
-
-+ ### `zip` and `zip_longest`
-Like `chain`, zip takes a list of dictionaries or an iterator that yields dictionaries or a `Rows` object as an argument. The argument updates the `Rows` object row by row until either one is depleted. 
-
-With `zip`, the above `fn4t1` can be rewritten as
-
-```python
-def fn4t1(rs):
-    rs2 = [{'col2_sum': sum(rs['col2'])}]
-    return rs.zip(rs2)
-```
-
-Another example,
-
-```python
-conn['t1_1'] = conn['t1'].zip({'idx': i} for i in range(100))
-```
-
-`zip_longest` creates empty columns when either one is depleted.
-
-+ ### `merge`
-
-The same interface as `join`. While `join` combines cross-producted rows from two tables,
-`merge` simply `zip_longest` them. For example when `join` combines 2 rows against 3 rows in each group,
-6 rows are generated while `merge` produces only 3 rows.
-
-
-+ ### `windowed`
-When you need to group a chunk of consecutive rows,
-
-```python
-conn['t1_1'] = conn['t1'].windowed(4, 2).fold(
-    sum=lambda rs: sum(rs['col2'])
-)
-```
-
-`fold` takes the first 4 consecutive rows(of course a `Rows` object) and the next 4 starting from the 3rd (skipping 2 rows) and so on. When rows less than or equal to 4 are left, it will be the last. 
-
-+ ### `order` and `group`
-
-Actually, `by` is a combination of `order` and `group`, you can control more precise by separating these processes, 
-
-```python
-conn['t1_col2sum_groupby_col1'] = conn['t1']\
-    .order('col1, col2 desc').group('col1')\
-    .map(fn4t1)
-```
-
-Now, `map` takes a `Rows` object where `col2` is sorted in descending order.
-
-The keyword `desc` can be either upper-cased, lower-cased or mixed. 
-
-The ascending order is the default.
- 
- + ### `index`
-
- ```python
-conn['t1'].index('index_column', start=1, step=2)
-conn['t1'].by('col1').index('group_index_column')
- ```
-
-+ ### `split`
- ```python
-# xs is a list of Rows
-xs = conn['t1'].by('col1').split()
- ```
-
-
-## Some remarks 
-
-- cross-join example
-
-    ```python
-    # table2 = conn['t1'] does not do any good.
-    # You should list it up. 
-    # Otherwise 'map' attempts to fetch 
-    # the table 't2' from the database 
-    # for every group by 'col1' 
-    table2 = conn['t2'].list()
-
-    def fn4t1():
-        def innerfn(rs):
-            ...do some work using table2
-            return something 
-        return innerfn
-
-    conn['some_table'] = conn['t1'].by('col1').map(fn4t1())
-    ```
-
-- `Rows` methods do not update objects directly. They create a new object every time a `Rows` method is invoked.
-
-    So the following code works as expected.
-    ```python
-    rs = conn['t1']
-    rs.by('col1').fold(col2_tot=sum(rs['col2']))
-    ```
-    In expression `sum(rs['col2'])`, `rs` represents a `Rows` object when the statement `rs = conn['t1']` is evaluated. Methods like `by` or `fold` in the statement do not affect `rs` in `sum(rs('col2'))`.
-
-    Take a close look at the next.
-
-    ```python
-    def fn4t1(rs):
-        # The original rs is not updated
-        # Only newrs holds the instruction to update the column 'col2' 
-        # (The update instruction will not be executed in the next statement, 
-        # newrs simply keeps the instruction here for the time it's really needed, 
-        # like for example, database insertion or content print-out)
-        newrs = rs.update(col2=lambda r: r['col2'] + 1)
-        return newrs.order('col2').zip(rs.order('col2 desc').rename(col2_1='col2'))
-
-    conn['t1_1'] = conn['t1'].by('col1').map(fn4t1)
-
-    ``` 
-
-- Since column names are dictionary keys, they are case-sensitive. However, column names in Sqlite3 (on which `tablemap` is powered) are case-insensitive by default. To avoid confusion, it is strongly recommended that you keep them lower-cased, and spaces stripped. 
-
-    `tablemap` does not automatically convert upper-case column names. Making any excessive assumptions on users' intentions might add more confusions. 
-
+# About
+
+Tablemap is a handy little Python data wrangling tool for whom Pandas or SQL feel clunky when problems
+touch just one small step further than their routine, ordinary circle.
+
+While a table is nothing but a list of dictionaries, oftentimes Pandas looks like a long way around. 
+It can wait for what it's really made.
+
+Some people might be happy if only they can easily chain up some processes they do on tables 
+without worrying too much about memory. Less on stackoverflow.com for arcane Pandas spells. This is for those. 
+
+# Installation
+
+Requires only built-in Python libraries. No dependencies.
+
+```
+pip install -u tablemap
+```
+
+
+# Tutorial
+
+## Saving tables in the database
+
+Let's create a table `t1` in `sample.db`. 
+
+```python
+from tablemap import Conn, Rows
+
+t1 = [
+    {'col1': 'a', 'col2': 4},
+    {'col1': 'a', 'col2': 5},
+    {'col1': 'b', 'col2': 1},
+]
+
+conn = Conn('sample.db')
+conn['t1'] = t1
+```
+
+The right-hand side of the assignment can be a list of dictionaries, an iterator that yields dictionaries, or an object fetched from the connection (`Rows` object, shows up soon), for example, `conn['t1']` on which you can chain up table-manipulating methods such as `map`, `update`, `by`, `chain`, and so on.
+
+Each dictionary represents a row in a table. For instance `{'col1': 'a', 'col2': 4}` is a row with two columns, `col1` and `col2`.
+
+Opening and closing the database is safely handled in the background. 
+
+
+To browse tables in the database,
+
+```python
+rs = conn['t1']
+print(rs)
+
+# to turn it into a familiar data structure,
+print(rs.list())
+
+# to see only part of it 
+rs1 = rs[1:]
+print(rs1)
+
+# rs[1:] creates a new object, rs is not modified.
+print(rs.size(), rs1.size())
+```
+
+If you prefer GUI, you can open up the file `sample.db` with software like [SQLiteStudio](https://sqlitestudio.pl/) or [DB Browser for SQLite](https://sqlitebrowser.org/). 
+
+Once you clean up the table, you may wish to begin the analysis with Pandas.
+
+```python
+import pandas as pd
+
+df = pd.DataFrame(conn['t1'].list())
+conn['t1_copy'] = df.to_dict('records')
+```
+
+## Rows objects
+`conn['t1']` is a `Rows` object. Rows objects can be created in two ways
+
+1. Pass a table name to Conn object, `conn['t1']` 
+2. Directly pass a list of dictionaries or a dictionary yielding iterator to the class `Rows`, for example, `Rows(t1)`
+
+Passing a column name to a `Rows` object returns a list of elements for the column, `Rows(t1)['col1'] == ['a', 'a', 'b']`
+
+A `Rows` object represents a list of dictionaries and they have a few methods to chain up to transform a table.
+
+*** 
+
+## Methods for table manipulation
+
++ ### `chain`
+
+To concatenate `t1` with itself,  
+
+```python
+conn['t1_double'] = conn['t1'].chain(conn['t1'])
+```
+
+A list of dictionaries or an iterator that yields dictionaries can be passed as an argument as well.
+
+```python
+conn['t1_double'] = conn['t1'].chain(t1)
+
+```
+
+Tables for concatenation must have the same columns. The order of the columns is not important.
+
+
++ #### A few to brag about. 
+
+    Some of the properties of this module that make data-wrangling easier 
+        
+    1. All the methods in this section create a new `Rows` object.  
+
+        ```python
+        rs = conn['t1']
+        rs1 = rs.chain(t1)
+        ```
+
+        `rs` and `rs1` are different objects, so `rs` is not `chain`ed.
+
+        ```python
+        t1 = Rows(t1)
+        t1_listed =t1.list() 
+        t1_listed[0]['col1'] = 'x'
+        # Invoke another list from t1, and it's a fresh one.
+        t1.list()[0]['col1'] != 'x' 
+        ```
+
+    2. `rs` (or `rs1`) does not contain any data in the table, yet. It simply holds instructions and is executed when it's needed. (when you want it to be saved in the database, to be printed out, to be listed up, or simply to get the size of it)
+
+        So you can easily combine all the methods safely and freely, for example, (`filter` is not covered yet, hopefully, it's self-evident.)
+
+        ```python
+        rs = conn['t1']
+        high = rs.filter(lambda r: r['col2'] > 4)
+        low = rs.filter(lambda r: r['col2'] < 2)
+        rs2 = high.chain(low)
+        ```
+
+        Since `rs2` simply holds instructions without actually performing operations, the above code requires very little computing power unless you want to save it in the database or see the result for yourself.  
+
+    3. Memory requirement is minimal. 
+
+        ```python
+        conn['t1_1'] = rs2
+        ```
+
+        Now it actually works because you are trying to save the rows `rs2` generates in the table `t1_1`. Still, `tablemap` does not load up all of `rs2` on memory. It loads and saves one-by-one. 
+
+    4. Opens and closes the database automatically and safely. Users don't have to worry about it. Even the keyboard interrupts (like ctrl-c) during the table insertion do not corrupt the database.
+
+ 
+
++ ### `filter` and `update`
+Each row is simply a dictionary with column names as keys, so you can access a column value by passing a column name to the row(dictionary). To create new columns or update the existing ones,
+
+```python
+# \ for line-continuation
+conn['t1_1'] = conn['t1']\
+    .filter(lambda r: r['col2'] > 2)\
+    .update(
+        col2=lambda r: r['col2'] + 1,
+        col3=lambda r: r['col1'] + str(r['col2'])
+    )
+```
+
+A lambda expression is a nameless function. In the expression `lambda r: r['col2'] > 2`, the parameter `r` represents a single dictionary and the whole expression returns an evaluated value of `r['col'] > 2` for each iteration.
+
+Columns are updated sequentially, so `col3` has `a5` and `a6`, not `a4` and `a5`.
+
+
++ ### `by` and `fold`
+
+To sum up `col2` grouped by `col1`,
+
+```python
+conn['t1_col2sum_groupby_col1'] = conn['t1'].by('col1')\
+    .fold(
+        col2_sum=lambda rs: sum(rs['col2']),
+        col2_min=lambda rs: min(rs['col2']),
+        col2_max=lambda rs: max(rs['col2']),
+    )
+```
+
+`by` takes fields as an arguement(list of field names or comma separated field names) for grouping and the next process (`fold` in this case) takes on each group (a `Rows` object).
+
+In the expression `lambda rs: sum(rs['col2'])`, the parameter `rs` represents a `Rows` object. So `rs['col2']` returns a list of elements in the column `col2`. And of course for that reason, you may chain up all the methods in this section.
+
+While `update` works on a dictionary, `fold` does on a `Rows` object. (`fold` folds n rows to one row. So the lambda expression in `fold` must return a single value, like a string or a number.)
+
+`fold` must be preceded by grouping methods such as `by` or `windowed` which shows up soon. `filter` may or may not be preceded by grouping methods. 
+
++ ### `rename`
+
+To replace old column names with new ones,
+
+```python
+conn['t1_1'].rename(
+    c2min='col2_min',
+    c2max='col2_max'
+)
+```
+
++ ### `join`
+
+To merge tables,
+
+```python
+conn['t2'] = [
+    {'col1': 'b', 'col3': -1},
+    {'col1': 'c', 'col3': 3},
+    {'col1': 'b', 'col3': ''},
+]
+
+conn['t1_col3'] = conn['t1'].by('col1')\
+    .join(conn['t2'].by('col1'), 'full')
+```
+
+There are 4 join types, 'inner', 'left', 'right', and 'full'. The default is 'inner'. You may want to check [this tutorial](https://www.w3schools.com/sql/sql_join.asp) if you are not familiar with these terms.
+
+Tables must be grouped to be joined.
+
+If the table `t1` and `t2` have columns with the same name, `t1` columns will be updated with `t2` columns.
+
+Empty strings represent missing values.
+
+
+
+
++ ### `distinct`
+To group the table `t1` by `col1` and to leave only the first row in each group, (removing duplicates) 
+
+```python
+conn['t1_1'] = conn['t1'].distinct('col1')
+```
+You can pass multiple columns to `distinct` as in `by`
+
++ ### `select` and `deselect` 
+You can pass columns to `select` or `deselect` to pick up or delete specific columns in a table
+
+```python
+conn['t1_1'] = conn['t1'].update(col3=lambda r: r['col2'] + 1)\
+    .deselect('col1, col2')
+```
+
+
++ ### slicing 
+
+To take the first 2 rows from table `t1`,
+
+```python
+print(conn['t1'][:2])
+```
+
+Negative values are not supported. Of course, you can chain up other methods after slicing. 
+
+Like the other methods, slicing does not execute the operation. `conn['t1'][:2]` holds the instruction to take the first two rows, not the rows themselves. However `print` function enforces taking the first two rows to print out on the screen. So it works as expected.
+
+Grouping methods like `by` or `windowed` may come right before slicing and the rows will be flattened. 
+
+`conn['t1']['col1']` is not slicing, it returns a list of column values, not a `Rows` object. 
+
++ ### `takewhile` and `dropwhile`
+`takewhile` and `dropwhile` take a predicate (a function that returns a value to be considered `True` or `False`, already seen it in `filter`) as an argument to do what these names suggest. Refer to [itertools.takewhile](https://docs.python.org/3/library/itertools.html#itertools.takewhile) and [itertools.dropwhile](https://docs.python.org/3/library/itertools.html#itertools.dropwhile)
+
+Grouping methods may be preceded right before these methods.
+
+
++ ### `map`
+
+When `update` or `fold` is not powerful enough, you can deal with a row or `Rows` in a more sophisticated way.
+
+```python
+# Some of you may feel uncomfortable with the naming.
+# This is just a lambda function for 'map'
+# Hard to justify spending time on naming a function used nowhere else.
+def fn4t1(rs):
+    # rs is a Rows object. 
+    # Now you can apply all the methods in this section.
+    # And again, since these methods create a new Rows object instead of modifying the original,
+    # it's safe to build any combinations as you want. 
+    tot = sum(rs['col2'])
+    # you don't always have to pass a function to `update`, same for `fold`
+    return rs[:1].update(col2_sum=tot)
+
+conn['t1_col2sum_groupby_col1'] = conn['t1'].by('col1')\
+    .map(fn4t1)\
+    .deselect('col2')
+```
+
+The argument for `map` is a function that returns a `Rows` object or a single dictionary, or None. It takes a single dictionary as an argument or a `Rows` object in case the previous process is `by`(`group`) or `windowed`.
+
+
+
++ ### `zip` and `zip_longest`
+Like `chain`, zip takes a list of dictionaries or an iterator that yields dictionaries or a `Rows` object as an argument. The argument updates the `Rows` object row by row until either one is depleted. 
+
+With `zip`, the above `fn4t1` can be rewritten as
+
+```python
+def fn4t1(rs):
+    rs2 = [{'col2_sum': sum(rs['col2'])}]
+    return rs.zip(rs2)
+```
+
+Another example,
+
+```python
+conn['t1_1'] = conn['t1'].zip({'idx': i} for i in range(100))
+```
+
+`zip_longest` creates empty columns when either one is depleted.
+
++ ### `merge`
+
+The same interface as `join`. While `join` combines cross-producted rows from two tables,
+`merge` simply `zip_longest` them. For example when `join` combines 2 rows against 3 rows in each group,
+6 rows are generated while `merge` produces only 3 rows.
+
+
+ + ### `index`
+To add an index column,
+
+ ```python
+conn['t1'].index('index_column', start=1, step=2)
+conn['t1'].by('col1').index('group_index_column')
+ ```
+
+
++ ### `windowed`
+When you need to group a chunk of consecutive rows,
+
+```python
+conn['t1_1'] = conn['t1'].windowed(4, 2).fold(
+    sum=lambda rs: sum(rs['col2'])
+)
+
+# works with `by`, for example
+conn['t1'].by('col1').windowed(3).index('cnt')
+```
+
+`fold` takes the first 4 consecutive rows(of course a `Rows` object) and the next 4 starting from the 3rd (skipping 2 rows) and so on. When rows less than or equal to 4 are left, it will be the last. 
+
+Grouped rows can also be windowed.
+
+```python
+print(conn['t1'].by('col1').windowed(3).index('group_no'))
+```
+
++ ### `order` and `group`
+
+Actually, `by` is a combination of `order` and `group`, you can control more precise by separating these processes, 
+
+```python
+conn['t1_col2sum_groupby_col1'] = conn['t1']\
+    .order('col1, col2 desc').group('col1')\
+    .map(fn4t1)
+```
+
+Now, `map` takes a `Rows` object where `col2` is sorted in descending order.
+
+The keyword `desc` can be either upper-cased, lower-cased or mixed. 
+
+The ascending order is the default.
+ 
+
+
++ ### `split`
+ ```python
+# xs is a list of Rows
+xs = conn['t1'].by('col1').split()
+ ```
+
+
+## Some remarks 
+
+- cross-join example
+
+    ```python
+    # table2 = conn['t1'] does not do any good.
+    # You should list it up. 
+    # Otherwise 'map' attempts to fetch 
+    # the table 't2' from the database 
+    # for every group by 'col1' 
+    table2 = conn['t2'].list()
+
+    def fn4t1(rs):
+        ...do some work using table2
+        return something 
+
+    conn['some_table'] = conn['t1'].by('col1').map(fn4t1)
+    ```
+
+- `Rows` methods do not update objects directly. They create a new object every time a `Rows` method is invoked.
+
+    So the following code works as expected.
+    ```python
+    rs = conn['t1']
+    rs.by('col1').fold(col2_tot=sum(rs['col2']))
+    ```
+    In expression `sum(rs['col2'])`, `rs` represents a `Rows` object when the statement `rs = conn['t1']` is evaluated. Methods like `by` or `fold` in the statement do not affect `rs` in `sum(rs('col2'))`.
+
+    Take a close look at the next.
+
+    ```python
+    def fn4t1(rs):
+        # The original rs is not updated
+        # Only newrs holds the instruction to update the column 'col2' 
+        # (The update instruction will not be executed in the next statement, 
+        # newrs simply keeps the instruction here for the time it's really needed, 
+        # like for example, database insertion or content print-out)
+        newrs = rs.update(col2=lambda r: r['col2'] + 1)
+        return newrs.order('col2').zip(rs.order('col2 desc').rename(col2_1='col2'))
+
+    conn['t1_1'] = conn['t1'].by('col1').map(fn4t1)
+
+    ``` 
+
+- Since column names are dictionary keys, they are case-sensitive. However, column names in Sqlite3 (on which `tablemap` is powered) are case-insensitive by default. To avoid confusion, it is strongly recommended that you keep them lower-cased, and spaces stripped. 
+
+    `tablemap` does not automatically convert upper-case column names. Making any excessive assumptions on users' intentions might add more confusions. 
+
 ## [API Documentation](https://tablemap.readthedocs.io/en/latest/tablemap.html#module-tablemap.tablemap)
```

### Comparing `tablemap-0.3.0/tablemap/tablemap.py` & `tablemap-0.3.1/tablemap/tablemap.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,20 +150,22 @@
 
         if hist[-1]['cmd'] == 'group':
             return [Rows(rows) for _, rows in pgen()]
 
         return [Rows(rows) for rows in pgen()]
 
     def index(self, field, start=0, step=1):
-        """Add an index column
+        """Adds an index column
 
         Parameters
         ----------
         field: str
+
         start: int (default 0)
+
         step: int (default 1)
 
         Returns
         -------
         Rows
         """
         def gen_single():
```

### Comparing `tablemap-0.3.0/test/test_core.py` & `tablemap-0.3.1/test/test_core.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,998 +1,998 @@
-import os
-import unittest
-from itertools import product
-from pathlib import Path
-
-from tablemap import Conn, Rows
-
-
-class TestCore(unittest.TestCase):
-    def setUp(self):
-        self.dbfile = 'test/sample.db'
-        self.dbfile1 = 'test/sample1.db'
-
-        self.t1 = [
-            {'col1': 'a', 'col2': 4},
-            {'col1': 'a', 'col2': 5},
-            {'col1': 'b', 'col2': 1},
-            {'col1': 'c', 'col2': 3},
-            {'col1': 'c', 'col2': 4},
-            {'col1': 'c', 'col2': 7},
-            {'col1': 'd', 'col2': 2},
-
-        ]
-
-        self.t2 = [
-            {'col1': 'd', 'col3': 3},
-            {'col1': 'b', 'col3': 1},
-            {'col1': 'e', 'col3': 3},
-            {'col1': 'e', 'col3': 4},
-            {'col1': 'd', 'col3': 2},
-        ]
-
-    def tearDown(self):
-        if Path(self.dbfile).is_file():
-            os.remove(self.dbfile)
-        if Path(self.dbfile1).is_file():
-            os.remove(self.dbfile1)
-
-    def test_takewhile_group(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-
-        self.assertEqual(conn['t1'].by('col1')
-                         .takewhile(lambda rs: rs['col1'][0] < 'c').list(),
-                         [{'col1': 'a', 'col2': 4},
-                          {'col1': 'a', 'col2': 5},
-                          {'col1': 'b', 'col2': 1}]
-                         )
-
-        self.assertEqual(conn['t1'].windowed(4, 2)
-                         .takewhile(lambda rs: rs.size() == 4).list(),
-                         [{'col1': 'a', 'col2': 4},
-                          {'col1': 'a', 'col2': 5},
-                          {'col1': 'b', 'col2': 1},
-                          {'col1': 'c', 'col2': 3},
-                          {'col1': 'b', 'col2': 1},
-                          {'col1': 'c', 'col2': 3},
-                          {'col1': 'c', 'col2': 4},
-                          {'col1': 'c', 'col2': 7}])
-
-    def test_dropwhile_group(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-
-        self.assertEqual(conn['t1'].by('col1')
-                         .dropwhile(lambda rs: rs['col1'][0] < 'c').list(),
-                         [{'col1': 'c', 'col2': 3},
-                          {'col1': 'c', 'col2': 4},
-                          {'col1': 'c', 'col2': 7},
-                          {'col1': 'd', 'col2': 2}])
-
-        self.assertEqual(conn['t1'].windowed(4, 2)
-                         .dropwhile(lambda rs: rs.size() == 4).list(),
-                         [{'col1': 'c', 'col2': 4},
-                          {'col1': 'c', 'col2': 7},
-                          {'col1': 'd', 'col2': 2}])
-
-    def test_split(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-
-        xs = conn['t1'].group('col1').split()
-        self.assertEqual(len(xs[0].list()), 2)
-        self.assertEqual(len(xs[1].list()), 1)
-        self.assertEqual(len(xs[2].list()), 3)
-        self.assertEqual(len(xs[3].list()), 1)
-
-        xs = conn['t1'].windowed(4, 2).split()
-        self.assertEqual(len(xs[0].list()), 4)
-        self.assertEqual(len(xs[1].list()), 4)
-        self.assertEqual(len(xs[2].list()), 3)
-
-        xs1 = xs[2].update(foo=4)
-        # test xs[1] is unaffected
-        self.assertEqual(xs[1].list(),
-                         [{'col1': 'b', 'col2': 1},
-                          {'col1': 'c', 'col2': 3},
-                          {'col1': 'c', 'col2': 4},
-                          {'col1': 'c', 'col2': 7}])
-
-    def test_size_group(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-        self.assertEqual(conn['t1'].group('col1').size(), 4)
-        self.assertEqual(conn['t1'].windowed(4, 2).size(), 3)
-
-    def test_index1(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-        conn['t1_1'] = conn['t1'].index('foo')
-        self.assertEqual(conn['t1_1']['foo'], [0, 1, 2, 3, 4, 5, 6])
-
-        conn['t1_1'] = conn['t1'].group('col1').index('foo', 1, 2)
-        self.assertEqual(conn['t1_1']['foo'], [1, 1, 3, 5, 5, 5, 7])
-        conn['t1_1'] = conn['t1'].windowed(4, 2).index('foo', 1, 2)
-        self.assertEqual(conn['t1_1']['foo'], [
-                         1, 1, 1, 1, 3, 3, 3, 3, 5, 5, 5])
-
-    def test_order_when_no_row(self):
-        rs1 = Rows([])
-        self.assertEqual(rs1.order('col1').list(), [])
-
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-        self.assertEqual(
-            conn['t1'].filter(lambda r: r['col2'] > 100).order('col1').list(),
-            [])
-
-    def test_size(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-
-        self.assertEqual(conn['t1'].size(), len(self.t1))
-        # size is executed while the connection is open
-        self.assertEqual(conn['t1'].update(n=lambda r: conn['t1'].size())["n"],
-                         [7] * 7)
-        # size is executed when the connection is closed
-        self.assertEqual(conn['t1'].update(n=conn['t1'].size())["n"],
-                         [7] * 7)
-
-        rs = Rows(self.t1)
-        self.assertEqual(rs.size(), len(self.t1))
-
-        rs1 = rs[3:6]
-        self.assertEqual(rs1.size(), 3)
-
-    def test_wierd(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-
-        xs = conn['t1']
-        self.assertEqual(xs.by('col1').fold(col2_tot=sum(xs['col2'])).list(),
-                         [{'col1': 'a', 'col2_tot': 26},
-                         {'col1': 'b', 'col2_tot': 26},
-                         {'col1': 'c', 'col2_tot': 26},
-                         {'col1': 'd', 'col2_tot': 26}])
-
-    def test_modification(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-
-        rs1 = conn['t1']
-        rs2 = rs1.update(col2=lambda r: r['col2'] + 1)
-
-        # the following code does not work, you cannot execute a fetch
-        # while another fetch is being done.
-        # So iter should not be exposed.
-        # for r1, r2 in zip(rs1._iter(), rs2._iter()):
-        #     print(r1, r2)
-
-        rs1 = rs1.list()
-        rs2 = rs2.list()
-
-        for r1, r2 in zip(rs1, rs2):
-            self.assertEqual(r1['col2'] + 1, r2['col2'])
-
-    def test_list_mod(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-        t1 = conn['t1']
-        t1_listed = t1.list()
-        t1_listed[0]['col1'] = 'x'
-        self.assertNotEqual(
-            t1.list()[0]['col1'], 'x'
-        )
-        self.assertEqual(
-            t1_listed[0]['col1'], 'x'
-        )
-
-    def test_list_mod1(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-
-        def tempfn(rs):
-            rslist = rs.list()
-            for r in rslist:
-                r['col2'] += 1
-            # this should not do anything
-            return rs
-
-        conn['t1_1'] = conn['t1'].by('col1').map(tempfn)
-        self.assertEqual(conn['t1_1'].list(), conn['t1'].list())
-
-    def test_do_later(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-
-        xs = conn['t1']
-        xs1 = xs.by('col1')
-        tot = sum(xs['col2'])
-        xs1 = xs1.fold(
-            col3=lambda rs: sum(rs['col2']),
-            col4=tot
-        )
-        self.assertEqual(xs1.list(),
-                         [{'col1': 'a', 'col3': 9, 'col4': 26},
-                          {'col1': 'b', 'col3': 1, 'col4': 26},
-                          {'col1': 'c', 'col3': 14, 'col4': 26},
-                          {'col1': 'd', 'col3': 2, 'col4': 26}])
-
-    def test_zip(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-
-        def tempfn(rs):
-            return rs.zip([
-                {'n': 1},
-                {'n': 2}
-            ])
-
-        conn['t1_1'] = conn['t1'].by('col1').map(tempfn)
-        self.assertEqual(conn['t1_1'].list(),
-                         [{'col1': 'a', 'col2': 4, 'n': 1},
-                          {'col1': 'a', 'col2': 5, 'n': 2},
-                          {'col1': 'b', 'col2': 1, 'n': 1},
-                          {'col1': 'c', 'col2': 3, 'n': 1},
-                          {'col1': 'c', 'col2': 4, 'n': 2},
-                          {'col1': 'd', 'col2': 2, 'n': 1}]
-                         )
-
-    def test_zip2(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-
-        conn['t1_1'] = conn['t1'].zip({'idx': i} for i in range(100))
-        self.assertEqual(conn['t1_1']['idx'], list(range(len(self.t1))))
-
-    def test_zip_longest(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-
-        def tempfn(rs):
-            return rs.zip_longest([
-                {'n': 1},
-                {'n': 2}
-            ])
-
-        conn['t1_1'] = conn['t1'].by('col1').map(tempfn)
-        self.assertEqual(conn['t1_1'].list(),
-                         [{'col1': 'a', 'col2': 4, 'n': 1},
-                          {'col1': 'a', 'col2': 5, 'n': 2},
-                          {'col1': 'b', 'col2': 1, 'n': 1},
-                          {'col1': '', 'col2': '', 'n': 2},
-                          {'col1': 'c', 'col2': 3, 'n': 1},
-                          {'col1': 'c', 'col2': 4, 'n': 2},
-                          {'col1': 'c', 'col2': 7, 'n': ''},
-                          {'col1': 'd', 'col2': 2, 'n': 1},
-                          {'col1': '', 'col2': '', 'n': 2}]
-                         )
-
-    def test_zip_longest2(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-
-        conn['t1_1'] = conn['t1'].zip_longest(({'n': i} for i in range(10)))
-        self.assertEqual(conn['t1_1'].list(),
-                         [{'col1': 'a', 'col2': 4, 'n': 0},
-                          {'col1': 'a', 'col2': 5, 'n': 1},
-                          {'col1': 'b', 'col2': 1, 'n': 2},
-                          {'col1': 'c', 'col2': 3, 'n': 3},
-                          {'col1': 'c', 'col2': 4, 'n': 4},
-                          {'col1': 'c', 'col2': 7, 'n': 5},
-                          {'col1': 'd', 'col2': 2, 'n': 6},
-                          {'col1': '', 'col2': '', 'n': 7},
-                          {'col1': '', 'col2': '', 'n': 8},
-                          {'col1': '', 'col2': '', 'n': 9}])
-
-        conn['t1_2'] = conn['t1'].zip_longest(({'n': i} for i in range(5)))
-        self.assertEqual(conn['t1_2'].list(),
-                         [{'col1': 'a', 'col2': 4, 'n': 0},
-                          {'col1': 'a', 'col2': 5, 'n': 1},
-                          {'col1': 'b', 'col2': 1, 'n': 2},
-                          {'col1': 'c', 'col2': 3, 'n': 3},
-                          {'col1': 'c', 'col2': 4, 'n': 4},
-                          {'col1': 'c', 'col2': 7, 'n': ''},
-                          {'col1': 'd', 'col2': 2, 'n': ''}])
-
-    def test_tee_n_new(self):
-        conn = Conn(self.dbfile)
-
-        def tempfn1(rs):
-            return rs.order('col2 desc').chain(rs.order('col2'))
-        conn['t10'] = self.t1
-
-        conn['t1_1'] = conn['t10'].by('col1').map(tempfn1)
-
-        self.assertEqual(conn['t1_1']['col2'],
-                         [5, 4, 4, 5, 1, 1, 7, 4, 3, 3, 4, 7, 2, 2])
-
-        def tempfn2(rs):
-            rs1 = rs.update(col2=lambda r: r['col2'] + 1)
-            return rs1.order('col2 desc').chain(rs.order('col2'))
-
-        conn['t1'] = self.t1
-        conn['t1_1'] = conn['t1'].by('col1').map(tempfn2)
-        self.assertEqual(conn['t1_1']['col2'],
-                         [6, 5, 4, 5, 2, 1, 8, 5, 4, 3, 4, 7, 3, 2])
-
-    def test_tee_n_new2(self):
-        conn = Conn(self.dbfile)
-
-        def tempfn(rs):
-            return rs.order('col2').zip(rs.order('col2 desc')
-                                        .rename(col2_1='col2'))
-
-        conn['t1'] = self.t1
-        conn['t1_1'] = conn['t1'].by('col1').map(tempfn)
-        xs = [{'col1': 'a', 'col2': 4, 'col2_1': 5},
-              {'col1': 'a', 'col2': 5, 'col2_1': 4},
-              {'col1': 'b', 'col2': 1, 'col2_1': 1},
-              {'col1': 'c', 'col2': 3, 'col2_1': 7},
-              {'col1': 'c', 'col2': 4, 'col2_1': 4},
-              {'col1': 'c', 'col2': 7, 'col2_1': 3},
-              {'col1': 'd', 'col2': 2, 'col2_1': 2}]
-        self.assertEqual(conn['t1_1'].list(), xs)
-
-        def tempfn1(rs):
-            rs1 = rs.update(col2=lambda r: r['col2'] + 1)
-            return rs1.order('col2').zip(rs.order('col2 desc')
-                                         .rename(col2_1='col2'))
-
-        conn['t1_1'] = conn['t1'].by('col1').map(tempfn1)
-
-        xs = [{'col1': 'a', 'col2': 5, 'col2_1': 5},
-              {'col1': 'a', 'col2': 6, 'col2_1': 4},
-              {'col1': 'b', 'col2': 2, 'col2_1': 1},
-              {'col1': 'c', 'col2': 4, 'col2_1': 7},
-              {'col1': 'c', 'col2': 5, 'col2_1': 4},
-              {'col1': 'c', 'col2': 8, 'col2_1': 3},
-              {'col1': 'd', 'col2': 3, 'col2_1': 2}]
-
-        self.assertEqual(conn['t1_1'].list(), xs)
-
-    def test_index(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-
-        def cnt():
-            n = 0
-
-            def innerfn(rs):
-                nonlocal n
-                n += 1
-                return rs.update(n=n)
-            return innerfn
-
-        conn['t1_1'] = conn['t1'].by('col1').map(cnt())
-        self.assertEqual(
-            conn['t1_1'].list(), [{'col1': 'a', 'col2': 4, 'n': 1},
-                                  {'col1': 'a', 'col2': 5, 'n': 1},
-                                  {'col1': 'b', 'col2': 1, 'n': 2},
-                                  {'col1': 'c', 'col2': 3, 'n': 3},
-                                  {'col1': 'c', 'col2': 4, 'n': 3},
-                                  {'col1': 'c', 'col2': 7, 'n': 3},
-                                  {'col1': 'd', 'col2': 2, 'n': 4}])
-
-    def test_fold1(self):
-        conn = Conn(self.dbfile)
-
-        def minmax(col):
-            def fn(rs):
-                xs = [r[col] for r in rs]
-                return [min(xs), max(xs)]
-            return fn
-
-        conn['t1'] = self.t1
-        conn['t1_1'] = conn['t1'].by('col1').fold(
-            sum=lambda rs: sum(rs['col2']),
-            mm0=lambda rs: min(rs['col2']),
-            mm1=lambda rs: max(rs['col2'])
-        )
-
-        self.assertEqual(conn['t1_1'].list(),
-                         [{'col1': 'a', 'sum': 9, 'mm0': 4, 'mm1': 5},
-                          {'col1': 'b', 'sum': 1, 'mm0': 1, 'mm1': 1},
-                          {'col1': 'c', 'sum': 14, 'mm0': 3, 'mm1': 7},
-                          {'col1': 'd', 'sum': 2, 'mm0': 2, 'mm1': 2}])
-
-        conn['t1_1'] = conn['t1'].windowed(4, 3).fold(
-            sum=lambda rs: sum(rs['col2']),
-            mm0=lambda rs: min(rs['col2']),
-            mm1=lambda rs: max(rs['col2'])
-        )
-        self.assertEqual(conn['t1_1'].list(),
-                         [{'sum': 13, 'mm0': 1, 'mm1': 5},
-                          {'sum': 16, 'mm0': 2, 'mm1': 7}
-                          ])
-
-        conn['t1_1'] = conn['t1'].windowed(4, 5).fold(
-            sum=lambda rs: sum(rs['col2']),
-            mm0=lambda rs: min(rs['col2']),
-            mm1=lambda rs: max(rs['col2'])
-        ).rename(
-            mm1='mm0',
-            mm0='mm1'
-        )
-        self.assertEqual(conn['t1_1'].list(),
-                         [{'sum': 13, 'mm1': 1, 'mm0': 5},
-                          {'sum': 9, 'mm1': 2, 'mm0': 7}
-                          ])
-
-    def test_by(self):
-        def sum_by_col1(rs):
-            tot = sum(rs['col2'])
-            return rs.update(col2=tot)[:1]
-
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-        conn['t1_sum'] = conn['t1'].by('col1')\
-            .map(sum_by_col1)
-
-        self.assertEqual(list(conn['t1_sum']._iter()),
-                         [{'col1': 'a', 'col2': 9},
-                          {'col1': 'b', 'col2': 1},
-                          {'col1': 'c', 'col2': 14},
-                          {'col1': 'd', 'col2': 2}]
-                         )
-        conn['t1_sum2'] = conn['t1']\
-            .by('col1').map(sum_by_col1)
-
-        self.assertEqual(conn['t1_sum'].list(), conn['t1_sum2'].list())
-
-    def test_chain(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-        conn['t1_double'] = conn['t1'].chain(conn['t1'])
-        self.assertEqual(conn['t1'].list() + conn['t1'].list(),
-                         conn['t1_double'].list())
-
-        conn['t1_double'] = conn['t1'].chain(self.t1)
-        self.assertEqual(conn['t1'].list() + conn['t1'].list(),
-                         conn['t1_double'].list())
-
-    def test_df(self):
-        import pandas as pd
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-        df = pd.DataFrame(conn['t1']._iter())
-        conn['t1_copy'] = df.to_dict('records')
-        self.assertEqual(conn['t1'].list(), conn['t1_copy'].list())
-
-    def test_by_after_map(self):
-        def sumit(rs):
-            tot = sum(rs['col2'])
-            return rs.update(tot=tot)
-
-        def count(rs):
-            n = len(rs.list())
-            return rs.update(cnt=n)
-
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-        conn['t1_sum'] = conn['t1'].by('col1')\
-            .map(sumit).by('tot').map(count)
-
-        # on another db
-        conn1 = Conn(self.dbfile1)
-        conn1['t1_sum'] = conn['t1'].by('col1').map(sumit).by('tot').map(count)
-        conn1['t1_sum2'] = conn['t1'].by('col1').map(sumit)\
-            .by('tot').map(count)._iter()
-
-        self.assertEqual(conn['t1_sum'].list(), conn1['t1_sum'].list())
-        self.assertEqual(conn['t1_sum'].list(), conn1['t1_sum2'].list())
-
-    def test_multiple_by(self):
-
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-        conn['t1_1'] = conn['t1'].update(col3=1).by('col1, col3')\
-            .map(lambda rs: rs)
-
-        conn['t1_2'] = conn['t1'].update(col3=1).by('col1').map(lambda rs: rs)
-        self.assertEqual(conn['t1_1'].list(), conn['t1_2'].list())
-
-        conn['t1_1_double'] = conn['t1_1']\
-            .chain(conn['t1'].update(col3=1).by('col1, col3')
-                   .map(lambda rs: rs))
-        conn['t1_1_double2'] = conn['t1_1'].chain(conn['t1_1'])
-
-        self.assertEqual(conn['t1_1_double'].list(),
-                         conn['t1_1_double2'].list())
-
-    def test_islice_group(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-
-        self.assertEqual(conn['t1'].by('col1')[1:3].list(),
-                         [{'col1': 'b', 'col2': 1},
-                          {'col1': 'c', 'col2': 3},
-                          {'col1': 'c', 'col2': 4},
-                          {'col1': 'c', 'col2': 7}])
-
-        self.assertEqual(conn['t1'].windowed(4, 2)[1:3].list(),
-                         [{'col1': 'b', 'col2': 1},
-                          {'col1': 'c', 'col2': 3},
-                          {'col1': 'c', 'col2': 4},
-                          {'col1': 'c', 'col2': 7},
-                          {'col1': 'c', 'col2': 4},
-                          {'col1': 'c', 'col2': 7},
-                          {'col1': 'd', 'col2': 2}
-                          ])
-
-    def test_islice(self):
-
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-        conn['t2'] = self.t2
-
-        self.assertEqual(len(conn['t1']._islice(3).list()), 3)
-        self.assertEqual(len(conn['t1']._islice(3, None).list()), 4)
-        self.assertEqual(len(conn['t1']._islice(0, None, 3).list()), 3)
-
-        self.assertEqual(len(conn['t1'][:3].list()), 3)
-        self.assertEqual(len(conn['t1'][3:].list()), 4)
-        self.assertEqual(len(conn['t1'][0::3].list()), 3)
-
-        xs = conn['t1']._iter()
-        ys = conn['t2']._iter()
-
-        conn['t1_2'] = ({**x, **y} for x, y in product(xs, ys))
-
-        n1 = len(conn['t1'].list())
-        n2 = len(conn['t2'].list())
-        n3 = len(conn['t1_2'].list())
-
-        self.assertEqual(n3, n1 * n2)
-
-        xs = conn['t1'][0:5].filter(lambda r: r['col2'] > 3)
-        ys = conn['t1'][0:8].filter(lambda r: r['col2'] > 3)
-
-        self.assertEqual(len(xs.list()), 3)
-        self.assertEqual(len(ys.list()), 4)
-
-    def test_takewhile(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-
-        self.assertEqual(len(conn['t1']
-                             .takewhile(lambda r: r['col2'] > 1).list()), 2)
-
-        self.assertEqual(len(conn['t1']
-                             .order('col2 desc')
-                             .takewhile(lambda r: r['col2'] > 1).list()), 6)
-
-    def test_dropwhile(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-
-        self.assertEqual(len(conn['t1']
-                             .dropwhile(lambda r: r['col2'] > 1).list()), 5)
-
-        self.assertEqual(len(conn['t1']
-                             .order('col2')
-                             .dropwhile(lambda r: r['col2'] < 4).list()), 4)
-
-    def test_windowed_group(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-
-        self.assertEqual(conn['t1'].by('col1').windowed(2, 1)
-                         .index('cnt').list(),
-                         [{'col1': 'a', 'col2': 4, 'cnt': 0},
-                          {'col1': 'a', 'col2': 5, 'cnt': 0},
-                          {'col1': 'b', 'col2': 1, 'cnt': 0},
-                          {'col1': 'b', 'col2': 1, 'cnt': 1},
-                          {'col1': 'c', 'col2': 3, 'cnt': 1},
-                          {'col1': 'c', 'col2': 4, 'cnt': 1},
-                          {'col1': 'c', 'col2': 7, 'cnt': 1},
-                          {'col1': 'c', 'col2': 3, 'cnt': 2},
-                          {'col1': 'c', 'col2': 4, 'cnt': 2},
-                          {'col1': 'c', 'col2': 7, 'cnt': 2},
-                          {'col1': 'd', 'col2': 2, 'cnt': 2}])
-
-        self.assertEqual(conn['t1'].windowed(3, 1).windowed(2, 1)
-                         .index('cnt').list(),
-
-                         [{'col1': 'a', 'col2': 4, 'cnt': 0},
-                          {'col1': 'a', 'col2': 5, 'cnt': 0},
-                          {'col1': 'b', 'col2': 1, 'cnt': 0},
-                          {'col1': 'a', 'col2': 5, 'cnt': 0},
-                          {'col1': 'b', 'col2': 1, 'cnt': 0},
-                          {'col1': 'c', 'col2': 3, 'cnt': 0},
-                          {'col1': 'a', 'col2': 5, 'cnt': 1},
-                          {'col1': 'b', 'col2': 1, 'cnt': 1},
-                          {'col1': 'c', 'col2': 3, 'cnt': 1},
-                          {'col1': 'b', 'col2': 1, 'cnt': 1},
-                          {'col1': 'c', 'col2': 3, 'cnt': 1},
-                          {'col1': 'c', 'col2': 4, 'cnt': 1},
-                          {'col1': 'b', 'col2': 1, 'cnt': 2},
-                          {'col1': 'c', 'col2': 3, 'cnt': 2},
-                          {'col1': 'c', 'col2': 4, 'cnt': 2},
-                          {'col1': 'c', 'col2': 3, 'cnt': 2},
-                          {'col1': 'c', 'col2': 4, 'cnt': 2},
-                          {'col1': 'c', 'col2': 7, 'cnt': 2},
-                          {'col1': 'c', 'col2': 3, 'cnt': 3},
-                          {'col1': 'c', 'col2': 4, 'cnt': 3},
-                          {'col1': 'c', 'col2': 7, 'cnt': 3},
-                          {'col1': 'c', 'col2': 4, 'cnt': 3},
-                          {'col1': 'c', 'col2': 7, 'cnt': 3},
-                          {'col1': 'd', 'col2': 2, 'cnt': 3}])
-
-    def test_windowed(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-
-        def add1(rs):
-            return rs.update(col2=lambda r: r['col2'] + 1)
-
-        self.assertEqual(conn['t1'].windowed(4, 2).map(add1).list(),
-                         [{'col1': 'a', 'col2': 5},
-                          {'col1': 'a', 'col2': 6},
-                          {'col1': 'b', 'col2': 2},
-                          {'col1': 'c', 'col2': 4},
-                          {'col1': 'b', 'col2': 2},
-                          {'col1': 'c', 'col2': 4},
-                          {'col1': 'c', 'col2': 5},
-                          {'col1': 'c', 'col2': 8},
-                          {'col1': 'c', 'col2': 5},
-                          {'col1': 'c', 'col2': 8},
-                          {'col1': 'd', 'col2': 3}])
-
-    def test_filter(self):
-        conn = Conn(self.dbfile)
-
-        conn['t1'] = self.t1
-        conn['t1_1'] = conn['t1'].filter(lambda r: r['col2'] > 2)
-
-        self.assertEqual(len(conn['t1_1'].list()), 5)
-
-    def test_filter_group(self):
-        conn = Conn(self.dbfile)
-
-        conn['t1'] = self.t1
-        conn['t1_1'] = conn['t1'].group('col1')\
-            .filter(lambda rs: rs.size() >= 2)
-
-        self.assertEqual(len(conn['t1_1'].list()), 5)
-
-    def test_filter_windowed(self):
-        conn = Conn(self.dbfile)
-
-        conn['t1'] = self.t1
-        conn['t1_1'] = conn['t1'].windowed(5, 1)\
-            .filter(lambda rs: rs.filter(lambda r: r['col2'] > 3).size() >= 3)
-        self.assertEqual(conn['t1_1'].list(),
-                         [{'col1': 'a', 'col2': 4},
-                          {'col1': 'a', 'col2': 5},
-                          {'col1': 'b', 'col2': 1},
-                          {'col1': 'c', 'col2': 3},
-                          {'col1': 'c', 'col2': 4},
-                          {'col1': 'a', 'col2': 5},
-                          {'col1': 'b', 'col2': 1},
-                          {'col1': 'c', 'col2': 3},
-                          {'col1': 'c', 'col2': 4},
-                          {'col1': 'c', 'col2': 7}])
-
-    def test_update(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-        conn['t1_1'] = conn['t1'].update(
-            col2=lambda r: r['col2'] + 1,
-            col3=lambda r: r['col1'] + str(r['col2'])
-        )
-        # table is fetched as it's inserted. not sure if it's a feature.
-        self.assertEqual(conn['t1_1'].list()[0],
-                         {'col1': 'a', 'col2': 5, 'col3': 'a5'})
-
-    def test_select(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-
-        conn['t1_1'] = conn['t1'].update(
-            col2=lambda r: r['col2'] + 1,
-            col3=lambda r: r['col1'] + str(r['col2'])
-        )
-
-        r = next(conn['t1_1'].select('col1, col3')._iter())
-        self.assertEqual(len(r), 2)
-
-        # test deselect
-        r = next(conn['t1_1'].deselect('col1, col3')._iter())
-        self.assertEqual(len(r), 1)
-
-    def test_join(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-        conn['t2'] = self.t2
-
-        conn['t1_1'] = conn['t1'].by('col1')\
-            .join(conn['t2'].by('col1'), "inner")
-
-        self.assertEqual(len(conn['t1_1'].list()), 3)
-
-        conn['t1_2'] = conn['t1'].by('col1')\
-            .join(conn['t2'].by('col1'), "left")
-
-        self.assertEqual(conn['t1_2'].list(),
-                         [{'col1': 'a', 'col2': 4, 'col3': ''},
-                          {'col1': 'a', 'col2': 5, 'col3': ''},
-                          {'col1': 'b', 'col2': 1, 'col3': 1},
-                          {'col1': 'c', 'col2': 3, 'col3': ''},
-                          {'col1': 'c', 'col2': 4, 'col3': ''},
-                          {'col1': 'c', 'col2': 7, 'col3': ''},
-                          {'col1': 'd', 'col2': 2, 'col3': 3},
-                          {'col1': 'd', 'col2': 2, 'col3': 2}])
-
-        conn['t1_3'] = conn['t1'].by('col1')\
-            .join(conn['t2'].by('col1'), "right")
-
-        self.assertEqual(conn['t1_3'].list(),
-                         [{'col1': 'b', 'col2': 1, 'col3': 1},
-                          {'col1': 'd', 'col2': 2, 'col3': 3},
-                          {'col1': 'd', 'col2': 2, 'col3': 2},
-                          {'col1': 'e', 'col2': '', 'col3': 3},
-                          {'col1': 'e', 'col2': '', 'col3': 4}])
-
-        conn['t1_4'] = conn['t1'].by('col1')\
-            .join(conn['t2'].by('col1'), "full")
-
-        self.assertEqual(conn['t1_4'].list(), [
-            {'col1': 'a', 'col2': 4, 'col3': ''},
-            {'col1': 'a', 'col2': 5, 'col3': ''},
-            {'col1': 'b', 'col2': 1, 'col3': 1},
-            {'col1': 'c', 'col2': 3, 'col3': ''},
-            {'col1': 'c', 'col2': 4, 'col3': ''},
-            {'col1': 'c', 'col2': 7, 'col3': ''},
-            {'col1': 'd', 'col2': 2, 'col3': 3},
-            {'col1': 'd', 'col2': 2, 'col3': 2},
-            {'col1': 'e', 'col2': '', 'col3': 3},
-            {'col1': 'e', 'col2': '', 'col3': 4}]
-        )
-
-    def test_join2(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-        conn['t2'] = self.t2
-
-        conn['t1_1'] = conn['t1'].chain([{'col1': 'd', 'col2': 9}, {
-            'col1': 'd', 'col2': 19}]).by('col1')\
-            .join(conn['t2'].by('col1'), 'full')
-
-        conn['t1_1'] = conn['t1'].chain([{'col1': 'd', 'col2': 9}, {
-            'col1': 'd', 'col2': 19}]).by('col1')\
-            .join(conn['t2'].by('col1'), 'full')
-
-        conn['t1_2'] = conn['t1'].chain([{'col1': 'd', 'col2': 9}, {
-            'col1': 'd', 'col2': 19}]).by('col1')\
-            .join(conn['t2'].by('col1'), 'full')\
-            .update(col4=lambda r: r['col3'] + 1 if r['col3'] else '')
-
-        self.assertEqual(conn['t1_1'].list(),
-                         [{'col1': 'a', 'col2': 4, 'col3': ''},
-                          {'col1': 'a', 'col2': 5, 'col3': ''},
-                          {'col1': 'b', 'col2': 1, 'col3': 1},
-                          {'col1': 'c', 'col2': 3, 'col3': ''},
-                          {'col1': 'c', 'col2': 4, 'col3': ''},
-                          {'col1': 'c', 'col2': 7, 'col3': ''},
-                          {'col1': 'd', 'col2': 2, 'col3': 3},
-                          {'col1': 'd', 'col2': 2, 'col3': 2},
-                          {'col1': 'd', 'col2': 9, 'col3': 3},
-                          {'col1': 'd', 'col2': 9, 'col3': 2},
-                          {'col1': 'd', 'col2': 19, 'col3': 3},
-                          {'col1': 'd', 'col2': 19, 'col3': 2},
-                          {'col1': 'e', 'col2': '', 'col3': 3},
-                          {'col1': 'e', 'col2': '', 'col3': 4}])
-
-    def test_join3(self):
-        rs1 = Rows(self.t1)
-        rs2 = Rows(self.t2)
-        rs = rs1.by('col1').join(rs2.by('col1'), 'left')
-        self.assertEqual(rs.list(),
-                         [{'col1': 'a', 'col2': 4, 'col3': ''},
-                          {'col1': 'a', 'col2': 5, 'col3': ''},
-                          {'col1': 'b', 'col2': 1, 'col3': 1},
-                          {'col1': 'c', 'col2': 3, 'col3': ''},
-                          {'col1': 'c', 'col2': 4, 'col3': ''},
-                          {'col1': 'c', 'col2': 7, 'col3': ''},
-                          {'col1': 'd', 'col2': 2, 'col3': 3},
-                          {'col1': 'd', 'col2': 2, 'col3': 2}])
-
-        self.assertEqual(rs1.list(), self.t1)
-
-    def test_join4(self):
-        rs1 = Rows(self.t1)
-        rs2 = Rows(self.t2)
-        rs1 = rs1.chain([{'col1': 'f', 'col2': 9},
-                        {'col1': 'f', 'col2': 8},
-                        {'col1': 'd', 'col2': 11},
-
-                         ])
-        rs1 = rs1.update(col4=lambda r: r['col2'] * 20)
-
-        rs2 = rs2.update(col2=lambda r: r['col3'] * 10)
-        rs3 = rs1.by('col1').join(rs2.by('col1'), 'full')
-        self.assertEqual(rs3.list(),
-                         [{'col1': 'a', 'col2': 4, 'col4': 80, 'col3': ''},
-                          {'col1': 'a', 'col2': 5, 'col4': 100, 'col3': ''},
-                          {'col1': 'b', 'col2': 10, 'col4': 20, 'col3': 1},
-                          {'col1': 'c', 'col2': 3, 'col4': 60, 'col3': ''},
-                          {'col1': 'c', 'col2': 4, 'col4': 80, 'col3': ''},
-                          {'col1': 'c', 'col2': 7, 'col4': 140, 'col3': ''},
-                          {'col1': 'd', 'col2': 30, 'col4': 40, 'col3': 3},
-                          {'col1': 'd', 'col2': 20, 'col4': 40, 'col3': 2},
-                          {'col1': 'd', 'col2': 30, 'col4': 220, 'col3': 3},
-                          {'col1': 'd', 'col2': 20, 'col4': 220, 'col3': 2},
-                          {'col1': 'e', 'col2': 30, 'col4': '', 'col3': 3},
-                          {'col1': 'e', 'col2': 40, 'col4': '', 'col3': 4},
-                          {'col1': 'f', 'col2': 9, 'col4': 180, 'col3': ''},
-                          {'col1': 'f', 'col2': 8, 'col4': 160, 'col3': ''},
-                          ])
-        conn = Conn(self.dbfile)
-        conn['t1'] = rs1
-        conn['t2'] = rs2
-        conn['t3'] = conn['t1'].by('col1').join(conn['t2'].by('col1'), 'full')
-        self.assertEqual(rs3.list(), conn['t3'].list())
-
-        rs3 = rs1.by('col1').join(rs2.by('col1'), 'left')
-        conn['t3'] = conn['t1'].by('col1').join(conn['t2'].by('col1'), 'left')
-        self.assertEqual(rs3.list(), conn['t3'].list())
-
-        rs3 = rs1.by('col1').join(rs2.by('col1'), 'right')
-        conn['t3'] = conn['t1'].by('col1').join(conn['t2'].by('col1'), 'right')
-        self.assertEqual(rs3.list(), conn['t3'].list())
-
-        rs3 = rs1.by('col1').join(rs2.by('col1'), 'inner')
-        conn['t3'] = conn['t1'].by('col1').join(conn['t2'].by('col1'), 'inner')
-        self.assertEqual(rs3.list(), conn['t3'].list())
-
-    def test_merge(self):
-        rs1 = Rows(self.t1)
-        rs2 = Rows(self.t2)
-        rs1 = rs1.chain([{'col1': 'f', 'col2': 9},
-                         {'col1': 'f', 'col2': 8}])
-        rs2 = rs2.chain([{'col1': 'a', 'col3': 91}])
-
-        rs1 = rs1.update(col4=lambda r: r['col2'] * 20)
-        rs2 = rs2.update(col2=lambda r: r['col3'] * 10)
-
-        rs3 = rs1.by('col1').merge(rs2.by('col1'), 'full')
-        self.assertEqual(rs3.list(),
-                         [{'col1': 'a', 'col2': 910, 'col4': 80, 'col3': 91},
-                          {'col1': 'a', 'col2': 5, 'col4': 100, 'col3': ''},
-                          {'col1': 'b', 'col2': 10, 'col4': 20, 'col3': 1},
-                          {'col1': 'c', 'col2': 3, 'col4': 60, 'col3': ''},
-                          {'col1': 'c', 'col2': 4, 'col4': 80, 'col3': ''},
-                          {'col1': 'c', 'col2': 7, 'col4': 140, 'col3': ''},
-                          {'col1': 'd', 'col2': 30, 'col4': 40, 'col3': 3},
-                          {'col1': 'd', 'col2': 20, 'col4': '', 'col3': 2},
-                          {'col1': 'e', 'col2': 30, 'col4': '', 'col3': 3},
-                          {'col1': 'e', 'col2': 40, 'col4': '', 'col3': 4},
-                          {'col1': 'f', 'col2': 9, 'col4': 180, 'col3': ''},
-                          {'col1': 'f', 'col2': 8, 'col4': 160, 'col3': ''}])
-
-        conn = Conn(self.dbfile)
-        conn['t1'] = rs1
-        conn['t2'] = rs2
-        conn['t3'] = conn['t1'].by('col1').merge(conn['t2'].by('col1'), 'full')
-        self.assertEqual(rs3.list(), conn['t3'].list())
-
-        rs3 = rs1.by('col1').merge(rs2.by('col1'), 'left')
-        conn['t3'] = conn['t1'].by('col1').merge(conn['t2'].by('col1'), 'left')
-        self.assertEqual(rs3.list(), conn['t3'].list())
-
-        rs3 = rs1.by('col1').merge(rs2.by('col1'), 'right')
-        conn['t3'] = conn['t1'].by('col1').merge(
-            conn['t2'].by('col1'), 'right')
-        self.assertEqual(rs3.list(), conn['t3'].list())
-
-        rs3 = rs1.by('col1').merge(rs2.by('col1'), 'inner')
-        conn['t3'] = conn['t1'].by('col1').merge(
-            conn['t2'].by('col1'), 'inner')
-        self.assertEqual(rs3.list(), conn['t3'].list())
-
-    def test_distinct(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-        conn['t1_1'] = conn['t1'].distinct('col1')
-        self.assertEqual(len(conn['t1_1'].list()), 4)
-        conn['t1_2'] = conn['t1'].distinct('col1, col2')
-        self.assertEqual(len(conn['t1_2'].list()), 7)
-
-    def test_order(self):
-        conn = Conn(self.dbfile)
-        conn['t1'] = self.t1
-
-        [g1, g2, g3, g4] = [list(xs) for _, xs in conn['t1']
-                            .order('col1, col2 desc').group('col1')._iter()]
-        self.assertEqual(
-            g1, [{'col1': 'a', 'col2': 5}, {'col1': 'a', 'col2': 4}]
-        )
-        self.assertEqual(g2, [{'col1': 'b', 'col2': 1}])
-        self.assertEqual(g3, [{'col1': 'c', 'col2': 7}, {
-                         'col1': 'c', 'col2': 4}, {'col1': 'c', 'col2': 3}])
-        self.assertEqual(g4, [{'col1': 'd', 'col2': 2}])
-
-    def test_readme(self):
-        t1 = [
-            {'col1': 'a', 'col2': 4},
-            {'col1': 'a', 'col2': 5},
-            {'col1': 'b', 'col2': 1},
-        ]
-
-        conn = Conn(self.dbfile)
-        conn['t1'] = t1
-
-        for r1, r2 in zip(conn['t1'].list(), conn['t1']._iter()):
-            self.assertEqual(r1, r2)
-
-        import pandas as pd
-
-        df = pd.DataFrame(conn['t1']._iter())
-        conn['t1_copy'] = df.to_dict('records')
-
-        self.assertEqual(conn['t1'].list(), conn['t1_copy'].list())
-
-        conn['t1_1'] = conn['t1']\
-            .filter(lambda r: r['col2'] > 2)\
-            .update(col2=lambda r: r['col2'] + 1)
-
-        self.assertEqual(conn['t1_1'].list()[0]['col2'], 5)
-
-        conn['t1_col2sum_groupby_col1'] = conn['t1'].by('col1')\
-            .fold(col2_sum=lambda rs: sum(rs['col2']))\
-            .deselect('col2')
-
-        conn['t1_col2sum_groupby_col1_1'] = conn['t1']\
-            .order('col1, col2 desc').group('col1')\
-            .fold(col2_sum=lambda rs: sum(rs['col2']))\
-            .deselect('col2')
-
-        self.assertEqual(conn['t1_col2sum_groupby_col1'].list(),
-                         conn['t1_col2sum_groupby_col1_1'].list())
-
-        conn['t1_double'] = conn['t1'].chain(conn['t1'])
-        self.assertEqual(len(conn['t1_double'].list()),
-                         2 * len(conn['t1'].list()))
-
-        conn['t1_double'] = conn['t1'].chain(t1)
-
-        self.assertEqual(len(conn['t1_double'].list()),
-                         2 * len(conn['t1'].list()))
-
-        conn['t1_1'] = conn['t1']\
-            .filter(lambda r: r['col2'] > 2)\
-            .update(
-            col2=lambda r: r['col2'] + 1,
-            col3=lambda r: r['col1'] + str(r['col2'])
-        )
-        self.assertEqual(conn['t1_1'].list(),
-                         [{'col1': 'a', 'col2': 5, 'col3': 'a5'},
-                          {'col1': 'a', 'col2': 6, 'col3': 'a6'}])
-
-        conn['t1_1'] = conn['t1'].update(col3=lambda r: r['col2'] + 1)\
-            .deselect('col1, col2')
-
-        self.assertEqual(conn['t1_1'].list(),
-                         [{'col3': 5}, {'col3': 6}, {'col3': 2}])
-
-        conn['t1_1'] = conn['t1'].distinct('col1')
-        self.assertEqual(conn['t1_1'].list(), [
-                         {'col1': 'a', 'col2': 4}, {'col1': 'b', 'col2': 1}])
-
-        conn['t2'] = [
-            {'col1': 'b', 'col3': -1},
-            {'col1': 'c', 'col3': 3},
-            {'col1': 'b', 'col3': ''},
-        ]
-
-        conn['t1_col3'] = conn['t1'].by('col1')\
-            .join(conn['t2'].by('col1'), 'full')
-
-        self.assertEqual(conn['t1_col3'].list(),
-                         [{'col1': 'a', 'col2': 4, 'col3': ''},
-                         {'col1': 'a', 'col2': 5, 'col3': ''},
-                         {'col1': 'b', 'col2': 1, 'col3': -1},
-                         {'col1': 'b', 'col2': 1, 'col3': ''},
-                          {'col1': 'c', 'col2': '', 'col3': 3}]
-                         )
+import os
+import unittest
+from itertools import product
+from pathlib import Path
+
+from tablemap import Conn, Rows
+
+
+class TestCore(unittest.TestCase):
+    def setUp(self):
+        self.dbfile = 'test/sample.db'
+        self.dbfile1 = 'test/sample1.db'
+
+        self.t1 = [
+            {'col1': 'a', 'col2': 4},
+            {'col1': 'a', 'col2': 5},
+            {'col1': 'b', 'col2': 1},
+            {'col1': 'c', 'col2': 3},
+            {'col1': 'c', 'col2': 4},
+            {'col1': 'c', 'col2': 7},
+            {'col1': 'd', 'col2': 2},
+
+        ]
+
+        self.t2 = [
+            {'col1': 'd', 'col3': 3},
+            {'col1': 'b', 'col3': 1},
+            {'col1': 'e', 'col3': 3},
+            {'col1': 'e', 'col3': 4},
+            {'col1': 'd', 'col3': 2},
+        ]
+
+    def tearDown(self):
+        if Path(self.dbfile).is_file():
+            os.remove(self.dbfile)
+        if Path(self.dbfile1).is_file():
+            os.remove(self.dbfile1)
+
+    def test_takewhile_group(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+
+        self.assertEqual(conn['t1'].by('col1')
+                         .takewhile(lambda rs: rs['col1'][0] < 'c').list(),
+                         [{'col1': 'a', 'col2': 4},
+                          {'col1': 'a', 'col2': 5},
+                          {'col1': 'b', 'col2': 1}]
+                         )
+
+        self.assertEqual(conn['t1'].windowed(4, 2)
+                         .takewhile(lambda rs: rs.size() == 4).list(),
+                         [{'col1': 'a', 'col2': 4},
+                          {'col1': 'a', 'col2': 5},
+                          {'col1': 'b', 'col2': 1},
+                          {'col1': 'c', 'col2': 3},
+                          {'col1': 'b', 'col2': 1},
+                          {'col1': 'c', 'col2': 3},
+                          {'col1': 'c', 'col2': 4},
+                          {'col1': 'c', 'col2': 7}])
+
+    def test_dropwhile_group(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+
+        self.assertEqual(conn['t1'].by('col1')
+                         .dropwhile(lambda rs: rs['col1'][0] < 'c').list(),
+                         [{'col1': 'c', 'col2': 3},
+                          {'col1': 'c', 'col2': 4},
+                          {'col1': 'c', 'col2': 7},
+                          {'col1': 'd', 'col2': 2}])
+
+        self.assertEqual(conn['t1'].windowed(4, 2)
+                         .dropwhile(lambda rs: rs.size() == 4).list(),
+                         [{'col1': 'c', 'col2': 4},
+                          {'col1': 'c', 'col2': 7},
+                          {'col1': 'd', 'col2': 2}])
+
+    def test_split(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+
+        xs = conn['t1'].group('col1').split()
+        self.assertEqual(len(xs[0].list()), 2)
+        self.assertEqual(len(xs[1].list()), 1)
+        self.assertEqual(len(xs[2].list()), 3)
+        self.assertEqual(len(xs[3].list()), 1)
+
+        xs = conn['t1'].windowed(4, 2).split()
+        self.assertEqual(len(xs[0].list()), 4)
+        self.assertEqual(len(xs[1].list()), 4)
+        self.assertEqual(len(xs[2].list()), 3)
+
+        xs1 = xs[2].update(foo=4)
+        # test xs[1] is unaffected
+        self.assertEqual(xs[1].list(),
+                         [{'col1': 'b', 'col2': 1},
+                          {'col1': 'c', 'col2': 3},
+                          {'col1': 'c', 'col2': 4},
+                          {'col1': 'c', 'col2': 7}])
+
+    def test_size_group(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+        self.assertEqual(conn['t1'].group('col1').size(), 4)
+        self.assertEqual(conn['t1'].windowed(4, 2).size(), 3)
+
+    def test_index1(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+        conn['t1_1'] = conn['t1'].index('foo')
+        self.assertEqual(conn['t1_1']['foo'], [0, 1, 2, 3, 4, 5, 6])
+
+        conn['t1_1'] = conn['t1'].group('col1').index('foo', 1, 2)
+        self.assertEqual(conn['t1_1']['foo'], [1, 1, 3, 5, 5, 5, 7])
+        conn['t1_1'] = conn['t1'].windowed(4, 2).index('foo', 1, 2)
+        self.assertEqual(conn['t1_1']['foo'], [
+                         1, 1, 1, 1, 3, 3, 3, 3, 5, 5, 5])
+
+    def test_order_when_no_row(self):
+        rs1 = Rows([])
+        self.assertEqual(rs1.order('col1').list(), [])
+
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+        self.assertEqual(
+            conn['t1'].filter(lambda r: r['col2'] > 100).order('col1').list(),
+            [])
+
+    def test_size(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+
+        self.assertEqual(conn['t1'].size(), len(self.t1))
+        # size is executed while the connection is open
+        self.assertEqual(conn['t1'].update(n=lambda r: conn['t1'].size())["n"],
+                         [7] * 7)
+        # size is executed when the connection is closed
+        self.assertEqual(conn['t1'].update(n=conn['t1'].size())["n"],
+                         [7] * 7)
+
+        rs = Rows(self.t1)
+        self.assertEqual(rs.size(), len(self.t1))
+
+        rs1 = rs[3:6]
+        self.assertEqual(rs1.size(), 3)
+
+    def test_wierd(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+
+        xs = conn['t1']
+        self.assertEqual(xs.by('col1').fold(col2_tot=sum(xs['col2'])).list(),
+                         [{'col1': 'a', 'col2_tot': 26},
+                         {'col1': 'b', 'col2_tot': 26},
+                         {'col1': 'c', 'col2_tot': 26},
+                         {'col1': 'd', 'col2_tot': 26}])
+
+    def test_modification(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+
+        rs1 = conn['t1']
+        rs2 = rs1.update(col2=lambda r: r['col2'] + 1)
+
+        # the following code does not work, you cannot execute a fetch
+        # while another fetch is being done.
+        # So iter should not be exposed.
+        # for r1, r2 in zip(rs1._iter(), rs2._iter()):
+        #     print(r1, r2)
+
+        rs1 = rs1.list()
+        rs2 = rs2.list()
+
+        for r1, r2 in zip(rs1, rs2):
+            self.assertEqual(r1['col2'] + 1, r2['col2'])
+
+    def test_list_mod(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+        t1 = conn['t1']
+        t1_listed = t1.list()
+        t1_listed[0]['col1'] = 'x'
+        self.assertNotEqual(
+            t1.list()[0]['col1'], 'x'
+        )
+        self.assertEqual(
+            t1_listed[0]['col1'], 'x'
+        )
+
+    def test_list_mod1(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+
+        def tempfn(rs):
+            rslist = rs.list()
+            for r in rslist:
+                r['col2'] += 1
+            # this should not do anything
+            return rs
+
+        conn['t1_1'] = conn['t1'].by('col1').map(tempfn)
+        self.assertEqual(conn['t1_1'].list(), conn['t1'].list())
+
+    def test_do_later(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+
+        xs = conn['t1']
+        xs1 = xs.by('col1')
+        tot = sum(xs['col2'])
+        xs1 = xs1.fold(
+            col3=lambda rs: sum(rs['col2']),
+            col4=tot
+        )
+        self.assertEqual(xs1.list(),
+                         [{'col1': 'a', 'col3': 9, 'col4': 26},
+                          {'col1': 'b', 'col3': 1, 'col4': 26},
+                          {'col1': 'c', 'col3': 14, 'col4': 26},
+                          {'col1': 'd', 'col3': 2, 'col4': 26}])
+
+    def test_zip(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+
+        def tempfn(rs):
+            return rs.zip([
+                {'n': 1},
+                {'n': 2}
+            ])
+
+        conn['t1_1'] = conn['t1'].by('col1').map(tempfn)
+        self.assertEqual(conn['t1_1'].list(),
+                         [{'col1': 'a', 'col2': 4, 'n': 1},
+                          {'col1': 'a', 'col2': 5, 'n': 2},
+                          {'col1': 'b', 'col2': 1, 'n': 1},
+                          {'col1': 'c', 'col2': 3, 'n': 1},
+                          {'col1': 'c', 'col2': 4, 'n': 2},
+                          {'col1': 'd', 'col2': 2, 'n': 1}]
+                         )
+
+    def test_zip2(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+
+        conn['t1_1'] = conn['t1'].zip({'idx': i} for i in range(100))
+        self.assertEqual(conn['t1_1']['idx'], list(range(len(self.t1))))
+
+    def test_zip_longest(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+
+        def tempfn(rs):
+            return rs.zip_longest([
+                {'n': 1},
+                {'n': 2}
+            ])
+
+        conn['t1_1'] = conn['t1'].by('col1').map(tempfn)
+        self.assertEqual(conn['t1_1'].list(),
+                         [{'col1': 'a', 'col2': 4, 'n': 1},
+                          {'col1': 'a', 'col2': 5, 'n': 2},
+                          {'col1': 'b', 'col2': 1, 'n': 1},
+                          {'col1': '', 'col2': '', 'n': 2},
+                          {'col1': 'c', 'col2': 3, 'n': 1},
+                          {'col1': 'c', 'col2': 4, 'n': 2},
+                          {'col1': 'c', 'col2': 7, 'n': ''},
+                          {'col1': 'd', 'col2': 2, 'n': 1},
+                          {'col1': '', 'col2': '', 'n': 2}]
+                         )
+
+    def test_zip_longest2(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+
+        conn['t1_1'] = conn['t1'].zip_longest(({'n': i} for i in range(10)))
+        self.assertEqual(conn['t1_1'].list(),
+                         [{'col1': 'a', 'col2': 4, 'n': 0},
+                          {'col1': 'a', 'col2': 5, 'n': 1},
+                          {'col1': 'b', 'col2': 1, 'n': 2},
+                          {'col1': 'c', 'col2': 3, 'n': 3},
+                          {'col1': 'c', 'col2': 4, 'n': 4},
+                          {'col1': 'c', 'col2': 7, 'n': 5},
+                          {'col1': 'd', 'col2': 2, 'n': 6},
+                          {'col1': '', 'col2': '', 'n': 7},
+                          {'col1': '', 'col2': '', 'n': 8},
+                          {'col1': '', 'col2': '', 'n': 9}])
+
+        conn['t1_2'] = conn['t1'].zip_longest(({'n': i} for i in range(5)))
+        self.assertEqual(conn['t1_2'].list(),
+                         [{'col1': 'a', 'col2': 4, 'n': 0},
+                          {'col1': 'a', 'col2': 5, 'n': 1},
+                          {'col1': 'b', 'col2': 1, 'n': 2},
+                          {'col1': 'c', 'col2': 3, 'n': 3},
+                          {'col1': 'c', 'col2': 4, 'n': 4},
+                          {'col1': 'c', 'col2': 7, 'n': ''},
+                          {'col1': 'd', 'col2': 2, 'n': ''}])
+
+    def test_tee_n_new(self):
+        conn = Conn(self.dbfile)
+
+        def tempfn1(rs):
+            return rs.order('col2 desc').chain(rs.order('col2'))
+        conn['t10'] = self.t1
+
+        conn['t1_1'] = conn['t10'].by('col1').map(tempfn1)
+
+        self.assertEqual(conn['t1_1']['col2'],
+                         [5, 4, 4, 5, 1, 1, 7, 4, 3, 3, 4, 7, 2, 2])
+
+        def tempfn2(rs):
+            rs1 = rs.update(col2=lambda r: r['col2'] + 1)
+            return rs1.order('col2 desc').chain(rs.order('col2'))
+
+        conn['t1'] = self.t1
+        conn['t1_1'] = conn['t1'].by('col1').map(tempfn2)
+        self.assertEqual(conn['t1_1']['col2'],
+                         [6, 5, 4, 5, 2, 1, 8, 5, 4, 3, 4, 7, 3, 2])
+
+    def test_tee_n_new2(self):
+        conn = Conn(self.dbfile)
+
+        def tempfn(rs):
+            return rs.order('col2').zip(rs.order('col2 desc')
+                                        .rename(col2_1='col2'))
+
+        conn['t1'] = self.t1
+        conn['t1_1'] = conn['t1'].by('col1').map(tempfn)
+        xs = [{'col1': 'a', 'col2': 4, 'col2_1': 5},
+              {'col1': 'a', 'col2': 5, 'col2_1': 4},
+              {'col1': 'b', 'col2': 1, 'col2_1': 1},
+              {'col1': 'c', 'col2': 3, 'col2_1': 7},
+              {'col1': 'c', 'col2': 4, 'col2_1': 4},
+              {'col1': 'c', 'col2': 7, 'col2_1': 3},
+              {'col1': 'd', 'col2': 2, 'col2_1': 2}]
+        self.assertEqual(conn['t1_1'].list(), xs)
+
+        def tempfn1(rs):
+            rs1 = rs.update(col2=lambda r: r['col2'] + 1)
+            return rs1.order('col2').zip(rs.order('col2 desc')
+                                         .rename(col2_1='col2'))
+
+        conn['t1_1'] = conn['t1'].by('col1').map(tempfn1)
+
+        xs = [{'col1': 'a', 'col2': 5, 'col2_1': 5},
+              {'col1': 'a', 'col2': 6, 'col2_1': 4},
+              {'col1': 'b', 'col2': 2, 'col2_1': 1},
+              {'col1': 'c', 'col2': 4, 'col2_1': 7},
+              {'col1': 'c', 'col2': 5, 'col2_1': 4},
+              {'col1': 'c', 'col2': 8, 'col2_1': 3},
+              {'col1': 'd', 'col2': 3, 'col2_1': 2}]
+
+        self.assertEqual(conn['t1_1'].list(), xs)
+
+    def test_index(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+
+        def cnt():
+            n = 0
+
+            def innerfn(rs):
+                nonlocal n
+                n += 1
+                return rs.update(n=n)
+            return innerfn
+
+        conn['t1_1'] = conn['t1'].by('col1').map(cnt())
+        self.assertEqual(
+            conn['t1_1'].list(), [{'col1': 'a', 'col2': 4, 'n': 1},
+                                  {'col1': 'a', 'col2': 5, 'n': 1},
+                                  {'col1': 'b', 'col2': 1, 'n': 2},
+                                  {'col1': 'c', 'col2': 3, 'n': 3},
+                                  {'col1': 'c', 'col2': 4, 'n': 3},
+                                  {'col1': 'c', 'col2': 7, 'n': 3},
+                                  {'col1': 'd', 'col2': 2, 'n': 4}])
+
+    def test_fold1(self):
+        conn = Conn(self.dbfile)
+
+        def minmax(col):
+            def fn(rs):
+                xs = [r[col] for r in rs]
+                return [min(xs), max(xs)]
+            return fn
+
+        conn['t1'] = self.t1
+        conn['t1_1'] = conn['t1'].by('col1').fold(
+            sum=lambda rs: sum(rs['col2']),
+            mm0=lambda rs: min(rs['col2']),
+            mm1=lambda rs: max(rs['col2'])
+        )
+
+        self.assertEqual(conn['t1_1'].list(),
+                         [{'col1': 'a', 'sum': 9, 'mm0': 4, 'mm1': 5},
+                          {'col1': 'b', 'sum': 1, 'mm0': 1, 'mm1': 1},
+                          {'col1': 'c', 'sum': 14, 'mm0': 3, 'mm1': 7},
+                          {'col1': 'd', 'sum': 2, 'mm0': 2, 'mm1': 2}])
+
+        conn['t1_1'] = conn['t1'].windowed(4, 3).fold(
+            sum=lambda rs: sum(rs['col2']),
+            mm0=lambda rs: min(rs['col2']),
+            mm1=lambda rs: max(rs['col2'])
+        )
+        self.assertEqual(conn['t1_1'].list(),
+                         [{'sum': 13, 'mm0': 1, 'mm1': 5},
+                          {'sum': 16, 'mm0': 2, 'mm1': 7}
+                          ])
+
+        conn['t1_1'] = conn['t1'].windowed(4, 5).fold(
+            sum=lambda rs: sum(rs['col2']),
+            mm0=lambda rs: min(rs['col2']),
+            mm1=lambda rs: max(rs['col2'])
+        ).rename(
+            mm1='mm0',
+            mm0='mm1'
+        )
+        self.assertEqual(conn['t1_1'].list(),
+                         [{'sum': 13, 'mm1': 1, 'mm0': 5},
+                          {'sum': 9, 'mm1': 2, 'mm0': 7}
+                          ])
+
+    def test_by(self):
+        def sum_by_col1(rs):
+            tot = sum(rs['col2'])
+            return rs.update(col2=tot)[:1]
+
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+        conn['t1_sum'] = conn['t1'].by('col1')\
+            .map(sum_by_col1)
+
+        self.assertEqual(list(conn['t1_sum']._iter()),
+                         [{'col1': 'a', 'col2': 9},
+                          {'col1': 'b', 'col2': 1},
+                          {'col1': 'c', 'col2': 14},
+                          {'col1': 'd', 'col2': 2}]
+                         )
+        conn['t1_sum2'] = conn['t1']\
+            .by('col1').map(sum_by_col1)
+
+        self.assertEqual(conn['t1_sum'].list(), conn['t1_sum2'].list())
+
+    def test_chain(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+        conn['t1_double'] = conn['t1'].chain(conn['t1'])
+        self.assertEqual(conn['t1'].list() + conn['t1'].list(),
+                         conn['t1_double'].list())
+
+        conn['t1_double'] = conn['t1'].chain(self.t1)
+        self.assertEqual(conn['t1'].list() + conn['t1'].list(),
+                         conn['t1_double'].list())
+
+    def test_df(self):
+        import pandas as pd
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+        df = pd.DataFrame(conn['t1']._iter())
+        conn['t1_copy'] = df.to_dict('records')
+        self.assertEqual(conn['t1'].list(), conn['t1_copy'].list())
+
+    def test_by_after_map(self):
+        def sumit(rs):
+            tot = sum(rs['col2'])
+            return rs.update(tot=tot)
+
+        def count(rs):
+            n = len(rs.list())
+            return rs.update(cnt=n)
+
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+        conn['t1_sum'] = conn['t1'].by('col1')\
+            .map(sumit).by('tot').map(count)
+
+        # on another db
+        conn1 = Conn(self.dbfile1)
+        conn1['t1_sum'] = conn['t1'].by('col1').map(sumit).by('tot').map(count)
+        conn1['t1_sum2'] = conn['t1'].by('col1').map(sumit)\
+            .by('tot').map(count)._iter()
+
+        self.assertEqual(conn['t1_sum'].list(), conn1['t1_sum'].list())
+        self.assertEqual(conn['t1_sum'].list(), conn1['t1_sum2'].list())
+
+    def test_multiple_by(self):
+
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+        conn['t1_1'] = conn['t1'].update(col3=1).by('col1, col3')\
+            .map(lambda rs: rs)
+
+        conn['t1_2'] = conn['t1'].update(col3=1).by('col1').map(lambda rs: rs)
+        self.assertEqual(conn['t1_1'].list(), conn['t1_2'].list())
+
+        conn['t1_1_double'] = conn['t1_1']\
+            .chain(conn['t1'].update(col3=1).by('col1, col3')
+                   .map(lambda rs: rs))
+        conn['t1_1_double2'] = conn['t1_1'].chain(conn['t1_1'])
+
+        self.assertEqual(conn['t1_1_double'].list(),
+                         conn['t1_1_double2'].list())
+
+    def test_islice_group(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+
+        self.assertEqual(conn['t1'].by('col1')[1:3].list(),
+                         [{'col1': 'b', 'col2': 1},
+                          {'col1': 'c', 'col2': 3},
+                          {'col1': 'c', 'col2': 4},
+                          {'col1': 'c', 'col2': 7}])
+
+        self.assertEqual(conn['t1'].windowed(4, 2)[1:3].list(),
+                         [{'col1': 'b', 'col2': 1},
+                          {'col1': 'c', 'col2': 3},
+                          {'col1': 'c', 'col2': 4},
+                          {'col1': 'c', 'col2': 7},
+                          {'col1': 'c', 'col2': 4},
+                          {'col1': 'c', 'col2': 7},
+                          {'col1': 'd', 'col2': 2}
+                          ])
+
+    def test_islice(self):
+
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+        conn['t2'] = self.t2
+
+        self.assertEqual(len(conn['t1']._islice(3).list()), 3)
+        self.assertEqual(len(conn['t1']._islice(3, None).list()), 4)
+        self.assertEqual(len(conn['t1']._islice(0, None, 3).list()), 3)
+
+        self.assertEqual(len(conn['t1'][:3].list()), 3)
+        self.assertEqual(len(conn['t1'][3:].list()), 4)
+        self.assertEqual(len(conn['t1'][0::3].list()), 3)
+
+        xs = conn['t1']._iter()
+        ys = conn['t2']._iter()
+
+        conn['t1_2'] = ({**x, **y} for x, y in product(xs, ys))
+
+        n1 = len(conn['t1'].list())
+        n2 = len(conn['t2'].list())
+        n3 = len(conn['t1_2'].list())
+
+        self.assertEqual(n3, n1 * n2)
+
+        xs = conn['t1'][0:5].filter(lambda r: r['col2'] > 3)
+        ys = conn['t1'][0:8].filter(lambda r: r['col2'] > 3)
+
+        self.assertEqual(len(xs.list()), 3)
+        self.assertEqual(len(ys.list()), 4)
+
+    def test_takewhile(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+
+        self.assertEqual(len(conn['t1']
+                             .takewhile(lambda r: r['col2'] > 1).list()), 2)
+
+        self.assertEqual(len(conn['t1']
+                             .order('col2 desc')
+                             .takewhile(lambda r: r['col2'] > 1).list()), 6)
+
+    def test_dropwhile(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+
+        self.assertEqual(len(conn['t1']
+                             .dropwhile(lambda r: r['col2'] > 1).list()), 5)
+
+        self.assertEqual(len(conn['t1']
+                             .order('col2')
+                             .dropwhile(lambda r: r['col2'] < 4).list()), 4)
+
+    def test_windowed_group(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+
+        self.assertEqual(conn['t1'].by('col1').windowed(2, 1)
+                         .index('cnt').list(),
+                         [{'col1': 'a', 'col2': 4, 'cnt': 0},
+                          {'col1': 'a', 'col2': 5, 'cnt': 0},
+                          {'col1': 'b', 'col2': 1, 'cnt': 0},
+                          {'col1': 'b', 'col2': 1, 'cnt': 1},
+                          {'col1': 'c', 'col2': 3, 'cnt': 1},
+                          {'col1': 'c', 'col2': 4, 'cnt': 1},
+                          {'col1': 'c', 'col2': 7, 'cnt': 1},
+                          {'col1': 'c', 'col2': 3, 'cnt': 2},
+                          {'col1': 'c', 'col2': 4, 'cnt': 2},
+                          {'col1': 'c', 'col2': 7, 'cnt': 2},
+                          {'col1': 'd', 'col2': 2, 'cnt': 2}])
+
+        self.assertEqual(conn['t1'].windowed(3, 1).windowed(2, 1)
+                         .index('cnt').list(),
+
+                         [{'col1': 'a', 'col2': 4, 'cnt': 0},
+                          {'col1': 'a', 'col2': 5, 'cnt': 0},
+                          {'col1': 'b', 'col2': 1, 'cnt': 0},
+                          {'col1': 'a', 'col2': 5, 'cnt': 0},
+                          {'col1': 'b', 'col2': 1, 'cnt': 0},
+                          {'col1': 'c', 'col2': 3, 'cnt': 0},
+                          {'col1': 'a', 'col2': 5, 'cnt': 1},
+                          {'col1': 'b', 'col2': 1, 'cnt': 1},
+                          {'col1': 'c', 'col2': 3, 'cnt': 1},
+                          {'col1': 'b', 'col2': 1, 'cnt': 1},
+                          {'col1': 'c', 'col2': 3, 'cnt': 1},
+                          {'col1': 'c', 'col2': 4, 'cnt': 1},
+                          {'col1': 'b', 'col2': 1, 'cnt': 2},
+                          {'col1': 'c', 'col2': 3, 'cnt': 2},
+                          {'col1': 'c', 'col2': 4, 'cnt': 2},
+                          {'col1': 'c', 'col2': 3, 'cnt': 2},
+                          {'col1': 'c', 'col2': 4, 'cnt': 2},
+                          {'col1': 'c', 'col2': 7, 'cnt': 2},
+                          {'col1': 'c', 'col2': 3, 'cnt': 3},
+                          {'col1': 'c', 'col2': 4, 'cnt': 3},
+                          {'col1': 'c', 'col2': 7, 'cnt': 3},
+                          {'col1': 'c', 'col2': 4, 'cnt': 3},
+                          {'col1': 'c', 'col2': 7, 'cnt': 3},
+                          {'col1': 'd', 'col2': 2, 'cnt': 3}])
+
+    def test_windowed(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+
+        def add1(rs):
+            return rs.update(col2=lambda r: r['col2'] + 1)
+
+        self.assertEqual(conn['t1'].windowed(4, 2).map(add1).list(),
+                         [{'col1': 'a', 'col2': 5},
+                          {'col1': 'a', 'col2': 6},
+                          {'col1': 'b', 'col2': 2},
+                          {'col1': 'c', 'col2': 4},
+                          {'col1': 'b', 'col2': 2},
+                          {'col1': 'c', 'col2': 4},
+                          {'col1': 'c', 'col2': 5},
+                          {'col1': 'c', 'col2': 8},
+                          {'col1': 'c', 'col2': 5},
+                          {'col1': 'c', 'col2': 8},
+                          {'col1': 'd', 'col2': 3}])
+
+    def test_filter(self):
+        conn = Conn(self.dbfile)
+
+        conn['t1'] = self.t1
+        conn['t1_1'] = conn['t1'].filter(lambda r: r['col2'] > 2)
+
+        self.assertEqual(len(conn['t1_1'].list()), 5)
+
+    def test_filter_group(self):
+        conn = Conn(self.dbfile)
+
+        conn['t1'] = self.t1
+        conn['t1_1'] = conn['t1'].group('col1')\
+            .filter(lambda rs: rs.size() >= 2)
+
+        self.assertEqual(len(conn['t1_1'].list()), 5)
+
+    def test_filter_windowed(self):
+        conn = Conn(self.dbfile)
+
+        conn['t1'] = self.t1
+        conn['t1_1'] = conn['t1'].windowed(5, 1)\
+            .filter(lambda rs: rs.filter(lambda r: r['col2'] > 3).size() >= 3)
+        self.assertEqual(conn['t1_1'].list(),
+                         [{'col1': 'a', 'col2': 4},
+                          {'col1': 'a', 'col2': 5},
+                          {'col1': 'b', 'col2': 1},
+                          {'col1': 'c', 'col2': 3},
+                          {'col1': 'c', 'col2': 4},
+                          {'col1': 'a', 'col2': 5},
+                          {'col1': 'b', 'col2': 1},
+                          {'col1': 'c', 'col2': 3},
+                          {'col1': 'c', 'col2': 4},
+                          {'col1': 'c', 'col2': 7}])
+
+    def test_update(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+        conn['t1_1'] = conn['t1'].update(
+            col2=lambda r: r['col2'] + 1,
+            col3=lambda r: r['col1'] + str(r['col2'])
+        )
+        # table is fetched as it's inserted. not sure if it's a feature.
+        self.assertEqual(conn['t1_1'].list()[0],
+                         {'col1': 'a', 'col2': 5, 'col3': 'a5'})
+
+    def test_select(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+
+        conn['t1_1'] = conn['t1'].update(
+            col2=lambda r: r['col2'] + 1,
+            col3=lambda r: r['col1'] + str(r['col2'])
+        )
+
+        r = next(conn['t1_1'].select('col1, col3')._iter())
+        self.assertEqual(len(r), 2)
+
+        # test deselect
+        r = next(conn['t1_1'].deselect('col1, col3')._iter())
+        self.assertEqual(len(r), 1)
+
+    def test_join(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+        conn['t2'] = self.t2
+
+        conn['t1_1'] = conn['t1'].by('col1')\
+            .join(conn['t2'].by('col1'), "inner")
+
+        self.assertEqual(len(conn['t1_1'].list()), 3)
+
+        conn['t1_2'] = conn['t1'].by('col1')\
+            .join(conn['t2'].by('col1'), "left")
+
+        self.assertEqual(conn['t1_2'].list(),
+                         [{'col1': 'a', 'col2': 4, 'col3': ''},
+                          {'col1': 'a', 'col2': 5, 'col3': ''},
+                          {'col1': 'b', 'col2': 1, 'col3': 1},
+                          {'col1': 'c', 'col2': 3, 'col3': ''},
+                          {'col1': 'c', 'col2': 4, 'col3': ''},
+                          {'col1': 'c', 'col2': 7, 'col3': ''},
+                          {'col1': 'd', 'col2': 2, 'col3': 3},
+                          {'col1': 'd', 'col2': 2, 'col3': 2}])
+
+        conn['t1_3'] = conn['t1'].by('col1')\
+            .join(conn['t2'].by('col1'), "right")
+
+        self.assertEqual(conn['t1_3'].list(),
+                         [{'col1': 'b', 'col2': 1, 'col3': 1},
+                          {'col1': 'd', 'col2': 2, 'col3': 3},
+                          {'col1': 'd', 'col2': 2, 'col3': 2},
+                          {'col1': 'e', 'col2': '', 'col3': 3},
+                          {'col1': 'e', 'col2': '', 'col3': 4}])
+
+        conn['t1_4'] = conn['t1'].by('col1')\
+            .join(conn['t2'].by('col1'), "full")
+
+        self.assertEqual(conn['t1_4'].list(), [
+            {'col1': 'a', 'col2': 4, 'col3': ''},
+            {'col1': 'a', 'col2': 5, 'col3': ''},
+            {'col1': 'b', 'col2': 1, 'col3': 1},
+            {'col1': 'c', 'col2': 3, 'col3': ''},
+            {'col1': 'c', 'col2': 4, 'col3': ''},
+            {'col1': 'c', 'col2': 7, 'col3': ''},
+            {'col1': 'd', 'col2': 2, 'col3': 3},
+            {'col1': 'd', 'col2': 2, 'col3': 2},
+            {'col1': 'e', 'col2': '', 'col3': 3},
+            {'col1': 'e', 'col2': '', 'col3': 4}]
+        )
+
+    def test_join2(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+        conn['t2'] = self.t2
+
+        conn['t1_1'] = conn['t1'].chain([{'col1': 'd', 'col2': 9}, {
+            'col1': 'd', 'col2': 19}]).by('col1')\
+            .join(conn['t2'].by('col1'), 'full')
+
+        conn['t1_1'] = conn['t1'].chain([{'col1': 'd', 'col2': 9}, {
+            'col1': 'd', 'col2': 19}]).by('col1')\
+            .join(conn['t2'].by('col1'), 'full')
+
+        conn['t1_2'] = conn['t1'].chain([{'col1': 'd', 'col2': 9}, {
+            'col1': 'd', 'col2': 19}]).by('col1')\
+            .join(conn['t2'].by('col1'), 'full')\
+            .update(col4=lambda r: r['col3'] + 1 if r['col3'] else '')
+
+        self.assertEqual(conn['t1_1'].list(),
+                         [{'col1': 'a', 'col2': 4, 'col3': ''},
+                          {'col1': 'a', 'col2': 5, 'col3': ''},
+                          {'col1': 'b', 'col2': 1, 'col3': 1},
+                          {'col1': 'c', 'col2': 3, 'col3': ''},
+                          {'col1': 'c', 'col2': 4, 'col3': ''},
+                          {'col1': 'c', 'col2': 7, 'col3': ''},
+                          {'col1': 'd', 'col2': 2, 'col3': 3},
+                          {'col1': 'd', 'col2': 2, 'col3': 2},
+                          {'col1': 'd', 'col2': 9, 'col3': 3},
+                          {'col1': 'd', 'col2': 9, 'col3': 2},
+                          {'col1': 'd', 'col2': 19, 'col3': 3},
+                          {'col1': 'd', 'col2': 19, 'col3': 2},
+                          {'col1': 'e', 'col2': '', 'col3': 3},
+                          {'col1': 'e', 'col2': '', 'col3': 4}])
+
+    def test_join3(self):
+        rs1 = Rows(self.t1)
+        rs2 = Rows(self.t2)
+        rs = rs1.by('col1').join(rs2.by('col1'), 'left')
+        self.assertEqual(rs.list(),
+                         [{'col1': 'a', 'col2': 4, 'col3': ''},
+                          {'col1': 'a', 'col2': 5, 'col3': ''},
+                          {'col1': 'b', 'col2': 1, 'col3': 1},
+                          {'col1': 'c', 'col2': 3, 'col3': ''},
+                          {'col1': 'c', 'col2': 4, 'col3': ''},
+                          {'col1': 'c', 'col2': 7, 'col3': ''},
+                          {'col1': 'd', 'col2': 2, 'col3': 3},
+                          {'col1': 'd', 'col2': 2, 'col3': 2}])
+
+        self.assertEqual(rs1.list(), self.t1)
+
+    def test_join4(self):
+        rs1 = Rows(self.t1)
+        rs2 = Rows(self.t2)
+        rs1 = rs1.chain([{'col1': 'f', 'col2': 9},
+                        {'col1': 'f', 'col2': 8},
+                        {'col1': 'd', 'col2': 11},
+
+                         ])
+        rs1 = rs1.update(col4=lambda r: r['col2'] * 20)
+
+        rs2 = rs2.update(col2=lambda r: r['col3'] * 10)
+        rs3 = rs1.by('col1').join(rs2.by('col1'), 'full')
+        self.assertEqual(rs3.list(),
+                         [{'col1': 'a', 'col2': 4, 'col4': 80, 'col3': ''},
+                          {'col1': 'a', 'col2': 5, 'col4': 100, 'col3': ''},
+                          {'col1': 'b', 'col2': 10, 'col4': 20, 'col3': 1},
+                          {'col1': 'c', 'col2': 3, 'col4': 60, 'col3': ''},
+                          {'col1': 'c', 'col2': 4, 'col4': 80, 'col3': ''},
+                          {'col1': 'c', 'col2': 7, 'col4': 140, 'col3': ''},
+                          {'col1': 'd', 'col2': 30, 'col4': 40, 'col3': 3},
+                          {'col1': 'd', 'col2': 20, 'col4': 40, 'col3': 2},
+                          {'col1': 'd', 'col2': 30, 'col4': 220, 'col3': 3},
+                          {'col1': 'd', 'col2': 20, 'col4': 220, 'col3': 2},
+                          {'col1': 'e', 'col2': 30, 'col4': '', 'col3': 3},
+                          {'col1': 'e', 'col2': 40, 'col4': '', 'col3': 4},
+                          {'col1': 'f', 'col2': 9, 'col4': 180, 'col3': ''},
+                          {'col1': 'f', 'col2': 8, 'col4': 160, 'col3': ''},
+                          ])
+        conn = Conn(self.dbfile)
+        conn['t1'] = rs1
+        conn['t2'] = rs2
+        conn['t3'] = conn['t1'].by('col1').join(conn['t2'].by('col1'), 'full')
+        self.assertEqual(rs3.list(), conn['t3'].list())
+
+        rs3 = rs1.by('col1').join(rs2.by('col1'), 'left')
+        conn['t3'] = conn['t1'].by('col1').join(conn['t2'].by('col1'), 'left')
+        self.assertEqual(rs3.list(), conn['t3'].list())
+
+        rs3 = rs1.by('col1').join(rs2.by('col1'), 'right')
+        conn['t3'] = conn['t1'].by('col1').join(conn['t2'].by('col1'), 'right')
+        self.assertEqual(rs3.list(), conn['t3'].list())
+
+        rs3 = rs1.by('col1').join(rs2.by('col1'), 'inner')
+        conn['t3'] = conn['t1'].by('col1').join(conn['t2'].by('col1'), 'inner')
+        self.assertEqual(rs3.list(), conn['t3'].list())
+
+    def test_merge(self):
+        rs1 = Rows(self.t1)
+        rs2 = Rows(self.t2)
+        rs1 = rs1.chain([{'col1': 'f', 'col2': 9},
+                         {'col1': 'f', 'col2': 8}])
+        rs2 = rs2.chain([{'col1': 'a', 'col3': 91}])
+
+        rs1 = rs1.update(col4=lambda r: r['col2'] * 20)
+        rs2 = rs2.update(col2=lambda r: r['col3'] * 10)
+
+        rs3 = rs1.by('col1').merge(rs2.by('col1'), 'full')
+        self.assertEqual(rs3.list(),
+                         [{'col1': 'a', 'col2': 910, 'col4': 80, 'col3': 91},
+                          {'col1': 'a', 'col2': 5, 'col4': 100, 'col3': ''},
+                          {'col1': 'b', 'col2': 10, 'col4': 20, 'col3': 1},
+                          {'col1': 'c', 'col2': 3, 'col4': 60, 'col3': ''},
+                          {'col1': 'c', 'col2': 4, 'col4': 80, 'col3': ''},
+                          {'col1': 'c', 'col2': 7, 'col4': 140, 'col3': ''},
+                          {'col1': 'd', 'col2': 30, 'col4': 40, 'col3': 3},
+                          {'col1': 'd', 'col2': 20, 'col4': '', 'col3': 2},
+                          {'col1': 'e', 'col2': 30, 'col4': '', 'col3': 3},
+                          {'col1': 'e', 'col2': 40, 'col4': '', 'col3': 4},
+                          {'col1': 'f', 'col2': 9, 'col4': 180, 'col3': ''},
+                          {'col1': 'f', 'col2': 8, 'col4': 160, 'col3': ''}])
+
+        conn = Conn(self.dbfile)
+        conn['t1'] = rs1
+        conn['t2'] = rs2
+        conn['t3'] = conn['t1'].by('col1').merge(conn['t2'].by('col1'), 'full')
+        self.assertEqual(rs3.list(), conn['t3'].list())
+
+        rs3 = rs1.by('col1').merge(rs2.by('col1'), 'left')
+        conn['t3'] = conn['t1'].by('col1').merge(conn['t2'].by('col1'), 'left')
+        self.assertEqual(rs3.list(), conn['t3'].list())
+
+        rs3 = rs1.by('col1').merge(rs2.by('col1'), 'right')
+        conn['t3'] = conn['t1'].by('col1').merge(
+            conn['t2'].by('col1'), 'right')
+        self.assertEqual(rs3.list(), conn['t3'].list())
+
+        rs3 = rs1.by('col1').merge(rs2.by('col1'), 'inner')
+        conn['t3'] = conn['t1'].by('col1').merge(
+            conn['t2'].by('col1'), 'inner')
+        self.assertEqual(rs3.list(), conn['t3'].list())
+
+    def test_distinct(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+        conn['t1_1'] = conn['t1'].distinct('col1')
+        self.assertEqual(len(conn['t1_1'].list()), 4)
+        conn['t1_2'] = conn['t1'].distinct('col1, col2')
+        self.assertEqual(len(conn['t1_2'].list()), 7)
+
+    def test_order(self):
+        conn = Conn(self.dbfile)
+        conn['t1'] = self.t1
+
+        [g1, g2, g3, g4] = [list(xs) for _, xs in conn['t1']
+                            .order('col1, col2 desc').group('col1')._iter()]
+        self.assertEqual(
+            g1, [{'col1': 'a', 'col2': 5}, {'col1': 'a', 'col2': 4}]
+        )
+        self.assertEqual(g2, [{'col1': 'b', 'col2': 1}])
+        self.assertEqual(g3, [{'col1': 'c', 'col2': 7}, {
+                         'col1': 'c', 'col2': 4}, {'col1': 'c', 'col2': 3}])
+        self.assertEqual(g4, [{'col1': 'd', 'col2': 2}])
+
+    def test_readme(self):
+        t1 = [
+            {'col1': 'a', 'col2': 4},
+            {'col1': 'a', 'col2': 5},
+            {'col1': 'b', 'col2': 1},
+        ]
+
+        conn = Conn(self.dbfile)
+        conn['t1'] = t1
+
+        for r1, r2 in zip(conn['t1'].list(), conn['t1']._iter()):
+            self.assertEqual(r1, r2)
+
+        import pandas as pd
+
+        df = pd.DataFrame(conn['t1']._iter())
+        conn['t1_copy'] = df.to_dict('records')
+
+        self.assertEqual(conn['t1'].list(), conn['t1_copy'].list())
+
+        conn['t1_1'] = conn['t1']\
+            .filter(lambda r: r['col2'] > 2)\
+            .update(col2=lambda r: r['col2'] + 1)
+
+        self.assertEqual(conn['t1_1'].list()[0]['col2'], 5)
+
+        conn['t1_col2sum_groupby_col1'] = conn['t1'].by('col1')\
+            .fold(col2_sum=lambda rs: sum(rs['col2']))\
+            .deselect('col2')
+
+        conn['t1_col2sum_groupby_col1_1'] = conn['t1']\
+            .order('col1, col2 desc').group('col1')\
+            .fold(col2_sum=lambda rs: sum(rs['col2']))\
+            .deselect('col2')
+
+        self.assertEqual(conn['t1_col2sum_groupby_col1'].list(),
+                         conn['t1_col2sum_groupby_col1_1'].list())
+
+        conn['t1_double'] = conn['t1'].chain(conn['t1'])
+        self.assertEqual(len(conn['t1_double'].list()),
+                         2 * len(conn['t1'].list()))
+
+        conn['t1_double'] = conn['t1'].chain(t1)
+
+        self.assertEqual(len(conn['t1_double'].list()),
+                         2 * len(conn['t1'].list()))
+
+        conn['t1_1'] = conn['t1']\
+            .filter(lambda r: r['col2'] > 2)\
+            .update(
+            col2=lambda r: r['col2'] + 1,
+            col3=lambda r: r['col1'] + str(r['col2'])
+        )
+        self.assertEqual(conn['t1_1'].list(),
+                         [{'col1': 'a', 'col2': 5, 'col3': 'a5'},
+                          {'col1': 'a', 'col2': 6, 'col3': 'a6'}])
+
+        conn['t1_1'] = conn['t1'].update(col3=lambda r: r['col2'] + 1)\
+            .deselect('col1, col2')
+
+        self.assertEqual(conn['t1_1'].list(),
+                         [{'col3': 5}, {'col3': 6}, {'col3': 2}])
+
+        conn['t1_1'] = conn['t1'].distinct('col1')
+        self.assertEqual(conn['t1_1'].list(), [
+                         {'col1': 'a', 'col2': 4}, {'col1': 'b', 'col2': 1}])
+
+        conn['t2'] = [
+            {'col1': 'b', 'col3': -1},
+            {'col1': 'c', 'col3': 3},
+            {'col1': 'b', 'col3': ''},
+        ]
+
+        conn['t1_col3'] = conn['t1'].by('col1')\
+            .join(conn['t2'].by('col1'), 'full')
+
+        self.assertEqual(conn['t1_col3'].list(),
+                         [{'col1': 'a', 'col2': 4, 'col3': ''},
+                         {'col1': 'a', 'col2': 5, 'col3': ''},
+                         {'col1': 'b', 'col2': 1, 'col3': -1},
+                         {'col1': 'b', 'col2': 1, 'col3': ''},
+                          {'col1': 'c', 'col2': '', 'col3': 3}]
+                         )
```

