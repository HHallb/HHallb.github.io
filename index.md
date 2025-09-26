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
    
    // Style the Welcome heading to match other page titles
    const welcomeHeading = document.querySelector('h1');
    if (welcomeHeading && welcomeHeading.textContent.includes('Welcome')) {
        welcomeHeading.style.fontSize = '2rem';
        welcomeHeading.style.fontWeight = '400';
        welcomeHeading.style.letterSpacing = '-1px';
        welcomeHeading.style.marginBottom = '30px';
        welcomeHeading.style.marginTop = '0';
        welcomeHeading.style.lineHeight = '1.15';
    }
});
</script>

# Welcome!

I work at the Division of Solid Mechanics at Lund University in Sweden. These pages present research in which I am involved and focus on numerical modeling and simulation of microstructure mechanics and microstructure evolution in crystalline materials and how this translates to macroscale material behavior. Main research topics include manifestations of plasticity at several length-scales, properties and influence of grain boundaries, recrystallization, grain growth and solid-state phase transformations. Both modeling of the physical mechanisms and implementation of efficient numerical simulation algorithms are targeted and combined with experimental materials characterization.

![PFC](/images/pfc_atoms.png)             | ![FE mesh](/images/grainMesh.png) |
![Deep drawing](/images/deep_drawing.png) | ![CA](/images/ca.png)             |

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
