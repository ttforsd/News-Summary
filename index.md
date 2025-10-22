<ul>
  {% assign sorted_news = site.news | sort: 'title' | reverse %}
  {% for item in sorted_news %}
    <li>
      <a href="{{ item.url | relative_url }}">{{ item.title }}</a>
    </li>
  {% endfor %}
</ul>