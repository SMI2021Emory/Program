---
title : Founder's talk
layout: default
order : 1
---

# {{page.title}}

{% assign sorted_sessions = site.session | sort:"order" %}
{% for session in sorted_sessions %}
  {% if session.type == "founder" %}
  <h2>
    <a href="{{ session.url | prepend: site.relative_url }}">
      {{ session.title }}
    </a>
  </h2>



  {% for speaker in session.speakers %}
  <p> 
  <b>{{speaker.name}}</b><br/>
    {{speaker.affil}} <br/> 
  {% if speaker.email %}
  Email: {{speaker.email}} <br/> 
  {% endif %}
  {% endfor %}


  <!-- <p>{{ session.content | markdownify }}</p> -->
  {% endif %}
{% endfor %}