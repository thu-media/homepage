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

**{{ pub.title }}**

*{{ pub.authors }}*

{{ pub.conference }} {% if pub.link %}[[Link]]({{ pub.link }}){% endif%} {% if pub.file %}[[PDF]]({{ pub.file }}){% endif%} {% if pub.code %}[[Code]]({{ pub.code }}){% endif%}

{% endfor %}
{% endfor %}
