---
title: SMI 2021 Program
---
# SMI 2021 Programs

<!-- Potentially store abstract/session information on this site

[invited sessions](docs/ses-invited.md) -->

{% for daysch in site.data.program.program %}

  <h2> {{daysch.date}} </h2>
  <table class="display" style="width: 100%">
        {% for prog in daysch.dayprog %}
            <tr>
                <td style="width: 140px">{{ prog.time }}</td>
                <td>{{ prog.title }}</td>
            </tr>
            {% if prog.ifsubprog %}
                {% for eachsubprog in prog.subprog %}
                    <tr>
                        <td> </td>
                        {% if eachsubprog.id %}
                            <td> <a href="/{{ eachsubprog.type }}/ses-{{ eachsubprog.id }}.html"> {{eachsubprog.id}} {{ eachsubprog.name }} </a>(organizer: {{ eachsubprog.organizer}})</td>
                        {% else %}
                            <td> <div style="color:red;"> {{eachsubprog.id}} {{ eachsubprog.name }} </div>(organizer: {{ eachsubprog.organizer}})</td>
                        {% endif %}
                        
                    </tr>
                {% endfor %}
            {% endif %}
        {% endfor %}
  </table>

{% endfor %}