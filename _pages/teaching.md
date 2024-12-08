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

### Undergraduate
Teaching Assistant for
- Introductory Microeconomics (First year)
- Introductory Macroeconomics (First year)
- International trade (Second year)

### Postgraduate
Teaching Assistant for
- Mathematics for Economics (Honors year)
- Econometrics (Honors year)
- Microeconomics (Game theory) (Masters)
- Economic History (Masters)

### Other
- Facilitator: Data science boot camp

{% for post in site.teaching reversed %}
  {% if post.category == 'taught' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}


## Teaching current
{% for post in site.teaching reversed %}
  {% if post.category == 'teaching' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}
