---
layout: home
title: "Blog"
---

## Post

<div class="row g-5 mb-5">
  <div class="col-md-12">
    {% for post in site.posts %}
      <p><a href="{{ site.github.url }}/{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%B %-d, %Y" }}</p>
    {% endfor %}
  </div>
  </div>
</div>