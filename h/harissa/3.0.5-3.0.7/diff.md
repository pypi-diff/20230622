# Comparing `tmp/harissa-3.0.5.tar.gz` & `tmp/harissa-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/harissa-3.0.5.tar", last modified: Sun May 15 22:52:25 2022, max compression
+gzip compressed data, was "dist/harissa-3.0.7.tar", last modified: Thu Jun 22 12:18:24 2023, max compression
```

## Comparing `harissa-3.0.5.tar` & `harissa-3.0.7.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 ulysseherbach   (501) staff       (20)        0 2022-05-15 22:52:25.936645 harissa-3.0.5/
--rw-r--r--   0 ulysseherbach   (501) staff       (20)     1522 2021-10-07 18:35:09.000000 harissa-3.0.5/LICENSE.txt
--rw-r--r--   0 ulysseherbach   (501) staff       (20)     1124 2022-05-15 22:52:25.936086 harissa-3.0.5/PKG-INFO
--rw-r--r--   0 ulysseherbach   (501) staff       (20)      437 2021-10-11 13:25:49.000000 harissa-3.0.5/README.md
-drwxr-xr-x   0 ulysseherbach   (501) staff       (20)        0 2022-05-15 22:52:25.921108 harissa-3.0.5/harissa/
--rw-r--r--   0 ulysseherbach   (501) staff       (20)      688 2022-05-15 22:19:47.000000 harissa-3.0.5/harissa/__init__.py
-drwxr-xr-x   0 ulysseherbach   (501) staff       (20)        0 2022-05-15 22:52:25.926866 harissa-3.0.5/harissa/inference/
--rw-r--r--   0 ulysseherbach   (501) staff       (20)      198 2022-05-15 22:16:34.000000 harissa-3.0.5/harissa/inference/__init__.py
--rw-r--r--   0 ulysseherbach   (501) staff       (20)     3559 2021-02-06 16:20:02.000000 harissa-3.0.5/harissa/inference/kinetics.py
--rw-r--r--   0 ulysseherbach   (501) staff       (20)     4656 2022-05-15 22:11:45.000000 harissa-3.0.5/harissa/inference/network.py
--rw-r--r--   0 ulysseherbach   (501) staff       (20)     4732 2022-05-15 22:14:48.000000 harissa-3.0.5/harissa/inference/network_fast.py
-drwxr-xr-x   0 ulysseherbach   (501) staff       (20)        0 2022-05-15 22:52:25.930252 harissa-3.0.5/harissa/model/
--rw-r--r--   0 ulysseherbach   (501) staff       (20)      172 2021-02-06 16:20:02.000000 harissa-3.0.5/harissa/model/__init__.py
--rw-r--r--   0 ulysseherbach   (501) staff       (20)     7519 2022-05-15 22:24:16.000000 harissa-3.0.5/harissa/model/base.py
--rw-r--r--   0 ulysseherbach   (501) staff       (20)      457 2021-09-26 20:57:37.000000 harissa-3.0.5/harissa/model/cascade.py
--rw-r--r--   0 ulysseherbach   (501) staff       (20)     2319 2021-09-26 20:57:31.000000 harissa-3.0.5/harissa/model/tree.py
-drwxr-xr-x   0 ulysseherbach   (501) staff       (20)        0 2022-05-15 22:52:25.933927 harissa-3.0.5/harissa/simulation/
--rw-r--r--   0 ulysseherbach   (501) staff       (20)       80 2022-05-15 22:06:50.000000 harissa-3.0.5/harissa/simulation/__init__.py
--rw-r--r--   0 ulysseherbach   (501) staff       (20)      222 2021-09-26 20:58:40.000000 harissa-3.0.5/harissa/simulation/base.py
--rw-r--r--   0 ulysseherbach   (501) staff       (20)     3012 2021-09-26 20:59:11.000000 harissa-3.0.5/harissa/simulation/ode.py
--rw-rw-r--   0 ulysseherbach   (501) staff       (20)     4837 2022-02-03 00:20:36.000000 harissa-3.0.5/harissa/simulation/pdmp.py
--rw-r--r--   0 ulysseherbach   (501) staff       (20)     5478 2022-05-15 21:53:20.000000 harissa-3.0.5/harissa/simulation/pdmp_fast.py
-drwxr-xr-x   0 ulysseherbach   (501) staff       (20)        0 2022-05-15 22:52:25.935256 harissa-3.0.5/harissa/utils/
--rw-r--r--   0 ulysseherbach   (501) staff       (20)       80 2022-05-15 22:19:06.000000 harissa-3.0.5/harissa/utils/__init__.py
-drwxr-xr-x   0 ulysseherbach   (501) staff       (20)        0 2022-05-15 22:52:25.924320 harissa-3.0.5/harissa.egg-info/
--rw-r--r--   0 ulysseherbach   (501) staff       (20)     1124 2022-05-15 22:52:25.000000 harissa-3.0.5/harissa.egg-info/PKG-INFO
--rw-r--r--   0 ulysseherbach   (501) staff       (20)      591 2022-05-15 22:52:25.000000 harissa-3.0.5/harissa.egg-info/SOURCES.txt
--rw-r--r--   0 ulysseherbach   (501) staff       (20)        1 2022-05-15 22:52:25.000000 harissa-3.0.5/harissa.egg-info/dependency_links.txt
--rw-r--r--   0 ulysseherbach   (501) staff       (20)       18 2022-05-15 22:52:25.000000 harissa-3.0.5/harissa.egg-info/requires.txt
--rw-r--r--   0 ulysseherbach   (501) staff       (20)        8 2022-05-15 22:52:25.000000 harissa-3.0.5/harissa.egg-info/top_level.txt
--rw-r--r--   0 ulysseherbach   (501) staff       (20)       38 2022-05-15 22:52:25.936817 harissa-3.0.5/setup.cfg
--rw-r--r--   0 ulysseherbach   (501) staff       (20)     1008 2021-10-11 13:30:42.000000 harissa-3.0.5/setup.py
+drwxr-xr-x   0 ulysseherbach   (501) staff       (20)        0 2023-06-22 12:18:24.314793 harissa-3.0.7/
+-rw-r--r--   0 ulysseherbach   (501) staff       (20)     1522 2021-10-07 18:35:09.000000 harissa-3.0.7/LICENSE.txt
+-rw-r--r--   0 ulysseherbach   (501) staff       (20)     2783 2023-06-22 12:18:24.314359 harissa-3.0.7/PKG-INFO
+-rw-r--r--   0 ulysseherbach   (501) staff       (20)     2073 2023-05-14 19:59:03.000000 harissa-3.0.7/README.md
+drwxr-xr-x   0 ulysseherbach   (501) staff       (20)        0 2023-06-22 12:18:24.302509 harissa-3.0.7/harissa/
+-rw-r--r--   0 ulysseherbach   (501) staff       (20)      710 2023-05-24 07:41:40.000000 harissa-3.0.7/harissa/__init__.py
+drwxr-xr-x   0 ulysseherbach   (501) staff       (20)        0 2023-06-22 12:18:24.306781 harissa-3.0.7/harissa/inference/
+-rw-r--r--   0 ulysseherbach   (501) staff       (20)      198 2022-05-15 22:16:34.000000 harissa-3.0.7/harissa/inference/__init__.py
+-rw-r--r--   0 ulysseherbach   (501) staff       (20)     3559 2021-02-06 16:20:02.000000 harissa-3.0.7/harissa/inference/kinetics.py
+-rw-r--r--   0 ulysseherbach   (501) staff       (20)     4666 2023-04-28 17:08:09.000000 harissa-3.0.7/harissa/inference/network.py
+-rw-r--r--   0 ulysseherbach   (501) staff       (20)     4754 2023-04-28 17:09:38.000000 harissa-3.0.7/harissa/inference/network_fast.py
+drwxr-xr-x   0 ulysseherbach   (501) staff       (20)        0 2023-06-22 12:18:24.308855 harissa-3.0.7/harissa/model/
+-rw-r--r--   0 ulysseherbach   (501) staff       (20)      172 2021-02-06 16:20:02.000000 harissa-3.0.7/harissa/model/__init__.py
+-rw-r--r--   0 ulysseherbach   (501) staff       (20)     7027 2023-04-30 17:38:03.000000 harissa-3.0.7/harissa/model/base.py
+-rw-r--r--   0 ulysseherbach   (501) staff       (20)      457 2021-09-26 20:57:37.000000 harissa-3.0.7/harissa/model/cascade.py
+-rw-r--r--   0 ulysseherbach   (501) staff       (20)     2416 2023-04-29 16:10:38.000000 harissa-3.0.7/harissa/model/tree.py
+drwxr-xr-x   0 ulysseherbach   (501) staff       (20)        0 2023-06-22 12:18:24.311702 harissa-3.0.7/harissa/simulation/
+-rw-r--r--   0 ulysseherbach   (501) staff       (20)       80 2022-05-15 22:06:50.000000 harissa-3.0.7/harissa/simulation/__init__.py
+-rw-r--r--   0 ulysseherbach   (501) staff       (20)      223 2023-04-29 12:24:38.000000 harissa-3.0.7/harissa/simulation/base.py
+-rw-r--r--   0 ulysseherbach   (501) staff       (20)     3004 2023-04-29 14:28:28.000000 harissa-3.0.7/harissa/simulation/ode.py
+-rw-rw-r--   0 ulysseherbach   (501) staff       (20)     4837 2022-02-03 00:20:36.000000 harissa-3.0.7/harissa/simulation/pdmp.py
+-rw-r--r--   0 ulysseherbach   (501) staff       (20)     5478 2022-05-15 21:53:20.000000 harissa-3.0.7/harissa/simulation/pdmp_fast.py
+drwxr-xr-x   0 ulysseherbach   (501) staff       (20)        0 2023-06-22 12:18:24.313686 harissa-3.0.7/harissa/utils/
+-rw-r--r--   0 ulysseherbach   (501) staff       (20)      200 2023-04-29 18:49:47.000000 harissa-3.0.7/harissa/utils/__init__.py
+-rw-r--r--   0 ulysseherbach   (501) staff       (20)     8798 2023-04-30 19:45:21.000000 harissa-3.0.7/harissa/utils/plot_network.py
+-rw-r--r--   0 ulysseherbach   (501) staff       (20)      617 2023-04-29 19:14:09.000000 harissa-3.0.7/harissa/utils/processing.py
+drwxr-xr-x   0 ulysseherbach   (501) staff       (20)        0 2023-06-22 12:18:24.304986 harissa-3.0.7/harissa.egg-info/
+-rw-r--r--   0 ulysseherbach   (501) staff       (20)     2783 2023-06-22 12:18:24.000000 harissa-3.0.7/harissa.egg-info/PKG-INFO
+-rw-r--r--   0 ulysseherbach   (501) staff       (20)      649 2023-06-22 12:18:24.000000 harissa-3.0.7/harissa.egg-info/SOURCES.txt
+-rw-r--r--   0 ulysseherbach   (501) staff       (20)        1 2023-06-22 12:18:24.000000 harissa-3.0.7/harissa.egg-info/dependency_links.txt
+-rw-r--r--   0 ulysseherbach   (501) staff       (20)       65 2023-06-22 12:18:24.000000 harissa-3.0.7/harissa.egg-info/requires.txt
+-rw-r--r--   0 ulysseherbach   (501) staff       (20)        8 2023-06-22 12:18:24.000000 harissa-3.0.7/harissa.egg-info/top_level.txt
+-rw-r--r--   0 ulysseherbach   (501) staff       (20)       38 2023-06-22 12:18:24.314977 harissa-3.0.7/setup.cfg
+-rw-r--r--   0 ulysseherbach   (501) staff       (20)     1132 2023-06-22 12:16:44.000000 harissa-3.0.7/setup.py
```

### Comparing `harissa-3.0.5/LICENSE.txt` & `harissa-3.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `harissa-3.0.5/harissa/inference/kinetics.py` & `harissa-3.0.7/harissa/inference/kinetics.py`

 * *Files identical despite different names*

