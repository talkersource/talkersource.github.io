---
title: Supplemental Information
description: about Talkers
---

{% assign last_modified_topic = site.info | sort: "updated" | last %}
The following list of articles is generated automatically, last updated: {{ last_modified_topic.updated }}

<style type="text/css">
  h3 { margin-top: 3em; margin-bottom: 10px; }
</style>

{% for topic in site.info %}
### {{ topic.title }}

{% if topic.excerpt %}{{ topic.excerpt }}{% endif %}

[Read more &raquo;]({{ topic.url }})

{% endfor %}
