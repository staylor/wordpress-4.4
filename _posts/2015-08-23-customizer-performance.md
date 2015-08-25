---
layout: post
title: Customizer Performance
permalink: /customizer-performance/
elevator_pitch: Customizer progress has been constant, there is even more room for big gains
---

Led by: `westonruter`, `celloexpressions`

Weston and Nick have been iterating on the Customizer pretty heavily for the past
several releases. Nav Menus are using a new technique that does partial refreshes to the
Customizer iframe, instead of full reloads. The benefits are already being seen
performance-wise.

On the burner for this release:

* [Partial Refresh](https://core.trac.wordpress.org/ticket/27355)
* potentially, [Transactions](https://core.trac.wordpress.org/ticket/30937)
* JS-Driven [Widgets](https://core.trac.wordpress.org/ticket/33507)

**Pros:**

* We are relying on the Customizer for Theme Options now, the experience needs to scale

**Cons:**

* The Customizer is a black box for many people, sometimes even more than Media is.
We need more people to take the plunge and learn these APIs.