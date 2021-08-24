---
layout: archive
#
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

Peer-reviewed publications
======

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

ArXiv preprints
======

https://arxiv.org/a/narayanchowdhury_a_1.html



{% include arxiv-widget.html %}
