---
title : Speakers
layout: default
order : 1
---

{% assign sorted_sessions = site.session | sort:"order" %}

<!-- Founder's talk -->

{% for session in sorted_sessions %}
  {% if session.type == "founder" %}
  <h2 style="color: #120659;">
    <a href="{{ session.url | prepend: site.relative_url }}">
      {{ session.title }}
    </a>
  </h2>

  {% for speaker in session.speakers %}
  
  <b>{{speaker.name}}</b><br/>
    {{speaker.affil}} <br/> 
  <b>Title</b>: <a href="{{ session.url | prepend: site.relative_url }}" style="color: #0073ee;">  {{ speaker.title }} </a><br/>
  {% endfor %}
  {% endif %}
{% endfor %}

<!-- Keynote talk -->

<h2 style="color: #120659;">Keynote Speakers</h2>


{% for session in sorted_sessions %}
  {% if session.type == "keynote" %}
  <!-- <h2>
    <a href="{{ session.url | prepend: site.relative_url }}">
      {{ session.title }}
    </a>
  </h2> -->

  {% for speaker in session.speakers %}
  
  
  <b>{{speaker.name}}</b><br/>
    {{speaker.affil}} <br/> 
  <b>Title</b>: <a href="{{ session.url | prepend: site.relative_url }}" style="color: #0073ee;"> {{speaker.title}}</a> <br/>
  {% endfor %}
  {% endif %}
{% endfor %}


<!-- Short course -->


{% assign scpage = site.pages | where: 'title', 'Short Course' %}

{% for item in scpage %}
<h2 style="color: #120659;">Short Course</h2>({{ item.url | prepend: site.relative_url }})
<b>Hui Lin</b>, Quan Reseacher at Google <br/>
<b>Title</b>: <a href="{{ item.url | prepend: site.relative_url }}" style="color: #0073ee;"> Introduction to Deep Learning <\a>
{% endfor %}


<!-- Software -->

<!--## Statistical Software for Imaging Analysis-->
<h2 style="color: #120659;">Statistical Software for Imaging Analysis</h2>


{% for session in sorted_sessions %}
  {% if session.type == "software" %}
  {% for speaker in session.speakers %}   
  <b>{{speaker.name}}</b>, {{speaker.affil}} <br/> 
  <a href="{{ '/docs/ses-software.html' | prepend: site.relative_url }}" style="color: #0073ee;">  {{speaker.title}} </a><br/>
  {% endfor %}
  {% endif %}
{% endfor %}

<!-- Invited -->

<!-- ## Speakers in Invited Oral Sessions and Collaborative Case-Studies -->
<h2 style="color: #120659;">Speakers in Invited Oral Sessions and Collaborative Case-Studies</h2>


{% assign sorted_speakers = site.data.speaker | sort:"lastname" %}

{% for speaker in sorted_speakers %}
  <b>{{speaker.name}}</b>, {{speaker.affil}} <br/> 
  <b>Title</b>: <a href="{{site.relative_url}}/sessions/ses-{{ speaker.ID | downcase }}.html" style="color: #0073ee;">  {{speaker.title}} </a><br/>
{% endfor %}

