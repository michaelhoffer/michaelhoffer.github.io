---
layout: default

---


{% for post in site.posts %}
{% if post.title contains 'Resume' %}
<article class="post">
	<header>
		<div class="title">
			<h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
			<p>{{ post.description }}</p>
		</div>
		<div class="meta">
			<time class="published" datetime="">{{ post.date | date: "%D" }}</time>
			<a href="#" class="author"><span class="name">{{ site.name }}</span><img src="/images/avatar.jpg" alt="" /></a>
		</div>
	</header>
	<!-- <a href="single.html" class="image featured"><img src="images/pic01.jpg" alt="" /></a> -->

	{{ post.content }}

	{% include postfooter.html %}
</article>
{% endif %}
{% endfor %}

			
