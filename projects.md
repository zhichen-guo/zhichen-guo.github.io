---
layout: page
title: Projects
permalink: /projects/
---

<ul class="post-list">
    {% assign date_format = site.minima.date_format | default: "%b %-d, %Y" %}
    {% assign posts = site.categories.projects | sort: 'date' | reverse %}
    {% for post in site.categories.projects %}
    <li class="post-item">
        <img src="{{ post.image | relative_url }}"/>
        <div>
        <span class="post-meta">{{ post.date | date: date_format }}</span>
        <h3>
            <a class="post-link" href="{{ post.url | relative_url }}">
            {{ post.title | escape }}
            </a>
            {{ post.excerpt }}
        </h3>
        </div>
    </li>
    {%- endfor -%}
</ul>
