# Comparing `tmp/CUQIpy-FEniCS-0.3.0.tar.gz` & `tmp/CUQIpy-FEniCS-0.3.0.post0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CUQIpy-FEniCS-0.3.0.tar", last modified: Wed Feb 22 09:55:08 2023, max compression
+gzip compressed data, was "CUQIpy-FEniCS-0.3.0.post0.dev5.tar", last modified: Thu Apr 27 13:30:34 2023, max compression
```

## Comparing `CUQIpy-FEniCS-0.3.0.tar` & `CUQIpy-FEniCS-0.3.0.post0.dev5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:55:08.186332 CUQIpy-FEniCS-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:55:08.186332 CUQIpy-FEniCS-0.3.0/CUQIpy_FEniCS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42467 2023-02-22 09:55:08.000000 CUQIpy-FEniCS-0.3.0/CUQIpy_FEniCS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-02-22 09:55:08.000000 CUQIpy-FEniCS-0.3.0/CUQIpy_FEniCS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 09:55:08.000000 CUQIpy-FEniCS-0.3.0/CUQIpy_FEniCS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 09:55:08.000000 CUQIpy-FEniCS-0.3.0/CUQIpy_FEniCS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-22 09:55:08.000000 CUQIpy-FEniCS-0.3.0/CUQIpy_FEniCS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-22 09:54:59.000000 CUQIpy-FEniCS-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42467 2023-02-22 09:55:08.186332 CUQIpy-FEniCS-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-02-22 09:54:59.000000 CUQIpy-FEniCS-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:55:08.186332 CUQIpy-FEniCS-0.3.0/cuqipy_fenics/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-02-22 09:54:59.000000 CUQIpy-FEniCS-0.3.0/cuqipy_fenics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-22 09:55:08.186332 CUQIpy-FEniCS-0.3.0/cuqipy_fenics/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11291 2023-02-22 09:54:59.000000 CUQIpy-FEniCS-0.3.0/cuqipy_fenics/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    18227 2023-02-22 09:54:59.000000 CUQIpy-FEniCS-0.3.0/cuqipy_fenics/pde.py
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-02-22 09:54:59.000000 CUQIpy-FEniCS-0.3.0/cuqipy_fenics/testproblem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-02-22 09:54:59.000000 CUQIpy-FEniCS-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-02-22 09:54:59.000000 CUQIpy-FEniCS-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 09:55:08.186332 CUQIpy-FEniCS-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-02-22 09:54:59.000000 CUQIpy-FEniCS-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:55:08.186332 CUQIpy-FEniCS-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13496 2023-02-22 09:54:59.000000 CUQIpy-FEniCS-0.3.0/tests/test_PDEModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-02-22 09:54:59.000000 CUQIpy-FEniCS-0.3.0/tests/test_geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:34.167682 CUQIpy-FEniCS-0.3.0.post0.dev5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:34.167682 CUQIpy-FEniCS-0.3.0.post0.dev5/CUQIpy_FEniCS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42478 2023-04-27 13:30:34.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/CUQIpy_FEniCS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-27 13:30:34.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/CUQIpy_FEniCS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:30:34.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/CUQIpy_FEniCS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 13:30:34.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/CUQIpy_FEniCS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 13:30:34.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/CUQIpy_FEniCS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 13:30:24.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42478 2023-04-27 13:30:34.167682 CUQIpy-FEniCS-0.3.0.post0.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-27 13:30:24.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:34.167682 CUQIpy-FEniCS-0.3.0.post0.dev5/cuqipy_fenics/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-27 13:30:24.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/cuqipy_fenics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-27 13:30:34.167682 CUQIpy-FEniCS-0.3.0.post0.dev5/cuqipy_fenics/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-04-27 13:30:24.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/cuqipy_fenics/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18227 2023-04-27 13:30:24.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/cuqipy_fenics/pde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-04-27 13:30:24.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/cuqipy_fenics/testproblem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-27 13:30:24.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-27 13:30:24.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 13:30:34.167682 CUQIpy-FEniCS-0.3.0.post0.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-27 13:30:24.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:34.167682 CUQIpy-FEniCS-0.3.0.post0.dev5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13498 2023-04-27 13:30:24.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/tests/test_PDEModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-27 13:30:24.000000 CUQIpy-FEniCS-0.3.0.post0.dev5/tests/test_geometry.py
```

### Comparing `CUQIpy-FEniCS-0.3.0/CUQIpy_FEniCS.egg-info/PKG-INFO` & `CUQIpy-FEniCS-0.3.0.post0.dev5/CUQIpy_FEniCS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CUQIpy-FEniCS
-Version: 0.3.0
+Version: 0.3.0.post0.dev5
 Summary: CUQIpy plugin for FEniCS
 Maintainer-email: "Nicolai A. B. Riis" <nabr@dtu.dk>, "Jakob S. Jørgensen" <jakj@dtu.dk>, "Amal M. Alghamdi" <amaal@dtu.dk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `CUQIpy-FEniCS-0.3.0/LICENSE` & `CUQIpy-FEniCS-0.3.0.post0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `CUQIpy-FEniCS-0.3.0/PKG-INFO` & `CUQIpy-FEniCS-0.3.0.post0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CUQIpy-FEniCS
