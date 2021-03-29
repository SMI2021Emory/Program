---
title: SMI 2021 Agenda
---
# SMI 2021 Agenda

<!-- Potentially store abstract/session information on this site

[invited sessions](docs/ses-invited.md) -->
{% assign sescount = 0 %}
{% for daysch in site.data.program.program %}

  <h2> {{daysch.date}} </h2>
  <table style="display: block; width: 100%">
        {% for prog in daysch.dayprog %}
            {% if prog.iscount %}
                {% assign sescount = sescount | plus:1 %}                
            {% endif %}
            <tr>
                <td style="width: 140px">{{ prog.time }}</td>
                {% assign currentcount = "" %}
                {% if prog.iscount %}
                    {% assign currentcount = sescount | append: ". " %}
                {% endif %}
                {% if prog.link %}
                    <td><a href="{{ prog.link | prepend: site.relative_url }}"> {{currentcount}}{{ prog.title }} </a></td>                    
                {% else %}
                    <td>{{currentcount}}{{ prog.title }}</td>
                {% endif %}                
            </tr>
            {% if prog.ifsubprog %}
                {% for eachsubprog in prog.subprog %}
                    {% assign sescount = sescount | plus:1 %}
                    <tr>
                        <td> </td>
                        {% if eachsubprog.id %}
                            <td> <a href="{{ site.relative_url }}/sessions/ses-{{ eachsubprog.id | downcase }}.html"> {{sescount | append: ". "}}{{ eachsubprog.name }} </a>(organizer: {{ eachsubprog.organizer}})</td>
                        {% else %}
                            <td> <div style="color:red;"> {{sescount | append: ". "}}{{ eachsubprog.name }} </div>(organizer: {{ eachsubprog.organizer}})</td>
                        {% endif %}                        
                    </tr>
                {% endfor %}
            {% endif %}
        {% endfor %}
  </table>

{% endfor %}