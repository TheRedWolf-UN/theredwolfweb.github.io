---
layout: default
title: Inicio
---

<section class="posts">

<h2>Últimos artículos</h2>

{% for post in site.posts limit:3 %}
<article class="post-preview">
    <h3>
        <a href="{{ post.url }}">{{ post.title }}</a>
    </h3>
    <p>{{ post.excerpt }}</p>
</article>
{% endfor %}

</section>