---
layout: default
title: 'Speculative Visions'
subtitle: 'Creative Explorations of Possible Futures'
description: 'Speculative fiction and creative works exploring alternative worlds, social transformation, and possible futures.'
featured_image: '/images/speculative-visions.jpg'
permalink: /speculative-visions/
---

<section class="single">
<div class="wrap" markdown="1">

## Imagining Alternative Worlds

These creative works explore questions of social transformation, alternative histories, and possible futures. They complement my academic research by envisioning the kinds of worlds we might create through understanding conflict, cooperation, and social change.

</div>
</section>

<section class="portfolio">

	<div class="content-wrap portfolio-wrap">

		<h2 style="text-align: center; margin-bottom: 3rem; position: relative; z-index: 10; background: white; padding: 1rem 0;">Creative Works</h2>

		{% assign sorted_speculative = site.speculative | sort: 'path' %}
		{% for work in sorted_speculative %}

		<div class="portfolio-item">

			<a class="portfolio-item__link" href="{{ work.url | relative_url }}">

				<div class="portfolio-item__image" style="min-height: 200px; background-color: #f5f5f5; display: flex; align-items: center; justify-content: center;">
					<img src="{{ work.featured_image | relative_url }}" alt="{{ work.title }}" style="width: 100%; height: 100%; object-fit: cover;" onerror="this.style.display='none'; this.parentNode.innerHTML='<div style=&quot;color: #666; font-size: 3rem;&quot;>🌍</div>';">
				</div>

				<div class="portfolio-item__content">
					<div class="portfolio-item__info">
						<h2 class="portfolio-item__title">{{ work.title }}</h2>
						<p class="portfolio-item__subtitle">{{ work.subtitle }}</p>
					</div>
				</div>

			</a>

		</div>

		{% endfor %}

	</div>

</section>