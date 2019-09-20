---
layout: about
title: 'Adrian Gonzalez'
subtitle: Desarrollador de software full-stack. Certified Scrum Master. AR/VR newbie. Músico. Melómano. Team player.
description: Quién soy y por que creé este blog
order: 3
nav-menu: true
header-menu: true
header-title: 'Acerca de mí'
image: images/authors/adrian.jpg
author: null
show_tile: false
---

<article class="post">
	<header>
		<div class="title">
			<h2><a href="#">{{ page.title }}</a></h2>
			<p>{{ page.subtitle }}</p>
		</div>
		<div class="meta author-photo-container">
			<!-- <time class="published" datetime="2015-10-18">October 18, 2015</time>
                        <a href="#" class="author"><span class="name">Jane Doe</span><img src="images/avatar.jpg" alt="" /></a> -->
			<div class="author-photo"><img src="{{ page.image | relative_url }}" alt="" /></div>
		</div>
	</header>

	<section>
		<header class="major">
			<h2>Acerca de mí</h2>
		</header>
		<ul class="icons">
			{% for smp in site.socialMediaProfiles %}
			<li><a href="{{smp.url}}" target="_blank" class="{{smp.icon}}"><span class="label">{{smp.label}}</span></a>
			</li>
			{% endfor %}
		</ul>
		<p>
			Soy desarrollador de software full-stack con {{ 'now' | date:"%Y" | minus : 2007 }} años de
			experiencia, principalmente especializado en tecnologías Microsoft, aunque recientemente
			orientado a realidad aumentada con wearables. Certificado como Scrum Master por Scrum Alliance.
		</p>
		<p>
			Además de desarrollo de software, me he dedicado al mismo tiempo a la administracion de
			servidores (IIS, SQL, Hyper-V, Exchange), administración de dominio, así como he coordinado equipos de
			soporte.
		</p>
	</section>

	<section>
		<header class="major">
			<h2>Skills/Intereses</h2>
		</header>
		<div class="row">
			<div class="6u 12u$(small)">
				<ul class="alt">
					<li>Patrones de Arquitectura de Software</li>
					<li>Patrones de diseño como MVC y MVVM</li>
					<li>Domain Driven Design</li>
					<li>Principios SOLID</li>
					<li>SCRUM</li>
					<li>Azure Cognitive Services</li>
				</ul>
			</div>
			<div class="6u$ 12u$(small)">
				<ul class="alt">
					<li>Networking</li>
					<li>Música: Casi de todo, menos reggaetton... lo siento</li>
					<li>C#, Typescript/Javascript, XAML, C++</li>
					<li>Angular, React y otros frameworks JS</li>
					<li>ASP.NET Core</li>
					<li>Entity Framework</li>
				</ul>
			</div>
		</div>
		<p>
			Si hay algun tema del que te gustaría discutir o leer, envíame un mensaje.
		</p>
	</section>

	<section>
		<header class="major">
			<h2>Por qué creé este blog</h2>
		</header>
		<p>
			Porque actualmente, la mayoría de la documentación, cursos y reviews acerca de tecnologías nuevas son casi
			exclusivamente en inglés.
			Este blog es mi manera de compartir, aportar e iniciar la conversación acerca de los temas que me parecen
			relevantes
			como desarrollador de software.
		</p>
		<p>
			Aunque este blog no permite comments directamente en los posts, si me gustaría llevar la discusión a otras
			plataformas donde pueda haber mas
			interacción como twitter o facebook.
		</p>
		<ul class="actions">
			<li><a href="all_posts.html" class="button next">Ir al blog</a></li>
		</ul>
	</section>
</article>
