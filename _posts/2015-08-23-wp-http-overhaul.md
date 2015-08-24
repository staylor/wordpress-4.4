---
layout: post
title: WP HTTP Overhaul
permalink: /wp-http-overhaul/
elevator_pitch: dd32 and rmmcue are going to try to replace the internals of the existing HTTP API with Requests.
---

Our internal HTTP API is showing its age. To support the kind of PHP apps that people
are making with WordPress, we need a more modern set of tools. Ryan McCue has authored a
library called [Requests](http://requests.ryanmccue.info/). He has also created a plugin called
[Requests-WPHTTP](https://github.com/rmccue/Requests-WPHTTP) that replaces the current internals
via filters. The goal is the actually replace the existing API's internals with Requests. We also
want to update Requests in the meantime to support things like [PSR-7](http://www.php-fig.org/psr/psr-7/).