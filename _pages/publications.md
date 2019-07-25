---
title: "Media Lab - Publications"
layout: gridlay
excerpt: "Media Lab at Tsinghua University"
sitemap: false
permalink: /publications
---


# Publications

{% for year in site.data.publist %}

## {{year.Year}}
<hr />

{% for pub in year.Publications %}

  {{ pub.title }} <br />
  <em>{{ pub.authors }} </em><br />
  <a href="{{ pub.link.url }}">{{ pub.link.display }}</a>

{% endfor %}
{% endfor %}
