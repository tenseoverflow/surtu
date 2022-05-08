---
layout: page-eng
title: Articles
permalink: /en/teataja/
respectiveEST: /teataja/
---

<h3>Articles (Teataja) published by Surtu's staff, in Estonian. (<a href="/feed.xml">RSS</a>)</h3>

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