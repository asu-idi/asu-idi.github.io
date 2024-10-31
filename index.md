---
---

<h1 style="text-align:center"> Exploring Frontiers of Intelligent Data Infrastructure </h1>

Data is the gold of the 21st century, which reflects, influences, and empowers our daily lives and changes the whole world. As modern data generation continues to surge due to the explosion of social media, e-business, big data, AR/VR, and all the applications, driven by new technologies like machine learning (ML), artificial intelligence (AI), big data, cloud computing, and the Internet of Things (IoT), our infrastructure to store, manage, and process this data must continuously evolve. Our research vision is to advance the foundation of data infrastructure, including storage systems, memory systems, and database systems, by creating Resilient, Adaptive, Intelligent, Sustainable, and Efficient (RAISE) systems that not only accommodate the scale of future data but also enable seamless integration with new technologies and hardware, such as disaggregated infrastructure and emerging storage/memory devices, new applications such as large language models and scientific analysis, and urgent need for sustainable and cost-effective system designs. To achieve the research goal of RAISE, our lab mainly focuses on the system-level innovations combined with the cross-stack co-designs. We are passionate about pushing the boundaries of data infrastructure.

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

<!-- Dummy Code using Glide.js -->
<!-- <div class="glide">
  <div class="glide__track" data-glide-el="track">
    <ul class="glide__slides">
      <li class="glide__slide">0</li>
      <li class="glide__slide">1</li>
      <li class="glide__slide">2</li>
    </ul>
  </div>
</div>

<script>
  new Glide('.glide').mount()
</script> -->


<!-- Dummy Code using Glider.js -->
<!-- <div class="glider">
  <div> 1 </div>
  <div> 2 </div>
  <div> 3 </div>
</div>

<script>
  new Glider(document.querySelector('.glider'), {
    slidesToShow: 1,
    dots: '#dots',
    draggable: true,
    arrows: {
      prev: '.glider-prev',
      next: '.glider-next'
    }
  });
</script> -->
