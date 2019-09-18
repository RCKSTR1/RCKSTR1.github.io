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

<!-- Latest Post  preview-->
{% for latestPost in site.posts limit:1 %}
<!-- Mini Post -->
{% include postpreview.html post=latestPost %}
{% else %}
{% endfor %}


<!-- Pagination -->
<!-- {% include pagination.html %} -->

{% include contactform.html %}