-Version: 0.3.0
+Version: 0.3.0.post0.dev5
 Summary: CUQIpy plugin for FEniCS
 Maintainer-email: "Nicolai A. B. Riis" <nabr@dtu.dk>, "Jakob S. Jørgensen" <jakj@dtu.dk>, "Amal M. Alghamdi" <amaal@dtu.dk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `CUQIpy-FEniCS-0.3.0/README.md` & `CUQIpy-FEniCS-0.3.0.post0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `CUQIpy-FEniCS-0.3.0/cuqipy_fenics/geometry.py` & `CUQIpy-FEniCS-0.3.0.post0.dev5/cuqipy_fenics/geometry.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import matplotlib.pyplot as plt
 import dolfin as dl
 import ufl
 
 __all__ = [
     'FEniCSContinuous',
     'FEniCSMappedGeometry',
-    'MaternExpansion'
+    'MaternKLExpansion'
 ]
 
 class FEniCSContinuous(Geometry):
 
     def __init__(self, function_space, labels = ['x', 'y']):
         self.function_space = function_space
         if self.physical_dim >2:
@@ -125,68 +125,79 @@
         else:
             return mapped_value_list
     
     def fun2par(self,f):
         raise NotImplementedError
 
 
-class MaternExpansion(_WrappedGeometry):
-    """A geometry class that builds spectral representation of Matern covariance operator on the given input geometry. We create the representation using the stochastic partial differential operator, equation (15) in (Roininen, Huttunen and Lasanen, 2014). Zero Neumann boundary conditions are assumed for the stochastic partial differential equation (SPDE) and the smoothness parameter :math:`\\nu` is set to 1. To generate Matern field realizations, the method :meth:`par2field` is used. The input `p` of this method need to be an `n=dim` i.i.d random variables that follow a normal distribution. 
+class MaternKLExpansion(_WrappedGeometry):
+    """A geometry class that builds spectral representation of Matern covariance operator on the given input geometry. We create the representation using the stochastic partial differential operator, equation (15) in (Roininen, Huttunen and Lasanen, 2014). Zero Neumann boundary conditions are assumed for the stochastic partial differential equation (SPDE) and the default value of the smoothness parameter :math:`\\nu` is set to 0.5. To generate Matern field realizations, the method :meth:`par2field` is used. The input `p` of this method need to be an `n=dim` i.i.d random variables that follow a normal distribution. 
 
     For more details about the formulation of the SPDE see: Roininen, L., Huttunen, J. M., & Lasanen, S. (2014). Whittle-Matérn priors for Bayesian statistical inversion with applications in electrical impedance tomography. Inverse Problems & Imaging, 8(2), 561.
 
     Parameters
     -----------
     geometry : cuqi.fenics.geometry.Geometry
         An input geometry on which the Matern field representation is built (the geometry must have a mesh attribute)
 
     length_scale : float
-        Length scale paramater (controls correlation length)
+        Length scale parameter (controls correlation length)
 
     num_terms: int
-        Number of expantion terms to represent the Matern field realization
+        Number of expansion terms to represent the Matern field realization
+
+    nu : float, default 0.5 
+        Smoothness parameter of the Matern field, must be greater then
+        zero.
 
     boundary_conditions : str
         Boundary conditions for the SPDE. Currently 'Neumann' for zero flux, and 'zero' for zero Dirichlet boundary conditions are supported.
 
     normalize : bool, default True
         If True, the Matern field expansion modes are normalized to have a unit norm.
 
     Example
     -------
     .. code-block:: python
 
         import numpy as np
         import matplotlib.pyplot as plt
