<pre direction="ltr">
    site
     {{ site | inspect }}
</pre>

_____


site.posts.size {{ site.posts.size }}
{% for cast in site.posts %}
  {{ site.baseurl }}{{ cast.url }}
{% endfor %}

   