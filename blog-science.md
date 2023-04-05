---
layout: default-with-comments
title: "Science Blog"
---

## Science Blog
*Don’t forget to leave a like and a comment to let me know what you think! 😊*

Here is [sample post](/_posts-science/2023-04-05-test.md_)

[Welcome to my science blog](/_posts-science/2023-04-05-Welcome%20to%20my%20science%20blog.md)

<div class="row g-5 mb-5">
  <div class="col-md-12 justify">
    {% for post in site.posts-science %}
      <p><a href="{{ site.github.url }}/{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%B %-d, %Y" }}</p>
    {% endfor %}
  </div>
</div>
