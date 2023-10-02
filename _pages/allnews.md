---
title: "News"
layout: textlay
sitemap: false
permalink: /allnews.html
---

{% if site.data.news %}
## News

<div class="jumbotron">
{% for article in site.data.news %}
<b>{{ article.date }}</b>

{{ article.headline }}
{% endfor %}
</div>
{% else %}
<meta http-equiv="refresh" content="0; {{ site.url }}{{ site.baseurl }}/404.html"></meta>
{% endif %}