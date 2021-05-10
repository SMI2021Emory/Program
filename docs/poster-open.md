---
title : Poster and Opening Mixer
layout: default
order : 4
---

<script>
function showFun(pID,pbnID) {
  var x = document.getElementById(pID);
  var bntext = document.getElementById(pbnID);
  if (x.style.display === "none") {
    x.style.display = "block";
    bntext.innerText = "Hide abstract";
  } else {
    x.style.display = "none";
    bntext.innerText = "Show abstract";
  }  
}
</script>

<script src="{{ site.baseurl }}/assets/js/pdfThumbnails/pdfThumbnails.js" data-pdfjs-src="{{site.baseurl }}/assets/js/pdfThumbnails/build/pdf.js"></script>

<h1 style="color: #120659;"> {{page.title}} </h1>
<h3> Poster Presenters: </h3>



{% for speaker in site.data.poster %}
<div class="poster" style="border: 1px solid black; margin: 20px;padding: 10px; box-shadow: 5px 5px 4px 5px #888888;">
  <div>
  <!-- <img alt= '{{speaker.id | prepend: "poster" }}' data-pdf-thumbnail-file="{{site.baseurl }}/assets/posters/{{speaker.id | prepend: "poster" }}.pdf" style="float: left;width: 22%;padding:1px;margin-right:10px;border: 5px solid Gainsboro"> -->
  <a target="_blank" href="{{site.baseurl }}/assets/posters/{{speaker.id | prepend: "poster" }}.jpg">
  <img class="psimg" alt= '{{speaker.id | prepend: "poster" }}' src="{{site.baseurl }}/assets/posters/{{speaker.id | prepend: "poster" }}.jpg" style="float: left;width: 22%;padding:1px;margin-right:10px;border: 5px solid Gainsboro">
  </a>
  {{speaker.id}}. <b>{{speaker.title}}</b> <br/>
  {{speaker.name}}<br/>
    {{speaker.affil}} 
    <div style="float: right;">
  <button id = "{{speaker.id | prepend: 'poster-bn'}}" class="btn btn-ps" onclick="showFun('{{speaker.id | prepend: "poster" }}','{{speaker.id | prepend: "poster-bn" }}')">Show abstract</button>
  </div><br/> 
  {% if speaker.email %}
  Email: {{speaker.email}}
  {% endif %}
  </div>
  <br/> 
  <div id = "{{speaker.id | prepend: 'poster'}}" style="display: none"> 
  <b> Abstract</b>: {{speaker.abstract}} 
  </div>
</div>
{% endfor %}


