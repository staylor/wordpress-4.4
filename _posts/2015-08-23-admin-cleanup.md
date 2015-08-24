---
layout: post
title: Admin Cleanup
permalink: /admin-cleanup/
elevator_pitch: Identify portions of the admin that could use a reboot
---

Led by: `wonderboymusic`, `helen`

* Admin Menu generation is not repeatable, needs to be encapsulated into an actual API [ticket](https://core.trac.wordpress.org/ticket/33418)
* Admin screens use raw PHP for templating, which is not templating. We should find ways to separate
the data from the markup to make it easier to switch out the raw PHP for another templating
language - Mustache, React, whatever. Even if we continue to use raw PHP, we can separate concerns
better.
* Select2/Dropdowns - the next iteration of scaling large datasets of user, posts, etc
* Page on Front perhaps with: Dave M and Folletto?