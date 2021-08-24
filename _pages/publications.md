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
{% include arxivwidget.html %}
