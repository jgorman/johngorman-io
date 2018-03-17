---
layout: page
title: johngorman.io
desc: A technology playgound for fun and learning. Currently an exploration
      of React and Ruby on Rails.
---

# Projects

I am learning ReactJS, React Native and related technologies and
this is my place to try things out!

## WiFi Watch

I use this all the time when at coffee shops, airports and at home
to keep an eye on my network connection quality.

When web page loading sucks, is it a problem with their site or
do I have a network issue on my end? If it is my problem is it
due to slowness or are there a lot of dropped packets?
How long has this been going on and is it getting worse? If the
network is completely failing, exactly how long has it been
inaccessible?

I keep wifi-watch running in a terminal tab and I can quickly look
at the tab to answer all of these questions at a glance.

<span style="color:red;">This should be red.</span>
<div id="wifi-watch"/>

<script>
    /*
  alert("A");
  window.onload = function() {
    $.get("http://localhost:3000/summary", function(data, status) {
      alert("Data: " + data + "\nStatus: " + status);
    });
  };
  alert("B");
  */
</script>


## Darkest Night Clock

I wrote the same exact night time clock app in both React.js and in React Native so that both the similarities and the differences between the two environments are clear.

## Cloud Server

I am experimenting with both front end and back end libraries and their deployment so I need to be able to easily spin up services on the open internet.

There is no easier and more flexible method for hosting than to spin up your own cloud server. I chose Linode due to simplicity and cost effectiveness. A 1GB instance costs $5 / month.

Set up [Node, Apache and SSL on Ubuntu](cloud-server).
