# Introduction
This repo is used to build the
[cpp-graph](https://github.com/goodfella/cpp-graph) project.  It
contains all the dependencies as git submodules and provides a top
level CMakeLists.txt file to help with build directory setup.

# Building

First step is to clone the submodules:
```shell
git submodule update --init
```

Then use cmake to build the code:
```shell
mkdir build
cd build
cmake ..
```
