---
layout: page
title: What is OMR?
menu: starter
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

# What is OMR?

**The Eclipse OMR project** consists of a highly integrated set of open source C and C++ components that can be used to build robust language runtimes that will support many different hardware and operating system platforms. These components include, but are not limited to: memory management, threading, platform port (abstraction) library, diagnostic file support, monitoring support, garbage collection, and native 'Just In Time' compilation.

**Licenses:** All Eclipse OMR project materials are made available under the Eclipse Public License V1.0 and the Apache 2.0 license. You can choose which license you wish to follow. Please see our LICENSE file for more details.

The initial set of **Eclipse OMR components** includes:

- **port**: platform porting library
- **thread**: a cross platform pthread-like threading library
- **util**: general utilities useful for building cross platform runtimes
- **omrsigcompat**: signal handling compatibility library
- **omrtrace**: tracing library for communication with IBM Health Center monitoring tools
- **tool**: code generation tools for the build system
- **gc**: garbage collection framework for managed heaps
- **vm**: APIs to manage per-interpreter and per-thread contexts
- **example**: demonstration code to show how a language runtime might consume Eclipse OMR components
- **fvtest**: a language-independent test framework so that Eclipse OMR components can be tested outside a language runtime

**Current consumers** of the Eclipse OMR technology:

- The **IBM J9 Virtual Machine** is the most comprehensive consumer. J9 is a high performance, scalable, enterprise class Java Virtual Machine implementation representing hundreds of person-years of effort. While not an open source project itself, J9 directly implements capabilities for Java by using the core implementations provided by Eclipse OMR.
- The **Ruby+OMR Technology Preview** project also consumes the Eclipse OMR components by modifying the CRuby project.
- A **SOM++ Smalltalk** runtime has been modified to use Eclipse OMR components.
- An experimental version of **CPython** using Eclipse OMR components has been created but is not currently available in the open. (Our focus has been on getting this code out into the open.)
