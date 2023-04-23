---
layout: home-with-comments
---

## Find Hilarious


<body>
	<div class="slideshow">
		<img src="/assets/img/all-pics/chemistry-joke-1.png" width="100%" height:765px>
        <img src="/assets/img/all-pics/chemistry-joke-2.png" width="100%" height:765px>
        <img src="/assets/img/all-pics/chemistry-joke-3.png" width="100%" height:765px>
        <img src="/assets/img/all-pics/chemistry-joke-4.png" width="100%" height:765px>
        <img src="/assets/img/all-pics/chemistry-joke-5.png" width="100%" height:765px>
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

