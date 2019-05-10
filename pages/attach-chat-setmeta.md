---
layout: page
title: Attach Chat setMeta
desc: Attach chat room.
permalink: /attach-chat-setmeta/
---
{% include env.html %}

# {{ page.title }}

This is the original `setMeta()` example.

{% capture text-capture %}
```html
<div style="height: 65vh">
  <div style="height: 60vh" class="attach-chat" />
</div>

<script src="{{sdk_url}}"></script>

<script>
  function setMeta(name, value) {
    var meta = document.createElement('meta');
    meta.setAttribute('property', name);
    meta.content = value;
    document.head.appendChild(meta);
  }
  setMeta('attach:api-key', '{{api_key}}');
  setMeta('attach:room:url', '{{room_url}}');
  setMeta('attach:chat:viewer-background-color', '#20B2AA');
  setMeta('attach:chat:editor-background-color', 'orangeRed');
  setMeta('attach:participants:avatar-border-radius', 'square');
  setMeta('attach:user:username', 'Charlotte');
  setMeta('attach:user:avatar', 'https://avatars.attach.live/avatar11.png');
</script>
```
{% endcapture %}

{% include widgets/toggle-field.html
   toggle-name="toggle-thats"
   button-text="View Code"
   toggle-text=text-capture %}

<div style="height: 65vh">
  <div style="height: 60vh" class="attach-chat" />
</div>

<script src="{{sdk_url}}"></script>

<script>
  function setMeta(name, value) {
    var meta = document.createElement('meta');
    meta.setAttribute('property', name);
    meta.content = value;
    document.head.appendChild(meta);
  }
  setMeta('attach:api-key', '{{api_key}}');
  setMeta('attach:room:url', '{{room_url}}');
  setMeta('attach:chat:viewer-background-color', '#20B2AA');
  setMeta('attach:chat:editor-background-color', 'orangeRed');
  setMeta('attach:participants:avatar-border-radius', 'square');
  setMeta('attach:user:username', 'Charlotte');
  setMeta('attach:user:avatar', 'https://avatars.attach.live/avatar11.png');
</script>
