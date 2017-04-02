---
---
# רשימת פרקים
{% assign episodes = site.pages | sort: "episode-number" %}
{% for p in episodes reversed %}
    <a href="{{ site.baseurl}}{{ p.url }}">{{ p.title }}</a><br>
{% endfor %}
