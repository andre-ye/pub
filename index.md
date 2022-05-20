---
layout: default
title: Home
---

View all articles below. Articles open in a new tab. Or, filter by [topic](#filter-by-topic) and [author](#filter-by-author).

<div class="posts">
  <em>
  {% for post in paginator.posts %}
      <li>
        <a href="{{ post.url | absolute_url }}" target="_blank">{{ post.title }}</a>
      </li>
  {% endfor %}
  </em>
</div>

---

## Filter by Topic

<!-- <div class="posts">
  {% assign tags =  site.posts | where: 'published', 'true' | map: 'topic' | join: ','  | split: ',' | uniq %}
  {% for tag in tags %}
      {{ tag }}
      <em>
      {% for post in paginator.posts %}
        {% if post.topic == tag %}
          <li>
            <a href="{{ post.url | absolute_url }}" target="_blank">{{ post.title }}</a>
          </li>
        {% endif %}
      {% endfor %}
      </em>
  {% endfor %}
</div> -->

---

## Filter by Author

<!-- <div class="pagination">
  {% if paginator.next_page %}
    <a class="pagination-item older" href="{{ paginator.next_page_path | absolute_url }}">Older</a>
  {% else %}
    <span class="pagination-item older">Older</span>
  {% endif %}
  {% if paginator.previous_page %}
    {% if paginator.page == 2 %}
      <a class="pagination-item newer" href="{{ '/' | absolute_url }}">Newer</a>
    {% else %}
      <a class="pagination-item newer" href="{{ paginator.previous_page_path | absolute_url }}">Newer</a>
    {% endif %}
  {% else %}
    <span class="pagination-item newer">Newer</span>
  {% endif %}
</div> -->
