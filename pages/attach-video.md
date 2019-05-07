---
layout: page
title: Attach Video
desc: Attach video call.
permalink: /attach-video/
---

# Attach Video

<div style="height: 60vh"
  class="attach-videocall"
  attach.api-key="prod_web_BF7EISmegubLJ2d5mWSQynTDF1WjmW0A"
  attach.room.url="https://johngorman.io"
  attach.videocall.local-background-color="steelblue"
  attach.videocall.remote-background-color="steelblue"
  attach.videocall.button-background-color="#FFC730"
  attach.videocall.local-preview=
    "https://assets.attach.live/unsplash/john-cobb-14128.jpg"
/>

<script>
  function attach_setup() {
    var boxes = Array.from(document.getElementsByClassName('attach-videocall'))
        .concat(Array.from(document.getElementsByClassName('attach-chat')));
    var head = document.getElementsByTagName('head')[0];

    boxes.forEach(function(box) {
      var attrs = box.attributes;
      for (var ii = 0; ii < attrs.length; ii++) {
        var attr = attrs.item(ii);
        if (attr.name.substr(0, 6) != 'attach') continue;
        var meta = document.createElement('meta');
        var name = attr.name.replace(/[_.]/g, ":");
        meta.setAttribute('property', name);
        meta.content = attr.value;
        head.appendChild(meta);
      }
    })
  }
  attach_setup();
</script>

<script src="https://video.attach.live/v1" defer></script>
