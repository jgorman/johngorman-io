---
layout: page
title: Attach Chat Set Meta
desc: Attach chat room.
permalink: /attach-chat-setmeta/
---

# Attach Chat Set Meta

{% capture text-capture %}
```html
<div style="height: 65vh">
  <div style="height: 60vh" class="attach-chat" />
</div>

<script>
  function setMeta(name, value) {
    var meta = document.createElement('meta');
    meta.setAttribute('property', name);
    meta.content = value;
    document.head.appendChild(meta);
  }
  setMeta('attach:api-key', 'dev_web_SoVksz30pxAMPFcT_23U9BguSSYztLHlE');
  setMeta('attach:room:url', 'https://johngorman.io');
  setMeta('attach:chat:viewer-background-color', '#20B2AA');
  setMeta('attach:chat:editor-background-color', 'orangeRed');
  setMeta('attach:participants:avatar-border-radius', 'square');
  setMeta('attach:user:username', 'Charlotte');
  setMeta('attach:user:avatar', 'https://avatars.attach.live/avatar11.png');
</script>

<script src="https://video.attach.live/v1" defer></script>
```
{% endcapture %}

{% include widgets/toggle-field.html
   toggle-name="toggle-thats"
   button-text="View Code"
   toggle-text=text-capture %}

<div style="height: 65vh">
  <div style="height: 60vh" class="attach-chat" />
</div>

<script>
  function setMeta(name, value) {
    var meta = document.createElement('meta');
    meta.setAttribute('property', name);
    meta.content = value;
    document.head.appendChild(meta);
  }
  setMeta('attach:api-key', 'dev_web_SoVksz30pxAMPFcT_23U9BguSSYztLHlE');
  setMeta('attach:room:url', 'https://johngorman.io');
  setMeta('attach:chat:viewer-background-color', '#20B2AA');
  setMeta('attach:chat:editor-background-color', 'orangeRed');
  setMeta('attach:participants:avatar-border-radius', 'square');
  setMeta('attach:user:username', 'Charlotte');
  setMeta('attach:user:avatar', 'https://avatars.attach.live/avatar11.png');
</script>

<script src="https://video.attach.live/v1" defer></script>
