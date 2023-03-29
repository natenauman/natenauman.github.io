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
			<h1>Personal Interests and Activities</h1>
		</header>

<!-- Content -->
Some of my extracurricular passions include oil painting, mountain climbing, running, and language-learning. I never get tired of studying new languages because it allows me to travel and connect deeply with people from across the world. I am conversational in French, Arabic, and Bengali. The combination of French and Arabic has allowed me to travel around North Africa on multiple occasions: I lived with a host family in Rabat, Morocco for 3 months after graduating high school and I embarked on a week of solo-traveling in Tunisia during the summer of 2022. Bengali is one of the richest languages on the planet since it boasts exceptional poetry and beautiful songs, and I was surprised to find that Bengali is more widely spoken than French. I recently won the State Department's Critical Language Scholarship to study Bengali full-time in Kolkata, India from June to August.<br><br>
	
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


<h2 style="text-align:center">Honors College Study Abroad in Italy (2022)</h2>
	In the summer of 2022, I traveled to Italy to explore its rich history and culture from the medieval period to the postmodern present. Italy is especially unique since all of these cultural and philosophical movements coexist beautifully. A significant amount of medieval, Renaissance, and modern architecture is well-preserved. This intensive study abroad was made possible by Purdue University's Honors College.<br><br>
	
<div class="slideshow-container">
  <div class="mySlides2">
    <img src="assets/images/italy_1.png" style="width:100%">
  </div>

  <div class="mySlides2">
    <img src="assets/images/italy_2.png" style="width:100%">
  </div>

  <div class="mySlides2">
    <img src="assets/images/italy_3.png" style="width:100%">
  </div>
	
  <div class="mySlides2">
    <img src="assets/images/italy_4.png" style="width:100%">
  </div>

  <a class="prev" onclick="plusSlides(-1, 1)">&#10094;</a>
  <a class="next" onclick="plusSlides(1, 1)">&#10095;</a>
</div>

<br><br>
	
<h2 style="text-align:center">Studying Arabic full-time in Rabat, Morocco (2019)</h2>
	In the summer of 2019, I received a full scholarship from the State Department to study Arabic through immersion. I had the privilege of volunteering at two centers in Rabat, Morocco by cooking and serving food. One of these two institutions was a women’s hospital. As I brought fried sweets to each woman’s bed, I listened to their stories, hopes, and hardships. This was one of the most humbling experiences of my life.<br><br>

<div class="slideshow-container">
  <div class="mySlides1">
    <img src="assets/images/rabat.png" style="width:100%">
  </div>
	
  <div class="mySlides1">
    <img src="assets/images/sunset.jpg" style="width:100%">
  </div>
	
  <div class="mySlides1">
    <img src="assets/images/ismael.jpg" style="width:100%">
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
