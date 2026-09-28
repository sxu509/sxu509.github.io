---
title: "Personal"
permalink: /personal/
redirect_from:
  - /life/
gallery:
  - image_path: pp.png
    alt: PP
  - image_path: Bobby.png
    alt: Bobby
---

When I’m not doing research, I love spending time with my partner and our two dogs, **PP and Bobby**. We enjoy going on hikes, taking weekend trips, and exploring new places together—but a lazy day at home with the dogs is pretty great, too.

<div class="personal-photos">
  {% for photo in page.gallery %}
  <figure>
    <img src="{{ photo.image_path | prepend: '/images/' | relative_url }}" alt="{{ photo.alt | escape }}">
    <figcaption>{{ photo.alt }}</figcaption>
  </figure>
  {% endfor %}
</div>