### Comparing `harissa-3.0.5/harissa/inference/network.py` & `harissa-3.0.7/harissa/inference/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,17 @@
     dq[1:,0] += np.sum(u, axis=0)
     # Interaction parameters
     dq[:,1:] += y.T @ u
     dq = l*grad_penalization(theta, theta0, t) - dq/C
     return dq.reshape(G**2)
 
 def infer_proteins(x, a):
-    """Estimate y directly from data."""
+    """
+    Estimate y directly from data.
+    """
     C, G = x.shape
     y = np.ones((C,G))
     z = np.ones((2,G))
     z[0] = a[0]/a[1]
     z[z<1e-5] = 1e-5
     az = a[1]*z
     for k in range(C):
```

### Comparing `harissa-3.0.5/harissa/inference/network_fast.py` & `harissa-3.0.7/harissa/inference/network_fast.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Core functions for network inference using likelihood maximization
-NB: Fast version using Numba
+NB: This is the fast version using Numba
 """
 import numpy as np
 from numpy import log
 from scipy.special import expit, gammaln, psi
 from scipy.optimize import minimize
 from numba import njit
 
@@ -107,15 +107,17 @@
     dq[1:,0] += np.sum(u, axis=0)
     # Interaction parameters
     dq[:,1:] += y.T @ u
     dq = l*grad_penalization(theta, theta0, t) - dq/C
     return dq.reshape(G**2)
 
 def infer_proteins(x, a):
-    """Estimate y directly from data."""
+    """
+    Estimate y directly from data.
+    """
     C, G = x.shape
     y = np.ones((C,G))
     z = np.ones((2,G))
     z[0] = a[0]/a[1]
     z[z<1e-5] = 1e-5
     az = a[1]*z
     for k in range(C):
```

### Comparing `harissa-3.0.5/harissa/model/base.py` & `harissa-3.0.7/harissa/model/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,17 +29,17 @@
             self.d = np.zeros((2,G))
             self.d[0] = np.log(2)/9 # mRNA degradation rates (per hour)
             self.d[1] = np.log(2)/46 # protein degradation rates (per hour)
             # Default network parameters
             self.basal = np.zeros(G)
             self.inter = np.zeros((G,G))
 
-    def get_kinetics(self, data, verb):
+    def get_kinetics(self, data, verb=False):
         """
