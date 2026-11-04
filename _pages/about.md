---
permalink: /
title: "MLCN 2027 – Machine Learning in Clinical Neuroimaging"
description: "MLCN 2027, the international workshop on Machine Learning in Clinical Neuroimaging, takes place at MICCAI 2027 in Auckland, New Zealand (27 September – 1 October 2027). Call for papers, keynotes, program and organizers."
hide_title: true
---
{% assign w = site.data.workshop %}
{% if w.banner != "" %}<figure class="mlcn-banner">
  <img src="{{ w.banner }}" alt="Auckland city skyline with the Sky Tower, seen from the Waitematā Harbour" width="1600" height="622" fetchpriority="high">
  <figcaption><span class="kicker">MICCAI {{ w.year }} workshop</span><span class="big">{{ w.city | split: ',' | first }} {{ w.year }}</span></figcaption>
</figure>{% endif %}

<h1>MLCN {{ w.year }}: Machine Learning in Clinical Neuroimaging</h1>
<p class="mlcn-meta">MICCAI {{ w.year }} · {{ w.city }} · {{ w.conference_dates }}</p>

<p class="mlcn-lead">In this international workshop on <b><i>Machine Learning in Clinical Neuroimaging</i></b> we bring together researchers in machine learning, neuroscience and tech-savvy clinicians to develop methods for complex neuroimaging data and to close the gap between those methods and clinical practice.</p>

{% if w.openreview == "" %}<div class="mlcn-highlight">We are preparing MLCN {{ w.year }}.<span>The call for papers, deadlines and keynote speakers follow the MICCAI {{ w.year }} workshop timeline. Workshop day: {{ w.workshop_date }}.</span></div>{% else %}<div class="mlcn-highlight">Submissions for MLCN {{ w.year }} are open.<span>Workshop day: {{ w.workshop_date }}.</span></div>{% endif %}

<div class="mlcn-buttons">
  <a class="mlcn-button" href="{% if w.openreview != "" %}{{ w.openreview }}{% else %}/submission_registration/{% endif %}">{% if w.openreview != "" %}Submit on OpenReview{% else %}Call for papers{% endif %}</a>
  <a class="mlcn-button secondary" href="{{ w.last.program }}">MLCN {{ w.last.year }} program</a>
</div>

<div class="mlcn-cards">
  <a class="mlcn-card" href="/submission_registration/"><span class="ic" aria-hidden="true"><svg viewBox="0 0 24 24"><path d="M14 3H7a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h10a2 2 0 0 0 2-2V8z"/><path d="M14 3v5h5"/><path d="M9 13h6M9 17h4"/></svg></span><span><strong>Call for papers</strong><span class="t">{% if w.openreview != "" %}Submissions open{% else %}Two tracks, opening soon{% endif %}</span></span><svg class="go" viewBox="0 0 24 24" aria-hidden="true"><path d="M9 6l6 6-6 6"/></svg></a>
  <a class="mlcn-card" href="/keynotes/"><span class="ic" aria-hidden="true"><svg viewBox="0 0 24 24"><rect x="9" y="3" width="6" height="11" rx="3"/><path d="M5 11a7 7 0 0 0 14 0"/><path d="M12 18v3M9 21h6"/></svg></span><span><strong>Keynotes</strong><span class="t">{% if w.keynotes.size > 0 %}Two invited talks{% else %}Two invited talks, announced soon{% endif %}</span></span><svg class="go" viewBox="0 0 24 24" aria-hidden="true"><path d="M9 6l6 6-6 6"/></svg></a>
  <a class="mlcn-card" href="/program/"><span class="ic" aria-hidden="true"><svg viewBox="0 0 24 24"><rect x="3" y="5" width="18" height="16" rx="2"/><path d="M3 10h18M8 3v4M16 3v4"/><path d="M7 14h3M7 17.5h6"/></svg></span><span><strong>Program</strong><span class="t">Orals, lightning talks and posters</span></span><svg class="go" viewBox="0 0 24 24" aria-hidden="true"><path d="M9 6l6 6-6 6"/></svg></a>
  <a class="mlcn-card" href="/community_organizers/"><span class="ic" aria-hidden="true"><svg viewBox="0 0 24 24"><circle cx="9" cy="8" r="3.2"/><path d="M3 20c0-3.3 2.7-6 6-6s6 2.7 6 6"/><circle cx="17.5" cy="9.5" r="2.5"/><path d="M16 14.3c3 .1 5 2.3 5 5.2"/></svg></span><span><strong>Community</strong><span class="t">Organizers and past editions since 2018</span></span><svg class="go" viewBox="0 0 24 24" aria-hidden="true"><path d="M9 6l6 6-6 6"/></svg></a>
</div>

<h2>Key dates</h2>
{% for d in w.dates %}<div class="mlcn-row"><strong>{{ d.label }}</strong><span class="date">{{ d.date }}</span></div>
{% endfor %}<div class="mlcn-row"><strong>Workshop</strong><span class="date">{{ w.workshop_date }}</span></div>

<h2>Sponsors</h2>
<div class="mlcn-sponsors">
  <a href="https://ai2d.med.upenn.edu"><img src="/images/AI2D_logo.png" alt="AI2D, University of Pennsylvania"></a>
  <a href="https://medicine.yale.edu/biomedical-imaging-institute"><img class="sq" src="/images/Yale_logo.jpg" alt="Yale Biomedical Imaging Institute"></a>
  <a href="https://www.ellis-jena.ai"><img class="sq" src="/images/ELLIS_JENA_1.png" alt="ELLIS Unit Jena"></a>
</div>

<h2>Frequently asked questions</h2>
<div class="mlcn-faq">
{% for q in w.faq %}<details{% if forloop.first %} open{% endif %}><summary>{{ q.q }}</summary><p>{{ q.a }}</p></details>
{% endfor %}</div>

<p class="mlcn-note">Papers from previous years are in the <a href="{{ w.proceedings }}">MLCN proceedings</a>; some talks are on our <a href="{{ w.youtube }}">YouTube channel</a>.</p>
