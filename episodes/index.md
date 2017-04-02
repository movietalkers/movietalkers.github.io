---

---
# רשימת פרקים
<div>

{% assign episodes = site.pages | sort: "episode-number" %}
{% for p in episodes reversed %}
    {% if p.episode-number >= 0 %}

        <h2> <a href="{{ site.baseurl }}{{ p.url }}">{{ p.title }}</a> </h2>

    {% endif %}
{% endfor %}

</div>
