---
layout: default
type: website
title: A site dedicated to the world's two best ingredients!
shortdescription: Chocolate Peanut Butter gallery features recipes, reviews, news, and more ... all about Chocolate and Peanut Butter!
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