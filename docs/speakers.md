---
title : Speakers
layout: default
order : 1
---

{% assign sorted_sessions = site.session | sort:"order" %}

<!-- Founder's talk -->

{% for session in sorted_sessions %}
  {% if session.type == "founder" %}
  <h2>
    <a href="{{ session.url | prepend: site.relative_url }}">
      {{ session.title }}
    </a>
  </h2>

  {% for speaker in session.speakers %}

  ![Photo]({{speaker.photolink}})
  
  <b>{{speaker.name}}</b><br/>
    {{speaker.affil}} <br/> 
  <b>Title</b>: <a href="{{ session.url | prepend: site.relative_url }}"> {{ speaker.title }} </a><br/>
  {% endfor %}
  {% endif %}
{% endfor %}

<!-- Keynote talk -->

{% for session in sorted_sessions %}
  {% if session.type == "keynote" %}
  <h2>
    <a href="{{ session.url | prepend: site.relative_url }}">
      {{ session.title }}
    </a>
  </h2>

  {% for speaker in session.speakers %}
  
  ![Photo]({{speaker.photolink}})
  
  <b>{{speaker.name}}</b><br/>
    {{speaker.affil}} <br/> 
  <b>Title</b>: <a href="{{ session.url | prepend: site.relative_url }}">{{speaker.title}}</a> <br/>
  {% endfor %}
  {% endif %}
{% endfor %}


<!-- Short course -->


{% assign scpage = site.pages | where: 'title', 'Short Course' %}
{% for item in scpage %}
## [Short course]({{ item.url | prepend: site.relative_url }})
   {{ item.content }}
{% endfor %}


<!-- Software -->

## Statistical Software for Imaging Analysis

{% for session in sorted_sessions %}
  {% if session.type == "software" %}
  {% for speaker in session.speakers %}   
  <b>{{speaker.name}}</b>, {{speaker.affil}} <br/> 
  <a href="{{ session.url | prepend: site.relative_url }}"> {{speaker.title}} </a><br/>
  {% endfor %}
  {% endif %}
{% endfor %}

<!-- Invited -->

## Speakers in Invited Oral Sessions

{% for session in sorted_sessions %}
  {% if session.type == "invited" %}
  {% for speaker in session.speakers %}   
  <b>{{speaker.name}}</b>, {{speaker.affil}} <br/> 
  <a href="{{ session.url | prepend: site.relative_url }}"> {{speaker.title}} </a><br/>
  {% endfor %}
  {% endif %}
{% endfor %}