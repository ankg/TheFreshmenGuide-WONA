---
layout: default
title:  "Departments"
date:   2015-06-26 12:28:01
categories: [section]
excerpt: Have a look at the respective departments of IIT Roorkee.
class: ch-img-4
cover: departments_cover.jpg
--- 	
<h1>Departments</h1>
<div class="container">
    <section class="main">
      <ul class="ch-grid">
        {% for post in site.posts %}
          {% if post.categories contains 'departments' %}
            <li>
             <a href="{{post.url | prepend: site.baseurl}}" target="_blank">
                <div class="ch-item {{post.class}}">
                  <div class="ch-info">
                    <h3>{{post.title}}</h3>
                    <p>{{post.excerpt}}</p>
                  </div>
                </div>
             </a>
            </li>
          {% endif %}
        {% endfor %}
      </ul>
    </section>
</div>