# Merlin++ 5.03

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2598428.svg)](https://doi.org/10.5281/zenodo.2598428)

Welcome to Merlin++!! We hope you enjoy your stay. The current version of Merlin++ is 5.02.

The follow provides a very quick build guide. For a full in-depth installation guide please
refer to the provided QuickStartGuide.pdf in the `Documentation` directory.

## Building Merlin++

Create a build directory, and cd into it.

To configure, run:

    cmake -DCMAKE_BUILD_TYPE=Release $PATH_TO_MERLIN_DIR

for example, if you created the build directory inside the `Merlin++` directory,

    cmake -DCMAKE_BUILD_TYPE=Release ..

To interactivly configure with more options, run:

    ccmake $PATH_TO_MERLIN_DIR

To build run:

    make OR make -jN

where 'N' is the number of CPUs available for parallel builds, e.g.

    make -j4

The libmerlin.so library will be built in the build directory.

To run a test script to confirm successfull installation run

    make test
    
Success!! Have fun with Merlin++!

## Merlin++ Documentation

You can find user information and other documentation in the `Documentation` directory.

For a full class library definitions and corresponding descriptions, run

    make doxygen

You can now find the generated 'doxygen' information in the current build directory. 






