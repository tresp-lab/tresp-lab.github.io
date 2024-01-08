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
    type: LMU
    year: 2022
    nowAt: Google Deepmind/ UK
  - name: Dr. Ahmed Frikha
    website: https://www.linkedin.com/in/sahandsharifzadeh/?locale=de_DE
    type: LMU
    year: 2022
    nowAt: Huawei, München
  - name: Dr. Zhen Han
    website: https://sites.google.com/view/zhenhan/home?authuser=0
    type: LMU
    year: 2022
    nowAt: Amazon/ UK
  - name: Dr. Jindong Gu
    website: https://jindonggu.github.io/
    type: LMU
    year: 2022
    nowAt: University of Oxford & Google Research/ UK
  - name: Dr. Max Berrendorf
    website: https://www.dbs.ifi.lmu.de/cms/personen/mitarbeiter/berrendorf/index.html
    type: LMU
    year: 2022
    nowAt: 
  - name: Dr. Zhiliang Wu
    website: https://zhiliangwu.github.io/
    type: LMU
    year: 2022
    nowAt: Siemens, München
  - name: Dr. Marcel Hildebrandt
    website: https://www.linkedin.com/in/marcel-hildebrandt-523805114/
    type: LMU
    year: 2021
    nowAt: Siemens, München
  - name: Dr. Rui Zhao
    website: https://ruizhaogit.github.io/
    type: LMU
    year: 2020
    nowAt: Tencent AI Lab & Robotics X/ China
  - name: Dr. Yunpu Ma
    website: https://www.dbs.ifi.lmu.de/cms/personen/mitarbeiter/ma/index.html
    type: LMU
    year: 2020
    nowAt:
  - name: Dr. Stephan Baier
    website: 
    type: LMU
    year: 2019
    nowAt:
  - name: Dr. Yinchong Yang
    website: https://www.xing.com/profile/Yinchong_Yang
    type: LMU
    year: 2018
    nowAt: Siemens, München
  - name: Dr. Cristóbal Esteban
    website: https://www.linkedin.com/in/cristobalesteban/
    type: LMU
    year: 2018
    nowAt:
  - name: Dr. Jonathan Boidol
    website: 
    type: LMU
    year: 2017
    nowAt:
  - name: Dr. Denis Krompaß
    website: https://www.linkedin.com/in/denis-krompa%C3%9F-0669b191/
    type: LMU
    year: 2015
    nowAt:
  - name: Dr. 
    website: 
    type: LMU
    year: 
    nowAt:
  - name: Dr. 
    website: 
    type: LMU
    year: 
    nowAt:
  - name: Dr. 
    website: 
    type: LMU
    year: 
    nowAt:
  - name: Dr. 
    website: 
    type: LMU
    year: 
    nowAt:
  - name: Dr. 
    website: 
    type: LMU
    year: 
    nowAt:
  - name: Dr. 
    website: 
    type: LMU
    year: 
    nowAt:
  - name: Dr. 
    website: 
    type: LMU
    year: 
    nowAt: 
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
