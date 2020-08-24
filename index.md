---
layout: default
---

{% for post in site.posts %}
  {% if post.published == true %}
  {{ post.date | date: "%b %-d, %Y" }}
  [{{ post.title }}]({{ post.url | prepend: site.baseurl }})
  {% endif %}
{% endfor %}
