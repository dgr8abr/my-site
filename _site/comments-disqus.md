The easiest and cleanest way to do it is to create a partial with the HTML that disqus provides in your _includes/ folder (e.g. _includes/disqus.html) and then just including it in your posts layout file (e.g. _layouts/post.md):

{% include disqus.html %}
You can see an example here: post layout and disqus partial.

