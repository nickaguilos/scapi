---
layout: default
image: /assets/images/og-image.jpg
---

<div class="archive fixed-width-container">
	<h1 class="section-heading">Updates</h1>

	{% for post in site.posts %}
	<div class="">
	    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
	    <div class="date-author">
	        <span class="author">{{ post.author }}</span> &middot;
	        <span class="post-meta">{{ post.date | date_to_long_string }}</span>
	    </div>
	    <p>{{ post.description }}</p>
	</div>
	{% endfor %}
</div>