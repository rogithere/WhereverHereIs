---
layout: page
title: "Wherever Here Is"
---

## Latest Posts

<div class="posts">
  {% for post in site.posts %}
    <article class="post">
      <h3><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h3>
      <div class="post-meta">
        <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time>
      </div>
      <div class="post-excerpt">
        {{ post.excerpt }}
      </div>
    </article>
    <hr />
  {% endfor %}
</div>