---
layout: page
title: blog
description: The Blog of Richard Van
---


<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>



<!--
### Ideas to write about

- My experience of quitting my job and traveling the world
- My experience unplugging from technology while traveling
- My experience with Windows -> Mac-->
