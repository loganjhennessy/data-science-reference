# Intro to TensorFlow

Google technology.

Designed specifically for neural networks. It can be used to perform
calculations as well, but it is optimized for neural networks.

Came from Scala. So some of the function calls have Scala-like syntax.

A **tensor** in this context can be thought of  as an array that may
have nay number of dimensions.

# TensorFlow calculations

## Errors

I'm getting the following error when I attemp to run .eval() on what
should be a decoded jpeg image (tf.image.decode_jpeg):

> ```OutOfRangeError: FIFOQueue '_0_input_producer' is closed and has```
> ```insufficient elements (requested 1, current size 0)```
>	```[[Node: ReaderReadV2_283 = ```
> ```ReaderReadV2[_device="/job:localhost/replica:0/task:0/cpu:0"]```
> ```(WholeFileReaderV2, input_producer)]]```

I'm not sure what's going on, but it breaks regardless of which version
of python  or TensorFlow I run. Need help from Matt or other instructor
on this one.


TensorFlow has lazy evaluation. It builds a graph that describes the
computation to perform, and then executes it.

A **constant** is just a constant value, an object that doesn't change.

TensorFlow defaults to storing floats using 32 bits, as opposed to
NumPy's default of 64 bits.

Broadcasting works similarly to NumPy. TensorFlow will fill in empty
dimensions.

Its often good to specify dimensions just for our own sanity.

# Pros and Cons of neural networks

# Basic neural network algorithms

# Simple  TensorFlow neural network
