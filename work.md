---
layout: default
permalink: /works
title: A.I.B
page_title: Work
page_intro : Welcome to my work page
page_link_phrase_2 : Here you can view all the things about my work in sales, and whole other things such as Music and etc.	
---


<div class="p-4 bg-grey-lightest">
	{% for work in site.data.settings.work %}
	<div>
		<a href="{{ site.github.url }}/{{ work.url }}	" class="text-xl text-grey-darker font-bold no-underline hover:text-black">
			{{ work.name }}    
		</a>
	</div>
<div class="mb-8 text-grey-darkest text-base leading-normal mt-2">
		<a href="{{ site.github.url }}/{{ work.url }}" class="text-grey-darker hover:text-black text-sm no-underline hover:underline">{{ work.description  }} </a>
	</div>
	{% endfor %}
</div>


