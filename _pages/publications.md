---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
classes: wide
---

Clicking on any of the links below will redirect you to the abstract and details of my contributions.

{% include base_path %}

{% assign publications_sorted = site.publications | sort: "date" %}
{% for post in publications_sorted %}
  {% include archive-single.html %}
{% endfor %}
