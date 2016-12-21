---
layout: page
title: Building
menu: guide
lang: en
---

[//]: # "*********************************************************************"
[//]: # "*"
[//]: # "*  Copyright IBM Corp. 2016  All Rights Reserved."
[//]: # "*"
[//]: # "*  This program and the accompanying materials are made available"
[//]: # "*  under the terms of the Eclipse Public License v1.0 and"
[//]: # "*  Apache License v2.0 which accompanies this distribution."
[//]: # "*"
[//]: # "*      The Eclipse Public License is available at"
[//]: # "*      http://www.eclipse.org/legal/epl-v10.html"
[//]: # "*"
[//]: # "*      The Apache License v2.0 is available at"
[//]: # "*      http://www.opensource.org/licenses/apache2.0.php"
[//]: # "*"
[//]: # "*  Contributors:"
[//]: # "*    <First author> - initial implementation and documentation"
[//]: # "*********************************************************************"

# Building

### How to build a standalone Eclipse OMR with a basic configuration

To build a standalone Eclipse OMR, run the following commands from the top of the source tree. The top of the Eclipe OMR source tree is the directory that contains `run_configure.mk`. Note that on Windows systems, you must use a shell script interpreter such as bash to run the configure command.

    # Generate autotools makefiles with SPEC-specific presets
    make -f run_configure.mk SPEC=linux_x86-64 OMRGLUE=./example/glue

    # Build
    make

    # Run tests (note that no contribution should cause new test failures in "make test")
    make test

Run the following command for a list of configure makefile targets:

    make -f run_configure.mk help

Run the following command for a list of build targets:

    make help
