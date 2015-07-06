---
layout: default
title:  "campus Groups"
date:   2015-06-26 12:28:01
categories: [section]
excerpt: Explore the various socities at IITR
class: ch-img-13
cover: groups_cover.jpg
--- 	
<h1>Campus Groups</h1>
<div class="container">
    <section class="main">
      <ul class="ch-grid">
        {% for post in site.posts %}
          {% if post.categories contains 'groups' %}
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
