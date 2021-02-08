---
title: vendor intelligence
layout: page
datafile: vendor-intelligence
sidenav: false
---

<section class="grid-container clearfix padding-left-0 padding-right-1">
<h1 style="margin-top:7px;">Vendor Intelligence</h1>
    <div class="grid-row">
        <p>The ITVMO maintains vendor-specific information for .gov and .mil agency IT acquisition professionals. Due to the sensitive nature of this information, we request that if you have vendor-specific pricing, product, or service questions to reach out directly to the ITVMO inbox at <a href="mailto:itvmo@gsa.gov">itvmo@gsa.gov</a>. </p>
    </div>
<!--<div class="width-mobile">-->
<table class="usa-table usa-table--stacked-header">
  {% for row in site.data.vendor-intelligence %}
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
<!--</div>-->
</section>