-        Compute the basal parameters of filtered genes.
+        Compute the basal parameters of all genes.
         """
         times = data[:,0]
         G = data[0].size
         # Kinetic values for each gene
         a = np.ones((3,G))
         for g in range(1,G):
             if verb: print(f'Calibrating gene {g}...')
@@ -49,15 +49,14 @@
             a[1,g] = np.max(at)
             a[2,g] = b
         self.a = a
 
     def fit(self, data, l=1, tol=1e-5, verb=False, use_numba=True):
         """
         Fit the network model to the data.
-        Return the list of successive objective function values.
         """
         x = data
         # Time points
         times = np.sort(list(set(x[:,0])))
         self.times = times
         # Default degradation rates
         C, G = x.shape
@@ -118,67 +117,52 @@
         # Activate the stimulus
         network.state['P'][0] = 1
         # Final simulation with stimulus
         sim = network.simulation(t, verb)
         m, p = sim['M'], sim['P']
         return Simulation(t, m, p)
 
-    def simulate_ode(self, t, burnin=None, verb=False):
+    def simulate_ode(self, t, M0=None, P0=None, burnin=None, verb=False):
         """
         Perform simulation of the network model (ODE version).
+        This is the slow-fast limit of the PDMP model, which is only
+        relevant when promoters & mRNA are much faster than proteins.
+        p: solution of a nonlinear ODE system involving proteins only
+        m: mean mRNA levels given protein levels (quasi-steady state)
         """
         # Check parameters
         check = ((self.a is None) + (self.d is None)
                 + (self.basal is None) + (self.inter is None))
         # Prepare time points
         if check: raise ValueError('Model parameters not specified yet')
         if self.inter is None: print('Interactions must be specified')
         if np.size(t) == 1: t = np.array([t])
         if np.any(t != np.sort(t)):
             raise ValueError('Time points must appear in increasing order')
-        if self.genes is None:
-            raise ValueError('genes not yet provided')
         # Import necessary modules
         from ..simulation.base import Simulation
         from ..simulation.ode import ApproxODE
-        v = [0] + self.genes
-        # Case 1 (no filtering): all genes are simulated
-        if self.filter is None:
-            a = self.a
-            d = self.d
-            basal = self.basal
-            inter = self.inter
-        # Case 2 (filtering): only filtered genes are simulated
-        else:
-            G = len(v)
-            a = np.zeros((3,G))
-            d = np.zeros((2,G))
-            basal = np.zeros(G)
-            inter = np.zeros((G,G))
-            for i in range(G):
-                a[0,i] = self.a[0,v[i]]
-                a[1,i] = self.a[1,v[i]]
-                a[2,i] = self.a[2,v[i]]
-                d[0,i] = self.d[0,v[i]]
-                d[1,i] = self.d[1,v[i]]
-                basal[i] = self.basal[v[i]]
-                for j in range(G):
-                    inter[i,j] = self.inter[v[i],v[j]]
+        a = self.a
+        d = self.d
+        basal = self.basal
+        inter = self.inter
         network = ApproxODE(a, d, basal, inter)
         # Burnin simulation without stimulus
-        if burnin is not None:
-            network.simulation([burnin], verb=verb)
+        if M0 is not None: network.state['M'][1:] = M0[1:]
+        if P0 is not None: network.state['P'][1:] = P0[1:]
+        if burnin is not None: network.simulation([burnin], verb)
         # Activate the stimulus
         network.state['P'][0] = 1
         # Final simulation with stimulus
-        sim = network.simulation(t, verb=verb)
+        sim = network.simulation(t, verb)
         m, p = sim['M'], sim['P']
-        return Simulation(self.genes, t, m, p)
+        return Simulation(t, m, p)
+
+#### Classes for simulations ####
 
-# Classes for simulations
 class Cascade(NetworkModel):
     """
     Particular network with a cascade structure.
     """
     def __init__(self, n_genes, autoactiv=False):
         # Get NetworkModel default features
         NetworkModel.__init__(self, n_genes)
```

### Comparing `harissa-3.0.5/harissa/model/tree.py` & `harissa-3.0.7/harissa/model/tree.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,15 +45,16 @@
     for i in range(n): tree[i].sort()
     return tuple([tuple(tree[i]) for i in range(n)])
 
 # Main function
 def tree(n_genes, weight=None):
     """
     Generate a random tree-like network model.
