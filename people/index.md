---
title: People
nav:
  order: 2
  tooltip: About our team
  display: true
---


# {% include icon.html icon="fa-solid fa-users" %}Team

{% include section.html %}

## Current Members

{% include list.html data="members" component="portrait" filters="role: pi" %}
{% include list.html data="members" component="portrait" filters="role: phd" %}
{% include list.html data="members" component="portrait" filters="role: grad" %}
{% include list.html data="members" component="portrait" filters="role: undergrad" %}

## Alumni

{% include list.html data="members" component="portrait" filters="role: alum" %}
