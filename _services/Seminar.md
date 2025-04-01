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

# 🎥 Previous Seminars

{% for seminar in site.data.seminar.previous %}
> ## **{{ seminar.order }}. {{ seminar.title }}**
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
> **Link:** [**Join / Watch Seminar**]({{ seminar.link }})
> 
> [![{{ seminar.title }}]({% if seminar.image contains "://" %}{{ seminar.image }}{% else %}{{ site.baseurl }}{{ seminar.image }}{% endif %})]({{ seminar.link }})
>
> ---
{% endfor %}

> **Explore highlights from recent seminars to gain valuable insights into Continual Learning.**
>
> ## 🌐 For a comprehensive view of all our seminars, visit:
> - 🎥 [**ContinualAI YouTube Channel**](https://www.youtube.com/@ContinualAI)
> - 📺 [**Seminar Playlist**](https://www.youtube.com/playlist?list=PLm6QXeaB-XkBMFxvgZvYjqhaPgGg8Um9Z)
>
> Stay connected with the ContinualAI community for updates on future events and discussions!

