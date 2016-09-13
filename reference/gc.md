---
layout: page
title: Garbage Collection 
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

# Garbage Collection

Architecture:
Heaps
	flat, generational, region based, segregated
		spaces, sub spaces, arenas, sub arena, memory pool
GCs
	global, generational, incremental, balanced
		parallel mark, sweep, compact, concurrent mark / sweep
		

parallel mark/sweep/compact collector and all supporting infrastructure.
Concurrent marking code
Parallel scavenger code
