---
layout: page
title: What is OMR?
menu: starter
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

# What is OMR?

**The Eclipse OMR project** consists of a highly integrated set of open source C and C++ components that can be used to build robust language runtimes that run on many different hardware and operating system platforms.

The core technology components include, but are not limited to: a platform porting library, a thread library, diagnostic services, monitoring services, a just-in-time compiler, and a garbage collector.

Other, developer-focused components, include build tools and utilities, a test framework, and demonstration code to show how a language runtime might consume Eclipse OMR components.

# Why should I use it?

Despite decades of research and development in building languages and runtimes, almost none of the popular language runtimes share any common components. Many runtimes implement their own interface to the operating system, their own garbage collector, their own asynchronous event handling, their own diagnostic formats and so on. However, by reusing the core facilities provided by Eclipse OMR and extending those facilities to cater for your language, you can cut down on the time and effort needed for development. And of course, sharing implementation technology for language runtimes also fosters enablement and adoption of newer, modern programming languages.

One of the most compelling reasons to use Eclipse OMR is the pedigree of the code. Many of the components have their roots in the **J9 virtual machine**; a high performance, scalable, enterprise class Java virtual machine implementation that represents hundreds of person-years of effort. Today, the J9 virtual machine consumes Eclipse OMR from the open project as part of it's build process before adding extensions that are required to make it a Java specific runtime. As such, OMR is already pervasive at an Enterprise level, operating in production environments around the world.

To prove that reuse is possible, here are some other consumers of the Eclipse OMR technology:

- The **Ruby+OMR Technology Preview** project also consumes the Eclipse OMR components by modifying the CRuby project.
- A **SOM++ Smalltalk** runtime has been modified to use Eclipse OMR components.
- An experimental version of **CPython** using Eclipse OMR components has been created but is not currently available in the open. (Our focus has been on getting this code out into the open.)

**Licenses:** All Eclipse OMR project materials are made available under the Eclipse Public License V1.0 and the Apache 2.0 license. You can choose which license you wish to follow. Please see our LICENSE file for more details.
