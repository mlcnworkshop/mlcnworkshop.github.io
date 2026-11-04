---
description: "Keynote speakers of the MLCN workshop (Machine Learning in Clinical Neuroimaging) at MICCAI, including all previous keynotes since 2018."
permalink: /keynotes/
title: "Keynote Speakers"
---
{% assign w = site.data.workshop %}
{% if w.keynotes.size == 0 %}
The keynote speakers for MLCN {{ w.year }} will be announced soon.
{% endif %}
{% for k in w.keynotes %}
## Keynote: {{ k.name }}
<img align="left" src="{{ k.photo }}" width="150 px" style="padding: 10px"> {{ k.bio }}
<br>
<br>
***Talk title: {{ k.title }}***
<br>
{{ k.abstract }}
<br>
<br>
<br>
{% endfor %}

## Previous Keynote Speakers
<br>
{% for h in site.data.history %}{{ h.year }} - {{ h.keynotes | replace: " · ", " || " }}
<br>
{% endfor %}
