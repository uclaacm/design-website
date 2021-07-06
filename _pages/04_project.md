---
title: ""
pagination:
  data: projects
  size: 1
  alias: project
  addAllPagesToCollections: true
layout: page.html
renderData:
  title: "{{ project.title }}"
permalink: "/projects/{{ project.filename }}/"
tags:
---
<section>
	<p class="title">{{ project.title }} </p>
	<img src="{{ site.baseurl }}/assets/projects/{{ project.image }}"></img>
	<p>{{ project.description }}</p>
</section>