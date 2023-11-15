---
layout: post
title: "I added a comment system to my Website!🚀"
---

🎉🎉🎉 Hey everyone! I am thrilled to announce that I've added a comment system to my page! 🚀🚀🚀 This is a huge milestone for me and I couldn't be happier. 😊

I started off by looking for different comment systems and finally found one that suited my needs - Disqus. The configuration was surprisingly easy! 💻 I created an HTML file with the Disqus code and then included it where I wanted to insert the comment system. And just like that, I did it! Each step was a new learning experience and I'm pleased that I was able to do it successfully. 🙌🏼

```
<div id="disqus_thread"></div>
<script>
var disqus_config = function () {
this.page.url = 'https://www.zhutaosheng.com/{{ page.url }}';
this.page.identifier = '{{ page.url | absolute_url }}';
};

(function() { // DON'T EDIT BELOW THIS LINE
var d = document, s = d.createElement('script');
s.src = 'https://zhutao.disqus.com/embed.js';
s.setAttribute('data-timestamp', +new Date());
(d.head || d.body).appendChild(s);
})();
</script>

<div class="row g-5 mb-5">
  {% include comments.html %}
</div>
```

Now, my website is open to everyone including guests, so please feel free to leave your comments! I would love to hear your thoughts and feedback. 🤗

Adding a comment system has not only enhanced the functionality of my website, but it has also provided me with an opportunity to connect with my audience on a more personal level. 💬 It's amazing to see how technology has made it possible to engage with people from all over the world. 🌎

So, if you haven't already checked out my page, head on over now and drop a comment! Let's connect and have a conversation. 🤝

#Disqus #Website #Feedback