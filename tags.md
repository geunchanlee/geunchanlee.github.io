---
layout: page
title: Tags
permalink: /tags/
description: >
    List of all tags
---

<div class="tags">
  <ul>
    {% for tag in site.tags %}
      <li>
        <b>
        <a href="{{ site.baseurl }}/tags/{{ tag[0] | downcase }}">{{ tag[0] | capitalize }}</a> [{{ tag[1].size }}]
        </b>
      </li>
    {% endfor %}
  </ul>
</div>