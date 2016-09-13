---
layout: page
title: Thread
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

# Thread Library

The Thread Library is a platform abstraction library for synchronization
constructs and low-level thread-related services. This library includes the following capabilities:

* Create and destroy threads
* Platform abstraction of synchronization constructs such as mutexes and condvrs
* Introspection of threads

Public APIs in the Thread Library are prefixed with "omrthread_".

The omrthread_ APIs offer capabilities that are not available from OS-level APIs,
such as:
* Multiplatform support
* Inspect and debug wait queues on locks and condvars
* Tune userspace spinlocking

To use the Thread Library, a thread must either be created by the library, or
attached to it using the omrthread_attach()/omrthread_attach_ex() API.

Thread Library APIs are not re-entrant. omrthread_ functions cannot call other
omrthread_ functions. Since omrthread_ functions are used by most other
components of OMR, omrthread_ functions must not have dependencies on any other
components of OMR.


