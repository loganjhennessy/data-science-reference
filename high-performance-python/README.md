# Motivation for high performance computing

Pretty simple. You have lots of data and some complex computations you
want to perform.

# Computing resources

* CPU
  - Used to just have a single core, but multi-core is becoming almost
    ubiquitous.
* RAM
* Storage
* GPU
  - These have thousands of cores

# Processes

Uses Python's `multiprocessing` module.

# Threads

Multiple threads are sharing one core.

In addition to using Python's `threading` module, you have the option
of using `multiprocessing.dummy`. This allows you to take advantage of
the easy multiprocessing API to do multi-threading.

# Parallelism

# Concurrency

# Measuring runtime
