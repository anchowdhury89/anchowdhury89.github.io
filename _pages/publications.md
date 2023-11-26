---
layout: archive
#
permalink: /publications/
author_profile: true
---

{% include base_path %}

Preprints
======

{% for post in site.preprints reversed %}
  <h3 class="archive__item-title" itemprop="headline">
    {% if post.paperurl %}
      <a href="{{ post.paperurl }}">{{ title }}</a>
    {% else %}
      <a>{{ title }}</a>
    {% endif %}
  </h3>

  {% if post.collection == 'teaching' %}
    <p> {{ post.type }}, {{ post.venue }}, {{ post.year | default: "1900-01-01" | date: "%Y" }} </p>
  {% elsif post.collection == 'preprints' %}
    <p> {{ post.citation }} </p>
    <!-- <p> {{ post.authors }} {{ post.venue }} {{ post.volpages }} {{ post.year | default: "1900-01-01" | date: "%Y" }} </p> -->
  {% elsif post.date %}
    <p class="page__date"><strong><i class="fa fa-fw fa-calendar" aria-hidden="true"></i> {{ site.data.ui-text[site.locale].date_label | default: "Published:" }}</strong> <time datetime="{{ post.date | default: "1900-01-01" | date_to_xmlschema }}">{{ post.date | default: "1900-01-01" | date: "%B %d, %Y" }}</time></p>
  {% endif %}
{% endfor %}


Published articles
======

{% for post in site.publications reversed %}
  <h3 class="archive__item-title" itemprop="headline">
    {% if post.paperurl %}
      <a href="{{ post.paperurl }}">{{ title }}</a>
    {% else %}
      <a>{{ title }}</a>
    {% endif %}
  </h3>

  {% if post.collection == 'teaching' %}
    <p> {{ post.type }}, {{ post.venue }}, {{ post.year | default: "1900-01-01" | date: "%Y" }} </p>
  {% elsif post.collection == 'publications' %}
    <p> {{ post.citation }} </p>
    <!-- <p> {{ post.authors }} {{ post.venue }} {{ post.volpages }} {{ post.year | default: "1900-01-01" | date: "%Y" }} </p> -->
  {% elsif post.date %}
    <p class="page__date"><strong><i class="fa fa-fw fa-calendar" aria-hidden="true"></i> {{ site.data.ui-text[site.locale].date_label | default: "Published:" }}</strong> <time datetime="{{ post.date | default: "1900-01-01" | date_to_xmlschema }}">{{ post.date | default: "1900-01-01" | date: "%B %d, %Y" }}</time></p>
  {% endif %}
{% endfor %}

***

[arXiv author page](https://arxiv.org/a/narayanchowdhury_a_1.html)

{% include arxiv-widget.html %}
