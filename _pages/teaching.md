---
layout: archive
title: "Teaching"
permalink: /teaching/
author_profile: true
---



{% if site.author.googlescholar %}
  You can also find my articles on <u><a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

## Modules Taught
{% for post in site.publications reversed %}
  {% if post.category == 'taught' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}


## Teaching current
{% for post in site.publications reversed %}
  {% if post.category == 'teaching' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}
