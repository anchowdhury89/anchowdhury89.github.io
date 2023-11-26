---
layout: archive
#
permalink: /publications/
author_profile: true
---

{% include base_path %}

Publications
======

{% for post in site.publications reversed %}
  {% include publications-single.html %}
{% endfor %}

Preprints
======

[https://arxiv.org/a/narayanchowdhury_a_1.html](https://arxiv.org/a/narayanchowdhury_a_1.html)

{% include arxiv-widget.html %}