-    Note: weight[i,j] is the probability weight of link (i) -> (j).
+    A tree with root 0 is sampled from the ‘weighted-uniform’ distribution,
+    where weight[i,j] is the probability weight of link (i) -> (j).
     """
     G = n_genes + 1
     if weight is not None:
         if weight.shape != (G,G):
             raise ValueError('Weight must be n_genes+1 by n_genes+1')
     else: weight = np.ones((G,G))
     # Enforcing the proper structure
@@ -69,8 +70,9 @@
             inter[i,j] = 10
     return basal, inter
 
 
 # Tests
 if __name__ == '__main__':
     basal, inter = tree(5)
+    print(basal)
     print(inter)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `harissa-3.0.5/harissa/simulation/ode.py` & `harissa-3.0.7/harissa/simulation/ode.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Perform simulations using the ODE model
 """
 import numpy as np
+from scipy.special import expit
 
 class ApproxODE:
     """
     ODE version of the network model (very rough approximation of the PDMP)
     """
     def __init__(self, a, d, basal, inter):
         # Kinetic parameters
@@ -20,55 +21,53 @@
         # Network parameters
         self.basal = basal
         self.inter = inter
         # Default state
         types = [('M','float'), ('P','float')]
         self.state = np.array([(0,0) for i in range(G)], dtype=types)
         # Simulation parameter
