---
layout: default
title: Case Studies
permalink: /case-studies/
---

<div class="home case-studies">
  <h1 class="pageTitle">Case Studies</h1>
  {%- assign case_studies = paginator.posts | default: site.posts -%}
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
  </div>
  <div class="pagination">
    {%- if paginator and paginator.previous_page -%}
    <a href="{{ paginator.previous_page_path | relative_url }}" class="previous button__outline">Newer Posts</a>
    {%- endif -%}
    {%- if paginator and paginator.next_page -%}
    <a href="{{ paginator.next_page_path | relative_url }}" class="next button__outline">Older Posts</a>
    {%- endif -%}
  </div>
</div>
