---
layout: home
permalink: /store
---

{% for my_page in site.pages %}
  {% if my_page.title %}
  <a class="page-link" href="{{ my_page.url | relative_url }}">{{ my_page.title | escape }}</a>
  {% endif %}
{% endfor %}