-        d0, d1, s1 = np.max(D0), np.max(D1), np.max(S1)
-        k0, k1, b = np.max(K0), np.max(K1), np.max(B)
-        self.euler_step = 0.01/np.max([d0, d1, s1, k0, k1, b])
+        self.euler_step = 1e-3/np.max(D1)
 
     def kon(self, p):
         """
         Interaction function kon (off->on rate), given protein levels p.
         """
-        Phi = np.exp(self.basal + p @ self.inter)
         K0, K1 = self.param['K0'], self.param['K1']
-        Kon = (K0 + K1*Phi)/(1 + Phi)
+        sigma = expit(self.basal + p @ self.inter)
+        Kon = (1-sigma)*K0 + sigma*K1
         Kon[0] = 0 # Ignore stimulus
         return Kon
 
     def step_ode(self, dt):
         """
         Euler step for the deterministic limit model.
         """
         M, P = self.state['M'], self.state['P']
         D0, D1, S1 = self.param['D0'], self.param['D1'], self.param['S1']
-        a, b = self.kon(P), self.param['B']
-        Mnew = (1 - dt*D0)*M + dt*a/b
-        Pnew = (1 - dt*D1)*P + dt*S1*M
+        a, b = self.kon(P)/D0, self.param['B'] # a = kon/d0, b = koff/s0
+        Mnew = a/b # Mean level of mRNA given protein levels
+        Pnew = (1 - dt*D1)*P + dt*S1*Mnew # Protein-only ODE system
         Mnew[0], Pnew[0] = M[0], P[0] # Discard stimulus
         self.state['M'], self.state['P'] = Mnew, Pnew
 
     def simulation(self, timepoints, verb=False):
         """
         Simulation of the deterministic limit model, which is relevant when
-        promoters/RNA are much faster than proteins.
-        1. ODE system involving proteins only
+        promoters and mRNA are much faster than proteins.
+        1. Nonlinear ODE system involving proteins only
         2. Mean level of mRNA given protein levels
         """
         G = self.basal.size
         dt = self.euler_step
         if np.size(timepoints) > 1:
             dt = np.min([dt, np.min(timepoints[1:] - timepoints[:-1])])
         types = [('M','float64'), ('P','float64')]
         sim = []
         T, c = 0, 0
