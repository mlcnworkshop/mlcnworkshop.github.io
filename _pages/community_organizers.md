---
description: "Organizing committee of the MLCN workshop (Machine Learning in Clinical Neuroimaging) and previous organizers since 2018."
permalink: /community_organizers/
title: "Community & Organizers"
---

<h2>Workshop organizers</h2>
<div class="mlcn-people">
<div class="mlcn-person"><span class="av">ND</span><div><a href="http://www.hellonicha.com"><span class="first">Nicha C.</span> <span class="last">Dvornek</span></a><p>Yale University, USA</p></div></div>
<div class="mlcn-person"><span class="av">MH</span><div><a href="https://www.nallab.org/pi"><span class="first">Mohamad</span> <span class="last">Habes</span></a><p>University of Texas Health Science Center San Antonio, USA</p></div></div>
<div class="mlcn-person"><span class="av">VK</span><div><a href="https://www.kyb.tuebingen.mpg.de/person/58996/2549"><span class="first">Vinod</span> <span class="last">Kumar</span></a><p>Max Planck Institute for Biological Cybernetics, Germany</p></div></div>
<div class="mlcn-person"><span class="av">ST</span><div><a href="https://www.med.upenn.edu/cbica/sindhujatg.html"><span class="first">Sindhuja</span> <span class="last">Tirumalaigovindarajan</span></a><p>University of Pennsylvania, USA</p></div></div>
<div class="mlcn-person"><span class="av">BS</span><div><a href="https://bellaspecktor.github.io"><span class="first">Bella</span> <span class="last">Specktor-Fadida</span></a><p>University of Haifa, Israel</p></div></div>
<div class="mlcn-person"><span class="av">TW</span><div><a href="https://mhm-lab.github.io"><span class="first">Thomas</span> <span class="last">Wolfers</span></a><p>University of Jena & ELLIS Unit Jena, Germany</p></div></div>
<div class="mlcn-person"><span class="av">YX</span><div><a href="http://www.healthx-lab.ca/people.html"><span class="first">Yiming</span> <span class="last">Xiao</span></a><p>Concordia University, Canada</p></div></div>
<div class="mlcn-person"><span class="av">YY</span><div><a href="https://podismine.github.io"><span class="first">Yanwu</span> <span class="last">Yang</span></a><p>Max Planck Institute for Intelligent Systems, Germany</p></div></div>
</div>

<h2>Previous organizers</h2>
{% for h in site.data.history %}<div class="mlcn-prev"><span class="y">{{ h.year }} · {{ h.city }}</span><p>{{ h.organizers }}</p></div>
{% endfor %}
