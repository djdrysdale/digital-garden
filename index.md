---
layout: default
---
# Moby Diction
Welcome to my digital notes. Hope you find them interesting.

{% for post in pagination.items %}

  <div class="card" style="width: 18rem;">
    <img src="..." class="card-img-top" alt="...">
    <div class="card-body">
      <p class="card-text">{{ post.data.description }}</p>
    </div>
  </div>


    <h2>{{ post.data.title }}</h2>
    <p></p>
    <a href="{{ post.url }}">Read more</a>
{% endfor %}
