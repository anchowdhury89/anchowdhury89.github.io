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

<script type="text/javascript">
<!--
var arxiv_authorid="http://arxiv.org/a/narayanchowdhury_a_1";
var arxiv_format="arxiv";
var arxiv_max_entries=0;       //show all articles
var arxiv_includeSummary=1;    //show abstracts (default is 0)
var arxiv_includeComments=0;   //do not show comments (default is 1)
//-->
</script>
<script type="text/javascript" src="http://arxiv.org/js/myarticles.js">
</script>
<div id="arxivfeed"><
/div>
