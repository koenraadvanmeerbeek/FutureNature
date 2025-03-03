---
layout: page
title: Publications
permalink: /publications/
---

{% assign publications = site.data.publications.publications | sort: "year" | reverse %}
{% assign project_members = site.data.project_members.members %}
{% assign count = publications.size %}

{% assign grouped_publications = publications | group_by: "year" %}

{% for group in grouped_publications %}
## {{ group.name }}

{% for pub in group.items %}
{% assign author_list = pub.authors | split: ";" %}

{{ count }}. 

{% for author in author_list %}
  {% assign author_trimmed = author | strip %}
  {% if project_members contains author_trimmed %}
    **{{ author_trimmed }}**
  {% else %}
    {{ author_trimmed }}
  {% endif %}
  {% if forloop.last == false %}; {% endif %}
{% endfor %}

({{ pub.year }}). {{ pub.title }}. {{ pub.journal }}. [DOI: {{ pub.doi }}]({{ pub.url }}).

{% assign count = count | minus: 1 %}
{% endfor %}

{% endfor %}
