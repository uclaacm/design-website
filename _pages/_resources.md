---
layout: page
title: Resources
permalink: "/resources/"
---

<div>
<img src="/assets/banners/resources_banner.jpg" style="height: 60vh; width: 100%; object-fit: cover;"/>
</div>

<div class="tabbar">
<button class="tablink" onclick="openPage('UX', this)" id="defaultOpen">UX</button>
<button class="tablink" onclick="openPage('Design', this)">Design</button>
<button class="tablink" onclick="openPage('Developer', this)">Developer</button>
</div>

<div id="UX" class="tabcontent">
<div class="stuff">
  <img width="313" height="210" background="url(http://goo.gl/vyAs27)">
  <div class="container-list">
      <h2>Paper and Pen</h2>
      <p> Overview of common concepts that come up in UX </p>
      <ul>
      <li>Coffee</li>
      <li>Tea</li>
      <li>Milk</li>
      </ul>
  </div>
</div>
<div class="stuff">
  <img width="313" height="210" background="url(http://goo.gl/vyAs27)">
  <div class="container-list">
      <h2>Paper and Pen</h2>
      <p> Overview of common concepts that come up in UX </p>
      <ul>
      <li>Coffee</li>
      <li>Tea</li>
      <li>Milk</li>
      </ul>
  </div>
</div>
</div>

<div id="Design" class="tabcontent">
  <h3>News</h3>
  <p>Some news this fine day!</p> 
</div>

<div id="Developer" class="tabcontent">
  <h3>Contact</h3>
  <p>Get in touch, or swing by for a cup of coffee.</p>
</div>


<script>
function openPage(pageName, elmnt, color) {
  // Hide all elements with class="tabcontent" by default */
  var i, asdf, tablinks;
  asdf = document.getElementsByClassName("tabcontent");
  for (i = 0; i < asdf.length; i++) {
    asdf[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablink");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].style.backgroundColor = "";
  }
  document.getElementById(pageName).style.display = "flex";
  elmnt.style.backgroundColor = color;
}
document.getElementById("defaultOpen").click();
</script>
