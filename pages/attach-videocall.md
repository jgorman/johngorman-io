---
layout: page
title: Attach Video Call
desc: Attach video call.
permalink: /attach-videocall/
---

# Attach Video Call

<div style="height: 60vh"
  class="attach-videocall"
  data-api-key="dev_web_SoVksz30pxAMPFcT_23U9BguSSYztLHlE"
  Xdata-api-key="prod_web_BF7EISmegubLJ2d5mWSQynTDF1WjmW0A"
  data-room:url="https://johngorman.io"
  data-videocall:local-background-color="steelblue"
  data-videocall:remote-background-color="steelblue"
  data-videocall:button-background-color="#FFC730"
  data-videocall:local-preview=
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
        if (attr.name.substr(0, 5) != 'data-') continue;
        var name = 'attach:' + attr.name.substring(5);
        var meta = document.createElement('meta');
        meta.setAttribute('property', name);
        meta.content = attr.value;
        head.appendChild(meta);
      }
    })
  }
  attach_setup();
</script>

<script src="https://video.attach.live/v1" defer></script>
