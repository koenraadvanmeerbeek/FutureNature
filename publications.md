---
layout: page
title: Publications
permalink: /publications/
---

{% assign publications = "" | split: "," %}

{% assign publications = publications | push: "2025|Preprint|Van Meerbeek, K.; Spreij, S.; Geuskens, M.; Liu, C.; Goossens, W.; Haesen, S.|Functional assisted migration to sustain ecosystem functions under climate change|*EcoEvoRxiv*|10.32942/X2PS61|https://doi.org/10.32942/X2PS61" %}

{% assign publications = publications | push: "2024|Journal|Fonteyn, W.; Serra‐Diaz, J.M.; Muys, B.; Van Meerbeek, K.|Incorporating climatic extremes using the GEV distribution improves SDM range edge performance|*Journal of Biogeography*|10.1111/jbi.15067|https://doi.org/10.1111/jbi.15067" %}

{% assign publications = publications | push: "2024|Journal|Liu, C.; Van Meerbeek, K.|Predicting the responses of European grassland communities to climate and land cover change|*Philosophical Transactions of the Royal Society B*, **379**(1902), 20230335|10.1098/rstb.2023.0335|https://doi.org/10.1098/rstb.2023.0335" %}

{% assign count = publications.size %}
{% assign grouped_publications = publications | group_by_exp: "item", "item | split: '|' | first" %}

{% for group in grouped_publications %}
## {{ group.name }}

{% for pub in group.items %}
{% assign details = pub | split: '|' %}
{{ count }}. **{{ details[2] }}** ({{ details[0] }}). {{ details[4] }}. {{ details[5] }}. [DOI: {{ details[6] }}]({{ details[7] }}).

{% assign count = count | minus: 1 %}
{% endfor %}

{% endfor %}
