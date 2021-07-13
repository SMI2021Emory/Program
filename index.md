---
title: SMI 2021 Agenda
---
<h1 style="color: #120659;"> SMI 2021 Agenda </h1>
In US Eastern Time
<br/>
<b>The Digital Program Book for the SMI 2021 conference contains the Zoom links for each of the sessions and was sent to all registered attendees on Monday, 5/10.  Please email yguo2 at emory.edu if you did not receive it.</b>

<!-- Potentially store abstract/session information on this site

[invited sessions](docs/ses-invited.md) -->
{% assign sescount = 0 %}
{% for daysch in site.data.program.program %}

  <h2 style="color: #120659;"> {{daysch.date}} </h2>
  <table style="display: block; width: 100%" >
        {% for prog in daysch.dayprog %}
            {% if prog.iscount %}
                {% assign sescount = sescount | plus:1 %}                
            {% endif %}
            <tr>
                {% assign betime = prog.time | split: "-"  %}
                <td style="width: 230px" align="center">{{ betime[0] | date: "%l:%M%P"}} - {{ betime[1] | date: "%l:%M%P"}}</td>
                {% assign currentcount = "" %}
                {% if prog.iscount %}
                    {% assign currentcount = sescount | append: ". " %}
                {% endif %}
                {% if prog.link %}
                  {% if prog.isrecorded %}
                    <td><a href="{{ prog.link | prepend: site.relative_url }}" style="color: #0073ee;"> {{currentcount}}{{ prog.title }} </a> (<a href="{{ prog.recording }}" style="color: #0073ee;"> Session Recording </a>) </td> 
                  {% else %}
                    <td><a href="{{ prog.link | prepend: site.relative_url }}" style="color: #0073ee;"> {{currentcount}}{{ prog.title }} </a> </td> 
                  {% endif %} 
                {% else %}
                    {% if prog.isopenremark %}
                        <td> {{currentcount}}{{ prog.title }} (<a href="{{ prog.recording }}" style="color: #0073ee;"> Session Recording </a>) </td>
                    {% else %}
                        <td>{{currentcount}}{{ prog.title }}</td>
                    {% endif %}
                {% endif %}                
            </tr>
            {% if prog.isopenremark %}
                <tr>
                  <td style="vertical-align: middle;"> <p style="text-align:right;"> 8:45am - 8:50am<br>8:50am - 8:55am<br>8:55am - 9:00am </p> </td>
                  <td style="vertical-align: middle;"> <p style="text-align:left;">
                      Ciprian Crainiceanu<br>
                    Robert Krafty <br>
                    Ying Guo</p> </td>
                </tr>
            {% endif %}
            {% if prog.ifsubprog %}
                {% for eachsubprog in prog.subprog %}
                    {% assign sescount = sescount | plus:1 %}
                    <tr>
                        <td> </td>
                        {% if eachsubprog.id %}
                            <td> <a href="{{ site.relative_url }}/sessions/ses-{{ eachsubprog.id | downcase }}.html" style="color: #0073ee;"> {{sescount | append: ". "}}{{ eachsubprog.name }}</a> (<a href="{{ eachsubprog.recording }}" style="color: #0073ee;"> Session Recording </a>) (organizer: {{ eachsubprog.organizer}})</td>
                        {% else %}
                            <td> <div style="color:red;"> {{sescount | append: ". "}}{{ eachsubprog.name }} </div>(organizer: {{ eachsubprog.organizer}})</td>
                        {% endif %}                        
                    </tr>
                {% endfor %}
            {% endif %}
        {% endfor %}
  </table>

{% endfor %}
