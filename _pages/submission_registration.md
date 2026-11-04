---
description: "Call for papers for MLCN 2027 (Machine Learning in Clinical Neuroimaging) at MICCAI 2027: tracks, topics, deadlines and submission requirements."
permalink: /submission_registration/
title: "Submission & Registration"
---
{% assign w = site.data.workshop %}

## Submission

{% if w.openreview != "" %}To submit a paper to the MLCN {{ w.year }} MICCAI workshop, first make sure you are registered on the OpenReview platform by signing up [here](https://openreview.net/signup).
Then, when logged in, visit the [workshop submission page]({{ w.openreview }}) and submit your paper via "MICCAI {{ w.year }} Workshop MLCN Submission".{% else %}The submission link for MLCN {{ w.year }} will be posted here once the call for papers opens. Submissions are handled through [OpenReview](https://openreview.net/signup).{% endif %}

## Important Dates
{% for d in w.dates %}{{ d.label }}: {{ d.date }}
<br>
{% endfor %}Workshop: {{ w.workshop_date }}
<br>

## Call for Papers

In the ***Machine Learning track***, we are seeking novel contributions that address current methodological gaps in analyzing high-dimensional, longitudinal, and heterogeneous clinical neuroscientific data using stable, scalable, and interpretable machine learning models.

In the ***Clinical Neuroimaging track***, we are interested in papers with an applied focus. We invite the community to submit conference contributions on machine learning approaches aimed at improving our understanding of complex brain disorders and moving the field closer to precision medicine.

Topics of interest include but are not limited to:
<ul>
    <li>Spatio-temporal, structural and longitudinal brain data analysis</li>
    <li>Graph theory and complex network analysis</li>
    <li>Model stability, interpretability and uncertainty in clinical predictions</li>
    <li>Scalable models for big and multi-site neuroimaging data, from preprocessing to modeling</li>
    <li>Multi-source data integration and multi-view learning</li>
    <li>Domain adaptation, data harmonization and transfer learning</li>
    <li>Unsupervised stratification of brain disorders</li>
    <li>Biomarker discovery, refinement of nosology and diagnostics, biological validation of clinical syndromes</li>
    <li>Treatment outcome and course prediction</li>
    <li>Wearable sensors</li>
    <li>Neurogenetics and brain imaging genetics</li>
    <li>Mechanistic modeling</li>
    <li>Brain aging</li>
    <li>Databases for machine learning</li>
</ul>

## Submission Requirements

<ul class="mlcn-checks">
    <li>Original, unpublished work within the scope above.</li>
    <li>Springer Lecture Notes in Computer Science (LNCS) format, at most 8 pages including figures and tables, plus up to 2 pages of references.{% if w.latex_template != "" %} These are the MICCAI {{ w.year }} <a href="{{ w.latex_template }}">LaTeX</a> and <a href="{{ w.word_template }}">MS Word</a> templates.{% endif %}</li>
    <li>Double-blind review: submissions must be anonymous.</li>
    <li>Please follow MICCAI guidelines regarding paper submission format, dual/double submission policy, conflicts of interest, plagiarism, and use of LLMs{% if w.miccai_guidelines != "" %} as described in the <a href="{{ w.miccai_guidelines }}">MICCAI paper submission guidelines</a>{% endif %}.</li>
</ul>
<p>Accepted papers are published in the MLCN proceedings alongside MICCAI {{ w.year }}.</p>
