---
layout: default
---

{% for post in site.posts limit: 10 %}
<div class="homeblock">
  <a href="{{ post.url }}">
    <h2 class="entry-title">{{ post.title }}</h2>
    <img src="{{ post.featureimage }}" />
  </a>
</div>
{% endfor %}


<a href="/archives">View all our posts in the CPB Archives!</a>