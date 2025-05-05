---
title: "Seminar Series 2025"
date: 2024-10-24T12:33:46+10:00
weight: 1
---

# 🌟 Seminar Series 2025

> **Description:**
>
> - Seminars hosted by **ContinualAI** bring together researchers and enthusiasts to discuss cutting-edge topics in **Continual Learning**. Each session lasts **60 minutes**, with **40 minutes of presentations**, delivered by the authors of recent groundbreaking research.
> - 📅 **Join us first Thursday of the month at 6 PM CET / 9 AM PT / 12 PM ET** for insights into the latest developments in Continual Learning.

## 🎥 Previous Seminars

{% assign sorted_prev = site.data.seminar.previous | sort: "order" | reverse %}
{% for seminar in sorted_prev %}
> ## **{{ forloop.index }}. {{ seminar.title }}**
>
> **Topic:** *"{{ seminar.topic }}"*
>
> {% if seminar.date %}
> **Date:** **{{ seminar.date }}**
> {% endif %}
>
> **Speakers:**
> {% for speaker in seminar.speakers %}
> - <small>**{{ speaker }}**</small>
> {% endfor %}
>
> {% if seminar.link %}
> **Link:** [**Join / Watch Seminar**]({{ seminar.link }})
> {% else %}
> **Link:** Coming soon
> {% endif %}
>
> [![{{ seminar.title }}]({% if seminar.image contains "://" %}{{ seminar.image }}{% else %}{{ site.baseurl }}{{ seminar.image }}{% endif %})]({{ seminar.link }})
>
> ---
{% endfor %}
