---
layout: page
title: Personal
description: Travel and language-learning
image: assets/images/tablemountain.jpg
nav-menu: true
---

<!-- Main -->
<div id="main" class="alt">

  <!-- One -->
<section id="one">
	<div class="inner">
		<header class="major">
			<h1>Photography</h1>
		</header>

<!-- Content -->
<h2 id="content">Studying Intermediate Arabic in Rabat, Morocco through NSLI-Y Immersion Program</h2>

<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {box-sizing: border-box}
.mySlides1, .mySlides2 {display: none}
img {vertical-align: middle;}

/* Slideshow container */
.slideshow-container {
  max-width: 1000px;
  position: relative;
  margin: auto;
}

/* Next & previous buttons */
.prev, .next {
  cursor: pointer;
  position: absolute;
  top: 50%;
  width: auto;
  padding: 16px;
  margin-top: -22px;
  color: white;
  font-weight: bold;
  font-size: 18px;
  transition: 0.6s ease;
  border-radius: 0 3px 3px 0;
  user-select: none;
}

/* Position the "next button" to the right */
.next {
  right: 0;
  border-radius: 3px 0 0 3px;
}

/* On hover, add a grey background color */
.prev:hover, .next:hover {
  background-color: #f1f1f1;
  color: black;
}
</style>
</head>
<body>

<h2 style="text-align:center">Multiple Slideshows</h2>

<p>Slideshow 1:</p>
<div class="slideshow-container">
  <div class="mySlides1">
    <img src="assets/images/sunset.jpg" style="width:100%">
  </div>

  <div class="mySlides1">
    <img src="assets/images/ocean.jpg" style="width:100%">
  </div>

  <div class="mySlides1">
    <img src="assets/images/minaret.jpg" style="width:100%">
  </div>

  <a class="prev" onclick="plusSlides(-1, 0)">&#10094;</a>
  <a class="next" onclick="plusSlides(1, 0)">&#10095;</a>
</div>

<p>Slideshow 2:</p>
<div class="slideshow-container">
  <div class="mySlides2">
    <img src="assets/images/minaret.jpg" style="width:100%">
  </div>

  <div class="mySlides2">
    <img src="assets/images/ocean.jpg" style="width:100%">
  </div>

  <div class="mySlides2">
    <img src="assets/images/sunset.jpg" style="width:100%">
  </div>

  <a class="prev" onclick="plusSlides(-1, 1)">&#10094;</a>
  <a class="next" onclick="plusSlides(1, 1)">&#10095;</a>
</div>

<script>
let slideIndex = [1,1];
let slideId = ["mySlides1", "mySlides2"]
showSlides(1, 0);
showSlides(1, 1);

function plusSlides(n, no) {
  showSlides(slideIndex[no] += n, no);
}

function showSlides(n, no) {
  let i;
  let x = document.getElementsByClassName(slideId[no]);
  if (n > x.length) {slideIndex[no] = 1}    
  if (n < 1) {slideIndex[no] = x.length}
  for (i = 0; i < x.length; i++) {
     x[i].style.display = "none";  
  }
  x[slideIndex[no]-1].style.display = "block";  
}
</script>

</body>
</html> 