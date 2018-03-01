---
layout: page
title: Components
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

# Components

Eclipse OMR is made up of shared, reusable, open-source core components for building language runtimes. These components include:

- **Garbage Collector (GC):** a garbage collection framework for managed heaps. Eclipse OMR includes several implementations: mark-and-sweep, generational, and parallel scavenger.
- **Port Library (port):** a platform abstraction (porting) library.
- **Thread Library (thread):** a cross platform threading library.
- **Utility Library (util):** a variety of utility libraries that provide functions for building cross platform runtimes.
- **Virtual Machine (VM):** APIs to manage per-interpreter and per-thread contexts.
- **Trace Library (omrtrace):** a tracing library for communication with IBM Health Center monitoring tools.
- **Signal Handling Compatibility Library (omrsigcompat):** a signal handling compatibility library.
- **Compiler:** for native code generation.
- **Diagnostic services:** _(to be contributed)_ Health Center provides a live view of runtime details, such as GC statistics and method profiling.
