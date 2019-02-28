---
layout: page
---

{% for repository in site.github.public_repositories %}
  * [{{ repository.name }}][{{ repository.html_url }}] Description: {{ repository.description }} Issues: {{ repository.open_issues }}
{% endfor %}
