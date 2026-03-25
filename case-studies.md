---
layout: default
title: Case Studies
permalink: /case-studies/
description: Structured case studies showing MESLO-driven estimating, operations, and digital system implementations.
---

<div class="home case-studies">
  <h1 class="pageTitle">Case Studies</h1>
  <p class="intro">
    Implementation snapshots from contractors and service operators working to
    improve estimating discipline, operating structure, and execution clarity.
  </p>

  <script type="application/ld+json">
  {
    "@context": "https://schema.org",
    "@type": "BreadcrumbList",
    "itemListElement": [
      {
        "@type": "ListItem",
        "position": 1,
        "name": "Home",
        "item": "{{ '/' | absolute_url }}"
      },
      {
        "@type": "ListItem",
        "position": 2,
        "name": "Case Studies",
        "item": "{{ '/case-studies/' | absolute_url }}"
      }
    ]
  }
  </script>

  <div class="featured-cases">
    <h2>Featured Case Studies</h2>
    <div class="posts noList">
      <article>
        <h3><a class="post-link" href="{{ '/case-studies/hvac-dispatch-system/' | relative_url }}">Automating Dispatch Response for Residential Contractor</a></h3>
        <p>Cut response times from hours to minutes with a dispatch app, intake routing, and SOPs.</p>
        <span class="tag">Automation / Operations</span>
      </article>
      <article>
        <h3><a class="post-link" href="{{ '/case-studies/estimating-framework/' | relative_url }}">Estimating Framework for Residential Contractor</a></h3>
        <p>Built a margin-aware estimating system with organized bid docs and repeatable takeoffs.</p>
        <span class="tag">Estimating / Cost Control</span>
      </article>
      <article>
        <h3><a class="post-link" href="{{ '/case-studies/real-estate-cloud-ops/' | relative_url }}">Real Estate Firm: Cloud Ops &amp; Reporting</a></h3>
        <p>Unified tooling, roles, and reporting for faster follow-up and leadership visibility.</p>
        <span class="tag">Digital Infrastructure</span>
      </article>
    </div>
  </div>

  {%- assign all_posts = paginator.posts | default: site.posts -%}
  {%- assign case_studies = all_posts | where_exp: "post", "post.lang != 'es'" -%}
  {%- assign featured_urls = "/case-studies/hvac-dispatch-system/,/case-studies/estimating-framework/,/case-studies/real-estate-cloud-ops/" | split: "," -%}
  <div class="posts noList">
    {%- for post in case_studies -%}
    {%- unless featured_urls contains post.url -%}
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
    {%- endunless -%}
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

  <div class="related-outcomes">
    <h2>Related Outcomes</h2>
    <ul>
      <li>Improved estimating clarity and margin control</li>
      <li>Reduced dispatch response time from hours to minutes</li>
      <li>Increased inbound leads through website improvements</li>
    </ul>
    <p><a href="{{ '/results/' | relative_url }}">View all results</a></p>
  </div>
</div>
