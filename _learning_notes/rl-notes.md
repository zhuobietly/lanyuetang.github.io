---
layout: single
title: "Reinforcement Learning Notes"
permalink: /notes/learning/ml/rl/
author_profile: true
---

A list of my Reinforcement Learning notes (PDF).

{% assign notes = site.data.rl_notes | sort: "date" | reverse %}

<ul>
{% for n in notes %}
  <li>
    <strong>{{ n.title }}</strong>
    — <a href="{{ n.pdf }}">PDF</a>
    {% if n.date %}<span style="opacity:0.6;"> ({{ n.date }})</span>{% endif %}
  </li>
{% endfor %}
</ul>
