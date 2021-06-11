---
layout: page
title: Resources
permalink: "/resources/"
---

<!-- <style>
/* Style tab links */
.tablink {
  background-color: white;
  color: #FE8D3C;
  float: left;
  border: none;
  outline: none;
  cursor: pointer;
  padding: 14px 16px;
  font-size: 17px;
  width: 33%;
}

.tablink:hover {
  background-color: #777;
}

/* Style the tab content (and add height:100% for full page content) */
.asdf {
  flex-direction: row;
  display: flex;
  color: white;
  justify-content:center;
  align-items:center;
  padding: 100px 200px;
  height: 100%;
}
.tabbar{
    padding-top: 100px;
    width:100%;
    display: flex;
    justify-content:center;
}
.container-list{
    display:flex;
    flex-direction:column
}
</style> -->



<div>
<img src="/assets/banners/resources_banner.jpg" style="height: 60vh; width: 100%; object-fit: cover;"/>
</div>

<div class="tabbar">
<button class="tablink" onclick="openPage('UX', this)" id="defaultOpen">UX</button>
<button class="tablink" onclick="openPage('Design', this)">Design</button>
<button class="tablink" onclick="openPage('Developer', this)">Developer</button>
</div>

<div id="UX" class="tabcontent">
<img width="313" height="210" background="url(http://goo.gl/vyAs27)">
<div class="container-list">
    <h1>Paper and Pen</h1>
    <h3>Overview of common concepts that come up in UX</h3>
    <ul>
    <li>Coffee</li>
    <li>Tea</li>
    <li>Milk</li>
    </ul>
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
