---
layout: post
title: Comments Overhaul
permalink: /comment-moderation-heartbeat/
elevator_pitch: Comment moderation might be able to take advantage of Heartbeat
---

Led by: `wonderboymusic`

Things that have been done:

* Overhauled comment caching
* Added `WP_Comment`
* All template functions now accept full comment object, in addition to just comment_ID
* Comment count for pending comments appears in the HTML title

Perhaps a UI upgrade while we're at it.

**Comment Moderation + Heartbeart**

On my recent [call for feedback post](https://make.wordpress.org/core/2015/08/19/wordpress-4-4-whats-on-your-wishlist/),
the comments came in quick, and many required moderation. If you keep the comments list table
moderation page open, there is no indication when new comments arrive. There is probably
some work we can do here with the Heartbeat API.

**Pros:**

* Live comment moderation, doesn't require refreshing the page to see new comments
or find out that there are comments to be moderated.
* a chance to make use of Heartbeat
* I recently dug into some of the ancient comment code to fix bubble counts dynamically when inline
moderation happens - this whole screen can be rewritten in Backbone, fairly easily.
