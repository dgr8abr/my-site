---
title: A.I.B - Books
permalink: "/books"
layout: default
page_title: Books
page_link_phrase_2: I love to read and write so This is where I compiled all the books
  that made me who I am.
---

<div class="p-4 bg-grey-lightest">
	{% for book in site.data.settings.books %}
	<div>
		<a href="{{ post.url }}" class="text-xl text-grey-dark font-bold no-underline hover:text-black">
			{{ book.name }}    
		</a>
	</div>
	<p class="text-grey-darkest text-base leading-normal mt-1">
			 {{ book.content | markdownify | strip_html | truncatewords: 30 }}
	</p>
	<div class="mb-8 text-grey-darkest text-base leading-normal mt-2">
		<a href="" class="text-grey-darker hover:text-black text-sm no-underline hover:underline">{{ book.description  }} </a>
	</div>
	{% endfor %}
</div>


