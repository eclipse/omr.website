---
layout: page
title: Thread
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


