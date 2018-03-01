---
layout: page
title: Port
menu: reference
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

# Portability library

The Port Library is a platform abstraction library for operating-system-level
services, excluding those handled by the Thread Library.

The Port Library is designed to be a standalone component that can be used to
add multiplatform support to many projects. Thus Port Library APIs must not
have dependencies on other OMR components, such as the Garbage Collector (GC) or Compiler. They can use
omrthread_ APIs.

In addition to abstracting platform-dependent details, Port Library APIs also
support diagnostic features such as tracing and memory usage tracking.

Port Library APIs are published through a table of function pointers, the
OMRPortLibrary structure.

Port Library APIs are conventionally invoked using convenience macros.
This facilitates abstraction of the function table implementation.

For example:

    OMRPORT_ACCESS_FROM_OMRVMTHREAD(omrVmThread);
    void *buffer = omrmem_allocate_memory(1024, OMRMEM_CATEGORY_MM);
