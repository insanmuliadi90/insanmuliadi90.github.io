---
layout: default
permalink: /karakter/
---

<div class="row test">
<h1>Tag: {{ site.karakter }}</h1>
<ul>
{% for post in site.karakter[page.karakter] %}
  <li><a href="{{ post.url }}">{{ post.title }}</a> ({{ post.date | date_to_string }})<br>
    {{ post.description }}
  </li>
{% endfor %}
</div>
