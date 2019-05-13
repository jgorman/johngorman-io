---
layout: page
title: Attach Chat Data Attributes
desc: Attach chat room.
permalink: /attach-chat-data/
---
{% include env.html %}

# {{ page.title }}

This is a working illustration of what using data attributes within
the target div could look like.

This contains a little snippet of code that translates `data-room-url` into
`room:url`.

{% capture text-capture %}
```html
<div style="height: 65vh">
  <div style="height: 60vh"
    class="attach-chat"
    data-api-key="{{api_key}}"
    data-room-url="{{room_url}}"
    data-chat-viewer-background-color="#20B2AA"
    data-chat-editor-background-color="orangeRed"
    data-participants-avatar-border-radius="square"
    data-user-username="Charlotte"
    data-user-avatar="https://avatars.attach.live/avatar11.png"
  />
</div>

<script src="{{sdk_url}}"></script>

<script>
  function attach_setup() {
    var tops = 'user room participants videocall chat overlay'.split(' ');
    var divs = Array.from(document.getElementsByClassName('attach-videocall'))
       .concat(Array.from(document.getElementsByClassName('attach-chat')));
    divs.forEach(function(div) {
      var attrs = div.attributes;
      for (var ii = 0; ii < attrs.length; ii++) {
        var attr = attrs.item(ii);
        if (attr.name.substr(0, 5) != 'data-') continue;

        // Translate data-room-url to attach:room:url
        var name = attr.name.substring(5);
        for (var jj = 0; jj < tops.length; jj++) {
          var top = tops[jj];
          if (name.substring(0, top.length + 1) == (top + '-')) {
            name = top + ':' + name.substring(top.length + 1);
            break;
          }
        }
        var name = 'attach:' + name;

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
    data-room-url="{{room_url}}"
    data-chat-viewer-background-color="#20B2AA"
    data-chat-editor-background-color="orangeRed"
    data-participants-avatar-border-radius="square"
    data-user-username="Charlotte"
    data-user-avatar="https://avatars.attach.live/avatar11.png"
  />
</div>

<script src="{{sdk_url}}"></script>

<script>
  function attach_setup() {
    var tops = 'user room participants videocall chat overlay'.split(' ');
    var divs = Array.from(document.getElementsByClassName('attach-videocall'))
       .concat(Array.from(document.getElementsByClassName('attach-chat')));
    divs.forEach(function(div) {
      var attrs = div.attributes;
      for (var ii = 0; ii < attrs.length; ii++) {
        var attr = attrs.item(ii);
        if (attr.name.substr(0, 5) != 'data-') continue;

        // Translate data-room-url to attach:room:url
        var name = attr.name.substring(5);
        for (var jj = 0; jj < tops.length; jj++) {
          var top = tops[jj];
          if (name.substring(0, top.length + 1) == (top + '-')) {
            name = top + ':' + name.substring(top.length + 1);
            break;
          }
        }
        var name = 'attach:' + name;

        var meta = document.createElement('meta');
        meta.setAttribute('property', name);
        meta.content = attr.value;
        document.head.appendChild(meta);
      }
    })
  }
  attach_setup();
</script>
