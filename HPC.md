## Python Task Views: High Performance Computing

Packages that help support HPC

| Functionality | (PyPi Link) |  Description / Remarks |
|---------| ----------- |------ | 
| Bindings to C/C++ | [Cython](https://cython.org/), [pybind11](https://pypi.org/project/pybind11/)  |   Python is slow compared to lower level / compiled languages. A common approach to make full use of existing CPU is to extend the language via bindings to a faster language |
| Bindings to other languages (Java, Rust) |  [py4j](https://pypi.org/project/py4j/) , [pyO3](https://pypi.org/project/pyo3-pack/)  |   
| Multi-threading  | Built-in (thread)  |   |
| Multi-core | [multiprocessing](https://pypi.org/project/multiprocessing/) | |
| Spark interface | [pySpark](https://pypi.org/project/pyspark/) |   |
| GPU Computing  | [pyCUDA](https://pypi.org/project/pycuda/)  |   Offered also built-in in some packages (e.g pytorch, tensorflow) |
| Distributed Data  | [dask](https://pypi.org/project/dask/) |   |
