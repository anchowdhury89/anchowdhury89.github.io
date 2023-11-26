---
layout: archive
#
permalink: /publications/
author_profile: true
---

{% include base_path %}

Preprints
-------

{% for post in site.preprints reversed %}
  {% include preprints-single.html %}
{% endfor %}
  
<br/><br/>

Published articles
--------

{% for post in site.publications reversed %}
  {% include publications-single.html %}
{% endfor %}

***

[arXiv author page](https://arxiv.org/a/narayanchowdhury_a_1.html){: .btn .btn--info}

{% include arxiv-widget.html %}
