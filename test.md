---
image : /images/podcast.jpg
---
<!-- {% include social.html %} -->
# מה זה מדברים בסרט?
בכל פעם שאתם הולכים לסרט זה קורה...
{% assign episodes = site.pages | sort: "episode-number" %}
{% for p in episodes reversed %}
    {% if p.episode-number >= 0 %}
		<p>{{ p }}</p>
    {% endif %}
{% endfor %}

asd