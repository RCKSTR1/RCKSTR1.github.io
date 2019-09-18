---
layout: home
title: Home
subtitle: 'Inicio, posts mas recientes, anuncios.'
description: null
order: 1
nav-menu: true
header-menu: false
image: null
author: null
show_tile: false
---

{% include randomquote.html %}

<!-- Latest Post  preview-->
{% for latestPost in site.posts limit:site.home-posts-preview-count %}
<!-- Mini Post -->
{% include postpreview.html post=latestPost %}
{% else %}
{% endfor %}


<!-- Pagination -->
<!-- {% include pagination.html %} -->

{% include contactform.html %}
