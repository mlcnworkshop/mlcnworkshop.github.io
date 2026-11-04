---
description: "Keynote speakers of the MLCN workshop (Machine Learning in Clinical Neuroimaging) at MICCAI, including all previous keynotes since 2018."
permalink: /keynotes/
title: "Keynote Speakers"
---
{% assign w = site.data.workshop %}
{% if w.keynotes.size == 0 %}
<div class="mlcn-highlight">The MLCN {{ w.year }} keynote speakers will be announced soon.</div>
{% else %}
{% for k in w.keynotes %}
<div class="mlcn-keynote">
  {% if k.photo %}<img src="{{ k.photo }}" alt="{{ k.name }}">{% endif %}
  <div><p class="mlcn-meta">Keynote {{ forloop.index }}</p><h2>{{ k.name }}</h2><p><strong>{{ k.title }}</strong></p><p>{{ k.abstract }}</p><p class="mlcn-small">{{ k.bio }}</p></div>
</div>
{% endfor %}
{% endif %}

<h2>Previous keynote speakers</h2>
<div class="mlcn-years">
{% for h in site.data.history %}  <div class="mlcn-year"><span class="y">{{ h.year }}</span><span class="c">MICCAI · {{ h.city }}</span><p>{{ h.keynotes | replace: " · ", "<br>" }}</p></div>
{% endfor %}</div>
