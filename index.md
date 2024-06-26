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

{% for item in news limit:5 %}
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

## Quick Links

{% capture text %}

{%
  include button.html
  link="publications"
  text="See our publications"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/photo.jpg"
  link="publications"
  title="Our Publications"
  text=text
%}

{% capture text %}

{%
  include button.html
  link="research"
  text="Browse our research"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/photo.jpg"
  link="research"
  title="Our Research"
  flip=true
  style="bare"
  text=text
%}

{% capture text %}

{%
  include button.html
  link="people"
  text="Meet our team"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/photo.jpg"
  link="people"
  title="Our Team"
  text=text
%}
