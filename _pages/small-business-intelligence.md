---
title: small business intelligence
layout: page
datafile: small-biz-inteligence
sidenav: false
---

<h1 style="margin-top:7px;">Small Business Intelligence</h1>
<!--<div class="width-mobile">-->
<table class="usa-table usa-table--stacked-header">
  {% for row in site.data.small-biz-inteligence %}
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
