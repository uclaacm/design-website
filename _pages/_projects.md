---
layout: page
title: Projects
permalink: "/projects/"
---

<section class="featured">
	<div class="left">
		<p>Featured<br>ACM Styleguide</p>
		<a class="button" href="https://design.uclaacm.com/" >Check it out</a>
	</div>
	<div class="right">
		<img src="{{ site.baseurl }}/assets/projects/designlaptop.png">
	</div>
</section>

<section class="projects">
	<p class="title">Check out our other projects</p>
	{% for project in projects %}<div class="col-3"><div class="links">
		<div class="project-links">
			<a href="{{ site.baseurl }}/projects/{{ project.filename }}"><img src="{{ site.baseurl }}/assets/projects/{{ project.image }}"></a>
		</div><p class="project-names">{{project.title}}</p></div>
	</div>{% endfor %}
</section>

<section>
	<p class="title">We also do graphic design work</p>
	<div class="slideshow">
	{% for design in designs %}<div class="slides"><img class="slideimage" src="{{ site.baseurl }}/assets/designs/{{ design.image }}"></div>{% endfor %}
		<button class="prev" onclick="addIndex(-2)">&#10094;</button>
		<button class="next" onclick="addIndex(2)">&#10095;</button>
	</div>
</section>

<script>
var index = 1;
showIndex(index);

function addIndex(n) {
  showIndex(index += n);
}

function showIndex(n) {
	var i;
	var x = document.getElementsByClassName("slides");
	if (n > x.length) {
		index = 1;
	}
	if (n < 1) {
		index = x.length;
	}
	for (i = 0; i < x.length; i++) {
		x[i].style.display = "none";  
	}
	x[index-1].style.display = "inline-block";
	if (index != x.length) {
		x[index].style.display = "inline-block";
	}
}
</script>