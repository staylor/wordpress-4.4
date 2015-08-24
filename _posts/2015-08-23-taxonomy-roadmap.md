---
layout: post
title: Taxonomy Roadmap
permalink: /taxonomy-roadmap/
elevator_pitch: boone has been tearing up the roadmap, will continue work this cycle
---

Based on my [call for feedback](https://make.wordpress.org/core/2015/08/19/wordpress-4-4-whats-on-your-wishlist/),
a lot of people want to see Term Meta land. Good for us: it's already on our
[Taxonomy Roadmap](https://make.wordpress.org/core/2013/07/28/potential-roadmap-for-taxonomy-meta-and-post-relationships/).

* Fix the most annoying bug in WordPress is [done](https://core.trac.wordpress.org/ticket/5809)
* Step 1 is [done](https://core.trac.wordpress.org/ticket/17689)
* Step 2 is [done](https://core.trac.wordpress.org/ticket/21950)
* Step 3 is [done](https://core.trac.wordpress.org/ticket/30261)

Things to do next:

* Potentially combine the 2 terms tables
* Do something like setting `$wpdb->terms` to `$wpdb->term_taxonomy`
* Hopefully land a `WP_Term` model
* make Term Meta a thing

@boone has been crushing all of this stuff. The next logical step is to keep going.
