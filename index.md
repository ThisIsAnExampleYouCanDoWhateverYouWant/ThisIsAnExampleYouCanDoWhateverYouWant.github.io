---
title:  "Welcome to this Homepage"
---


**Latest Anouncement**

{% for post in site.posts limit:1 %}
**[{{ post.title }}]({{ post.url }})**:
    
> {{ post.excerpt }}

{% endfor %}


---

---

I did it in 30 minutes, so please don't judge.
Here is some **bold** text and I could also add some [example](https://www.example.com) links. Embedding pictures and videos would work as well.

Usually there should be space for a nice menu... but I do not have time to make it nice so here we go:

1. [about]({% link about.md %})
2. [calendar]({% link calendar.md %})
3. [scoreboard]({% link scores.md %})
4. [anouncements]({% link anounce.md %})


