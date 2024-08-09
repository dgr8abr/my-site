---
layout: default
---

<h2 class="post_title">
  {{ page.title }}
  {% if page.date %}
  {% endif %}
  
      <!-- <h1 class="text-jumbo wt-bold m-xs-b-6 no-line-height tight-letters">CSS Utility Classes and &quot;Separation of Concerns&quot</h1> -->
</h2>
    <small class="text-sm">{{ page.date | date_to_string }}</small>

      

  <div class="mt-6 markdown js-blog-post-body flex-center">

{{ content }}

</div>