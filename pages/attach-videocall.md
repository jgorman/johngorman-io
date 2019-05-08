---
layout: page
title: Attach Video Call
desc: Attach video call.
permalink: /attach-videocall/
---

# Attach Video Call

{% capture text-capture %}
```html
<div style="height: 60vh" class="attach-videocall" />

<script>
  function setMeta(name, value) {
    var meta = document.createElement('meta');
    meta.setAttribute('property', name);
    meta.content = value;
    document.head.appendChild(meta);
  }
  setMeta('attach:api-key', 'prod_web_BF7EISmegubLJ2d5mWSQynTDF1WjmW0A');
  setMeta('attach:room:url', 'https://johngorman.io');
  setMeta('attach:videocall:local-background-color', 'steelblue');
  setMeta('attach:videocall:remote-background-color', 'steelblue');
  setMeta('attach:videocall:local-preview',
    'https://assets.attach.live/unsplash/john-cobb-14128.jpg');
</script>

<script src="https://video.attach.live/v1" defer></script>
```
{% endcapture %}

{% include widgets/toggle-field.html
   toggle-name="toggle-thats"
   button-text="View Code"
   toggle-text=text-capture %}

<div style="height: 60vh" class="attach-videocall" />

<script>
  function setMeta(name, value) {
    var meta = document.createElement('meta');
    meta.setAttribute('property', name);
    meta.content = value;
    document.head.appendChild(meta);
  }
  //setMeta('attach:api-key', 'dev_web_SoVksz30pxAMPFcT_23U9BguSSYztLHlE');
  setMeta('attach:api-key', 'prod_web_BF7EISmegubLJ2d5mWSQynTDF1WjmW0A');
  setMeta('attach:room:url', 'https://johngorman.io');
  setMeta('attach:videocall:local-background-color', 'steelblue');
  setMeta('attach:videocall:remote-background-color', 'steelblue');
  setMeta('attach:videocall:local-preview',
    'https://assets.attach.live/unsplash/john-cobb-14128.jpg');
</script>

<script src="https://video.attach.live/v1" defer></script>
