---
layout: page
title: Attach Chat Bug
desc: Attach chat bug.
permalink: /attach-chat-bug/
---
{% include env.html key="dev" %}

# {{ page.title }}

Scroll down to the bottom of the page. You will see that the chat text
input box is obscured by the red api key message.

```
[ATTACH Get your own free api key]
```

The workaround is to wrap the chat div in a taller div.

```html
<div style="height: 65vh">
  <div style="height: 60vh" class="attach-chat" />
</div>
```

{% capture text-capture %}
```html
<div style="height: 100vh" class="attach-chat" />

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

<div style="height: 100vh" class="attach-chat" />

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
