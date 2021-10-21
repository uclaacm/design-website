---
title: ""
pagination:
  data: events
  size: 1
  alias: event
  addAllPagesToCollections: true
layout: page.html
renderData:
  title: "{{ event.title }}"
permalink: "/events/{{ event.filename }}/"
tags:
---
<section>
	<p class="title">{{ event.title }} </p>
	<p>{{ event.month }} {{event.date}}</p>
	<p>{{ event.time }}</p>
	<a href="{{ event.link }}">{{ event.linkname }}</a><br>
	<img src="{{ site.baseurl }}/assets/events/{{ event.image }}"></img>
	<p>{{ event.description }}</p>
</section>