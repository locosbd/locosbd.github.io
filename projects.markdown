---
title: Projects
date: 2019-06-11 00:36:00 Z
layout: page
---

<h1 class="page-title">{{ page.title | escape }}</h1>

## **Ongoing Projects:**

{% for post in site.categories.Ongoing %}
          <span class="title"><a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></span>
          <p>
             {{ post.content | truncatewords: 40 }}
          </p>
          <a href="{{ post.url | relative_url }}" class="secondary-content"><i class="material-icons">navigate_next</i></a>
        
        {% endfor %}
       