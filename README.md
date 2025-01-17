# tiny-process-library
A small platform independent library making it simple to create and stop new processes in C++, as well as writing to stdin and reading from stdout and stderr of a new process.

This library was created for, and is used by the C++ IDE project [juCi++](https://gitlab.com/cppit/jucipp).

### Features
* No external dependencies
* Simple to use
* Platform independent
  * Creating processes using executables is supported on all platforms
  * Creating processes using functions is only possible on Unix-like systems
* Read separately from stdout and stderr using anonymous functions
* Write to stdin
* Kill a running process (SIGTERM is supported on Unix-like systems)
* Correctly closes file descriptors/handles

### Usage
See [examples.cpp](examples.cpp).

### Get, compile and run

#### Unix-like systems
```sh
git clone https://github.com/koradeh/tiny-process-library.git
cd tiny-process-library
mkdir build
cd build
cmake ..
make
./examples
```

#### Windows with MSYS2 (https://msys2.github.io/)
```sh
git clone https://github.com/koradeh/tiny-process-library.git
 cd tiny-process-library
mkdir build
cd build
cmake -G"MSYS Makefiles" ..
make
./examples
```
