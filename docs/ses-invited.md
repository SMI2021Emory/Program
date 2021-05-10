---
title : Invited Sessions
layout: default
order : 1
---

# {{page.title}}

<!-- The links to each invited session are below


| Session Name  | Session Time  | Zoom Link  |
|---|---|---|
| [Statistical methods for neuroimaging studies of Alzheimer’s Disease](invited_sessions/ses-I-1.md)  | May  | Zoom link here  |
| [Statistical methods for neuroimaging studies of Alzheimer’s Disease](invited_sessions/ses-I-1.md)  | May  | Zoom link here  | -->

{% assign sorted_sessions = site.session | sort:"order" %}
{% for session in sorted_sessions %}
  {% if session.type == "invited" %}
  <h2>
    <a href="{{ session.url | prepend: site.relative_url }}">
      Session {{ session.ID }}: {{ session.title }}
    </a>
  </h2>

  <p>
  <b>Organizer</b>: {{session.organizer.name}} <br/> 
   {{session.organizer.affil}} <br/> 
   {% if session.organizer.email %}
   Email: {{session.organizer.email}} <br/> 
   {% endif %}
  </p>
  
  <p>
  <b>Chair</b>: {{session.chair.name}}<br/> 
  {{session.chair.affil}} <br/> 
  {% if session.chair.email %}
  Email: {{session.chair.email}}<br/> 
  {% endif %}
  </p>

<h3> Speakers: </h3>

  {% for speaker in session.speakers %}
  <p> 
  <b>{{speaker.id}}. {{speaker.name}}. {{speaker.speakertime}}</b><br/>
    {{speaker.affil}} <br/> 
  {% if speaker.email %}
  Email: {{speaker.email}} <br/> 
  {% endif %}
  <p> <b>Title</b>: {{speaker.title}} <br/>
  <b> Abstract</b>: {{speaker.abstract}} </p>
  {% endfor %}


  <!-- <p>{{ session.content | markdownify }}</p> -->
  {% endif %}
{% endfor %}
