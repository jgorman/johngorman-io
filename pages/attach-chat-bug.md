---
layout: page
title: Attach Chat Bug
desc: Attach chat bug.
permalink: /attach-chat-bug/
---

# Attach Chat Bug

Scroll down to the bottom of the page. You will see that the chat text
input box is obscured by the red api key message.

```
    [ATTACH Get your own free api key]
```

The workaround is to wrap the chat div in a taller div.

```
    <div style="height: 65vh">
      <div style="height: 60vh" class="attach-chat" />
    </div>
```

  <div style="height: 120vh"
    class="attach-chat"
    Xattach.api-key="dev_web_SoVksz30pxAMPFcT_23U9BguSSYztLHlE"
    attach.api-key="prod_web_BF7EISmegubLJ2d5mWSQynTDF1WjmW0A"
    attach.room.url="https://johngorman.io"
    attach.chat.viewer-background-color="#20B2AA"
    attach.chat.editor-background-color="orangeRed"
    attach.participants.avatar-border-radius="square"
    attach.user.username="Charlotte"
    attach.user.avatar="https://avatars.attach.live/avatar11.png"
  />

<script>
  function attach_setup() {
    var boxes = Array.from(document.getElementsByClassName('attach-videocall'))
        .concat(Array.from(document.getElementsByClassName('attach-chat')));
    var head = document.getElementsByTagName('head')[0];

    boxes.forEach(function(box) {
      var attrs = box.attributes;
      for (var ii = 0; ii < attrs.length; ii++) {
        var attr = attrs.item(ii);
        if (attr.name.substr(0, 6) != 'attach') continue;
        var meta = document.createElement('meta');
        var name = attr.name.replace(/[_.]/g, ":");
        meta.setAttribute('property', name);
        meta.content = attr.value;
        head.appendChild(meta);
      }
    })
  }
  attach_setup();
</script>

<script src="https://video.attach.live/v1" defer></script>
