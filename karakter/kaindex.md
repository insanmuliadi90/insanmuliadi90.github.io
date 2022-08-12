---
layout: default
permalink: /karakter/
---

<div class="row test">
{% for post in site.karakter %}
    <article class="archive-item">
      <h4><a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a></h4>
    </article>
{% endfor %}
</div>
