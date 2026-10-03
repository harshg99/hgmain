---
layout: page
title: projects
permalink: /projects/
description: Selected research and engineering projects, newest first.
nav: true
nav_order: 2
years: [2026, 2025, 2024, 2023, 2022]
---

<div class="project-list">
  {% for year in page.years %}
    {% assign projects_for_year = site.data.projects | where: "year", year %}
    {% if projects_for_year.size > 0 %}
      <section class="project-year-group" aria-labelledby="projects-{{ year }}">
        <h2 id="projects-{{ year }}" class="project-year">{{ year }}</h2>
        {% for project in projects_for_year %}
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
        {% endfor %}
      </section>
    {% endif %}
  {% endfor %}
</div>
