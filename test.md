---
layout: home
title: "Test"
---

## Test Page

<a href="https://github.com/zhutaosheng/zhutaosheng.github.io/edit/main/{{ page.path }}" target="_blank" rel="noopener noreferrer">Edit on GitHub</a>


<p><a href="{{ site.github.url }}">site.github.url</a></p>
<p><a href="{{ github.url }}">github.url</a></p>
<p><a href="{{ site.url }}">site.url</a></p>
<p><a href="{{ site }}">site</a></p>
<p><a href="{{ url }}">url</a></p>
<p><a href="{{ url.site }}">url.site</a></p>


<div class="row g-5 mb-5">
  <div class="col-md-12">
    {% for post in site.posts %}
      <p><a href="{{ site.github.url }}/{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%B %-d, %Y" }}</p>
    {% endfor %}
  </div>
</div>
