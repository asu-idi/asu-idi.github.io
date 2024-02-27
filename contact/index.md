---
title: Contact
nav:
  order: 5
  tooltip: Email, address, and location
  display: true
---

# {% include icon.html icon="fa-regular fa-envelope" %}Contact

We are always working on exciting new ideas. If you are interested in 
collaborating with us, or if you have any questions, we would love to hear.

{%
  include button.html
  type="email"
  text="zhichao.cao@asu.edu"
  link="zhichao.cao@asu.edu"
%}

{% include section.html %}

{% capture col1 %}

Brickyard Engineering is the home to the Intelligent Data Infrastructure Lab (IDI). You will often find one of our team members in the vicinity of the following address:

**Street Address** <br>
699 S. Mill Ave. <br>
Tempe, AZ 85281

**Building Code** <br>
BYENG

{% endcapture %}

{% capture col2 %}

{%
  include figure.html
  image="images/BrickyardASU.jpeg"
  caption="Our Home @ ASU"
%}

{% endcapture %}

{% include cols.html col1=col1 col2=col2 %}
