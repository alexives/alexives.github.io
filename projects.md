---
layout: page
title: Projects
permalink: /projects/
---
I do a variety of projects, from portable kegorators to failing at diy keyboards, all of my project posts get categorized here. Take a look!
<ul class="posts">
{% for post in site.posts %}
  {% if post.layout == 'project' %}
    <li>
      <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
      <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
    </li>
  {% endif %}
{% endfor %}
</ul>