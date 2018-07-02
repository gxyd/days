Day 1
=====

start time: 1:02 PM

AI \supset ML \supset \DL.

* At its core, *ML is a simple way of achieving AI*.
* ML is currently the most successful approach to AI.

*Deep learning is one of the approaches to Machine learning*. Other approaches include decision tree learning, inductive logic programming, clustering, reinforcement learning and Bayesian networks, among others.

Deep learning was inspired by the structure and function of the brain, namely the interconnecting of many neurons. ANN's are algorithms that mimic the biological structure of the brain.

In ANN's, there are neurons which have discrete layers and connections to other neurons. Depth is created by using these multiple layers instead of a single one.

Some commonly heard ML/AI libraries:
* Keras
* Theano
* scikit-learn
* Tensorflow
* Apache MXNet
* PyTorch

Learning NumPy?
---------------

* I am planning that going through the NumPy tutorial for the moment
* Would help me better understand the scikit-learn tutorial.

Main object -> "homogeneous" (i.e. all elements are of the same type) "multidimensional" (1 or more dimensions) array.

For ex, `[1, 2, 1]` has *one axis* with *three elements* in it => length = 3.
```
[[1., 0., 0.],
 [0., 1., 2.]]
```

has *two axes*, first one has a length of 2, the second axis has a length of 3.
`ndarray` it is called.

Attributes of `ndarray`:
------------------------

`ndarray.ndim`: number of axes (dimensions) of the array.
`ndarray.shape`: the dimensions of the array.
```
>>> a = np.array([[1, 0, 0], [0, 1, 2]], dtype=np.float)
>>> a.ndim
2
>>> a.shape
(2, 3)
>>> a.size
6
```

Basic operations
----------------
Arithmetic operators on arrays apply *elementwise*.
```
>>> a = np.array([20, 30, 40, 50])
>>> b = np.arange(4)
>>> c = a - b
>>> c
array([20, 29, 38, 47])
>>> b**2
array([0, 1, 4, 9])
>>> a < 35
array([ True, True, False, False])
```

Universal functions
-------------------

functions such as `exp`, `sin`, `cos`. In NumPy these are called `ufunc` (*universal functions*).
NumPy functions operate elementwise on an array, producing an array as output.

```
>>> B = np.arange(3)
>>> np.exp(B)
array([1.        , 2.71828183, 7.3890561 ])
```

i.e. `ufunc` is a function that operates on `ndarrays` in an element-by-element basis.
