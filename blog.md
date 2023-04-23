---
layout: home-with-comments
title: "Blog"
---

## Post
*Don’t forget to leave a like and a comment to let me know what you think! 😊*

<div class="row g-5 mb-5">
  <div class="col-md-12">
    {% for post in site.posts %}
      <p><a href="{{ site.github.url }}/{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%B %-d, %Y" }}</p>
    {% endfor %}
  </div>
  </div>
</div>