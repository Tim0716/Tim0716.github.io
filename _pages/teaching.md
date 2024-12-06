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
- TA: Introductory Microeconomics (First year)
- TA: Introductory Macroeconomics (First year)
- TA: International trade (Second year)

### Postgraduate
- TA: Mathematics for Economics (Honors year)
- TA: Econometrics (Honors year)
- TA: Microeconomics (Game theory) (Masters)
- TA: Economic History (Masters)

### Other
- Facilitator: Data science Boot camp

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
