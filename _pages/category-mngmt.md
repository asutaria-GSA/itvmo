---
title: category-management
layout: page
datafile: category-mngt
sidenav: false
---

<h1 style="margin-top:7px;">Category Management</h1>
<div class="usa-table-container--scrollable">
<table class="usa-table">
<caption></caption>
  {% for row in site.data.category-mngt %}
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
