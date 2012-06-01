---
layout : layout
title : Home
---

<div class="entry-container">
	<div class='entry'>
		<h1 class="entry">All Posts</h1>
		<span class="postdate">{{ page.date | date: "%e %B, %Y"  }}
			{% for tag in page.tags %}
				<li><a href="/tag/{{ tag }}">{{ tag }}</a></li>
			{% endfor %}
		</span>
		<ul class="postArchive">
		{% for post in site.posts %}
			<li>
				<span class="olderpostdate"> {{ post.date | date: "%d %b"  }} </span> <a class="postlink" href="{{ post.id }}">{{ post.title }}</a>
			</li>
		{% endfor %}
		</ul>
	</div>
</div>


