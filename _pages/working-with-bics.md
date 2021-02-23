---
title: Working with BICs
layout: page
datafile: working-with-bics
sidenav: false
---

<section class="grid-container clearfix padding-left-0 padding-right-1">
<h1 class="margin-top-0">Working with BICs</h1>
    <div class="grid-row">
    <p>The ITVMO works closely with the IT Best-in-Class (BIC) solution providers and can help identify the BIC or Government-wide Contract Vehicle (GWAC) that bests meets your agency’s needs. Please reach out to the ITVMO inbox at <a href="mailto:itvmo@gsa.gov">itvmo@gsa.gov</a> with any questions or suggestions for additional resources.
    </p>
    </div>
<div class="usa-table-container--scrollable">
<table class="usa-table">
  {% for row in site.data.working-with-bics %}
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
</section>
<!--
<section class="grid-container clearfix padding-left-0 padding-right-1">
<h1 style="margin-top:7px;">Working with BICs</h1>
    <div class="grid-row">
        <p style="font-size:2rem;font-weight:bold;">Coming Soon!</p>
    </div>
</section>-->