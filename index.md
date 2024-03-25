---
layout: home
title: "Home"
---

## Hey, I'm Zhutao Sheng 👋

*The fresh air and sunshine can always really make me happy* 



<body>
	<div class="slideshow">
		<img src="/assets/img/home-pic-1.jpg" width="100%">
        <img src="/assets/img/home-pic-2.jpg" width="100%">
	</div>
</body>





<style>
    .slideshow {
        position: relative;
        width: 100%;
        height: 400px;
        overflow: hidden;
    }
    .slideshow img {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        object-fit: cover;
        transition: opacity 1s ease-in-out;
    }
    .slideshow img:last-child {
        opacity: 0;
    }
    .slideshow:hover img:first-child {
        opacity: 0;
    }
    .slideshow:hover img:last-child {
        opacity: 1;
    }
</style>
