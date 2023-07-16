---
layout: default
permalink: /
title: A.I.B
page_title: Blogs
page_intro : Welcome to my site, here you can view all the things about me, now check blogs below.
---

<div class="p-4 bg-grey-lightest">
	{% for post in site.posts %}
	<div>
		<a href="#" class="text-xl text-grey-darker font-bold no-underline hover:text-black">
			{{ post.title }}       
		</a>
	</div>
	<p class="text-grey-darkest text-base leading-normal mt-1">
			 {{ post.content | markdownify | strip_html | truncatewords: 30 }}
	</p>
	<div class="mb-8 text-grey-darkest text-base leading-normal mt-2">
		<a href="" class="text-grey-darker hover:text-black text-sm no-underline hover:underline">Read this blog post &rarr;</a>
	</div>
	{% endfor %}
</div>


<!-- 
<section>
	{% for post in site.posts %}
	<div class="project-container">
		<a href="{{ site.github.url }}/projects/{{ project.url }}">
			<div class="project-unit" data-folder="{{ site.github.url }}/projects/{{ project.url }}" style="background-image: url({{ site.github.url }}/assets/img/projects/{{ project.url }}/thumbnail.jpg)">
				<div class="project-overlay">
					<strong>{{ post.title }} <i class="fa fa-arrow-right" aria-hidden="true"></i></strong>
				</div>
			</div>
		</a>
	</div>
	{% endfor %}
</section>
 -->