---
layout: page
title: Components
menu: reference
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
