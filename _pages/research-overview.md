---
layout: default
title: Research Overview
subtitle: Projects in Conflict, Violence, and Social Movements
description: Overview of David Sorge's research projects on conflict escalation, de-escalation, and violence in South Asia.
featured_image: /images/social.jpg
permalink: /research-overview/
---

<section class="portfolio">

	<div class="content-wrap portfolio-wrap">

		{% for project in site.research reversed %}

		<div class="portfolio-item">

			<a class="portfolio-item__link" href="{{ project.url | relative_url }}">

				<div class="portfolio-item__image">
					<img src="{{ project.featured_image | relative_url }}" alt="{{ project.title }}">
				</div>

				<div class="portfolio-item__content">
					<div class="portfolio-item__info">
						<h2 class="portfolio-item__title">{{ project.title }}</h2>
						<p class="portfolio-item__subtitle">{{ project.subtitle }}</p>
					</div>
				</div>

			</a>

		</div>

		{% endfor %}

	</div>

</section>