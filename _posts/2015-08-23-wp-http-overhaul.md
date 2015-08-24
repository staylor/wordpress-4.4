---
layout: post
title: WP HTTP Overhaul
permalink: /wp-http-overhaul/
elevator_pitch: Let's replace the internals of the existing WP HTTP API with Requests.
---

Led by: `dd32`, `rmccue`

Our internal HTTP API is showing its age. To support the kind of PHP apps that people
are making with WordPress, we need a more modern set of tools. Ryan McCue has authored a
library called [Requests](http://requests.ryanmccue.info/). He has also created a plugin called
[Requests-WPHTTP](https://github.com/rmccue/Requests-WPHTTP) that replaces the current internals
via filters. The goal is the actually replace the existing API's internals with Requests. We also
want to update Requests in the meantime to support things like [PSR-7](http://www.php-fig.org/psr/psr-7/).

Dion will be the decider here. Ryan has already done a lot of work. `WP_Http` will remain backwards-compatible
while using more Requests bits internally. The advantage is that we also get Requests, which users
can start using directly, without using `WP_Http`.

I want to make sure the feature set is robust and that the APIs feel cutting-edge. [Guzzle](http://guzzle.readthedocs.org/en/latest/)
is bleeding-edge PHP library that does HTTP right and has a full feature set - includes a [Promises/A+](https://promisesaplus.com/)
implementation and [PSR-7 compliant interfaces](http://guzzle.readthedocs.org/en/latest/psr7.html).