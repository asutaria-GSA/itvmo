---
title: Emerging Technology
layout: page
datafile: emerging-technology
sidenav: false
---

<section class="grid-container clearfix padding-left-0 padding-right-1">
<h1 class="margin-top-0">Emerging Technology</h1>
    <div class="grid-row">
      <p>The ITVMO compiles information pertaining to emerging and innovative technologies and how to procure them. Please reach out to the ITVMO inbox at <a href="mailto:itvmo@gsa.gov">itvmo@gsa.gov</a> with any questions or suggestions for additional resources.</p>
    </div>
<div class="usa-table-container--scrollable">
<table class="usa-table">
<caption></caption>
  {% for row in site.data.emerging-technology %}
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
<h1 style="margin-top:7px;">Emerging Technology</h1>
    <div class="grid-row">
       <p style="font-size:2rem;font-weight:bold;">Coming Soon!</p>
    </div>
</section>-->     