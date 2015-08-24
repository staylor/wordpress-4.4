---
layout: post
title: OO WordPress
permalink: /oo-wordpress/
elevator_pitch: Rewrite some internals as classes and cleanup some project quirks
---

Led by: `boone`, `pento`, `wonderboymusic`

Rewrite some internals as classes and cleanup some project quirks

* plugin API overhaul via `WP_Hook` and [friends](https://core.trac.wordpress.org/ticket/17817)
* More models: `WP_Comment` ([here](https://core.trac.wordpress.org/ticket/32619)) and
`WP_Term` (over [here](https://core.trac.wordpress.org/ticket/14162))
* consider moving `class` definitions out of multi-1000-line files that contain functions (via `svn cp`)
and into their own files - this would make autoloading possible via a classmap (there are plenty
of reasons to not do this, just saying it would be possible)