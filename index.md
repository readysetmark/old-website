---
layout : layout
title : Home
---

<div class="entry-container">
	<div class='entry'>
		<h1 class="entry">All Posts</h1>
		<ul class="postArchive">
		{% for post in site.posts %}
			<li>
				<span class="postdate"> {{ post.date | date: "%e %B, %Y"  }} </span> <a class="postlink" href="{{ post.id }}">{{ post.title }}</a>
			</li>
		{% endfor %}
		</ul>
	</div>
</div>


