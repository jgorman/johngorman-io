---
layout: page
title: Attach Chat Query
desc: Attach chat room.
permalink: /attach-chat-query/
---

# Attach Chat Query

None of these combinations of `attach:` and [#&] worked.

Currently running the first option: `&attach:`.

{% capture text-capture %}
```html
<div style="height: 65vh">
  <div style="height: 60vh" class="attach-chat" />
</div>

<script src="https://video.attach.live/v1#attach:api-key=prod_web_BF7EISmegubLJ2d5mWSQynTDF1WjmW0A&attach:room:url=https://johngorman.io" defer></script>

<script src="https://video.attach.live/v1#attach:api-key=prod_web_BF7EISmegubLJ2d5mWSQynTDF1WjmW0A#attach:room:url=https://johngorman.io" defer></script>

<script src="https://video.attach.live/v1#api-key=prod_web_BF7EISmegubLJ2d5mWSQynTDF1WjmW0A&room:url=https://johngorman.io" defer></script>

<script src="https://video.attach.live/v1#api-key=prod_web_BF7EISmegubLJ2d5mWSQynTDF1WjmW0A#room:url=https://johngorman.io" defer></script>
```
{% endcapture %}

{% include widgets/toggle-field.html
   toggle-name="toggle-thats"
   button-text="View Code"
   toggle-text=text-capture %}

<div style="height: 65vh">
  <div style="height: 60vh" class="attach-chat" />
</div>

<script src="https://video.attach.live/v1#attach:api-key=prod_web_BF7EISmegubLJ2d5mWSQynTDF1WjmW0A&attach:room:url=https://johngorman.io" defer></script>
