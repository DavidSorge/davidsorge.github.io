---
layout: default
title: 'Teaching Overview'
subtitle: 'Creating Spaces to Practice the Community of Truth'
description: 'My teaching philosophy centers on creating spaces where students practice critical thinking, dialogue across difference, and connection between research and real-world challenges.'
featured_image: '/images/teaching-philosophy.jpg'
permalink: /teaching-overview/
---

<section class="portfolio">

	<div class="content-wrap portfolio-wrap">

		<h2 style="text-align: center; margin-bottom: 2rem; position: relative; z-index: 10; background: white; padding: 1rem 0;">Teaching Portfolio</h2>

		{% assign quotes = "YES! YES!! YES!!! Prof. Sorge is seriously one of the best professors in the department… he is so passionate about the material and does his best to cultivate this same passion and interest in the students he teaches.|Student, Social Theory, Fall 2024~He made a class that could have been really difficult and dense, interesting, diverse and fun, while still pushing and challenging us.|Student, Social Theory, Spring 2025~His attentiveness to every student in the class and his efforts to create a welcoming environment contribute to the positive learning experience. Additionally, the course content is academically stimulating, making it especially valuable for students eager to explore the complexities of the contemporary world.|Student, Global Sociology, Fall 2023~David absolutely created an accessible and inclusive course experience. I struggle to think of a professor who has done this better.|Student, Social Dynamics of Violence, Spring 2025~One of the main reasons I decided to be a Sociology major was because of Professor Sorge.|Student, The Social Life of Emotions, Spring 2025" | split: "~" %}

		{% assign sorted_courses = site.teaching | sort: 'path' %}
		{% for course in sorted_courses %}

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

		<!-- Show quote after courses 2, 3, 5, 7, 9 -->
		{% if forloop.index == 2 %}
			{% assign quote_parts = quotes[0] | split: "|" %}
			{% assign quote_text = quote_parts[0] %}
			{% assign quote_attribution = quote_parts[1] %}

			<div class="portfolio-item" style="background: white; border-radius: 8px; border: 1px solid #e9ecef;">
				<div style="padding: 2rem; color: #1e6091; text-align: center; min-height: 200px; display: flex; flex-direction: column; justify-content: center;">
					<blockquote style="font-style: italic; font-size: 1.1rem; line-height: 1.6; margin: 0 0 1rem 0; border: none; padding: 0; color: #1e6091;">
						"{{ quote_text }}"
					</blockquote>
					<cite style="font-size: 0.9rem; opacity: 0.8; font-weight: 300; color: #1e6091;">
						— {{ quote_attribution }}
					</cite>
				</div>
			</div>
		{% endif %}

		{% if forloop.index == 4 %}
			{% assign quote_parts = quotes[1] | split: "|" %}
			{% assign quote_text = quote_parts[0] %}
			{% assign quote_attribution = quote_parts[1] %}

			<div class="portfolio-item" style="background: white; border-radius: 8px; border: 1px solid #e9ecef;">
				<div style="padding: 2rem; color: #1e6091; text-align: center; min-height: 200px; display: flex; flex-direction: column; justify-content: center;">
					<blockquote style="font-style: italic; font-size: 1.1rem; line-height: 1.6; margin: 0 0 1rem 0; border: none; padding: 0; color: #1e6091;">
						"{{ quote_text }}"
					</blockquote>
					<cite style="font-size: 0.9rem; opacity: 0.8; font-weight: 300; color: #1e6091;">
						— {{ quote_attribution }}
					</cite>
				</div>
			</div>
		{% endif %}

		{% if forloop.index == 6 %}
			{% assign quote_parts = quotes[2] | split: "|" %}
			{% assign quote_text = quote_parts[0] %}
			{% assign quote_attribution = quote_parts[1] %}

			<div class="portfolio-item" style="background: white; border-radius: 8px; border: 1px solid #e9ecef;">
				<div style="padding: 2rem; color: #1e6091; text-align: center; min-height: 200px; display: flex; flex-direction: column; justify-content: center;">
					<blockquote style="font-style: italic; font-size: 1.1rem; line-height: 1.6; margin: 0 0 1rem 0; border: none; padding: 0; color: #1e6091;">
						"{{ quote_text }}"
					</blockquote>
					<cite style="font-size: 0.9rem; opacity: 0.8; font-weight: 300; color: #1e6091;">
						— {{ quote_attribution }}
					</cite>
				</div>
			</div>
		{% endif %}

		{% if forloop.index == 7 %}
			{% assign quote_parts = quotes[3] | split: "|" %}
			{% assign quote_text = quote_parts[0] %}
			{% assign quote_attribution = quote_parts[1] %}

			<div class="portfolio-item" style="background: white; border-radius: 8px; border: 1px solid #e9ecef;">
				<div style="padding: 2rem; color: #1e6091; text-align: center; min-height: 200px; display: flex; flex-direction: column; justify-content: center;">
					<blockquote style="font-style: italic; font-size: 1.1rem; line-height: 1.6; margin: 0 0 1rem 0; border: none; padding: 0; color: #1e6091;">
						"{{ quote_text }}"
					</blockquote>
					<cite style="font-size: 0.9rem; opacity: 0.8; font-weight: 300; color: #1e6091;">
						— {{ quote_attribution }}
					</cite>
				</div>
			</div>
		{% endif %}

		{% if forloop.index == 9 %}
			{% assign quote_parts = quotes[4] | split: "|" %}
			{% assign quote_text = quote_parts[0] %}
			{% assign quote_attribution = quote_parts[1] %}

			<div class="portfolio-item" style="background: white; border-radius: 8px; border: 1px solid #e9ecef;">
				<div style="padding: 2rem; color: #1e6091; text-align: center; min-height: 200px; display: flex; flex-direction: column; justify-content: center;">
					<blockquote style="font-style: italic; font-size: 1.1rem; line-height: 1.6; margin: 0 0 1rem 0; border: none; padding: 0; color: #1e6091;">
						"{{ quote_text }}"
					</blockquote>
					<cite style="font-size: 0.9rem; opacity: 0.8; font-weight: 300; color: #1e6091;">
						— {{ quote_attribution }}
					</cite>
				</div>
			</div>
		{% endif %}

		{% endfor %}

	</div>

</section>

<section class="single">
<div class="wrap" markdown="1">


## Teaching Philosophy

A brief statement of my teaching philosophy is available [here](docs/Sorge_Teaching_Statement.pdf), and my reflections on the importance of justice, equity, diversity, and inclusion in the classroom is available [here](docs/Sorge_JEDI_Statement.pdf).


</div>
</section>