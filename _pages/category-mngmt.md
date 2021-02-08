---
title: category-management
layout: page
datafile: category-mngt
sidenav: false
---

<h1 style="margin-top:7px;">Category Management</h1>
<!--<div class="width-mobile">-->
<table class="usa-table usa-table--stacked-header">
  {% for row in site.data.category-mngt %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th data-label="" class="row-color">{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    {% endif %}

    {% tablerow pair in row %}
      {{ pair[1] }}
    {% endtablerow %}
  {% endfor %}
</table>
<!--</div>-->
<!--
<section class="grid-container clearfix padding-left-0 padding-right-1">
    <h1 style="margin-top:7px;">Category Management</h1>
    <div class="grid-row">
        <p style="font-size:2rem;font-weight:bold;">Coming Soon!</p>
            <table class="usa-table usa-table--stacked-header">
                <caption></caption>
                <thead>
                    <tr>
                    <th scope="col">Problem Statement</th>
                    <th scope="col">Document</th>
                    <th scope="col">Description</th>
                    <th scope="col">Download</th>
                    <th scope="col">Last Updated</th>
                    <th scope="col">Tags</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                    <th data-label="Problem Statement" scope="row">I need a template to speed my IT Acquisitions</th>
                    <td data-label="Document title">Template (hyperlinked)</td>
                    <td data-label="Description">This is a template to speed IT acquisitions at you agency</td>
                    <td data-label="Download">ITVMO MAX</td>
                    <td data-label="Last Updated">MM/DD/YYYY</td>
                    <td data-label="Tag">IT Acquisition; Category Management; Templates</td>
                    </tr>
                    <tr>
                    <th data-label="Problem Statement" scope="row">What are the IT CM Strategic Initiatives for FY21</th>
                    <td data-label="Document title">IT CM Initiatives Presentation</td>
                    <td data-label="Description">This IT CM Strategic Initiatives slide deck highlights priority projects for fiscal year 2021</td>
                    <td data-label="Download">pptx</td>
                    <td data-label="Last Updated">MM/DD/YYYY</td>
                    <td data-label="Tag">Category Management; Strategic Initiatives</td>
                    </tr>
                    <tr>
                    <th data-label="Problem Statement" scope="row"></th>
                    <td data-label="Document title"></td>
                    <td data-label="Description"></td>
                    <td data-label="Download"></td>
                    <td data-label="Last Updated"></td>
                    <td data-label="Tag"></td>
                    </tr>
                    <tr>
                    <th scope="row"></th>
                    <td data-label="Document title"></td>
                    <td data-label="Description"></td>
                    <td data-label="Download"></td>
                    <td data-label="Last Updated"></td>
                    <td data-label="Tag"></td>
                    </tr>
                </tbody>
            </table>
    </div>
</section>-->
