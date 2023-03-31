

```

url: "https://www.zhutaosheng.com" # the base hostname & protocol for your site, e.g. http://example.com
baseurl: "/blog" # the subpath of your site, e.g. /blog
title: "Zhutao Sheng" # the name of your site, e.g. ACME Corp.
description: "The only way to do great work is to love what you do - Steve Jobs"

---
permalink: /404.html
---
------------------------------------------------------

## home-water-is-not-wet.png
<div style="text-align:center;">
<img src="/assets/img/home-water-is-not-wet.png" width="400" /><br />
<small>Water is not wet. "Wet" is just a term people use to describe the feeling of water.</small><br />
<small>Image source:
<a href="https://unsplash.com/photos/V-afy242gY4">
Johnny Brown, CC0, via Unsplash
</a></small>
</div>


<br>

## Coding 🐙
<img class="6563686f202d6e202234636550757368324d61696e22207c20787864" src="https://user-images.githubusercontent.com/3750940/100553934-25a84a00-325f-11eb-974e-f5b61dcb44b3.png" height="172" alt="Zhutao hard at work" /> <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=zhutaosheng&layout=compact&theme=vue&hide=PHP&langs_count=6" height="172" alt="Top languages card" />    

<br>


------------------------------------------------------
<img src="/assets/img/2023-Maine-Cultures/DSC01102.jpg" width="100%">

<img src="/assets/img/my-bike/mybike.JPG" alt="My bike" width="100%">


<br>
------------------------------------------------------

## Instagram update!📸 

*Don't forget to leave a like and a comment to let me know what you think! 😊* [@zhtuao.s](https://www.instagram.com/zhtuao.s)

<div class="row g-5 mb-5">

{% include instagram-SnapWidget.html %}

</div>

------------------------------------------------------
## picture include
<div style="text-align:center;">
<img src="{{ site.github.url }}/assets/img/home-water-is-not-wet.png" width="400" /><br />
<small>Water is not wet. "Wet" is just a term people use to describe the feeling of water.</small><br />
<small>Image source:
<a href="https://unsplash.com/photos/V-afy242gY4">
Johnny Brown, CC0, via Unsplash
</a></small>
</div>

------------------------------------------------------

## contact
<div class="row g-5 mb-5">
  <div>
    <h3 class="fw-bold border-bottom pb-3 mb-5">Contact</h3>
    {% for contact in site.data.settings.contacts %}
    <div class="row g-5 mb-5">
      <div class="col-md-8">
        <h4>{{ contact.name }}</h4>
        <p>Email: {{ contact.email }}</p>
        <p>Department: {{ contact.department }}</p>
        <p>Institution: {{ contact.institution }}</p>
      </div>
      <div class="col-md-4">
        <img src="{{ site.github.url }}/{{ contact.image }}" alt="Contact" width="50%">
      </div>
    </div>
    {% endfor %}
  </div>
</div> 


------------------------------------------------------

## include publications.html
<div class="row g-5 mb-5">
  <div>
    <h3 class="fw-bold border-bottom pb-3 mb-5">Publications</h3>
    {% if page.title == "Home" %}
      {% for item in site.data.publications.featured %}
        <p><a href="{{ item.url }}">{{ item.name }}</a></p>
      {% endfor %}
    {% else %}
      {% for item in site.data.publications.index %}
        <p><a href="{{ item.url }}">{{ item.name }}</a></p>
      {% endfor %}
    {% endif %}
  </div>
</div>


## layout/contact.html
{% for contact in site.data.settings.contacts %}
<div class="row g-5 mb-5">
<div class="col-md-8">
    <h4>{{ contact.name }}</h4>
    <p>Email: {{ contact.email }}</p>
    <p>Department: {{ contact.department }}</p>
    <p>Institution: {{ contact.institution }}</p>
</div>
<div class="col-md-4">
    <img src="{{ site.github.url }}/{{ contact.image }}" alt="Contact" width="50%">
</div>
</div>
{% endfor %}
------------------------------------------------------
## Comments System

<div id="disqus_thread"></div>
<script>
    /**
    *  RECOMMENDED CONFIGURATION VARIABLES: EDIT AND UNCOMMENT THE SECTION BELOW TO INSERT DYNAMIC VALUES FROM YOUR PLATFORM OR CMS.
    *  LEARN WHY DEFINING THESE VARIABLES IS IMPORTANT: https://disqus.com/admin/universalcode/#configuration-variables    */
    
    var disqus_config = function () {
    this.page.url = 'https://www.zhutaosheng.com/{{ page.url }}';
    this.page.identifier = '{{ page.url | absolute_url }}';
    };
    
    /*
    var disqus_config = function () {
    this.page.url = PAGE_URL;  // Replace PAGE_URL with your page's canonical URL variable
    this.page.identifier = PAGE_IDENTIFIER; // Replace PAGE_IDENTIFIER with your page's unique identifier variable
    };
    */
    (function() { // DON'T EDIT BELOW THIS LINE
    var d = document, s = d.createElement('script');
    s.src = 'https://zhutao.disqus.com/embed.js';
    s.setAttribute('data-timestamp', +new Date());
    (d.head || d.body).appendChild(s);
    })();
</script>
<noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>
------------------------------------------------------




```