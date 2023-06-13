---
layout: page
title: GPU platforms
permalink: /gpu/
gpu_platforms:
  - name: Pascal (DMI)
    hardware: 1x Nvidia A100 80GB
    access: Email Tore Wulf (twu@dmi.dk)
    project: ASIP
  - name: ATOS (ECMWF)
    hardware: 72x Nvidia A100
    access: https://confluence.ecmwf.int/display/EWCLOUDKB/GPU+support+at+ECMWF
  - name: European Weather Cloud
    hardware: 36x Nvidia A100 (TBC), imminently available (June 2023)
    access: pilot access only
  - name: LUMI (EuroHPC)
    hardware: 2560x4x AMD MI250x
    access: https://docs.lumi-supercomputer.eu/firststeps/
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

- [EuroHPC JU - supercomputers](https://eurohpc-ju.europa.eu/about/our-supercomputers_en)
