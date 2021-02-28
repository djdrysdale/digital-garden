---
layout: default
title: Moby Diction
pagination:
  data: collections.posts
  size: 3
  reverse: true
---

Hi. I'm David Drysdale.

I'm a design strategist and researcher based in London, Ontario, Canada.

It's my mission to help people, teams, and organizations think more strategically, make better decisions, and achieve better results.

## Recent blog posts

<div class="row py-4">

  {% for post in pagination.items %}
    <div class="card-body col-12 col-md-4 border-bottom py-10 px-10">
        <p class="card-text">
          <a href="{{ post.url }}">{{ post.data.title }}</a>
        </p>
        <p class="card-text">
          {{ note.data.description }}
        </p>
        <p>
          <a href="{{ note.url }}">Read more...</a>
        </p>

    </div>
  {% endfor %}

</div>
<!--
  {% for post in pagination.items %}

      <div class="col-sm-6">
        <div class="card">
          <div class="card-body">
          <h5 class="card-title">{{ post.data.title }}</h5>
          <h6 class="card-subtitle mb-2 text-muted">{{ post.data.category }}</h6>
          <p class="card-text">{{ post.data.description }}</p>
          <a href="{{ post.url }}" class="btn btn-primary">Read more</a>
        </div>
      </div>

  {% endfor %}

{% include recentposts.html %}
-->
