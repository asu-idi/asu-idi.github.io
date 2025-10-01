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

{% assign curr_by_role = site.data.members_current | group_by: "role" %}
{% for role_group in curr_by_role %}
### {{ role_group.name }}s

<ul style="margin: 0px 0;">
{% assign sorted_curr = role_group.items | sort: "year" | reverse %}
{% for curr in sorted_curr %}
  <li style="margin: 1px 0;"><strong>{{ curr.name }}</strong></li>
{% endfor %}
</ul>

{% endfor %}


## Alumni

{% assign alum_by_role = site.data.members_alum | group_by: "role" %}
{% for role_group in alum_by_role %}
### {{ role_group.name }}s

<ul style="margin: 0px 0;">
{% assign sorted_alums = role_group.items | sort: "year" | reverse %}
{% for alum in sorted_alums %}
  <li style="margin: 1px 0;"><strong>{{ alum.name }}</strong></li>
{% endfor %}
</ul>

{% endfor %}
