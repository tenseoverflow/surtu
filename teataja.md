---
layout: page
title: Teataja
permalink: /teataja/
---

<h3>Artiklid (<a href="/feed.xml">RSS</a>)</h3>

<div id="recents">

<ul>
{% for post in site.posts %}
<li> 
<time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%b %d, %Y" }}</time> &#8212; <a id="{{ post.id }}" href="{{ post.url }}">{{ post.title }}</a>
<p>{{ post.description }}</p>
</li>
{% endfor %}
</ul>
</div>