---
layout: default
---

<section>
  {% for post in site.posts limit: 5 %}
    <article>
      <header>
        <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
        <span>
          <time datetime="{{ post.date | date:"%Y-%m-%d" }}">{{ post.date | date:"%Y-%m-%d" }}</time>
        </span>
      </header>
      <section class="post">
        <p>{{ post.summary }}</p>
      </section>
    </article>
  {% endfor %}
</section>

<div id="archive-ref">
  <a href="/archive.html" class="circle-wrapper">
  <div class="circle">&nbsp;</div>
  <div class="circle">&nbsp;</div>
  <div class="circle">&nbsp;</div>
  </a>
</div>