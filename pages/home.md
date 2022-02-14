---
title: Home
header: Hey there!
layout: default
permalink: /
---

<img src="/static/site_images/sam.jpg" class="profile_img">


I'm Sam, a Data Engineer, and Musician.

On this site, you can find a number of programming projects I've worked on, as well as a list of the albums I have released or contributed on.

Down below, you can find links to my various social media platforms, where you can get in touch with me.

## Skills
<div class="skills">
  {% assign skills = site.data.skills | sort:"value" | reverse %}
  {% for skill in skills limit:6 %}
    <hr>
    <label>{{skill.name}}</label>
    <br>
    <progress value="{{skill.value}}" max="100"></progress>
  {% endfor %}
  <hr>
</div>
