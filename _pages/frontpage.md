---
layout     : default
permalink  : '/index.html'
---

Navigate using the course selector on the header. For every course you'll find a number of covered subjects and some resources per subject.

## Last resources

{% assign resources_by_date = site.resources | sort: 'date' %}
<ul>
{% for resource in resources_by_date reversed limit:5 %}
{% include resource_li.html resource=resource %}
{% endfor %}
</ul>

Subscribe to the [resources feed]({{ site.baseurl }}{% link _pages/atom_resources.xml %})

