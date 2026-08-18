---
layout: default
title: Home
description: Homepage for the Cal Poly Data Design Lab.
---

<section class="hero">
  <div class="hero-brand">
    <img class="hero-logo" src="{{ '/assets/img/logo.svg' | relative_url }}" alt="" width="96" height="96">
    <div>
      <p class="eyebrow">{{ site.data.site_settings.institution }}</p>
      <h1>{{ site.data.site_settings.lab_name }}</h1>
    </div>
  </div>
  <p class="subtitle">{{ site.data.site_settings.tagline }}</p>
  <p>
    We study how people make sense of data and build tools that help communities,
    researchers, and practitioners analyze, visualize, and communicate with data.
    Our work sits at the intersection of <em>data science</em>,
    <em>data visualization</em>, and <em>human-computer interaction</em>.
  </p>
  
  <p class="button-row">
    <a class="button" href="{{ '/projects/' | relative_url }}">Explore projects</a>
    <a class="button secondary" href="{{ '/join/' | relative_url }}">Join the lab</a>
  </p>
</section>


<section>
  <h2>Upcoming events</h2>
  <p>Join us for reading groups, colloquia, invited speakers, and other lab events.</p>
  {% include event-calendar.html events=site.data.events.upcoming limit=1 %}
  <p class="button-row">
    <a class="button secondary" href="{{ '/events/' | relative_url }}">View all events</a>
  </p>
</section>

<section>
  <h2>Ongoing projects</h2>
  {% include project-list.html projects=site.data.projects.ongoing %}
</section>

<section>
  <h2>Affiliated people</h2>
  <h3>Faculty</h3>
  {% include people-list.html people=site.data.people.faculty %}
  <h3>Students</h3>
  {% include people-list.html people=site.data.people.students %}
</section>
