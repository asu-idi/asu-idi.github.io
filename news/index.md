---
title: News
nav:
  order: 6
  display: false
---

# {% include icon.html icon="fa-solid fa-scroll" %}News

{% assign news = site.data.news 
  | sort: 'date'
  | reverse
%}

{% for item in news %}
{%
  include news.html
  date=item.date
  type=item.type
  content=item.title
  subtype=item.subtype
%}
{% endfor %}