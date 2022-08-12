---
layout: default
permalink: /karakter/
---

<div class="post row kar-row">
<h1>{{ page.karakter }}</h1>
<ul>
{% for post in site.karakter[page.karakter] %}
  <li><a href="{{ post.url }}">{{ post.title }}</a> ({{ post.date | date_to_string }})<br>
    {{ post.description }}
  </li>
{% endfor %}
</ul>
</div>
