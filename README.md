---
---

# community

{% for category in site.categories %}
  <h2>{{ category[0] }}</h2>
  {% for post in category[1] %}
  <h3><a href="{{ site.github.baseurl }}{{ post.url }}">{{ post.title }}</a></h3>
  <ul class="tags">
    {% for tag in post.tags %}
    <li>{{ tag }}</li>
    {% endfor %}
  </ul>
  {% endfor %}
{% endfor %}
