---
title: Scoreboard
---

# Highscores

| Rank | Name          | Score |
|------|---------------|-------|
| 1    | EvilHacker123 | 2781  |
| 2    | TryHard_25    | 473   |
| 3    | NoName        | 12    |
| 4    | ApplePie1997  | 1     |

Scores were last updated: **Never**



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
