---
layout: page
title: Port
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

# Portability library

The Port Library is a platform abstraction library for operating-system-level
services, excluding those handled by the Thread Library.

The Port Library is designed to be a standalone component that can be used to
add multiplatform support to many projects. Thus Port Library APIs must not
have dependencies on other OMR components, such as GC or JIT. They can use
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



