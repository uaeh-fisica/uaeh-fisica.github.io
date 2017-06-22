---
layout: page
permalink: /miembros/
title: Miembros
description: Miembros del grupo de física
---

<ul class="post-list">
{% for miembro in site.miembros reversed %}
    <li>
        <h2><a class="miembro-title" href="{{ miembro.url | prepend: site.baseurl }}">{{ miembro.title }}</a></h2>
        <p>{{ miembro.description }}</p>
        <br/>
        <hr/>
      </li>
{% endfor %}
</ul>


