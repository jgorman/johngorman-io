---
layout: page
title: Attach Chat setProperty
desc: Attach chat room.
permalink: /attach-chat-setproperty/
---
{% include env.html %}

# {{ page.title }}

The `setProperty()` function cannot currently set the `api-key` property.

The `room:url` property seems to be set, but it emits an error message.

This example works around this using the `setMeta()` method.

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

  attachSdk.setProperty('attach:chat:viewer-background-color', '#20B2AA');
  attachSdk.setProperty('attach:chat:editor-background-color', 'orangeRed');
  attachSdk.setProperty('attach:participants:avatar-border-radius', 'square');
  attachSdk.setProperty('attach:user:username', 'Charlotte');
  attachSdk.setProperty('attach:user:avatar', 'https://avatars.attach.live/avatar11.png');
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

  attachSdk.setProperty('attach:chat:viewer-background-color', '#20B2AA');
  attachSdk.setProperty('attach:chat:editor-background-color', 'orangeRed');
  attachSdk.setProperty('attach:participants:avatar-border-radius', 'square');
  attachSdk.setProperty('attach:user:username', 'Charlotte');
  attachSdk.setProperty('attach:user:avatar', 'https://avatars.attach.live/avatar11.png');
</script>
