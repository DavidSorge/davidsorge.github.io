---
layout: default
title: 'Teaching Overview'
subtitle: 'Creating Spaces to Practice the Community of Truth'
description: 'My teaching philosophy centers on creating spaces where students practice critical thinking, dialogue across difference, and connection between research and real-world challenges.'
featured_image: '/images/teaching-philosophy.jpg'
permalink: /teaching-overview/
---

<section class="single">

	<div class="wrap">

		<h2>Teaching Philosophy</h2>

		<p>"To teach is to create a space in which the community of truth is practiced," and this captures the soul of my teaching. I want students to cultivate transferable skills: the ability to read critically, think sociologically, engage in dialogue across difference, and connect research to real-world challenges.</p>

		<h3>Creating Space</h3>

		<p>My pedagogy grows out of active and experiential learning, built around the cycle of encounter and reflection. Students engage with material before class, then participate in small-group dialogue and collaborative activities that help them process and apply concepts. These give quieter students room to participate in ways they might not in larger group discussions.</p>

		<h3>Nurturing Communities of Truth</h3>

		<p>I center methods that build teamwork and empathy, even in challenging material. Students practice sociological sympathy—seeing the world through perspectives that may initially feel uncomfortable, but that expand their capacity for understanding.</p>

		<h3>Supporting Practice</h3>

		<p>Behind the ideals are structures that help students grow. I align assignments with transferable skills and design portfolio projects that connect to students' goals and interests. The results have been breathtaking: documentaries, podcasts, policy briefs, and creative projects that demonstrate deep engagement with course material.</p>

		<p><em>"One of the main reasons I decided to be a Sociology major was because of Professor Sorge."</em> — Student feedback</p>

	</div>

</section>

<section class="portfolio">

	<div class="content-wrap portfolio-wrap">

		<h2 style="text-align: center; margin-bottom: 2rem; position: relative; z-index: 10; background: white; padding: 1rem 0;">My Courses</h2>

		{% for course in site.teaching reversed %}

		<div class="portfolio-item">

			<a class="portfolio-item__link" href="{{ course.url | relative_url }}">

				<div class="portfolio-item__image" style="min-height: 200px; background-color: #f5f5f5; display: flex; align-items: center; justify-content: center;">
					<img src="{{ course.featured_image | relative_url }}" alt="{{ course.title }}" style="width: 100%; height: 100%; object-fit: cover;" onerror="this.style.display='none'; this.parentNode.innerHTML='<div style=&quot;color: #666; font-size: 3rem;&quot;>📚</div>';">
				</div>

				<div class="portfolio-item__content">
					<div class="portfolio-item__info">
						<h2 class="portfolio-item__title">{{ course.title }}</h2>
						<p class="portfolio-item__subtitle">{{ course.subtitle }}</p>
					</div>
				</div>

			</a>

		</div>

		{% endfor %}

	</div>

</section>