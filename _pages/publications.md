---
layout: archive
title: "Publications"
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

<html>
<script type="text/javascript">
<!--
var arxiv_authorid = "narayanchowdhury_a_1";
//--></script>
<script type="text/javascript" src="https://arxiv.org/js/myarticles.js"></script>
</html>