-        from cuqi.fenics.geometry import MaternExpansion, FEniCSContinuous
+        from cuqi.fenics.geometry import MaternKLExpansion, FEniCSContinuous
         from cuqi.distribution import Gaussian
         import dolfin as dl
         
         mesh = dl.UnitSquareMesh(20,20)
         V = dl.FunctionSpace(mesh, 'CG', 1)
         geometry = FEniCSContinuous(V)
-        MaternGeometry = MaternExpansion(geometry, 
+        MaternGeometry = MaternKLExpansion(geometry, 
                                         length_scale = .2,
                                         num_terms=128)
         
         MaternField = Gaussian(mean=np.zeros(MaternGeometry.dim),
                         cov=np.eye(MaternGeometry.dim),
                         geometry= MaternGeometry)
         
         samples = MaternField.sample()
         samples.plot()
 
     """
 
-    def __init__(self, geometry, length_scale, num_terms, boundary_conditions='Neumann', normalize=True): 
+    def __init__(self, geometry, length_scale, num_terms, nu=0.5, boundary_conditions='Neumann', normalize=True): 
+
+        if nu <= 0:
+            raise ValueError("Smoothness parameter nu must be positive")
+        
+        if not isinstance(geometry, (FEniCSMappedGeometry, FEniCSContinuous)):
+            raise ValueError("Matern KL expansion is only implemented "+ 
+                             "for cuqipy_fenics geometries")
         super().__init__(geometry)
         if not hasattr(geometry, 'mesh'):
             raise NotImplementedError
         self._length_scale = length_scale
-        self._nu = 1
+        self._nu = nu
         self._num_terms = num_terms
         self._eig_val = None
         self._eig_vec = None
         self._boundary_conditions = boundary_conditions
         self._normalize = normalize
 
     @property
@@ -216,15 +227,19 @@
     @property
     def boundary_conditions(self):
         return self._boundary_conditions
 
     @property
     def normalize(self):
         return self._normalize
-
+    
+    @property
+    def physical_dim(self):
+        """Returns the physical dimension of the geometry, e.g. 1, 2 or 3"""
+        return self.geometry.physical_dim
 
     def __repr__(self) -> str:
         return "{} on {}".format(self.__class__.__name__,self.geometry.__repr__())
 
     def par2fun(self,p):
         return self.geometry.par2fun(self.par2field(p))
 
@@ -241,16 +256,22 @@
         if self._eig_vec is None and self._eig_val is None:
             self._build_basis() 
 	   
         p = self._process_values(p)
         Ns = p.shape[-1]
         field_list = np.empty((self.geometry.par_dim,Ns))
 
+        nu = self.nu
+        d = self.physical_dim
         for idx in range(Ns):
-            field_list[:,idx] = self.eig_vec@( np.sqrt(self.eig_val)*p[...,idx] )
+            # For more details about the formulation below, see section 4.3 in
+            # Chen, V., Dunlop, M. M., Papaspiliopoulos, O., & Stuart, A. M.
+            # (2018). Dimension-robust MCMC in Bayesian inverse problems.
+            # arXiv preprint arXiv:1803.03344.
+            field_list[:,idx] = self.eig_vec@( self.eig_val**((nu+d/2)/2)*p[...,idx] )
 
         if len(field_list) == 1:
             return field_list[0]
         else:
             return field_list
 
     def _build_basis(self):
```

### Comparing `CUQIpy-FEniCS-0.3.0/cuqipy_fenics/pde.py` & `CUQIpy-FEniCS-0.3.0.post0.dev5/cuqipy_fenics/pde.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-FEniCS-0.3.0/cuqipy_fenics/testproblem.py` & `CUQIpy-FEniCS-0.3.0.post0.dev5/cuqipy_fenics/testproblem.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-FEniCS-0.3.0/pyproject.toml` & `CUQIpy-FEniCS-0.3.0.post0.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `CUQIpy-FEniCS-0.3.0/tests/test_PDEModel.py` & `CUQIpy-FEniCS-0.3.0.post0.dev5/tests/test_PDEModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
         dirichlet_bc=poisson2.bc,
         observation_operator=None,
         reuse_assembled=False)
 
     # Create domain geometry
     fenics_continuous_geo = cuqipy_fenics.geometry.FEniCSContinuous(
         poisson1.parameter_function_space)
-    domain_geometry = cuqipy_fenics.geometry.MaternExpansion(
+    domain_geometry = cuqipy_fenics.geometry.MaternKLExpansion(
         fenics_continuous_geo, length_scale=.1, num_terms=5)
 
     # Create range geometry
     range_geometry = cuqipy_fenics.geometry.FEniCSContinuous(
         poisson1.solution_function_space)
 
     # Create cuqi forward model (two models corresponding to two PDE objects)
```

### Comparing `CUQIpy-FEniCS-0.3.0/tests/test_geometry.py` & `CUQIpy-FEniCS-0.3.0.post0.dev5/tests/test_geometry.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 import dolfin as dl
-import cuqipy_fenics
+from cuqipy_fenics.geometry import FEniCSContinuous, MaternKLExpansion
 import numpy as np
+import pytest
 
-def test_MaternExpansion():
-    """Test creating a MaternExpansion geometry"""
-    mesh = dl.UnitSquareMesh(20,20)
+
+def test_MaternKLExpansion():
+    """Test creating a MaternKLExpansion geometry"""
+    mesh = dl.UnitSquareMesh(20, 20)
     V = dl.FunctionSpace(mesh, 'CG', 1)
-    geometry = cuqipy_fenics.geometry.FEniCSContinuous(V)
-    MaternGeometry = cuqipy_fenics.geometry.MaternExpansion(geometry, 
-                                    length_scale = .2,
-                                    num_terms=128)
-    assert(MaternGeometry.num_terms == 128 and np.isclose(MaternGeometry.length_scale, .2))
+    geometry = FEniCSContinuous(V)
+    MaternGeometry = MaternKLExpansion(geometry,
+                                     length_scale=.2,
+                                     num_terms=128)
+    assert (MaternGeometry.num_terms == 128 and np.isclose(
+        MaternGeometry.length_scale, .2))
 
 
-def test_MaternExpansion_basis(copy_reference):
-    """Test MaternExpansion geometry basis building"""
+def test_MaternKLExpansion_basis(copy_reference):
+    """Test MaternKLExpansion geometry basis building"""
 
-    # Create the MaternExpansion geometry
+    # Create the MaternKLExpansion geometry
     np.random.seed(0)
     mesh = dl.UnitSquareMesh(20, 20)
     V = dl.FunctionSpace(mesh, 'CG', 1)
-    geometry = cuqipy_fenics.geometry.FEniCSContinuous(V)
-    MaternGeometry = cuqipy_fenics.geometry.MaternExpansion(geometry,
-                                                            length_scale=.2,
-                                                            num_terms=128,
-                                                            normalize=False)
+    geometry = FEniCSContinuous(V)
+    MaternGeometry = MaternKLExpansion(geometry,
+                                     length_scale=.2,
+                                     num_terms=128,
+                                     normalize=False)
 
     # Build the basis
     MaternGeometry._build_basis()
 
     # Read the reference eigenvalues and eigenvectors
     samples_orig_file = copy_reference("data/MaternExpansion_basis.npz")
     expected_eig_pairs = np.load(samples_orig_file)
@@ -41,7 +44,28 @@
     # Assert that the eigenvectors match the reference, up to sign
     for i in range(MaternGeometry.num_terms):
         assert (np.allclose(MaternGeometry.eig_vec[:, i], expected_eig_vec[:, i]) or np.allclose(
             MaternGeometry.eig_vec[:, i], -expected_eig_vec[:, i]))
 
     # Assert that the eigenvectors has the correct shape
     assert expected_eig_vec.shape == (441, 128)
+
+
+@pytest.mark.parametrize("nu, valid",
+                         [(0, False), (0.01, True), (-1, False)])
+def test_MaternKLExpansion_nu(nu, valid):
+    """Test passing nu to the MaternKLExpansion geometry"""
+    mesh = dl.UnitSquareMesh(20, 20)
+    V = dl.FunctionSpace(mesh, 'CG', 1)
+    geometry = FEniCSContinuous(V)
+
+    if valid:
+        MaternGeometry = MaternKLExpansion(geometry,
+                                         length_scale=0.2,
+                                         nu=nu,
+                                         num_terms=128)
+    else:
+        with pytest.raises(ValueError):
+            MaternGeometry = MaternKLExpansion(geometry,
+                                             length_scale=0.2,
+                                             nu=nu,
+                                             num_terms=128)
```

