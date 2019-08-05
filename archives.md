---
layout: default
---
{% assign lastyear = 1902  %}
<ul class="postlist">
  {% for post in site.posts %}
  	{% assign postyear = post.date | date: "%Y"  %}
  	{% if postyear != lastyear %}
  		{% assign lastyear = postyear  %}	
  		<li><h3>{{ lastyear }}</h3></li>
  	{% endif %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>