---
layout: default
title: WordPress 4.4
---

{% for post in site.posts %}
<h3><a id="{{ post.slug }}" href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h3>
{{ post.content }}
{% endfor %}