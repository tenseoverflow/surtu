---
layout: page
title: Raamatud
permalink: /raamatud/
---

<h3>Valik meie kirjastatud raamatutest:</h3>

<section>
{% for item in site.books %}
<div class="book">
<div class="book-pic">
<img src="{{ item.pic }}" alt="{{ item.title }} photo" />
</div>
<div class="book-desc">
<h2>{{ item.title }}</h2>
<p>{{ item.description }}</p>
<a href="{{ item.url }}" style="font-size: 2em;">Osta</a>
</div>
</div>
<hr>
{% endfor %}
</section>