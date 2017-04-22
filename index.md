---
image : /images/podcast.jpg
---

# מה זה מדברים בסרט?
בכל פעם שאתם הולכים לסרט זה קורה...

מישהו בשורה 13 בצד מחליט שהסרט צריך ערוץ קומנטרי בלייב, וכל הקולנוע צריך לסבול.

מכירים?

אז האיש הזה הוא אנחנו! וכשירות לציבור החלטנו אחת ולתמיד להקליט את ההגיגים שלנו, שיהיה לדורות הבאים.
# אז מה נשמע?
{% assign episodes = site.pages | sort: "episode-number" %}
{% assign lst = episodes.last.episode-number | minus: 3 %}
<!-- # {{ lst }} -->
<table style="border: 0px; border-collapse: collapse; width:1000px;">
{% for p in episodes reversed %}
    {% if p.episode-number > lst %}
    <tr>
        <td style="width:200px">
            <img src="..{{ p.image }}" style="display:inline-block; height: 200px; width: 200px;">
        </td>
        <td style="text-align: right; padding-right: 20px;">
            <h2> <a href="{{ site.baseurl }}{{ p.url }}">{{ p.title }}</a> </h2>
            <p>{{p.content}}</p>
            <iframe width="100%" height="100" scrolling="no" frameborder="no" src="https://podswell.com/demoplayer/podswell/sha/{{ p.ep-file }}?name=movietalker"></iframe>
        </td>
    </tr>
    {% endif %}
{% endfor %}
</table>
# [רשימת כל הפרקים](/episodes)
<!-- # אני רוצה עוד מכל הטוב הזה!
שום בעיה, הנה [רשימת כל הפרקים שלנו](/episodes) וחוץ מזה אפשר להרשם לרסס שלנו פה למעלה
 -->
#  מי אנחנו
![מדברים בסרט - התמונה]({{ page.image }})
## דין לנגסם
> כבר בכיתה ב' זכה בתואר המחייב 'יש לו פוטנציאל אבל הוא לא מנצל אותו' מהמורה שולה.
> מאוחר יותר, בכיתה ט, שבר את שיא ההרשמות על דיבור בכיתה

## זהר זקס
> נושא בתואר לרלרן של כבוד מאז שנת 2015, אז דיבר במשך 45 דקות על ההבדל בין תפוז סיני.
> מאוחר יותר נזרק מהקרנה בשעת תרבות בבית האבות 'גיל לזיקנה'

<!-- ##  פרק 4.
<div>
<iframe width="500" height="100" scrolling="no" frameborder="no" src="http://podswell.com/demoplayer/podswell/sha/26d752cbb2b7379fad8bb1b6186ed790c6a083ae.mp3?name=movietalker"></iframe>
</div>

##  פרק 2 - בייסקטבול - עושים שיגועים.
<div>
<iframe width="500" height="100" scrolling="no" frameborder="no" src="https://podswell.com/demoplayer/podswell/sha/b979b57cc9d86b45b347641e2536b6b9b05ef9d3.mp3?name=movietalker"></iframe>
</div>

##  פרק 1 - בלייד ראנר - להוולד, לעשות צבא, למות.
<div>
<iframe width="500" height="100" scrolling="no" frameborder="no" src="https://podswell.com/demoplayer/podswell/sha/b979b57cc9d86b45b347641e2536b6b9b05ef9d3.mp3?name=movietalker"></iframe>

</div>

## פרק אפס
<div>
<iframe width="500" height="100" scrolling="no" frameborder="no" src="https://podswell.com/demoplayer/podswell/sha/5a0c93fca21c4212aa598c73d6eb249bd36c3e75.mp3?name=movietalker"></iframe>
</div> -->




