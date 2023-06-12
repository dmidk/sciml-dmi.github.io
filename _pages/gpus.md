---
layout: page
title: GPU platforms
permalink: /gpu/
gpu_platforms:
  - name: Pascal (DMI)
    hardware: 1x A100 80GB
    access: Email Tore Wulf (twu@dmi.dk)
    project: ASIP
  - name: ATOS (ECMWF)
    hardware:
    access:
  - name: European Weather Cloud
    hardware:
    access:
  - name: LUMI
    hardware:
    access:
  - name: EuroHPC
    hardware:
    access:
---

Below is an overview of GPU platforms available for research by staff at DMI:

<h2>GPU platforms</h2>

<table>
<tr>
<th>Name</th>
<th>Hardware</th>
<th>Access</th>
<th>Project</th>
</tr>

{% for platform in page.gpu_platforms %}
<tr>
<td>{{platform.name}}</td>
<td>{{platform.hardware}}</td>
<td>{{platform.access}}</td>
<td>{{platform.project}}</td>
</tr>
{% endfor %}

</table>
