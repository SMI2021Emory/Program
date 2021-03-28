---
title: SMI 2021 Programs
---
# SMI 2021 Programs

<!-- Potentially store abstract/session information on this site

[invited sessions](docs/ses-invited.md) -->

{% for daysch in site.data.program.program %}

  <h2> {{daysch.date}} </h2>
  <table style="display: block; width: 100%">
        {% for prog in daysch.dayprog %}
            <tr>
                <td style="width: 140px">{{ prog.time }}</td>
                {% if prog.link %}
                    <td><a href="{{ prog.link | prepend: site.relative_url }}"> {{ prog.title }} </a></td>                    
                {% else %}
                    <td>{{ prog.title }}</td>
                {% endif %}                
            </tr>
            {% if prog.ifsubprog %}
                {% for eachsubprog in prog.subprog %}
                    <tr>
                        <td> </td>
                        {% if eachsubprog.id %}
                            <td> <a href="{{ site.relative_url }}/sessions/ses-{{ eachsubprog.id | downcase }}.html"> {{eachsubprog.id}} {{ eachsubprog.name }} </a>(organizer: {{ eachsubprog.organizer}})</td>
                        {% else %}
                            <td> <div style="color:red;"> {{eachsubprog.id}} {{ eachsubprog.name }} </div>(organizer: {{ eachsubprog.organizer}})</td>
                        {% endif %}                        
                    </tr>
                {% endfor %}
            {% endif %}
        {% endfor %}
  </table>

{% endfor %}