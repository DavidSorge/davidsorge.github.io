---
layout: default
title: 'DANGA Lab Overview'
subtitle: 'Dynamics of Aggression and Nonviolent Group Action'
description: 'The DANGA Lab investigates how violence emerges, diffuses, and can be transformed through computational methods and collaborative research.'
featured_image: '/images/danga-lab.jpg'
permalink: /danga-overview/
---

<section class="single">

	<div class="wrap">

		<h2>About DANGA Lab</h2>

		<p>The <strong>Dynamics of Aggression and Nonviolent Group Action (DANGA) Lab</strong> brings together students and faculty to investigate ethno-religious violence, social movements, and transformative justice approaches. "DANGA" means "riot" in Hindi, reflecting our focus on understanding how violence emerges and how it can be transformed.</p>

		<h3>Research Focus</h3>

		<p>Our research operates across three interconnected levels:</p>

		<ul>
		<li><strong>Micro:</strong> Emotional dynamics of violent confrontation and de-escalation</li>
		<li><strong>Meso:</strong> Movement ecology and tactical diffusion patterns</li>
		<li><strong>Macro:</strong> Media networks, religious fields, and postcolonial state structures</li>
		</ul>

		<h3>Methods & Approach</h3>

		<ul>
		<li><strong>Computational text analysis</strong> of news reports and social media</li>
		<li><strong>GIS mapping</strong> of conflict patterns and diffusion</li>
		<li><strong>Ethnographic video analysis</strong> of collective action</li>
		<li><strong>"Human-in-the-loop"</strong> machine learning for protest event coding</li>
		<li><strong>Multi-modal analysis</strong> combining text, images, and video</li>
		</ul>

		<h3>Current Projects</h3>

		<ul>
		<li><strong>All-India Protest Event Dataset:</strong> Developing comprehensive database of collective action events using computational methods (supported by NSF ACCESS)</li>
		<li><strong>Riot Action Sequences:</strong> Computational models of escalation and de-escalation patterns</li>
		<li><strong>Media Diffusion Networks:</strong> Mapping how unrest spreads through vernacular media networks</li>
		</ul>

		<h3>Student Training</h3>

		<p>DANGA Lab provides undergraduate researchers with training in:</p>
		<ul>
		<li>Qualitative and computational research methods</li>
		<li>Data visualization and analysis</li>
		<li>Collaborative scholarship practices</li>
		<li>Connections between academic research and social justice</li>
		</ul>

		<h3>Resources & Tools</h3>

		<ul>
		<li><strong>Computational Resources:</strong> Access to high-performance computing through NSF ACCESS</li>
		<li><strong>Software Training:</strong> Python, R, GIS, qualitative analysis software</li>
		<li><strong>Data Sources:</strong> Times of India archives, social media APIs, government datasets</li>
		<li><strong>Research Library:</strong> Specialized collection on South Asian politics and social movements</li>
		</ul>

	</div>

</section>

<section class="portfolio">

	<div class="content-wrap portfolio-wrap">

		<h2 style="text-align: center; margin-bottom: 2rem; position: relative; z-index: 10; background: white; padding: 1rem 0;">Lab Members</h2>

		{% for member in site.danga reversed %}

		<div class="portfolio-item">

			<a class="portfolio-item__link" href="{{ member.url | relative_url }}">

				<div class="portfolio-item__image" style="min-height: 200px; background-color: #f5f5f5; display: flex; align-items: center; justify-content: center;">
					<img src="{{ member.featured_image | relative_url }}" alt="{{ member.title }}" style="width: 100%; height: 100%; object-fit: cover;" onerror="this.style.display='none'; this.parentNode.innerHTML='<div style=&quot;color: #666; font-size: 3rem;&quot;>👤</div>';">
				</div>

				<div class="portfolio-item__content">
					<div class="portfolio-item__info">
						<h2 class="portfolio-item__title">{{ member.title }}</h2>
						<p class="portfolio-item__subtitle">{{ member.subtitle }}</p>
					</div>
				</div>

			</a>

		</div>

		{% endfor %}

	</div>

</section>