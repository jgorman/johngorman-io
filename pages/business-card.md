---
layout: blank
title: Business Card
desc: John Gorman's business card.
permalink: /business-card/
---

<style>

#particles-js
{
  width: 700px;
  height: 400px;
}

#logo-jgio
{
  top: 15px;
}

.text
{
  position: absolute;
  font-size: 30px;
  color: #ffd700;
  opacity: 0.8;
}

.contact
{
  bottom: 10px;
  left: 25px;
}

.skills
{
  bottom: 10px;
  right: 25px;
}

</style>

<div id="particles-js">

  {% include logo-jgio.html %}

  <div class="text contact">
    John Gorman<br/>
    john@johngorman.io<br/>
    US +1-617-804-0412<br/>
    CA +1-902-222-2777
  </div>

  <div class="text skills">
    Applications Done Right<br/>
    Requirements Analysis<br/>
    Database Design<br/>
    Rails & React
  </div>

  <script src="https://cdn.jsdelivr.net/npm/particles.js@2.0.0/particles.min.js" crossorigin="anonymous"></script>
  <script>particlesJS.load('particles-js', '/assets/particles.json');</script>

</div>

