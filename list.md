---
layout: page
---
<ul>
{% for repository in site.github.public_repositories %}
 <li><a href="{{ repository.html_url }}">{{ repository.name }}</a><br />
  Description: {{ repository.description }}<br />
  Issues: {{ repository.open_issues }}
 </li>
{% endfor %}
</ul>
