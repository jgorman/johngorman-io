---
layout: page
title: Attach Chat Data Attributes
desc: Attach chat room.
permalink: /attach-chat-data/
---
{% include env.html %}

# {{ page.title }}

This is a working illustration of what using data attributes within
the target div would look like.

When this is implemented, all of the data attributes will contain
only dashes as separators. Eg: `data-room-url`.

{% capture text-capture %}
```html
<div style="height: 65vh">
  <div style="height: 60vh"
    class="attach-chat"
    data-api-key="{{api_key}}"
    data-room:url="{{room_url}}"
    data-chat:viewer-background-color="#20B2AA"
    data-chat:editor-background-color="orangeRed"
    data-participants:avatar-border-radius="square"
    data-user:username="Charlotte"
    data-user:avatar="https://avatars.attach.live/avatar11.png"
  />
</div>

<script src="{{sdk_url}}"></script>

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
```
{% endcapture %}

{% include widgets/toggle-field.html
   toggle-name="toggle-thats"
   button-text="View Code"
   toggle-text=text-capture %}

<div style="height: 65vh">
  <div style="height: 60vh"
    class="attach-chat"
    data-api-key="{{api_key}}"
    data-room:url="{{room_url}}"
    data-chat:viewer-background-color="#20B2AA"
    data-chat:editor-background-color="orangeRed"
    data-participants:avatar-border-radius="square"
    data-user:username="Charlotte"
    data-user:avatar="https://avatars.attach.live/avatar11.png"
  />
</div>

<script src="{{sdk_url}}"></script>

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
