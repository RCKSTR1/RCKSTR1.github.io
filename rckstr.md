---
title: Acerca de mi
myname: Adrian Gonzalez
layout: aboutme
description: 'Desarrollador de software full-stack. Certified Scrum Master. AR/VR newbie. Músico. Melómano. Team
player.'
image: assets/images/aboutMeBanner.jpg
nav-menu: true
---

<!-- Main -->
<div id="main">

	<!-- Two -->
	<section id="one" class="spotlights">
		<section>
			<a href="generic.html" class="image">
				<img src="assets/images/pic09.jpg" alt="" data-position="center center" />
			</a>
			<div class="content">
				<div class="inner">
					<header class="major">
						<h3>Acerca de mí</h3>
					</header>
					<ul class="icons">
						{% if site.twitter_url %}
						<li><a href="{{ site.twitter_url }}" class="icon alt fa-twitter" target="_blank"><span class="label">Twitter</span></a></li>
						{% endif %}
						{% if site.googleplus_url %}
						<li><a href="{{ site.googleplus_url }}" class="icon alt fa-google-plus" target="_blank"><span class="label">Google+</span></a></li>
						{% endif %}
						{% if site.facebook_url %}
						<li><a href="{{ site.facebook_url }}" class="icon alt fa-facebook" target="_blank"><span class="label">Facebook</span></a></li>
						{% endif %}
						{% if site.instagram_url %}
						<li><a href="{{ site.instagram_url }}" class="icon alt fa-instagram" target="_blank"><span class="label">Instagram</span></a></li>
						{% endif %}
						{% if site.pinterest_url %}
						<li><a href="{{ site.pinterest_url }}" class="icon alt fa-pinterest" target="_blank"><span class="label">Pinterest</span></a></li>
						{% endif %}
						{% if site.gitlab_url %}
						<li><a href="{{ site.gitlab_url }}" class="icon alt fa-gitlab" target="_blank"><span class="label">GitLab</span></a></li>
						{% endif %}
						{% if site.github_url %}
						<li><a href="{{ site.github_url }}" class="icon alt fa-github" target="_blank"><span class="label">GitHub</span></a></li>
						{% endif %}
						{% if site.slack_url %}
						<li><a href="{{ site.slack_url }}" class="icon alt fa-slack" target="_blank"><span class="label">Slack</span></a></li>
						{% endif %}
						{% if site.linkedin_url %}
						<li><a href="{{ site.linkedin_url }}" class="icon alt fa-linkedin" target="_blank"><span class="label">LinkedIn</span></a></li>
						{% endif %}
						{% if site.stackoverflow_url %}
						<li><a href="{{ site.stackoverflow_url }}" class="icon alt fa-stack-overflow" target="_blank"><span class="label">Stack Overflow</span></a></li>
						{% endif %}
					</ul>
					<p>
						Soy desarrollador de software full-stack con {{ 'now' | date:"%Y" | minus : 2007 }} años de
						experiencia, principalmente especializado en tecnologías Microsoft, aunque recientemente
						orientado a realidad aumentada con wearables. Certificado como Scrum Master por Scrum Alliance.
					</p>
					<p>
						Además de desarrollo de software, me he dedicado al mismo tiempo a la administracion de
						servidores (IIS, SQL, Forefront), administración de dominio, así como he coordinado equipos de
						soporte.
					</p>
				</div>
			</div>
		</section>
	</section>

	<section id="two">
		<div class="inner">
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
		</div>
	</section>

	<!-- Three -->
	<section id="three">
		<div class="inner">
			<header class="major">
				<h2>Por qué creé este blog</h2>
			</header>
			<p>
				Porque actualmente, la mayoría de la documentación, cursos y reviews acerca de tecnologías nuevas son casi exclusivamente en inglés. 
				Este blog es mi manera de compartir, aportar e iniciar la conversación acerca de los temas que me parecen relevantes como desarrollador de software.
			</p>
			<p>
				Aunque este blog no permite comments directamente en los posts, si me gustaría llevar la discusión a otras plataformas donde pueda haber mas
				interacción como twitter o facebook.
			</p>
			<ul class="actions">
				<li><a href="all_posts.html" class="button next">Ir al blog</a></li>
			</ul>
		</div>
	</section>

</div>