-        ### The core loop for simulation and recording
+        # Core loop for simulation and recording
         for t in timepoints:
             while T < t:
                 self.step_ode(dt)
                 T += dt
                 c += 1
             M, P = self.state['M'], self.state['P']
             sim += [np.array([(M[i],P[i]) for i in range(1,G)], dtype=types)]
```

### Comparing `harissa-3.0.5/harissa/simulation/pdmp.py` & `harissa-3.0.7/harissa/simulation/pdmp.py`

 * *Files identical despite different names*

### Comparing `harissa-3.0.5/harissa/simulation/pdmp_fast.py` & `harissa-3.0.7/harissa/simulation/pdmp_fast.py`

 * *Files identical despite different names*

### Comparing `harissa-3.0.5/harissa.egg-info/SOURCES.txt` & `harissa-3.0.7/harissa.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,8 +16,10 @@
 harissa/model/cascade.py
 harissa/model/tree.py
 harissa/simulation/__init__.py
 harissa/simulation/base.py
 harissa/simulation/ode.py
 harissa/simulation/pdmp.py
 harissa/simulation/pdmp_fast.py
-harissa/utils/__init__.py
+harissa/utils/__init__.py
+harissa/utils/plot_network.py
+harissa/utils/processing.py
```

### Comparing `harissa-3.0.5/setup.py` & `harissa-3.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 from setuptools import setup, find_packages
 import harissa
 
 setup(
 
     name='harissa',
- 
+
     version=harissa.__version__,
- 
+
     packages=find_packages(),
- 
+
     author='Ulysse Herbach',
- 
+
     author_email='ulysse.herbach@inria.fr',
- 
+
     description=('Tools for mechanistic gene network inference '
         'from single-cell data'),
- 
+
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
 
-    install_requires=['numpy', 'scipy', 'numba'],
- 
     url='https://github.com/ulysseherbach/harissa',
 
     classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
@@ -34,8 +32,19 @@
     platforms='any',
 
     license='BSD-3-Clause',
     license_file='LICENSE.txt',
 
     keywords=('stochastic gene expression, gene regulatory networks, '
         'single-cell transcriptomics'),
+
+    python_requires='>=3.8',
+
+    install_requires=[
+        'numpy>=1.20',
+        'scipy>=1.7',
+        'numba>=0.55',
+        'matplotlib>=3.4',
+        'networkx>=2.6',
+    ],
+
 )
```

