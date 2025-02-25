---
---

<h1 style="text-align:center"> Exploring Frontiers of Intelligent Data Infrastructure </h1>

Data is the gold of the 21st century, which reflects, influences, and empowers our daily lives and changes the whole world. As modern data generation continues to surge due to the explosion of social media, e-business, big data, AR/VR, and all the applications, driven by new technologies like machine learning (ML), artificial intelligence (AI), big data, cloud computing, and the Internet of Things (IoT), our infrastructure to store, manage, and process this data must continuously evolve. Our research vision is to advance the foundation of data infrastructure, including storage systems, memory systems, and database systems, by creating Resilient, Adaptive, Intelligent, Sustainable, and Efficient (RAISE) systems that not only accommodate the scale of future data but also enable seamless integration with new technologies and hardware, such as disaggregated infrastructure and emerging storage/memory devices, new applications such as large language models and scientific analysis, and urgent need for sustainable and cost-effective system designs. To achieve the research goal of RAISE, our lab mainly focuses on the system-level innovations combined with the cross-stack co-designs. We are passionate about pushing the boundaries of data infrastructure.

{% include section.html %}

<b>Hiring!</b> <br>
Recruiting 1-2 fully funded Ph.D. students for Fall 2025, focusing on research areas related to data systems for LLMs (e.g., KV-cache, offloading, vector databases, and hierarchical databases). Currently collaborating closely with Meta and the ORNL National Laboratory in this field.

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
  subtype=item.subtype
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

## Gallery

{% include grid-gallery.html %}