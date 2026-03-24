---
layout: archive
title: "Talks and presentations"
permalink: /talks/
author_profile: true
classes: wide
---

{% assign non_fun_talks = site.talks | where_exp: "item", "item.type != 'Fun Talk'" | sort: "date" | reverse %}
{% assign fun_talks = site.talks | where: "type", "Fun Talk" | sort: "date" | reverse %}

{% for post in non_fun_talks %}
  {% include archive-single.html %}
{% endfor %}

{% if fun_talks.size > 0 %}
<hr>
<h2>Fun talks</h2>
{% for post in fun_talks %}
  {% include archive-single.html %}
{% endfor %}
{% endif %}
