---
layout: page
---

<ul>
 {% assign sorted = site.github.public_repositories | sort: 'pushed_at', 'last' %}
 {% for repository in sorted %}
  <li><a href="{{ repository.html_url }}">{{ repository.name }}</a><br />
   Description: {{ repository.description }}<br />
   Open Issues: {{ repository.open_issues }}<br />
   Open Issue Count: {{ repository.open_issues_count }}<br />
   Created At: {{ repository.created_at }}<br />
   Updated At: {{ repository.updated_at }}<br />
   Pushed At: {{ repository.pushed_at }}<br />
  </li>
 {% endfor %}
</ul>
