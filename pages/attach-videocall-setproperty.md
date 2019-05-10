---
layout: page
title: Attach Video Call setProperty
desc: Attach video call.
permalink: /attach-videocall-setproperty/
---
{% include env.html %}

# {{ page.title }}

{% capture text-capture %}
```html
<div style="height: 60vh" class="attach-videocall" />

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

  attachSdk.setProperty('attach:videocall:local-background-color', 'steelblue');
  attachSdk.setProperty('attach:videocall:remote-background-color', 'steelblue');
  attachSdk.setProperty('attach:videocall:local-preview',
    'https://assets.attach.live/unsplash/john-cobb-14128.jpg');
</script>
```
{% endcapture %}

{% include widgets/toggle-field.html
   toggle-name="toggle-thats"
   button-text="View Code"
   toggle-text=text-capture %}

<div style="height: 60vh" class="attach-videocall" />

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

  attachSdk.setProperty('attach:videocall:local-background-color', 'steelblue');
  attachSdk.setProperty('attach:videocall:remote-background-color', 'steelblue');
  attachSdk.setProperty('attach:videocall:local-preview',
    'https://assets.attach.live/unsplash/john-cobb-14128.jpg');
</script>
