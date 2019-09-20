---
layout: allposts
title: 'Blog'
subtitle: 'Todos los posts.'
landing-title: 'Past flying cars and time machines'
description: null
order: 2
nav-menu: true
header-menu: true
image: null
author: null
show_tile: false
---

{% if site.posts.size != 0 %}
{% for post in site.posts %}

{% for author in site.authors %}
{% if author.id == post.author %}
{% assign postAuthor = author %}
{% break %}
{% endif %}
{% endfor %}

{% assign mod=forloop.index|modulo:2%}

{% if mod == 1%}
<div class="row uniform">
    {% endif %}

    <div class="6u 12u(medium)">

        <div class="row">
            <div class="12u">
                <!-- Mini Post -->
                <article class="mini-post">
                    <header>
                        <h3><a href="{{ post.url  | relative_url }}">{{post.title}}</a></h3>
                        <time class="published" datetime="{{ post.date }}">{{ post.date | date: '%B %d, %Y' }}
                            <br>Por {{postAuthor.name}}</time>
                    </header>
                    <a href="{{ post.url  | relative_url }}" class="image"><img src="{{post.image}}" alt="" /></a>
                </article>

            </div>
        </div>
    </div>
    {% if mod == 0%}
</div>
{% endif %}
{% endfor %}
</div>
{% else %}
<div class="row uniform">
    <h2>Ningún post todavía. </h2>
    <span class="image fit"><img src="assets/images/this_is_fine.jpg" alt="" /></span>
</div>
{% endif %}
