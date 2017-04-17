---

---
# רשימת פרקים
<div>

{% assign episodes = site.pages | sort: "episode-number" %}
<table>
{% for p in episodes reversed %}
    {% if p.episode-number >= 0 %}
    <tr>
        <td>
            <img src="..{{ p.image }}" style="display:inline-block; height: 100px; width: 100px;">
        </td>
        <td>
            <h2> <a href="{{ site.baseurl }}{{ p.url }}">{{ p.title }}</a> </h2>
        </td>
    </tr>
    {% endif %}
{% endfor %}
</table>

</div>
