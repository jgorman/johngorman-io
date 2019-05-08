---
layout: page
title: Attach Chat setProperty
desc: Attach chat room.
permalink: /attach-chat-setproperty/
---

# Attach Chat setProperty

{% capture text-capture %}
```html
<div style="height: 65vh">
  <div style="height: 60vh" class="attach-chat" />
</div>

<script src="https://video.attach.live/v1"></script>

<script>
  attachSdk.setProperty('attach:api-key', 'dev_web_SoVksz30pxAMPFcT_23U9BguSSYztLHlE');
  attachSdk.setProperty('attach:room:url', 'https://johngorman.io');
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

<script src="https://video.attach.live/v1"></script>

<script>
  attachSdk.setProperty('attach:api-key', 'dev_web_SoVksz30pxAMPFcT_23U9BguSSYztLHlE');
  //attachSdk.setProperty('attach:api-key', 'prod_web_BF7EISmegubLJ2d5mWSQynTDF1WjmW0A');
  attachSdk.setProperty('attach:room:url', 'https://johngorman.io');
  attachSdk.setProperty('attach:chat:viewer-background-color', '#20B2AA');
  attachSdk.setProperty('attach:chat:editor-background-color', 'orangeRed');
  attachSdk.setProperty('attach:participants:avatar-border-radius', 'square');
  attachSdk.setProperty('attach:user:username', 'Charlotte');
  attachSdk.setProperty('attach:user:avatar', 'https://avatars.attach.live/avatar11.png');
</script>
