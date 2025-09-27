---
layout: page
title: Home
---

<script>
document.addEventListener('DOMContentLoaded', function() {
    // Find and hide the auto-generated page title that says "Home"
    const pageContent = document.querySelector('.page-content');
    if (pageContent) {
        const firstH1 = pageContent.querySelector('h1');
        if (firstH1 && firstH1.textContent.trim() === 'Home') {
            firstH1.style.display = 'none';
        }
    }
});
</script>

# **Welcome!**

Here, I present ongoing research focused on numerical modeling and simulation of microstructure mechanics and evolution in crystalline materials, and how these phenomena influence macroscale material behavior.
My main research interests include:

- Grain boundary mechanics
- Plasticity across multiple length scales
- Recrystallization and grain growth
- Phase transformations

This work combines modeling of physical mechanisms with the development of efficient numerical algorithms integrated with experimental materials characterization.

![PFC](/images/pfc_atoms.png)             | ![FE mesh](/images/grainMesh.png) |
![Deep drawing](/images/deep_drawing.png) | ![CA](/images/ca.png)             |
[Metal foam](/images/metal_foam.png)             

## News

<div class="home">
  {%- if site.posts.size > 0 -%}
    <ul class="post-list">
      {%- for post in site.posts -%}
      <li>
        {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
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
  {%- endif -%}
</div>
