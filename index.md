---
layout: page
title: Dshining - Let the data shine for you!
tagline: Supporting tagline
---
{% include JB/setup %}

{% for post in site.posts limit:8 %}
   <!-- here add you post markup -->
   <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
   <p class="post_title">
    <span class="date">{{post.date | date: "%Y-%m-%d"}}</span>
  </p>
  <br>
  <div class="content">
    {{ post.content | split: '<!-- more -->' | first }}
  </div>
  <br>
{% endfor %}



