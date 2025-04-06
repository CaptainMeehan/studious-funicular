---
title: Projects
layout: default
---

# Projects  
Here are some of my game projects and game engine experiments.

<div class="project-grid">

  <!-- Project 1 -->
  <div class="project-card" onclick="openModal('modal1')">
    <img src="/assets/images/menu.gif" alt="Modular UI">
    <h3>Modular UI</h3>
    <p>A modular UI with JSON + editor support.</p>
  </div>

  <!-- Project 2 -->
  <div class="project-card" onclick="openModal('modal2')">
    <img src="/assets/images/project2.png" alt="Project 2">
    <h3>Project 2</h3>
    <p>A game mechanic experiment.</p>
  </div>

</div>

<!-- Modals -->

<!-- Modal 1 -->
<div class="modal" id="modal1">
  <div class="modal-content">
    <span class="close-button" onclick="closeModal('modal1')">&times;</span>
    <h2>Modular UI</h2>
    <img src="/assets/images/menu.gif" alt="Modular UI">
    <p>This project focuses on building a modular UI system that's easy to implement and export from an editor as JSON. It uses nlohmann to load these files and create the entire UI structure at runtime.</p>
    <a href="https://github.com/CaptainMeehan/modular-ui" target="_blank">View on GitHub</a>
  </div>
</div>

<!-- Modal 2 -->
<div class="modal" id="modal2">
  <div class="modal-content">
    <span class="close-button" onclick="closeModal('modal2')">&times;</span>
    <h2>Project 2</h2>
    <img src="/assets/images/project2.png" alt="Project 2">
    <p>Short description of the project with additional detail, screenshots, and explanation of your goals or technologies.</p>
  </div>
</div>
