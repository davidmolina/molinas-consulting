---
layout: default
title: Estudios de Caso
permalink: /estudios-de-caso/
lang: es
---

<div class="home case-studies">
  <h1 class="pageTitle">Estudios de Caso</h1>
  {%- assign all_posts = paginator.posts | default: site.posts -%}
  {%- assign case_studies = all_posts | where: "lang", "es" -%}
  <div class="posts noList">
    {%- for post in case_studies -%}
    <article>
      <span class="date">{{ post.date | date: '%B %d, %Y' }}</span>
      <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </h3>
      <p>
        {%- if post.description -%}
          {{ post.description }}
        {%- else -%}
          {{ post.excerpt | strip_html }}
        {%- endif -%}
      </p>
    </article>
    {%- endfor -%}
    {%- if case_studies.size == 0 -%}
    <article>
      <h3>Proximamente</h3>
      <p>Estamos publicando estudios de caso en espanol.</p>
    </article>
    {%- endif -%}
  </div>
  <div class="pagination">
    {%- if paginator and paginator.previous_page -%}
    <a href="{{ paginator.previous_page_path | relative_url }}" class="previous button__outline">Publicaciones nuevas</a>
    {%- endif -%}
    {%- if paginator and paginator.next_page -%}
    <a href="{{ paginator.next_page_path | relative_url }}" class="next button__outline">Publicaciones anteriores</a>
    {%- endif -%}
  </div>
</div>
