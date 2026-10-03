---
layout: page
title: projects
permalink: /projects/
<<<<<<< HEAD
description: Hands-on research and engineering projects, newest first.
nav: true
nav_order: 2
years: [2025, 2024, 2023, 2022, 2021, 2020, 2019, 2018, "Earlier"]
=======
description: Selected research and engineering projects, newest first.
nav: true
nav_order: 2
years: [2026, 2025, 2024, 2023, 2022]
>>>>>>> 61ab5982abc27bf1f17e6387ca6b616b1ea1c821
---

<div class="project-list">
  {% for year in page.years %}
    {% assign projects_for_year = site.data.projects | where: "year", year %}
    {% if projects_for_year.size > 0 %}
      <section class="project-year-group" aria-labelledby="projects-{{ year }}">
        <h2 id="projects-{{ year }}" class="project-year">{{ year }}</h2>
        {% for project in projects_for_year %}
<<<<<<< HEAD
          <article class="project-entry">
            <a class="project-main" href="{{ project.url | relative_url }}">
              <div class="project-icon" aria-hidden="true"><i class="fas {{ project.icon }}"></i></div>
              <div class="project-entry-content">
                <h3>{{ project.title }}</h3>
                <span class="project-summary">{{ project.description }}</span>
              </div>
            </a>
            {% if project.code %}
              <div class="project-links">
                <a href="{{ project.code }}" target="_blank" rel="noopener noreferrer">Code <span aria-hidden="true">↗</span></a>
              </div>
            {% endif %}
          </article>
=======
          <article class="project-entry">
            <div class="project-icon" aria-hidden="true"><i class="fas {{ project.icon }}"></i></div>
            <div class="project-entry-content">
              <h3>{{ project.title }}</h3>
              <p>{{ project.description }}</p>
              <div class="project-links">
                {% for link in project.links %}
                  <a href="{{ link.url }}" target="_blank" rel="noopener noreferrer">{{ link.label }}</a>
                {% endfor %}
              </div>
            </div>
          </article>
>>>>>>> 61ab5982abc27bf1f17e6387ca6b616b1ea1c821
        {% endfor %}
      </section>
    {% endif %}
  {% endfor %}
</div>
