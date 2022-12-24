---
layout: default

---


{%- comment -%}
{% for post in site.posts %}
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

	{{ post.excerpt }}

	{% include postfooter.html %}
</article>
{% endfor %}
{%- endcomment -%}


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


<!-- Post -->
<!-- 
<article class="post">
	<header>
		<div class="title">
			<h2><a href="single.html">Magna sed adipiscing</a></h2>
			<p>Lorem ipsum dolor amet nullam consequat etiam feugiat</p>
		</div>
		<div class="meta">
			<time class="published" datetime="2015-11-01">November 1, 2015</time>
			<a href="#" class="author"><span class="name">Jane Doe</span><img src="images/avatar.jpg" alt="" /></a>
		</div>
	</header>
	<a href="single.html" class="image featured"><img src="images/pic01.jpg" alt="" /></a>
	<p>Mauris neque quam, fermentum ut nisl vitae, convallis maximus nisl. Sed mattis nunc id lorem euismod placerat. Vivamus porttitor magna enim, ac accumsan tortor cursus at. Phasellus sed ultricies mi non congue ullam corper. Praesent tincidunt sed tellus ut rutrum. Sed vitae justo condimentum, porta lectus vitae, ultricies congue gravida diam non fringilla.</p>
	<footer>
		<ul class="actions">
			<li><a href="single.html" class="button large">Continue Reading</a></li>
		</ul>
		<ul class="stats">
			<li><a href="#">General</a></li>
			<li><a href="#" class="icon solid fa-heart">28</a></li>
			<li><a href="#" class="icon solid fa-comment">128</a></li>
		</ul>
	</footer>
</article>
-->


<!-- Pagination -->
<!-- <ul class="actions pagination">
	<li><a href="" class="disabled button large previous">Previous Page</a></li>
	<li><a href="#" class="button large next">Next Page</a></li>
</ul> -->


			