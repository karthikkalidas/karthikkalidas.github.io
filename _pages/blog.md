---
title: "Blog"
layout: archive
permalink: /blog/
author_profile: true
---
{% include group-by-array collection=site.posts field="title" %}
{% for title in group_names %}
  {% assign posts = group_items[forloop.index0] %}
  {% for post in posts %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %}
