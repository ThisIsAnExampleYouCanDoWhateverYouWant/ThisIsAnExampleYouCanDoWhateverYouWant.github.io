---
title: Scoreboard
---

# Highscores

<table>
  {% for row in site.data.scores %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    {% endif %}

    {% tablerow pair in row %}
      {{ pair[1] }}
    {% endtablerow %}
  {% endfor %}
</table>


Scores were last updated: **Never**

{% include menu.md %}
