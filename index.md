---
layout: default
---
# Moby Diction
Welcome to my digital notes. Hope you find them interesting.

{% for post in pagination.items %}
    <h2>{{ post.data.title }}</h2>
    <p>{{ post.data.description }}</p>
    <a href="{{ post.url }}">Read more</a>

  <div class="card" style="width: 18rem;">
    <div class="card-body">
      <h5 class="card-title">{{ post.data.title }}</h5>
      <h6 class="card-subtitle mb-2 text-muted">{{ post.data.category }}</h6>
      <p class="card-text">{{ post.data.description }}</p>
      <a href="{{ post.url }}" class="card-link">Read more</a>
    </div>
  </div>

{% endfor %}

{% for post in pagination.items %}
    <h2>{{ post.data.title }}</h2>
    <p>{{ post.data.description }}</p>
    <a href="{{ post.url }}">Read more</a>
{% endfor %}
