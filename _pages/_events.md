---
layout: page
title: Events
permalink: "/events/"
---

<section class="featured">
	<div class="left">
		<p>This Week</p>
		<a class="button" href="{{ events[0].link }}">Join the Event</a>
	</div>
	<img class="right" src="{{ site.baseurl }}/assets/events/{{ events[0].image }}">
</section>

<section class="events">
	<p class="title">Upcoming</p>
	{% for event in events %}<div class="date">{{ event.month }}<br>{{ event.day }}</div>
		<div class="event-info">
			<a class="link" href="{{ site.baseurl}}/events/{{event.filename }}">{{ event.title }}</a><br>
			{{ event.time }}<br>
			<a href="{{ event.link }}">{{ event.linkname }}</a><br><br>
			{{ event.description }}
		</div>
		<div class="event-image">
			<img width="250px" src="{{ site.baseurl }}/assets/events/{{ event.image }}">
		</div>{% endfor %}
	
</section>
<section class="recordings">
	<p class="title">Past Recordings</p>
	{% for recording in recordings %}<a class="recording" href="{{ recording.link }}">{{ recording.title }}</a>
		<hr>{% endfor %}
	<a class="more" href="{{ site.baseurl }}/recordings/">See More</a>

</section>