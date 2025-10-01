---
layout: default
title: Research Overview
subtitle: Projects in Conflict, Violence, and Social Movements
description: Overview of David Sorge's research projects on conflict escalation, de-escalation, and violence in South Asia.
featured_image: /images/social.jpg
permalink: /research-overview/
---

<img src="../images/Sorge_Research_Program.png" alt="David Sorge's Research Agenda" style="max-width: 100%; height: auto;"/>

<section class="single" style="padding-bottom: 1rem;">
<div class="wrap" markdown="1">

A brief statement of my research agenda is available [here](docs/Sorge_Research_Statement.pdf), and a more detailed version is available [here](docs/Sorge_Research_Statement_long.pdf)

</div>
</section>

<section class="portfolio" style="padding-top: 1rem;">

	<div class="content-wrap portfolio-wrap">

		{% assign sorted_research = site.research | sort: 'path' %}
		{% for project in sorted_research %}

		<div class="portfolio-item">

			<a class="portfolio-item__link" href="{{ project.url | relative_url }}">

				<div class="portfolio-item__image">
					<img src="{{ project.featured_image | relative_url }}" alt="{{ project.title }}" style="width: 100%; height: 100%; object-fit: cover;" onerror="this.style.display='none'; this.parentNode.innerHTML='<div style=&quot;color: #666; font-size: 3rem;&quot;>📊</div>';">
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

