---
layout: blank
title: Business Card
desc: John Gorman's business card.
permalink: /business-card/
---

<style>

#particles-js
{
  background-color: #b61924;
  width: 700px;
  height: 400px;
  position: relative;
}

#logo-jgio
{
  position: absolute;
  top: 30px;
  left: 25px;
  font-size: 50px;
}

#logo
{
  height: 50px;
  width: 50px;
}

#contact
{
  position: absolute;
  top: 100px;
  left: 25px;
  font-size: 30px;
  color: #ffd700;
  opacity: 0.7;
}

#skills
{
  position: absolute;
  bottom: 10px;
  right: 25px;
  font-size: 30px;
  color: #ffd700;
  opacity: 0.7;
}

</style>

<div id="particles-js">

  <div id="logo-jgio">
    <img id="logo" src="/images/jg-logo.svg"/>
    <span style="color:blue">johngorman</span
    ><span style="color:black">.</span
    ><span style="color:red">io</span>
  </div>

  <div id="contact">
    John Gorman<br/>
    john@johngorman.io<br/>
    978-880-2527<br/>
    New York NY
  </div>

  <div id="skills">
    Applications Done Right<br/>
    Requirements Analysis<br/>
    Database Design<br/>
    Rails & React
  </div>

  <script src="https://cdn.jsdelivr.net/npm/particles.js@2.0.0/particles.min.js" crossorigin="anonymous"></script>
  <script>particlesJS.load('particles-js', '/assets/particles.json');</script>

</div>

