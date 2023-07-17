---
layout: home
title: "Home"
---

## Homepage 👋

*It was the best of times, it was the worst of times, it was the age of wisdom, it was the age of foolishness, it was the epoch of belief, it was the epoch of incredulity, it was the season of Light, it was the season of Darkness, it was the spring of hope, it was the winter of despair.*



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
