---
layout: single
permalink: /blog/
---
{% include group-by-array collection=site.posts field="title" %}
{% for title in group_names %}
  {% assign posts = group_items[forloop.index0] %}
  {% for post in posts %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %}
