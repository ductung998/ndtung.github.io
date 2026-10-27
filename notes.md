---
layout: default
title: Notes
permalink: /notes/
---
<p class="eyebrow">Notes & writing</p>
<h1>Notes</h1>
<p class="muted">Mỗi bài viết là một file Markdown trong thư mục <code>_posts</code>. Danh sách bài viết sẽ tự động cập nhật.</p>
{% for post in site.posts %}
<article class="post-list-item">
  <p class="number">{{ post.date | date: "%d %b %Y" }} · {{ post.categories | join: ", " }}</p>
  <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
  <p>{{ post.excerpt | strip_html | truncate: 220 }}</p>
  <a class="text-link" href="{{ post.url | relative_url }}">Read more →</a>
</article>
{% endfor %}
