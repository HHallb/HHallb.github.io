---
layout: page
title: Projects  
permalink: /projects/
---

<style>
.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 30px;
  margin: 30px 0;
}

.projects-grid > a {
  text-decoration: none;
  color: inherit;
  display: block;
}

.project-card {
  background: #fff;
  border: 1px solid #e1e4e8;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
  cursor: pointer;
  height: 100%;
}

.project-card:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(0,0,0,0.15);
}

.project-card {
  background: #fff;
  border: 1px solid #e1e4e8;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}

.project-image {
  width: 100%;
  height: 200px;
  object-fit: cover;
  display: block;
}

.project-content {
  padding: 20px;
}

.project-title {
  font-size: 1.4em;
  font-weight: 600;
  margin: 0 0 10px 0;
  color: #000000 !important;
}

.project-title a,
.project-title a:link,
.project-title a:visited {
  color: #000000 !important;
  text-decoration: none !important;
}

.project-title a:hover,
.project-title a:active {
  color: #0366d6 !important;
  text-decoration: underline !important;
}

.project-description {
  color: #586069;
  line-height: 1.5;
  margin: 0;
}

.project-tags {
  margin-top: 15px;
}

.tag {
  display: inline-block;
  background: #f1f8ff;
  color: #0366d6;
  padding: 4px 8px;
  border-radius: 12px;
  font-size: 0.8em;
  margin-right: 5px;
  margin-bottom: 5px;
}
</style>

<div class="projects-grid">
  <div class="project-card">
    <img src="/images/metal_foam_collage.png" alt="Metal Foams" class="project-image">
    <div class="project-content">
      <h3 class="project-title">Metal Foams</h3>
      <p class="project-description">
        Combining synchrotron-based tomography and diffraction measurements with numerical simulations to understand the mechanical behavior and microstructure evolution of metal foams.
      </p>
      <div class="project-tags">
        <span class="tag">Finite Element</span>
        <span class="tag">Microstructure</span>
        <span class="tag">Synchrotron</span>
        <span class="tag">Tomography</span>
      </div>
    </div>
  </div>

  <a href="/pyPFC/">
    <div class="project-card">
      <img src="/images/pfc_atoms.png" alt="pyPFC" class="project-image">
      <div class="project-content">
        <h3 class="project-title" style="color: #000000 !important;">pyPFC</h3>
        <p class="project-description">
          An open-source Python package for phase field crystal simulations. Object-oriented code designed for GPU acceleration, suitable for algorithm development and scientific investigations.
        </p>
        <div class="project-tags">
          <span class="tag">Python</span>
          <span class="tag">GPU Computing</span>
          <span class="tag">Phase Field Crystal</span>
          <span class="tag">Open Source</span>
        </div>
      </div>
    </div>
  </a>

  <div class="project-card">
    <img src="/images/grainMesh.png" alt="Grain Boundary Mechanics" class="project-image">
    <div class="project-content">
      <h3 class="project-title">Grain Boundary Mechanics</h3>
      <p class="project-description">
        Numerical modeling of grain boundary behavior in polycrystalline materials, focusing on the mechanical properties and influence of grain boundaries on material response.
      </p>
      <div class="project-tags">
        <span class="tag">Grain Boundaries</span>
        <span class="tag">Grain Boundary Junctions</span>
        <span class="tag">Polycrystals</span>
        <span class="tag">Computational Mechanics</span>
      </div>
    </div>
  </div>

  <a href="/rex_gg/">
    <div class="project-card">
      <img src="/images/ca.png" alt="Recrystallization and Grain Growth" class="project-image">
      <div class="project-content">
        <h3 class="project-title" style="color: #000000 !important;">Recrystallization and Grain Growth</h3>
        <p class="project-description">
          Numerical modeling of recrystallization and grain growth by different approaches.
        </p>
        <div class="project-tags">
          <span class="tag">Recrystallization</span>
          <span class="tag">Grain Growth</span>
          <span class="tag">Nucleation</span>
          <span class="tag">Grain Boundaries</span>
        </div>
      </div>
    </div>
  </a>

  <a href="/phase_trans/">
    <div class="project-card">
      <img src="/images/transformation_surface.png" alt="Phase Transformation" class="project-image">
      <div class="project-content">
        <h3 class="project-title" style="color: #000000 !important;">Phase Transformation</h3>
        <p class="project-description">
          Numerical modeling of phase transformations by different approaches.
        </p>
        <div class="project-tags">
          <span class="tag">Recrystallization</span>
          <span class="tag">Grain Growth</span>
          <span class="tag">Nucleation</span>
          <span class="tag">Grain Boundaries</span>
        </div>
      </div>
    </div>
  </a>

  <div class="project-card">
    <img src="/images/deep_drawing.png" alt="Metal Forming" class="project-image">
    <div class="project-content">
      <h3 class="project-title">Metal Forming Processes</h3>
      <p class="project-description">
        Computational modeling of metal forming processes, such as deep drawing and forging. Integration of microstructure evolution with process simulation.
      </p>
      <div class="project-tags">
        <span class="tag">Manufacturing</span>
        <span class="tag">Process Simulation</span>
        <span class="tag">Plasticity</span>
        <span class="tag">Forming</span>
        <span class="tag">Forging</span>
      </div>
    </div>
  </div>
</div>
