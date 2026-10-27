---
layout: default
title: Home
---
<section class="hero">
  <p class="eyebrow">Pharmaceutical Information Technology</p>
  <h1>Duc Tung <span>Nguyen</span></h1>
  <p class="subtitle">Dược học · Dữ liệu · Công nghệ · Học thuật</p>
  <p class="motto">“Better data. Better decisions. For a healthier tomorrow.”</p>
  <hr class="rule">
  <p><a class="button primary" href="{{ '/research/' | relative_url }}">Explore my work</a>
  <a class="button" href="{{ '/notes/' | relative_url }}">Read my notes</a></p>
</section>

<section>
  <h2 class="section-title">Fields of interest</h2>
  <div class="cards">
    <article class="card"><p class="number">01 / DATA</p><h3>Pharmaceutical Data</h3><p>Data standardization, analytics, visualization and decision support in pharmacy.</p><a class="text-link" href="{{ '/research/' | relative_url }}">Explore →</a></article>
    <article class="card"><p class="number">02 / RESEARCH</p><h3>Health Economics & HTA</h3><p>Economic evaluation, hospital finance and evidence-informed healthcare decisions.</p><a class="text-link" href="{{ '/projects/' | relative_url }}">Projects →</a></article>
    <article class="card"><p class="number">03 / TECHNOLOGY</p><h3>AI & Software</h3><p>Practical applications of AI, automation and software development in pharmacy.</p><a class="text-link" href="{{ '/projects/' | relative_url }}">View projects →</a></article>
  </div>
</section>

<section class="split">
  <div>
    <h2 class="section-title">Recent notes</h2>
    {% assign posts = site.posts | slice: 0, 5 %}
    {% if posts.size > 0 %}
      {% for post in posts %}
      <div class="post-row"><time>{{ post.date | date: "%d %b %Y" }}</time><a href="{{ post.url | relative_url }}">{{ post.title }}</a></div>
      {% endfor %}
    {% else %}
      <p class="muted">Chưa có bài viết. Thêm file Markdown vào thư mục <code>_posts</code>.</p>
    {% endif %}
    <p><a class="text-link" href="{{ '/notes/' | relative_url }}">All notes →</a></p>
  </div>
  <div>
    <h2 class="section-title">YouTube</h2>
    <div class="placeholder"><strong>Video / channel</strong><p>Thay nội dung này bằng video nhúng hoặc liên kết kênh YouTube.</p><a class="text-link" href="https://www.youtube.com/" target="_blank" rel="noopener">Visit YouTube ↗</a></div>
  </div>
</section>
<div class="quote">“Học hôm nay, ứng dụng ngày mai.”</div>
