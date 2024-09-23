---
---

<h1 style="text-align:center"> Exploring frontiers in database, storage, and data infrastructure </h1>

The Intelligent Data Infrastructure (IDI) research lab delves into database systems, storage technologies, and next-generation data infrastructure. We tackle emerging challenges, designing cutting-edge solutions to advance data management and analysis in today's dynamic digital landscape. Our work spans a wide range of topics, including distributed systems, cloud computing, machine learning, and data analytics. We are passionate about pushing the boundaries of data infrastructure.

{% include section.html %}

## News

{% assign news = site.data.news 
  | sort: 'date'
  | reverse
%}

{% for item in news limit:10 %}
{%
  include news.html
  date=item.date
  type=item.type
  content=item.title
%}
{% endfor %}

{%
  include button.html
  link="news"
  text="See all news"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}
