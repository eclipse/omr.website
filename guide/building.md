---
layout: page
title: Building
menu: guide
lang: en
---

[//]: # "*******************************************************************************"
[//]: # "* Copyright (c) 2016, 2018 IBM Corp. and others"
[//]: # "*"
[//]: # "* This program and the accompanying materials are made available under"
[//]: # "* the terms of the Eclipse Public License 2.0 which accompanies this"
[//]: # "* distribution and is available at https://www.eclipse.org/legal/epl-2.0/"
[//]: # "* or the Apache License, Version 2.0 which accompanies this distribution and"
[//]: # "* is available at https://www.apache.org/licenses/LICENSE-2.0."
[//]: # "*"
[//]: # "* This Source Code may also be made available under the following"
[//]: # "* Secondary Licenses when the conditions for such availability set"
[//]: # "* forth in the Eclipse Public License, v. 2.0 are satisfied: GNU"
[//]: # "* General Public License, version 2 with the GNU Classpath"
[//]: # "* Exception [1] and GNU General Public License, version 2 with the"
[//]: # "* OpenJDK Assembly Exception [2]."
[//]: # "*"
[//]: # "* [1] https://www.gnu.org/software/classpath/license.html"
[//]: # "* [2] http://openjdk.java.net/legal/assembly-exception.html"
[//]: # "*"
[//]: # "* SPDX-License-Identifier: EPL-2.0 OR Apache-2.0 OR GPL-2.0 WITH Classpath-exception-2.0 OR LicenseRef-GPL-2.0 WITH Assembly-exception"
[//]: # "*******************************************************************************"

# Building

### How to Build a Standalone Eclipse OMR with a basic configuration

To build standalone Eclipse OMR, run the following commands from the root of the
source tree.

    # Create a build directory and cd into it
    mkdir build
    cd build

    #generate the build system using cmake
    cmake ..

    # Build (you can optionally compile in parallel by adding -j<N> to the make command)
    make

    # Run tests (note that no contribution should cause new test failures in testing).
    # Use the `-V` option to see verbose output from the tests.
    ctest [-V]

### Building Eclipse OMR on Windows using Visual Studio

The following instructions below demonstrate the steps to build Eclipse OMR on Windows
using Visual Studios. In the example Visual Studio 11 2012 Win64 is being used.
You can easily switch this to the version of Visual Studio you would like to use.

    # Create a build directory and cd into it
    mkdir build
    cd build

    #generate the build system using cmake
    cmake -G "Visual Studio 11 2012 Win64" ..

    # Build
    cmake --build .

    # Run tests (note that no contribution should cause new test failures in "make test")
    ctest

