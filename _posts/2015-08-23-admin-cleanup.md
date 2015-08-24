---
layout: post
title: Admin Cleanup
permalink: /admin-cleanup/
elevator_pitch: Identify portions of the admin that could use a reboot
---

Led by: `wonderboymusic`, `helen`

Our admin PHP templates are a junk drawer and eschew all best practices for building scalable
templating and routing systems. While implementing Controllers and switching to a real templating
language are perhaps out of scope, we can definitely make improvements to how our data is generated
and how our admin templates are stitched together. There are always UX improvements to be made as well.

* Admin Menu generation is not repeatable, needs to be encapsulated into an actual API - [ticket](https://core.trac.wordpress.org/ticket/33418)
* Admin screens use raw PHP for templating, which is not templating. We should find ways to separate
the data from the markup to make it easier to switch out the raw PHP for another templating
language - Mustache, React, whatever. Even if we continue to use raw PHP, we can separate concerns
better.
* Select2/Dropdowns - the next iteration of scaling large datasets of user, posts, etc
* Page on Front perhaps: with Dave M and Folletto?

**Pros:**

* The WordPress admin code becomes more elegant
* Data can be exposed via REST routes - getting the admin menu, etc
* Data is retrievable in a way that makes building admins via REST possible