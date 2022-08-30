# ArrayList-Lab-work
## Overview  For this assignment you will complete the implementation of the array-backed list data structure (`ArrayList`) started during class, so that it supports (nearly) all the [common](https://docs.python.org/3/library/stdtypes.html#common-sequence-operations) and [mutable](https://docs.python.org/3/library/stdtypes.html#mutable-sequence-types) sequence operations.

## Implementation Details

For the `ArrayList`'s underlying data storage mechanism you will use the [NumPy array](https://numpy.org/doc/stable/reference/arrays.html), as described in class. You will be using a very limited subset of the available APIs for working with NumPy arrays, however. Specifically, you may use:

- [`empty`](https://numpy.org/doc/stable/reference/generated/numpy.empty.html) for creating empty arrays. You will be calling it like this (assuming the numpy library has been imported as `np`, as we always do): `np.empty(N, dtype=object)`. This will create an empty array of size `N`, each slot of which can be used to store a reference to an arbitrary Python object.

- Valid, *positive* indexes into arrays. It will be your job in the implementation of `ArrayList` to check for valid indexes and to translate negative indexes into positive ones.

- `len(arr)` to get the length (i.e., number of slots) of array `arr`. Note that this will not generally coincide with the number of actual elements in the list!cls


**You should not use any other array-related functions provided by NumPy!** Notably, `delete`, `insert`, `append`, `resize`, and others, are off limits. Using them to carry out list operations is, generally speaking, less efficient than the manual approach outlined in class. Also, it's important that you learn how to implement them yourself. Breaking this rule will result in significant score reduction(s).

