---
layout: post
title: Comment Moderation + Heartbeart
permalink: /comment-moderation-heartbeat/
elevator_pitch: Comment moderation might be able to take advantage of Heartbeat
---

Led by: `wonderboymusic`

On my recent [call for feedback post](https://make.wordpress.org/core/2015/08/19/wordpress-4-4-whats-on-your-wishlist/),
the comments came in quick, and many required moderation. If you keep the comments list table
moderation page open, there is no indication when new comments arrive. There is probably
some work we can do here with the Heartbeat API.

I recently dug into some of the ancient comment code to fix bubble counts dynamically when inline
moderation happens.

**Pros:**
* Live comment moderation, doesn't require refreshing the page to see new comments
or find out that there are comments to be moderated.
* a chance to make use of Heartbeat

**Cons:** The JS that powers the list table screen for comments now is old and painful to work with.