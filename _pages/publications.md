---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}


<h2>Journal Articles</h2>
{% for post in site.publications reversed %}
  {% if post.pubtype == 'journal' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

<h2>Book Chapters</h2>
{% for post in site.publications reversed %}
  {% if post.pubtype == 'book chapter' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

<h2>Book Translations</h2>
{% for post in site.publications reversed %}
  {% if post.pubtype == 'translation' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}
