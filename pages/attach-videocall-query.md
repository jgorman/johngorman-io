---
layout: page
title: Attach Video Call Query
desc: Attach video call.
permalink: /attach-videocall-query/
---
{% include env.html env="dev" %}

# {{ page.title }}

{% capture text-capture %}
```html
<div style="height: 60vh" class="attach-videocall" />

<script src="{{sdk_url}}#api-key={{api_key}}&room:url={{room_url}}&videocall:local-background-color=steelblue&videocall:remote-background-color=steelblue&videocall:local-preview=https://assets.attach.live/unsplash/john-cobb-14128.jpg&participants:avatar-border-radius=square&user:username=Charlotte&user:avatar=https://avatars.attach.live/avatar11.png"></script>
```
{% endcapture %}

{% include widgets/toggle-field.html
   toggle-name="toggle-thats"
   button-text="View Code"
   toggle-text=text-capture %}

<div style="height: 60vh" class="attach-videocall" />

<script src="{{sdk_url}}#api-key={{api_key}}&room:url={{room_url}}&videocall:local-background-color=steelblue&videocall:remote-background-color=steelblue&videocall:local-preview=https://assets.attach.live/unsplash/john-cobb-14128.jpg&participants:avatar-border-radius=square&user:username=Charlotte&user:avatar=https://avatars.attach.live/avatar11.png"></script>
