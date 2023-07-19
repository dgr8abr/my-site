---
layout: default
page_title: Columns 
title: Columns -- AIB
permalink: /columns
page_intro : Welcome to my site, These are my columns, I write about politics and social issues because I care about life and my country.
---
<div>
	{% for column in site.data.settings.column %}
	<div>
		<a href="{{ site.github.url }}/{{ column.url }}" class="text-xl text-grey-darker font-bold no-underline hover:text-black">
			{{ column.name }}       
		</a>
	</div>
	<p class="text-grey-darkest text-base leading-normal mt-1">
			 {{ column.content | markdownify | strip_html | truncatewords: 30 }}
	</p>
	<div class="mb-8 text-grey-darkest text-base leading-normal mt-2">
		<a href="{{ site.github.url }}/{{ column.url }}" class="text-grey-darker hover:text-black text-sm no-underline hover:underline">Read this column posted on {{ column.date | date_to_string: "ordinal", "US" }}</a>
	</div>
	{% endfor %}
</div>