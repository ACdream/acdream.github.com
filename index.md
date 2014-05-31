---
published: true
layout: "no-section"
title: ACdream
---

<!--<link rel="stylesheet" href="http://fonts.googleapis.com/css?family=Gloria+Hallelujah|Cabin+Sketch:700"/>-->
<section id="about">

<!--[if lt IE 9]>
<link rel="stylesheet" href="http://fonts.googleapis.com/css?family=Arvo|Amethysta"/>
<h1 style='color: rgb(0, 3, 85);font-family: "Arvo"; font-size: 2000%; line-height: 1.0em; margin: 0 0 0 0; text-align: center;'>ACdream Page</h1>
<![endif]-->

<!--[if !IE]>-->
<link href='/files/fonts/CherrySwash.css' rel='stylesheet' type='text/css'>
<img src="http://acdream.info/img/logo.png"></img>
<h1 style='color: rgb(0, 3, 85);font-family: "Cherry Swash",cursive; font-size: 200%; line-height: 3.0em; margin: 0 0 0 0; text-align: center;'>ACdream Page</h1>

 
</section>
<section id="posts">
  <h1>Wall of New Posts <img src="http://pic.yupoo.com/van9ogh_v/CXOI1D3s/KaYE.png" alt="feed" style="width: 300px" ></a></h1>
  <ul class="posts">
{% assign count = 0 %}
{% for post in site.posts %}
  {% assign count = count | plus: 1 %}
  {% if count < 12 %} 
  <li><span class="date">{{ post.date | date_to_string }}</span> -
  <a href="{{ post.url }}"{% if post.subtitle %} title="{{ post.subtitle | escape }}"{% endif %}><strong>{{ post.title }}</strong></a></li>
  {% endif %}
{% endfor %}
  </ul>
  <li style="text-align: right" ><a href="archive.html"><strong>Click Here, More! >> </strong></a></li>
</section>
