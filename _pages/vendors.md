---
title: The Vendors
layout: page
datafile: vendors
sidenav: false
---

<section class="grid-container clearfix padding-left-0 padding-right-1">
<h1 class="margin-top-0">For Vendors</h1>
    <div class="grid-row">
          <p style="margin-bottom:-5px;">If you are a vendor and would like to work with the ITVMO to make IT product and service acquisitions easier for federal agencies, please reach out to the ITVMO inbox at <a href="mailto:itvmo@gsa.gov">itvmo@gsa.gov</a> and provide the following information:
          <ul style="margin-bottom:-4px;">
             <li>Vendor name</li>
             <li>Contact information</li>
             <li>Industry or service area</li>
             <li>Ideas to improve government IT acquisitions</li>
             <li>Any relevant resources you would like to share with agencies</li>
          </ul></p>
    </div>
<!--
<div class="usa-table-container--scrollable">
<table class="usa-table">
  {% for row in site.data.vendors %}
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
</div>-->
</section>