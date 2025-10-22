<ul>
  {% for item in site.news %}
    <li>
      <a href="{{ item.url | relative_url }}">{{ item.title }}</a>
      ({{ item.date | date: "%B %d, %Y" }})
    </li>
  {% endfor %}
</ul>