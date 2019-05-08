---
layout: page
title: Attach Chat Data
desc: Attach chat room.
permalink: /attach-chat-data/
---

# Attach Chat Data

{% capture text-capture %}
```html
<div style="height: 65vh">
  <div style="height: 60vh"
    class="attach-chat"
    data-api-key="prod_web_BF7EISmegubLJ2d5mWSQynTDF1WjmW0A"
    data-room:url="https://johngorman.io"
    data-chat:viewer-background-color="#20B2AA"
    data-chat:editor-background-color="orangeRed"
    data-participants:avatar-border-radius="square"
    data-user:username="Charlotte"
    data-user:avatar="https://avatars.attach.live/avatar11.png"
  />
</div>

<script>
  function attach_setup() {
    var boxes = Array.from(document.getElementsByClassName('attach-videocall'))
        .concat(Array.from(document.getElementsByClassName('attach-chat')));
    boxes.forEach(function(box) {
      var attrs = box.attributes;
      for (var ii = 0; ii < attrs.length; ii++) {
        var attr = attrs.item(ii);
        if (attr.name.substr(0, 5) != 'data-') continue;
        var name = 'attach:' + attr.name.substring(5);
        var meta = document.createElement('meta');
        meta.setAttribute('property', name);
        meta.content = attr.value;
        document.head.appendChild(meta);
      }
    })
  }
  attach_setup();
</script>

<script src="https://video.attach.live/v1" defer></script>
```
{% endcapture %}

{% include widgets/toggle-field.html
   toggle-name="toggle-thats"
   button-text="View Code"
   toggle-text=text-capture %}

<div style="height: 65vh">
  <div style="height: 60vh"
    class="attach-chat"
    Xdata-api-key="dev_web_SoVksz30pxAMPFcT_23U9BguSSYztLHlE"
    data-api-key="prod_web_BF7EISmegubLJ2d5mWSQynTDF1WjmW0A"
    data-room:url="https://johngorman.io"
    data-chat:viewer-background-color="#20B2AA"
    data-chat:editor-background-color="orangeRed"
    data-participants:avatar-border-radius="square"
    data-user:username="Charlotte"
    data-user:avatar="https://avatars.attach.live/avatar11.png"
  />
</div>

<script>
  function attach_setup() {
    var boxes = Array.from(document.getElementsByClassName('attach-videocall'))
        .concat(Array.from(document.getElementsByClassName('attach-chat')));
    boxes.forEach(function(box) {
      var attrs = box.attributes;
      for (var ii = 0; ii < attrs.length; ii++) {
        var attr = attrs.item(ii);
        if (attr.name.substr(0, 5) != 'data-') continue;
        var name = 'attach:' + attr.name.substring(5);
        var meta = document.createElement('meta');
        meta.setAttribute('property', name);
        meta.content = attr.value;
        document.head.appendChild(meta);
      }
    })
  }
  attach_setup();
</script>

<script src="https://video.attach.live/v1" defer></script>
