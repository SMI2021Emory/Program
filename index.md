---
title: Test Site for SMI 2021 Program
---
### Test Site for SMI 2021 Program

Potentially store abstract/session information on this site

[invited sessions](docs/ses-invited.md)

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
                        <td>{{ eachsubprog.name }} (organizer: {{ eachsubprog.organizer}})</td>
                    </tr>
                {% endfor %}
            {% endif %}
        {% endfor %}
  </table>

{% endfor %}