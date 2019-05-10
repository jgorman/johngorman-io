---
layout: page
title: Attach Chat Query
desc: Attach chat room.
permalink: /attach-chat-query/
---
{% include env.html env="dev" %}

# {{ page.title }}

{% capture text-capture %}
```html
<div style="height: 65vh">
  <div style="height: 60vh" class="attach-chat" />
</div>

<script src="{{sdk_url}}#api-key={{api_key}}&room:url={{room_url}}&chat:viewer-background-color=#20B2AA&chat:editor-background-color=orangeRed&participants:avatar-border-radius=square&user:username=Charlotte&user:avatar=https://avatars.attach.live/avatar11.png"></script>
```
{% endcapture %}

{% include widgets/toggle-field.html
   toggle-name="toggle-thats"
   button-text="View Code"
   toggle-text=text-capture %}

<div style="height: 65vh">
  <div style="height: 60vh" class="attach-chat" />
</div>

<script src="{{sdk_url}}#api-key={{api_key}}&room:url={{room_url}}&chat:viewer-background-color=#20B2AA&chat:editor-background-color=orangeRed&participants:avatar-border-radius=square&user:username=Charlotte&user:avatar=https://avatars.attach.live/avatar11.png"></script>
