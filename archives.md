---
title: Post Archives
layout: default
type: website
---
<h1>Chocolate Peanut Butter Posts</h1>
<p>Between 2008-2014, I published 384 posts about the best ingredient combination in the world. You can read them all!</p>

{% assign lastyear = 1902  %}
<ul class="postlist">
  {% for post in site.posts %}
  	{% assign postyear = post.date | date: "%Y"  %}
  	{% if postyear != lastyear %}
  		{% assign lastyear = postyear  %}	
  		<li class="archive-year">{{ lastyear }}</li>
  	{% endif %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>