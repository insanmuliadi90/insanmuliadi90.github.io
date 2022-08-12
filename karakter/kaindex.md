---
layout: default
permalink: /karakter/
---

<div class="row test">
{% for karakter in site.karakter %}
  <div class="archive-group">
    {% capture karakter_name %}{{ karakter | first }}{% endcapture %}
    <div id="#{{ karakter_name | slugize }}"></div>
    <h3 class="category-head">{{ karakter_name }}</h3>
    <a name="{{ category_name | slugize }}"></a>
    {% for post in site.karakter[karakter_name] %}
    <article class="archive-item">
      <h4><a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a></h4>
    </article>
    {% endfor %}
  </div>
{% endfor %}
</div>
