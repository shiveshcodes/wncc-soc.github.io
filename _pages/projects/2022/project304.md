---
layout: project
title: Seasons of Code
project: Light (Rendering) Engine
topics:
    - Development
mentors:
    - Divyansh Tiwari
    - Tirthankar Majumdar
    
mentees:
- 5-6
    
permalink: /soc/projects/2023/project304
---

<h2 class="display1 m-3 p-3 text-center project-title">{{page.project}}</h2>

{% for project in site.data.settings.soc-items %}
{% if project.title == page.project %}
<div class ="img-soc d-block"> 
    <img src="{{ site.baseurl }}/{{ project.image }}" alt="{{ project.project}}" class="image-1">
    <img src="{{ site.baseurl }}/{{ project.image }}" alt="{{ project.project}}" class="image-2">
    <img src="{{ site.baseurl }}/{{ project.image }}" alt="{{ project.project}}" class="image-3">
    <img src="{{ site.baseurl }}/{{ project.image }}" alt="{{ project.project}}" class="image-4">
</div>
<div class = "mobile-img-soc">
  <img src="{{ site.baseurl }}/{{ project.image }}"  width = "300" height="300" alt="{{ project.project}}" class="border rounded">
  </div>
<div>
    <br>
    <ul>
        {% for topic in page.topics %}
        <li style = "display: inline"><h4 class="text-primary text-center">{{topic}}</h4></li>
        {% endfor %}
    </ul>
    <br>
    <h4 class="display3  ">Mentors :</h4> 
    <ul>
        {% for mentor in page.mentors %}
        <li><p class="lead">{{mentor}}</p></li>
        {% endfor %}
    </ul>
    <h4 class="display3  ">Mentees :</h4> 
    <ul>
        {% for mentee in page.mentees %}
        <li><p class="lead">{{mentee}}</p></li>
        {% endfor %}
    </ul>
</div>
<div>
    <p class="display3 project-desc" style = "font-size:22px;" >
        <br>
   https://github.com/Physicc/Light

Light is a lightweight game engine written in C++17. It is currently in development and is not yet ready for use

You will be working in developing and designing rendering algorithms, and implement the rendering subsystem of the game engine. Some of the systems you will be working on:
1) Material System
2) Blinn-Phong Shading System
3) PBR Shading System
4) Shadows
<br>
PreReqs:
<br>
Come with lots of Enthusiasm. No pre requisites as such. 
</p>
<div class ="d-flex">
<div>
    <h4 class="display3" style="margin:40px 0px 40px 0px;">Tentative Timeline :</h4>
    <table class = "table table-striped">
  <thead>
    <tr>
      <th>Week Number</th>
      <th>Tasks to be Completed</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Week 1</strong></td>
      <td> Learn basics of rendering from learnopengl.com</td>
    </tr>
    <tr>
      <td><strong>Week 2</strong></td>
      <td> Implement basic rendering system using core opengl</td>
    </tr>
    <tr>
      <td><strong>Week 3  </strong></td>
      <td>Setup and walkthrough the Light codebase on system </td>
    </tr>
    <tr>
      <td><strong>Week 4  </strong></td>
      <td>Directional Lights, Spot Lights</td>
    </tr>
    <tr>
      <td><strong>Week 5  </strong></td>
      <td>Directional Light, Spot Light Shadow Maps</td>
    </tr>
    <tr>
      <td><strong>Week 6-7 </strong></td>
      <td>Material System</td>
    </tr>
    <tr>
      <td><strong>Week 8</strong></td>
      <td>Physically Based Rendering System </td>
    </tr>
        </tbody>
    </table>
</div>
</div>
{% endif %}
{% endfor %}
