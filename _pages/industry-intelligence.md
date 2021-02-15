---
title: industry intelligence
layout: page
datafile: industry-intelligence
sidenav: false
---

<h1 style="margin-top:7px;">Industry Intelligence</h1>
<div class="usa-table-container--scrollable">
<table class="usa-table">
  {% for row in site.data.industry-intelligence %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th class="row-color">{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    {% endif %}

    {% tablerow pair in row %}
      {{ pair[1] }}
    {% endtablerow %}
  {% endfor %}
</table>
</div>
<!--
<section class="grid-container clearfix padding-left-0 padding-right-1">
<h1 style="margin-top:7px;">Industry Intelligence</h1>
    <div class="grid-row">
        <p style="font-size:2rem;font-weight:bold;">Coming Soon!</p>
    </div>
</section>-->