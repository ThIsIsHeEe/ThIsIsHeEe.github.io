---
layout: default
title: Archive
---

# 게시글 모음

<!-- {% assign postsByYearMonth = site.posts | group_by_exp: "post", "post.date | date: '%B %Y'" %}
{% for yearMonth in postsByYearMonth %}
  <h2>{{ yearMonth.name }}</h2>
  <ul>
    {% for post in yearMonth.items %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %} -->


<h1>Java Posts</h1>
<ul>
  {% assign java_posts = site.posts | where: "category", "Java" | sort: "date" %}
    {% for post in java_posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
    {% endfor %}
</ul>



<h1>Spring Posts</h1>
<ul>
  {% assign spring_posts = site.posts | where: "category", "Spring" | sort: "date" %}
    {% for post in spring_posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
    {% endfor %}
</ul>