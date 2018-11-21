# CMake C++ boilerplate with google test and google benchmark

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![Build Status](https://travis-ci.org/akanmuratcimen/cmakecppboilerplate.svg?branch=master)](https://travis-ci.org/akanmuratcimen/cmakecppboilerplate)

A cross-platform C++17 boilerplate project with google test and google benchmark libraries.

This project template using git submodule to include google benchmark and google test repositories.

    $ git clone https://github.com/akanmuratcimen/cmakecppboilerplate
    $ cd cmakecppboilerplate
    $ git submodule init && git submodule update
    $ git clone https://github.com/google/googletest lib/benchmark/googletest

# Build and Test

On Linux/Unix:

    $ mkdir build
    $ cd build
    $ cmake ..
    $ make
    $ make test

On Windows:

> You can use MSBuild command line tool or simply use Visual Studio to build the project on windows.

    $ mkdir build
    $ cd build
    $ cmake ..
    $ msbuild boilerplate.sln
