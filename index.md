---
permalink: /
title: "Home"
layout: single
author_profile: true
classes: wide
search: true
---

### <i class="fas fa-flask"> Research interests

Our main research interests are on the performance evaluation, simulation, design and experimentation on networked systems with particular focus on Programmable networks, Traffic generation, and Network Monitoring.

### <i class="fas fa-newspaper"></i> News

<ul  style="list-style-type:none;">
{% for post in site.posts limit:5 %}
  <li> <a href="{{ post.url }}"><b>{{ post.date | date: "%Y-%m" }}:</b> {{ post.title }}</a> </li>
{% endfor %}
</ul>

### <i class="fas fa-newspaper"> Publications

{% bibliography %}

<script>
  dets=document.getElementsByName("det");
  console.log(5+1);
  for(let i = 0; i < dets.length; i++) {
    dets[i].addEventListener("toggle", (event) => {
      if (dets[i].open) {
        dets[i].style.display = "block";
      }
      else{
        dets[i].style.display = "inline-block"; 
      }
    });
   }
</script>