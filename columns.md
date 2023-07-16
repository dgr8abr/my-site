---
layout: default
title: Columns
permalink: /columns
page_intro : Welcome to my site, These are my columns, I write about politics and social issues because I care about life and my country.

---
# Columns
<div>
	{% for post in site.columns %}
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