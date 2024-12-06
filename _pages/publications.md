---
layout: archive
title: "Research"
permalink: /publications/
author_profile: true
---
<!---
[Journal Articles](#journal-articles)\
[Conference Papers](#conference-papers)\
[White Papers](#white-papers)\
[Academic](#academic)\
[Presentations](#presentations)
-->
{% if site.author.googlescholar %}
  You can also find my articles on <u><a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

## Job Market Paper
{% for post in site.publications reversed %}
  {% if post.pubtype == 'jmp' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}


## Working Papers
{% for post in site.publications reversed %}
  {% if post.pubtype == 'workingpapers' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

<!---
## White Papers
{% for post in site.publications reversed %}
  {% if post.pubtype == 'whitepaper' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}


## Academic
{% for post in site.publications reversed %}
  {% if post.pubtype == 'academic' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

## Presentations
{% for post in site.publications reversed %}
  {% if post.pubtype == 'presentation' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

-->