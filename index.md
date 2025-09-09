---
layout: default
---

<div class="home">
  {%- if page.title -%}
    <h1 class="page-heading">{{ page.title }}</h1>
  {%- endif -%}

  <h2>Welcome to Duy's Blog</h2>
  
  <h3>About Me</h3>
  <p>I'm Duy, originally from Can Loc, Ha Tinh, Vietnam. I graduated from Ha Tinh Gifted High School and later earned both my bachelor's and master's degrees in Computer Science from The University of Aizu in Japan.</p>
  
  <p>I joined Fast Accounting Co Ltd in 2019 as their first Software Engineer and have been with the company since. After successfully building several core products and experiencing the company's IPO in 2023, I was promoted to Principal Engineer in 2024. Currently, I'm leading the AI Agent team, focusing on cutting-edge AI solutions.</p>
  
  <p>This blog is a place for me to keep track of knowledge I learn in various topics including AI, Software Engineering, Real Estate Investment, etc. I share insights, learning experiences, and analysis across these areas that capture my interest and professional development.</p>

  {{ content }}

  {%- if site.posts.size > 0 -%}
    <h2 class="post-list-heading">Recent Posts</h2>
    <ul class="post-list">
      {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
      {%- for post in site.posts -%}
      <li>
        <span class="post-meta">{{ post.date | date: date_format }}</span>
        <h3>
          <a class="post-link" href="{{ post.url | relative_url }}">
            {{ post.title | escape }}
          </a>
        </h3>
        {%- if site.show_excerpts -%}
          {{ post.excerpt }}
        {%- endif -%}
      </li>
      {%- endfor -%}
    </ul>

    <p class="feed-subscribe">
      <a href="{{ 'feed.xml' | relative_url }}">
        <svg class="svg-icon orange">
          <use xlink:href="{{ 'assets/minima-social-icons.svg#rss' | relative_url }}"></use>
        </svg><span>Subscribe</span>
      </a>
    </p>
  {%- endif -%}

</div>
