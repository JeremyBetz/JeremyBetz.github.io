---
layout: page
title: Archive
permalink: /archive/
---

Earlier writing and project notes are kept here as a record of the site’s history.

<ul class="archive-list">
{% for post in site.posts %}
  <li>
    <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
    <span class="date">{{ post.date | date: "%B %e, %Y" }}</span>
  </li>
{% endfor %}
</ul>
