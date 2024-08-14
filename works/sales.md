---
title: Sales Career
permalink: "/work/sales"
layout: default
page_title: Sales and Marketing
author: aib
page_intro: Welcome to my work page
page_link_phrase_2: This is where I will compile my sales tools and portfolio.
---

<div class="mt-8 p-4 bg-grey-lightest">
	{% for sale in site.data.settings.sales %}
	<div>
		<a href="{{ site.github.url }}/{{ sale.url }}" class="text-xl text-grey-dark font-bold no-underline hover:text-black">
			{{ sale.name }} 
		</a>
	</div>
	<p class="text-grey-darkest text-base leading-normal mt-1">
			 {{ sale.description | markdownify | strip_html | truncatewords: 20 }}
	</p>
	<div class="mb-8 text-grey-darkest text-base leading-normal mt-2">
		<a href="" class="text-grey-darker hover:text-black text-sm 	no-underline hover:underline">Lorem20 </a>
	</div>
	{% endfor %}
</div>



