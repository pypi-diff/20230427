# Comparing `tmp/biobear-0.2.0.tar.gz` & `tmp/biobear-0.3.0.tar.gz`

## Comparing `biobear-0.2.0.tar` & `biobear-0.3.0.tar`

### file list

```diff
@@ -1,43 +1,54 @@
--rw-r--r--   0        0        0      332 1970-01-01 00:00:00.000000 biobear-0.2.0/Cargo.toml
--rw-r--r--   0     1001      123     2566 2023-04-24 15:23:51.000000 biobear-0.2.0/.github/workflows/release.yml
--rw-r--r--   0     1001      123      890 2023-04-24 15:23:51.000000 biobear-0.2.0/.github/workflows/test.yml
--rw-r--r--   0     1001      123     4135 2023-04-24 15:23:51.000000 biobear-0.2.0/.gitignore
--rw-r--r--   0     1001      123     1055 2023-04-24 15:23:51.000000 biobear-0.2.0/LICENSE
--rw-r--r--   0     1001      123       68 2023-04-24 15:23:51.000000 biobear-0.2.0/Makefile
--rw-r--r--   0     1001      123     5677 2023-04-24 15:23:51.000000 biobear-0.2.0/README.md
--rw-r--r--   0     1001      123      167 2023-04-24 15:23:51.000000 biobear-0.2.0/cz.json
--rw-r--r--   0     1001      123      555 2023-04-24 15:23:51.000000 biobear-0.2.0/pyproject.toml
--rw-r--r--   0     1001      123      453 2023-04-24 15:23:51.000000 biobear-0.2.0/python/biobear/__init__.py
--rw-r--r--   0     1001      123      895 2023-04-24 15:23:51.000000 biobear-0.2.0/python/biobear/bam_reader.py
--rw-r--r--   0     1001      123      536 2023-04-24 15:23:51.000000 biobear-0.2.0/python/biobear/compression.py
--rw-r--r--   0     1001      123      969 2023-04-24 15:23:51.000000 biobear-0.2.0/python/biobear/fasta_reader.py
--rw-r--r--   0     1001      123      991 2023-04-24 15:23:51.000000 biobear-0.2.0/python/biobear/fastq_reader.py
--rw-r--r--   0     1001      123      373 2023-04-24 15:23:51.000000 biobear-0.2.0/python/biobear/gff_reader.py
--rw-r--r--   0     1001      123      840 2023-04-24 15:23:51.000000 biobear-0.2.0/python/biobear/vcf_reader.py
--rw-r--r--   0     1001      123     6152 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/data/bedcov.bam
--rw-r--r--   0     1001      123     7608 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/data/bedcov.bam.bai
--rw-r--r--   0     1001      123     1749 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/data/file.vcf
--rw-r--r--   0     1001      123     8296 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/data/index.vcf.gz
--rw-r--r--   0     1001      123      212 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/data/index.vcf.gz.tbi
--rw-r--r--   0     1001      123       41 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/data/test.fasta
--rw-r--r--   0     1001      123       58 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/data/test.fasta.gz
--rw-r--r--   0     1001      123      286 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/data/test.fastq
--rw-r--r--   0     1001      123      134 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/data/test.fastq.gz
--rw-r--r--   0     1001      123      112 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/data/test.gff
--rw-r--r--   0     1001      123     4302 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/data/vcf_file.vcf
--rw-r--r--   0     1001      123     1669 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/data/vcf_file.vcf.gz
--rw-r--r--   0     1001      123      254 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/data/vcf_file.vcf.gz.tbi
--rw-r--r--   0     1001      123      822 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/test_bam_reader.py
--rw-r--r--   0     1001      123      855 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/test_fasta_reader.py
--rw-r--r--   0     1001      123      855 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/test_fastq_reader.py
--rw-r--r--   0     1001      123      399 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/test_gff_reader.py
--rw-r--r--   0     1001      123      901 2023-04-24 15:23:51.000000 biobear-0.2.0/python/tests/test_vcf_reader.py
--rw-r--r--   0     1001      123       20 2023-04-24 15:23:51.000000 biobear-0.2.0/requirements-dev.txt
--rw-r--r--   0     1001      123     8562 2023-04-24 15:23:51.000000 biobear-0.2.0/src/bam_reader.rs
--rw-r--r--   0     1001      123     3991 2023-04-24 15:23:51.000000 biobear-0.2.0/src/fasta_reader.rs
--rw-r--r--   0     1001      123     4420 2023-04-24 15:23:51.000000 biobear-0.2.0/src/fastq_reader.rs
--rw-r--r--   0     1001      123     4949 2023-04-24 15:23:51.000000 biobear-0.2.0/src/gff_reader.rs
--rw-r--r--   0     1001      123      640 2023-04-24 15:23:51.000000 biobear-0.2.0/src/lib.rs
--rw-r--r--   0     1001      123     8074 2023-04-24 15:23:51.000000 biobear-0.2.0/src/vcf_reader.rs
--rw-r--r--   0     1001      123    37528 2023-04-24 15:24:48.000000 biobear-0.2.0/Cargo.lock
--rw-r--r--   0        0        0     6116 1970-01-01 00:00:00.000000 biobear-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      379 1970-01-01 00:00:00.000000 biobear-0.3.0/Cargo.toml
+-rw-r--r--   0     1001      123     2566 2023-04-27 14:22:00.000000 biobear-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0     1001      123      865 2023-04-27 14:22:00.000000 biobear-0.3.0/.github/workflows/smoke-test.yml
+-rw-r--r--   0     1001      123      107 2023-04-27 14:22:00.000000 biobear-0.3.0/.github/workflows/smoketest.py
+-rw-r--r--   0     1001      123      891 2023-04-27 14:22:00.000000 biobear-0.3.0/.github/workflows/test.yml
+-rw-r--r--   0     1001      123     4135 2023-04-27 14:22:00.000000 biobear-0.3.0/.gitignore
+-rw-r--r--   0     1001      123     1055 2023-04-27 14:22:00.000000 biobear-0.3.0/LICENSE
+-rw-r--r--   0     1001      123       71 2023-04-27 14:22:00.000000 biobear-0.3.0/Makefile
+-rw-r--r--   0     1001      123    17139 2023-04-27 14:22:00.000000 biobear-0.3.0/README.md
+-rw-r--r--   0     1001      123      186 2023-04-27 14:22:00.000000 biobear-0.3.0/cz.json
+-rw-r--r--   0     1001      123      238 2023-04-27 14:22:00.000000 biobear-0.3.0/docs.bash
+-rw-r--r--   0     1001      123      565 2023-04-27 14:22:00.000000 biobear-0.3.0/pyproject.toml
+-rw-r--r--   0     1001      123      482 2023-04-27 14:22:00.000000 biobear-0.3.0/python/biobear/__init__.py
+-rw-r--r--   0     1001      123     2270 2023-04-27 14:22:00.000000 biobear-0.3.0/python/biobear/bam_reader.py
+-rw-r--r--   0     1001      123      720 2023-04-27 14:22:00.000000 biobear-0.3.0/python/biobear/compression.py
+-rw-r--r--   0     1001      123     1369 2023-04-27 14:22:00.000000 biobear-0.3.0/python/biobear/fasta_reader.py
+-rw-r--r--   0     1001      123     1463 2023-04-27 14:22:00.000000 biobear-0.3.0/python/biobear/fastq_reader.py
+-rw-r--r--   0     1001      123     1229 2023-04-27 14:22:00.000000 biobear-0.3.0/python/biobear/gff_reader.py
+-rw-r--r--   0     1001      123     2175 2023-04-27 14:22:00.000000 biobear-0.3.0/python/biobear/vcf_reader.py
+-rw-r--r--   0     1001      123     6152 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/bedcov.bam
+-rw-r--r--   0     1001      123     7608 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/bedcov.bam.bai
+-rw-r--r--   0     1001      123     1749 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/file.vcf
+-rw-r--r--   0     1001      123     8296 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/index.vcf.gz
+-rw-r--r--   0     1001      123      212 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/index.vcf.gz.tbi
+-rw-r--r--   0     1001      123       41 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/test.fasta
+-rw-r--r--   0     1001      123       58 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/test.fasta.gz
+-rw-r--r--   0     1001      123      286 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/test.fastq
+-rw-r--r--   0     1001      123      134 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/test.fastq.gz
+-rw-r--r--   0     1001      123      112 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/test.gff
+-rw-r--r--   0     1001      123       91 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/test.gff.gz
+-rw-r--r--   0     1001      123     4302 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/vcf_file.vcf
+-rw-r--r--   0     1001      123     1669 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/vcf_file.vcf.gz
+-rw-r--r--   0     1001      123      254 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/data/vcf_file.vcf.gz.tbi
+-rw-r--r--   0     1001      123      800 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/test_bam_reader.py
+-rw-r--r--   0     1001      123     1205 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/test_fasta_reader.py
+-rw-r--r--   0     1001      123     1154 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/test_fastq_reader.py
+-rw-r--r--   0     1001      123      919 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/test_gff_reader.py
+-rw-r--r--   0     1001      123      898 2023-04-27 14:22:00.000000 biobear-0.3.0/python/tests/test_vcf_reader.py
+-rw-r--r--   0     1001      123       20 2023-04-27 14:22:00.000000 biobear-0.3.0/requirements-dev.txt
+-rw-r--r--   0     1001      123     6470 2023-04-27 14:22:00.000000 biobear-0.3.0/src/bam_reader/bam_batch.rs
+-rw-r--r--   0     1001      123     6442 2023-04-27 14:22:00.000000 biobear-0.3.0/src/bam_reader.rs
+-rw-r--r--   0     1001      123      565 2023-04-27 14:22:00.000000 biobear-0.3.0/src/batch.rs
+-rw-r--r--   0     1001      123     3635 2023-04-27 14:22:00.000000 biobear-0.3.0/src/fasta_reader/fasta_batch.rs
+-rw-r--r--   0     1001      123     3673 2023-04-27 14:22:00.000000 biobear-0.3.0/src/fasta_reader.rs
+-rw-r--r--   0     1001      123     3365 2023-04-27 14:22:00.000000 biobear-0.3.0/src/fastq_reader/fastq_batch.rs
+-rw-r--r--   0     1001      123     3360 2023-04-27 14:22:00.000000 biobear-0.3.0/src/fastq_reader.rs
+-rw-r--r--   0     1001      123     5084 2023-04-27 14:22:00.000000 biobear-0.3.0/src/gff_reader/gff_batch.rs
+-rw-r--r--   0     1001      123     3294 2023-04-27 14:22:00.000000 biobear-0.3.0/src/gff_reader.rs
+-rw-r--r--   0     1001      123      720 2023-04-27 14:22:00.000000 biobear-0.3.0/src/lib.rs
+-rw-r--r--   0     1001      123      938 2023-04-27 14:22:00.000000 biobear-0.3.0/src/to_arrow.rs
+-rw-r--r--   0     1001      123     5804 2023-04-27 14:22:00.000000 biobear-0.3.0/src/vcf_reader/vcf_batch.rs
+-rw-r--r--   0     1001      123     4941 2023-04-27 14:22:00.000000 biobear-0.3.0/src/vcf_reader.rs
+-rw-r--r--   0     1001      123    37575 2023-04-27 14:23:06.000000 biobear-0.3.0/Cargo.lock
+-rw-r--r--   0        0        0    17587 1970-01-01 00:00:00.000000 biobear-0.3.0/PKG-INFO
```

