---
layout: default
pagination:
  data: collections.notes
  size: 9
---
# Notes

These are my notes.

## Most recent notes

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
