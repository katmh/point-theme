---
title: Blog
---

{% for post in site.posts %}
## [{{ post.title }}]({{ post.url }})

*{{ post.date | date: '%B %d, %Y' }}*

{{ post.content | strip_html | truncatewords: 70 }} [Read more]({{ post.url }})
{% endfor %}