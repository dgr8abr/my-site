---
layout: default
permalink: /blogs
title: A.I.B -- Blogs
page_title: Blogs

page_link_phrase_2 : Welcome to my Blogs page, here you can view all the things about me, now check all my blogs below. Click here to be updated with my RSS feeds.

page_link_phrase : sales professional
---	

<div class="p-4 mt-2">
	{% for post in site.posts %}
	<div>
		<a href="{{ post.url }}" class="text-xl text-grey-dark font-bold no-underline hover:text-black">
			{{ post.title }}    
		</a>
	</div>
	<p class="text-grey-darkest text-base leading-normal mt-1">
			 {{ post.content | markdownify | strip_html | truncatewords: 20 }}
	</p>
	<div class="mb-8 text-grey-darkest text-base leading-normal mt-2">
		<a href="" class="text-grey-darker hover:text-black text-sm no-underline hover:underline">Read this blog post that was Posted on : {{ post.date | date_to_string }} </a>
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