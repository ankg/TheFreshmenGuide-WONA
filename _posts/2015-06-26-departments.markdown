---
layout: default
title:  "Departments"
date:   2015-06-26 12:28:01
categories: [section]
excerpt: A highly factual, precisely calculated dose of all that a faccha needs to know about the branches that exist or pretend to exist in IITR.
class: ch-img-4
cover: departments_cover.jpg
--- 	
<div class="container">
    <section class="main">
      <ul class="ch-grid">
        {% for post in site.posts %}
          {% if post.categories contains 'departments' %}
            <li>
             <a href="{{post.url}}" target="_blank">
                <div class="ch-item {{post.class}}">
                  <div class="ch-info">
                    <h3>{{post.title}}</h3>
                  </div>
                </div>
             </a>
            </li>
          {% endif %}
        {% endfor %}
      </ul>
    </section>
</div>