### Comparing `biobear-0.2.0/.github/workflows/release.yml` & `biobear-0.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `biobear-0.2.0/.github/workflows/test.yml` & `biobear-0.3.0/.github/workflows/test.yml`

 * *Files 0% similar despite different names*

```diff
@@ -28,9 +28,10 @@
                   python -m pip install --upgrade pip
                   pip install virtualenv
                   virtualenv venv
                   source venv/bin/activate
                   pip install -r requirements-dev.txt
                   cargo build
                   maturin develop
+
                   ruff check python/
                   pytest
```

### Comparing `biobear-0.2.0/.gitignore` & `biobear-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `biobear-0.2.0/LICENSE` & `biobear-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobear-0.2.0/pyproject.toml` & `biobear-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,16 @@
   {name = "WHERE TRUE devs", email = "thauck+biobear@wheretrue.com"},
 ]
 classifiers = [
   "Programming Language :: Rust",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = ["polars>=0.17.0"]
+dependencies = ["polars[pyarrow]>=0.17.0"]
+
 license = {file = "LICENSE"}
 name = "biobear"
 readme = "README.md"
 requires-python = ">=3.7"
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
```

### Comparing `biobear-0.2.0/python/biobear/fastq_reader.py` & `biobear-0.3.0/python/biobear/fasta_reader.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,44 @@
-import os
+"""FASTA file reader."""
+from pathlib import Path
 
-from .biobear import _FastqReader, _FastqGzippedReader
+from .biobear import (
+    _FastaReader,
+    _FastaGzippedReader,
+)
 from biobear.compression import Compression
 
+import pyarrow as pa
+import pyarrow.dataset as ds
 import polars as pl
 
-class FastqReader:
-    def __init__(
-        self,
-        path: os.PathLike,
-        compression: Compression = Compression.INFERRED
-    ):
-        """Read a fastq file.
+
+class FastaReader:
+    def __init__(self, path: Path, compression: Compression = Compression.INFERRED):
+        """Read a fasta file.
 
         Args:
-            path (Path): Path to the fastq file.
+            path (Path): Path to the fasta file.
 
         Kwargs:
             compression (Compression): Compression type of the file. Defaults to
                 Compression.INFERRED.
 
         """
-        if compression == Compression.INFERRED:
-            compression = compression.from_file(path)
+        self.compression = compression.infer_or_use(path)
 
-        if compression == Compression.GZIP:
-            self._fastq_reader = _FastqGzippedReader(str(path))
+        if self.compression == Compression.GZIP:
+            self._fasta_reader = _FastaGzippedReader(str(path))
         else:
-            self._fastq_reader = _FastqReader(str(path))
+            self._fasta_reader = _FastaReader(str(path))
 
     def read(self) -> pl.DataFrame:
-        return self.to_polars()
+        """Read the fasta file and return a polars DataFrame."""
+        return pl.from_arrow(self.to_arrow_record_batch_reader().read_all())
 
-    def to_polars(self) -> pl.DataFrame:
-        contents = self._fastq_reader.read()
-        return pl.read_ipc(contents)
+    def to_arrow_scanner(self) -> ds.Scanner:
+        """Convert the fasta reader to an arrow scanner."""
+        return ds.Scanner.from_batches(self.to_arrow_record_batch_reader())
+
+    def to_arrow_record_batch_reader(self) -> pa.RecordBatchReader:
+        """Convert the fasta reader to an arrow batch reader."""
+        return self._fasta_reader.to_pyarrow()
```

### Comparing `biobear-0.2.0/python/tests/data/bedcov.bam` & `biobear-0.3.0/python/tests/data/bedcov.bam`

 * *Files identical despite different names*

### Comparing `biobear-0.2.0/python/tests/data/bedcov.bam.bai` & `biobear-0.3.0/python/tests/data/bedcov.bam.bai`

 * *Files identical despite different names*

### Comparing `biobear-0.2.0/python/tests/data/file.vcf` & `biobear-0.3.0/python/tests/data/file.vcf`

 * *Files identical despite different names*

### Comparing `biobear-0.2.0/python/tests/data/index.vcf.gz` & `biobear-0.3.0/python/tests/data/index.vcf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.2.0/python/tests/data/vcf_file.vcf` & `biobear-0.3.0/python/tests/data/vcf_file.vcf`

 * *Files identical despite different names*

### Comparing `biobear-0.2.0/python/tests/data/vcf_file.vcf.gz` & `biobear-0.3.0/python/tests/data/vcf_file.vcf.gz`

 * *Files identical despite different names*

### Comparing `biobear-0.2.0/python/tests/test_bam_reader.py` & `biobear-0.3.0/python/tests/test_bam_reader.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,27 +7,30 @@
 from biobear import BamReader, BamIndexedReader
 
 DATA = Path(__file__).parent / "data"
 
 
 def test_bam_reader():
     reader = BamReader(DATA / "bedcov.bam")
-    df = reader.to_polars()
+    df = reader.read()
 
     assert len(df) == 61
 
+
 def test_bam_reader_no_file():
-    with pytest.raises(FileNotFoundError):
+    with pytest.raises(OSError):
         BamReader("test.bam")
 
+
 def test_bam_indexed_reader():
     reader = BamIndexedReader(DATA / "bedcov.bam", DATA / "bedcov.bam.bai")
     df = reader.query("chr1", 12203700, 12205426)
 
     assert len(df) == 1
 
     with pytest.raises(ValueError):
         reader.query("1", 12203700, 12205426)
 
+
 def test_bam_indexed_reader_no_file():
-    with pytest.raises(FileNotFoundError):
+    with pytest.raises(OSError):
         BamIndexedReader("test.bam", "test.bam.bai")
```

### Comparing `biobear-0.2.0/python/tests/test_fasta_reader.py` & `biobear-0.3.0/python/tests/test_fastq_reader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,48 @@
 # Test the fasta reader can be converted to a polars dataframe
 
 from pathlib import Path
+
 import pytest
 
-from biobear import FastaReader
+from biobear import FastqReader
 from biobear.compression import Compression
 
 DATA = Path(__file__).parent / "data"
 
 
-def test_fasta_reader():
-    fasta_reader = FastaReader(DATA / "test.fasta")
-    df = fasta_reader.to_polars()
+def test_fastq_reader():
+    fastq_reader = FastqReader(DATA / "test.fastq")
+    df = fastq_reader.read()
 
     assert len(df) == 2
 
 
-def test_fasta_gzipped_reader():
+def test_fastq_gzipped_reader():
     # Test that the gzip compression is inferred
-    fasta_reader = FastaReader(DATA / "test.fasta.gz")
-    df = fasta_reader.to_polars()
+    fastq_reader = FastqReader(DATA / "test.fastq.gz")
+    df = fastq_reader.read()
 
     assert len(df) == 2
 
     # Test that the gzip compression is explicitly set
-    fasta_reader = FastaReader(DATA / "test.fasta.gz", Compression.GZIP)
-    df = fasta_reader.to_polars()
+    fastq_reader = FastqReader(DATA / "test.fastq.gz", Compression.GZIP)
+    df = fastq_reader.read()
 
     assert len(df) == 2
 
 
-def test_fasta_reader_no_file():
-    with pytest.raises(FileNotFoundError):
-        FastaReader("test.fasta")
+def test_to_arrow_scanner():
+    fastq_reader = FastqReader(DATA / "test.fastq")
+    scanner = fastq_reader.to_arrow_scanner()
+
+    assert scanner.count_rows() == 2
+
+    gzipped_fastq_reader = FastqReader(DATA / "test.fastq.gz")
+    scanner = gzipped_fastq_reader.to_arrow_scanner()
+
+    assert scanner.count_rows() == 2
+
+
+def test_fastq_reader_no_file():
+    with pytest.raises(OSError):
+        FastqReader("test.fastq")
```

### Comparing `biobear-0.2.0/python/tests/test_vcf_reader.py` & `biobear-0.3.0/python/tests/test_vcf_reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,29 +11,33 @@
 
 def test_vcf_reader():
     reader = VCFReader(DATA / "vcf_file.vcf")
     df = reader.read()
 
     assert len(df) == 15
 
+
 def test_vcf_reader_missing_file():
-    with pytest.raises(FileNotFoundError):
+    with pytest.raises(OSError):
         VCFReader("test.vcf")
 
+
 def test_vcf_indexed_reader_read():
     reader = VCFIndexedReader(DATA / "vcf_file.vcf.gz")
     df = reader.read()
 
     assert len(df) == 15
 
+
 def test_vcf_indexed_reader_query():
     reader = VCFIndexedReader(DATA / "vcf_file.vcf.gz")
     df = reader.query("1")
 
     assert len(df) == 11
 
     with pytest.raises(ValueError):
         reader.query("chr1")
 
+
 def test_vcf_indexed_reader_query_missing_file():
-    with pytest.raises(OSError):
+    with pytest.raises(ValueError):
         VCFIndexedReader("test.vcf.gz")
```

### Comparing `biobear-0.2.0/src/fastq_reader.rs` & `biobear-0.3.0/src/fastq_reader/fastq_batch.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,50 @@
-use pyo3::prelude::*;
-
-use arrow::array::*;
-use arrow::datatypes::*;
-use arrow::ipc::writer::FileWriter;
-use arrow::record_batch::RecordBatch;
-use pyo3::types::PyBytes;
-
-use std::io::BufReader;
-use std::sync::Arc;
+use std::{io::BufRead, sync::Arc};
 
+use arrow::{
+    array::GenericStringBuilder,
+    datatypes::{DataType, Field, Schema},
+    error::ArrowError,
+    record_batch::RecordBatch,
+};
 use noodles::fastq::Reader;
 
-struct FastqBatch {
+use crate::batch::BearRecordBatch;
+
+pub struct FastqBatch {
     names: GenericStringBuilder<i32>,
     descriptions: GenericStringBuilder<i32>,
     sequences: GenericStringBuilder<i32>,
     qualities: GenericStringBuilder<i32>,
-
-    schema: Schema,
 }
 
-impl FastqBatch {
-    fn new() -> Self {
-        let schema = Schema::new(vec![
+pub trait FastqSchemaTrait {
+    fn fastq_schema(&self) -> Schema {
+        Schema::new(vec![
             Field::new("name", DataType::Utf8, false),
             Field::new("description", DataType::Utf8, true),
             Field::new("sequence", DataType::Utf8, false),
             Field::new("quality", DataType::Utf8, false),
-        ]);
+        ])
+    }
+}
+
+impl FastqSchemaTrait for FastqBatch {}
 
+impl FastqBatch {
+    pub fn new() -> Self {
         Self {
             names: GenericStringBuilder::<i32>::new(),
             descriptions: GenericStringBuilder::<i32>::new(),
             sequences: GenericStringBuilder::<i32>::new(),
             qualities: GenericStringBuilder::<i32>::new(),
-            schema,
         }
     }
 
-    fn add(&mut self, record: noodles::fastq::Record) {
+    pub fn add(&mut self, record: noodles::fastq::Record) {
         let name = std::str::from_utf8(record.name()).unwrap();
         self.names.append_value(name);
 
         let desc = record.description();
         if desc.is_empty() {
             self.descriptions.append_null();
         } else {
@@ -54,107 +56,58 @@
         let sequence = std::str::from_utf8(record_sequence).unwrap();
         self.sequences.append_value(sequence);
 
         let record_quality = record.quality_scores().as_ref();
         let quality = std::str::from_utf8(record_quality).unwrap();
         self.qualities.append_value(quality);
     }
+}
 
+impl BearRecordBatch for FastqBatch {
     fn to_batch(&mut self) -> RecordBatch {
         let names = self.names.finish();
         let descriptions = self.descriptions.finish();
         let sequences = self.sequences.finish();
         let qualities = self.qualities.finish();
 
         RecordBatch::try_new(
-            Arc::new(self.schema.clone()),
+            Arc::new(self.fastq_schema()),
             vec![
                 Arc::new(names),
                 Arc::new(descriptions),
                 Arc::new(sequences),
                 Arc::new(qualities),
             ],
         )
         .unwrap()
     }
-
-    fn to_ipc(&mut self) -> Vec<u8> {
-        let batch = self.to_batch();
-
-        let mut ipc = Vec::new();
-        {
-            let mut writer = FileWriter::try_new(&mut ipc, &self.schema).unwrap();
-            writer.write(&batch).unwrap();
-
-            writer.finish().unwrap();
-        }
-        ipc
-    }
-}
-
-#[pyclass(name = "_FastqReader")]
-pub struct FastqReader {
-    reader: Reader<BufReader<std::fs::File>>,
-}
-
-#[pymethods]
-impl FastqReader {
-    #[new]
-    fn new(path: &str) -> PyResult<Self> {
-        let file = std::fs::File::open(path)?;
-        let reader = Reader::new(BufReader::new(file));
-
-        Ok(Self { reader })
-    }
-
-    pub fn read(&mut self) -> PyResult<PyObject> {
-        let mut batch = FastqBatch::new();
-
-        for record in self.reader.records() {
-            let record = record?;
-            batch.add(record);
-        }
-
-        let ipc = batch.to_ipc();
-        Ok(Python::with_gil(|py| PyBytes::new(py, &ipc).into()))
-    }
-
-    pub fn __enter__(slf: Py<Self>) -> Py<Self> {
-        slf
-    }
-
-    pub fn __exit__(&mut self, _exc_type: PyObject, _exc_value: PyObject, _traceback: PyObject) {}
 }
 
-#[pyclass(name = "_FastqGzippedReader")]
-pub struct FastqGzippedReader {
-    reader: Reader<BufReader<flate2::read::GzDecoder<std::fs::File>>>,
-}
-
-#[pymethods]
-impl FastqGzippedReader {
-    #[new]
-    fn new(path: &str) -> PyResult<Self> {
-        let file = std::fs::File::open(path)?;
-        let reader = Reader::new(BufReader::new(flate2::read::GzDecoder::new(file)));
-
-        Ok(Self { reader })
-    }
-
-    pub fn read(&mut self) -> PyResult<PyObject> {
-        let mut batch = FastqBatch::new();
-
-        for record in self.reader.records() {
-            let record = record?;
-            batch.add(record);
+pub fn add_next_fastq_record_to_batch<R: BufRead>(
+    reader: &mut Reader<R>,
+    n_records: usize,
+) -> Option<Result<RecordBatch, ArrowError>> {
+    let mut fastq_batch = FastqBatch::new();
+
+    for _ in 0..n_records {
+        let mut record = noodles::fastq::Record::default();
+        let record_read_result = reader.read_record(&mut record);
+
+        match record_read_result {
+            Ok(0) => {
+                let record_batch = fastq_batch.to_batch();
+
+                if record_batch.num_rows() == 0 {
+                    return None;
+                } else {
+                    return Some(Ok(record_batch));
+                }
+            }
+            Ok(_) => {
+                fastq_batch.add(record);
+            }
+            Err(e) => return Some(Err(ArrowError::ExternalError(Box::new(e)))),
         }
-
-        let ipc = batch.to_ipc();
-        Ok(Python::with_gil(|py| PyBytes::new(py, &ipc).into()))
-    }
-
-    pub fn __enter__(slf: Py<Self>) -> Py<Self> {
-        slf
     }
 
-    pub fn __exit__(&mut self, _exc_type: PyObject, _exc_value: PyObject, _traceback: PyObject) {}
+    Some(Ok(fastq_batch.to_batch()))
 }
```

### Comparing `biobear-0.2.0/src/gff_reader.rs` & `biobear-0.3.0/src/gff_reader/gff_batch.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,63 +1,65 @@
-use std::fs::File;
-use std::io::BufReader;
-use std::sync::Arc;
-use std::vec;
-
-use arrow::ipc::writer::FileWriter;
-use arrow::record_batch::RecordBatch;
-use pyo3::prelude::*;
-
-use arrow::array::*;
-use arrow::datatypes::*;
-use pyo3::types::PyBytes;
+use std::{io::BufRead, str::FromStr, sync::Arc};
 
-struct GFFBatch {
+use arrow::{
+    array::{Float32Builder, GenericStringBuilder, Int64Builder},
+    datatypes::{DataType, Field, Schema},
+    error::ArrowError,
+    record_batch::RecordBatch,
+};
+use noodles::gff::Line;
+
+use crate::batch::BearRecordBatch;
+
+pub trait GFFSchemaTrait {
+    fn gff_schema(&self) -> Schema {
+        Schema::new(vec![
+            Field::new("seqname", DataType::Utf8, false),
+            Field::new("source", DataType::Utf8, true),
+            Field::new("feature", DataType::Utf8, false),
+            Field::new("start", DataType::Int64, false),
+            Field::new("end", DataType::Int64, false),
+            Field::new("score", DataType::Float32, true),
+            Field::new("strand", DataType::Utf8, false),
+            Field::new("phase", DataType::Utf8, true),
+            Field::new("attributes", DataType::Utf8, true),
+        ])
+    }
+}
+
+pub struct GFFBatch {
     seqnames: GenericStringBuilder<i32>,
     sources: GenericStringBuilder<i32>,
     feature_types: GenericStringBuilder<i32>,
     starts: Int64Builder,
     ends: Int64Builder,
     scores: Float32Builder,
     strands: GenericStringBuilder<i32>,
     phases: GenericStringBuilder<i32>,
     attributes: GenericStringBuilder<i32>,
-
-    schema: Schema,
 }
 
-impl GFFBatch {
-    fn new() -> Self {
-        let file_schema = Schema::new(vec![
-            Field::new("seqname", DataType::Utf8, false),
-            Field::new("source", DataType::Utf8, true),
-            Field::new("feature", DataType::Utf8, false),
-            Field::new("start", DataType::Int64, false),
-            Field::new("end", DataType::Int64, false),
-            Field::new("score", DataType::Float32, true),
-            Field::new("strand", DataType::Utf8, false),
-            Field::new("phase", DataType::Utf8, true),
-            Field::new("attributes", DataType::Utf8, true),
-        ]);
+impl GFFSchemaTrait for GFFBatch {}
 
+impl GFFBatch {
+    pub fn new() -> Self {
         Self {
             seqnames: GenericStringBuilder::<i32>::new(),
             sources: GenericStringBuilder::<i32>::new(),
             feature_types: GenericStringBuilder::<i32>::new(),
             starts: Int64Builder::new(),
             ends: Int64Builder::new(),
             scores: Float32Builder::new(),
             strands: GenericStringBuilder::<i32>::new(),
             phases: GenericStringBuilder::<i32>::new(),
             attributes: GenericStringBuilder::<i32>::new(),
-            schema: file_schema,
         }
     }
 
-    fn add(&mut self, record: noodles::gff::Record) {
+    pub fn add(&mut self, record: noodles::gff::Record) {
         self.seqnames.append_value(record.reference_sequence_name());
         self.sources.append_value(record.source());
         self.feature_types.append_value(record.ty());
         self.starts.append_value(record.start().get() as i64);
         self.ends.append_value(record.end().get() as i64);
         self.scores.append_option(record.score());
         self.strands.append_value(record.strand().to_string());
@@ -71,87 +73,80 @@
             let mut attr_str = String::new();
             for entry in attrs.into_iter() {
                 attr_str.push_str(&format!("{}={};", entry.key(), entry.value()));
             }
             self.attributes.append_value(&attr_str);
         }
     }
+}
 
+impl BearRecordBatch for GFFBatch {
     fn to_batch(&mut self) -> RecordBatch {
         let seqnames = self.seqnames.finish();
         let sources = self.sources.finish();
         let feature_types = self.feature_types.finish();
         let starts = self.starts.finish();
         let ends = self.ends.finish();
         let scores = self.scores.finish();
         let strands = self.strands.finish();
         let phases = self.phases.finish();
         let attributes = self.attributes.finish();
 
         RecordBatch::try_new(
-            Arc::new(self.schema.clone()),
+            Arc::new(self.gff_schema()),
             vec![
                 Arc::new(seqnames),
                 Arc::new(sources),
                 Arc::new(feature_types),
                 Arc::new(starts),
                 Arc::new(ends),
                 Arc::new(scores),
                 Arc::new(strands),
                 Arc::new(phases),
                 Arc::new(attributes),
             ],
         )
         .unwrap()
     }
-
-    fn to_ipc(&mut self) -> Vec<u8> {
-        let batch = self.to_batch();
-
-        let mut ipc = Vec::new();
-        {
-            let mut writer = FileWriter::try_new(&mut ipc, &self.schema).unwrap();
-            writer.write(&batch).unwrap();
-
-            writer.finish().unwrap();
-        }
-        ipc
-    }
 }
 
-#[pyclass(name = "_GFFReader")]
-pub struct GFFReader {
-    reader: noodles::gff::Reader<BufReader<File>>,
-}
+pub fn add_next_gff_record_to_batch<R: BufRead>(
+    reader: &mut noodles::gff::Reader<R>,
+    n_records: Option<usize>,
+) -> Option<Result<RecordBatch, ArrowError>> {
+    let mut gff_batch = GFFBatch::new();
+    for _ in 0..n_records.unwrap_or(2048) {
+        let mut buffer = String::new();
+
+        match reader.read_line(&mut buffer) {
+            Ok(0) => {
+                let arrow_batch = gff_batch.to_batch();
 
-#[pymethods]
-impl GFFReader {
-    #[new]
-    fn new(path: &str) -> PyResult<Self> {
-        let file = File::open(path)?;
-        let reader = noodles::gff::Reader::new(BufReader::new(file));
+                if arrow_batch.num_rows() == 0 {
+                    return None;
+                }
 
-        Ok(Self { reader })
-    }
+                return Some(Ok(arrow_batch));
+            }
+            Ok(_) => {
+                let line_result = Line::from_str(&buffer);
 
-    fn read(&mut self) -> PyResult<PyObject> {
-        let mut batch = GFFBatch::new();
-        for record in self.reader.records() {
-            let record = match record {
-                Ok(record) => record,
-                Err(e) => {
-                    return Err(PyErr::new::<pyo3::exceptions::PyIOError, _>(format!(
-                        "Error reading record: {}",
-                        e
-                    )))
+                match line_result {
+                    Ok(line) => match line {
+                        Line::Record(record) => {
+                            gff_batch.add(record);
+                        }
+                        _ => {}
+                    },
+                    Err(e) => {
+                        return Some(Err(ArrowError::ExternalError(Box::new(
+                            std::io::Error::new(std::io::ErrorKind::InvalidData, e.to_string()),
+                        ))))
+                    }
                 }
-            };
-            batch.add(record);
+            }
+            Err(e) => return Some(Err(ArrowError::from(e))),
         }
-
-        let ipc = batch.to_ipc();
-        Ok(Python::with_gil(|py| {
-            let pybytes = PyBytes::new(py, &ipc);
-            pybytes.into()
-        }))
     }
+
+    Some(Ok(gff_batch.to_batch()))
 }
```

### Comparing `biobear-0.2.0/src/lib.rs` & `biobear-0.3.0/src/lib.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 use pyo3::prelude::*;
 
 mod bam_reader;
+mod batch;
 mod fasta_reader;
 mod fastq_reader;
 mod gff_reader;
+mod to_arrow;
 mod vcf_reader;
 
 #[pymodule]
 fn biobear(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<fasta_reader::FastaReader>()?;
     m.add_class::<fasta_reader::FastaGzippedReader>()?;
 
     m.add_class::<fastq_reader::FastqReader>()?;
     m.add_class::<fastq_reader::FastqGzippedReader>()?;
 
     m.add_class::<gff_reader::GFFReader>()?;
+    m.add_class::<gff_reader::GFFGzippedReader>()?;
+
     m.add_class::<bam_reader::BamReader>()?;
     m.add_class::<bam_reader::BamIndexedReader>()?;
+
     m.add_class::<vcf_reader::VCFReader>()?;
     m.add_class::<vcf_reader::VCFIndexedReader>()?;
+
     Ok(())
 }
```

### Comparing `biobear-0.2.0/Cargo.lock` & `biobear-0.3.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
  "arrow-ipc",
  "arrow-json",
  "arrow-ord",
  "arrow-row",
  "arrow-schema",
  "arrow-select",
  "arrow-string",
+ "pyo3",
 ]
 
 [[package]]
 name = "arrow-arith"
 version = "37.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8d967b42f7b12c91fd78acd396b20c2973b184c8866846674abbb00c963e93ab"
@@ -214,14 +215,17 @@
 ]
 
 [[package]]
 name = "arrow-schema"
 version = "37.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a16b88a93ac8350f0200b1cd336a1f887315925b8dd7aa145a37b8bdbd8497a4"
+dependencies = [
+ "bitflags 2.2.1",
+]
 
 [[package]]
 name = "arrow-select"
 version = "37.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98e8a4d6ca37d5212439b24caad4d80743fcbb706706200dd174bb98e68fe9d8"
 dependencies = [
@@ -251,15 +255,15 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "biobear"
-version = "0.2.0"
+version = "0.3.0"
 dependencies = [
  "arrow",
  "flate2",
  "noodles",
  "pyo3",
 ]
 
@@ -1189,17 +1193,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "termcolor"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
 dependencies = [
```

