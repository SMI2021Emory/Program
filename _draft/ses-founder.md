---
title : Founder's talk
layout: default
order : 1
---



{% assign sorted_sessions = site.session | sort:"order" %}
{% for session in sorted_sessions %}
  {% if session.type == "founder" %}
  <h1>
    <a href="{{ session.url | prepend: site.relative_url }}">
      {{ session.title }}
    </a>
  </h1>



  {% for speaker in session.speakers %}
  <p> 
  <b>{{speaker.name}}</b><br/>
    {{speaker.affil}} <br/> 
  {% if speaker.email %}
  Email: {{speaker.email}} <br/> 
  {% endif %}
    <b>Title</b>: {{speaker.title}} <br/>
  {% endfor %}


  <!-- <p>{{ session.content | markdownify }}</p> -->
  {% endif %}
{% endfor %}