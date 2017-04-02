---
layout: trace
---

# Jsonify
{{ site | jsonify }}
# inspect
{{ site | inspect }}


_____


site.posts.size {{ site.posts.size }}
{% for cast in site.posts %}
  {{ site.baseurl }}{{ cast.url }}
{% endfor %}

     
