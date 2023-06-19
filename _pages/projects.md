---
layout: page
title: Projects
permalink: /projects/
ml_projects:
  - name: ASIP (Copernicus)
    aim: sea ice mapping in radar imagery
    website: https://ocean.dmi.dk/asip/
    contact:
        name: Tore Wulf
        email: twu@dmi.dk
  - name: EUMETSAT fellowship
    aim: extending assimilation of sattellite microwave observations over seaice
    contact:
        name: Fabrizio Baordo
        email: fab@dmi.dk
  - name: PRECISE
    aim: emulation regional climate (surface mass-balance) over ice-sheets
    contact:
        name: Ruth Mottram
        email: rum@dmi.dk
  - name: RopeWalk
    aim: digitise hand-written ship data-table observations
    contact:
        name: Martin Stendel
        email: mas@dmi.dk
  - name: ACCORD
    aim: use of machine learning in Limited Area Model Numerical Weather Prediction
    contact:
        name: Henrik Feddersen
        email: hf@dmi.dk
  - name: Destination Earth WP2.4 
    aim: On-Demand Extremes Digital Twin code adaptation to CPU and accelerators - use of ML techniques
    contact:
        name: Peter Ukkonen, Tommaso Benacchio
        email: puk@dmi.dk, tbo@dmi.dk
---

Below is an overview of research projects involving the use of machine learning at DMI:

<h2>Research projects</h2>

<table>
<tr>
<th>Name</th>
<th>Aim</th>
<th>Website</th>
<th>Contact</th>
</tr>

{% for project in page.ml_projects %}
<tr>
<td>{{project.name}}</td>
<td>{{project.aim}}</td>
<td>
{% if project.website %}
<a href="{{ project.website }}">{{project.website}}</a>
{% endif %}
</td>
<td>
{% if project.contact.name and project.contact.email %}
<a href="mailto:{{ project.contact.email }}">{{project.contact.name}}</a>
{% endif %}
</td>
</tr>
{% endfor %}

</table>
