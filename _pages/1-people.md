---
layout: page
permalink: /people/
title: People
description: 
nav: true
nav_order: 1

staff:
  title: Team Members
  people:
    - name: Volker Tresp
      description: Prof. Dr. and Head of Tresp Lab
      website: https://www.dbs.ifi.lmu.de/~tresp/
      picture: people/tresp.jpeg
    - name: Yunpu Ma
      description: Postdoc
      website: https://www.dbs.ifi.lmu.de/cms/personen/mitarbeiter/ma/index.html
      picture: people/yunpu-ma.jpg
    - name: Hang Li
      description: PhD Student
      website: https://hangligit.github.io/
      picture: people/demo.jpg
    - name: Shuo Chen
      description: PhD Student (2023 - Present)
      website: https://chenxshuo.github.io
      picture: people/shuo.png
      interests: multimodal models, robustness, vision-language models
alumni:
  title: Alumni
  people:
  - name: Dr. Sahand Sharifzadeh
    website: https://www.linkedin.com/in/sahandsharifzadeh/?locale=de_DE
    type: PhD
    year: 2022
    nowAt: Google Deepmind
  - name: Dr. Zhen Han
    website: https://sites.google.com/view/zhenhan/home?authuser=0
    type: PhD
    year: 2022
    nowAt: Amazon
  - name: Dr. Jindong Gu
    website: https://jindonggu.github.io/
    type: PhD
    year: 2022
    nowAt: University of Oxford & Google Research
  
---

<div class="projects">

TBD

<h2 class="category">{{page.staff.title}}</h2>
  <div class="grid">
    {%- for person in page.staff.people -%}
        <article class="grid-item card">
          {% if person.picture -%}
            <img class=" rounded-circle" src="/assets/img/{{person.picture}}" alt="Portrait ({{person.name}})" width="auto" height="auto">
          {%- else -%}
            <img class=" rounded-circle" src="/assets/img/prof_pic.jpg" alt="Portrait ({{person.name}})" width="auto" height="auto">
          {%- endif -%}
        <div class="card-body">
          <!-- <h2 class="card-title">{{person.name}}</h2> -->
          <h2 class="card-title">
            {% if person.website -%}
              <a href="{{person.website}}">{{person.name}}</a>
            {%- else -%}
              {{person.name}}
            {%- endif -%}
          </h2>
          <div class="card-text">
            {{person.description}}
            <!-- {{person.interests}} -->
            <!-- <p style="margin-bottom: 0rem;">{{person.description}}</p> 
            <ul class="network-icon" aria-hidden="true">
            {% if person.website -%}
              <li><a href="{{person.website}}"><i class="fas fa-globe"></i></a></li>
            {%- endif -%}
            {% if person.email -%}
              <li><a role="button" class="email" style="color: var(--global-theme-color)"><i class="fas fa-envelope"></i></a></li>
            {%- endif -%}
            {% if person.googlescholar -%}
              <li><a href="{{person.googlescholar}}"><i class="ai ai-google-scholar"></i></a></li>
            {%- endif -%}
            {% if person.github -%}
              <li><a href="{{person.github}}"><i class="fab fa-github"></i></a></li>
            {%- endif -%}
            {% if person.twitter -%}
              <li><a href="{{person.twitter}}"><i class="fab fa-twitter"></i></a></li>
            {%- endif -%}
          </ul>
          {% if person.email -%}
            <div class="email hidden">
              <p>{{ person.email }}</p>
            </div>
          {%- endif -%} -->
            </div>
          </div>
        </article>
    {%- endfor -%}
  </div>



  <h2 class="category"> Former Ph.D. Students </h2>
  <ul>
  {%- for person in page.alumni.people -%}
    <li>{% if person.website -%}
              <a href="{{person.website}}">{{person.name}} </a>
            {%- else -%}
              {{person.name}}
        {%- endif -%}
        ({{person.type}}, {{person.year}}), now at {{person.nowAt}}</li>
  {%- endfor -%}
  </ul>
  TBD
</div>
