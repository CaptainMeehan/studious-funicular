---
title: Projects
layout: default
---

# Projects  
Here are some of my game projects and game engine experiments.

<div class="project-grid">

  <!-- Project 1 -->
  <div class="project-card" onclick="openModal('modal1')">
    <h2>Modular UI</h2>
    <p>A modular UI that is easy to adapt to a new project</p>
    <img src="{{ '/assets/images/menu.gif' | relative_url }}" alt="menu">
  <figcaption><i>UI adapted to our game A.I Quit</i></figcaption>
  </div>

  <!-- Project 2 -->
  <div class="project-card" onclick="openModal('modal2')">
    <img src="{{ '/assets/images/meehan.gif' | relative_url }}" alt="menu">
    <h3>Game engine base</h3>
    <p>A game engine experiment with water reflection and procedural generation using dx11 and some of my base math classes.</p>
  </div>

</div>

<!-- Modals -->

<!-- Modal 1 -->
<div class="modal" id="modal1">
  <div class="modal-content">
    <span class="close-button" onclick="closeModal('modal1')">&times;</span>
    <h2>Modular UI</h2><a href="https://github.com/CaptainMeehan/modular-ui" target="_blank">View on GitHub</a>
    <img src="{{ '/assets/images/menu.gif' | relative_url }}" alt="menu">
  <figcaption><i>UI adapted to our game A.I Quit</i></figcaption>
    <p>This project focuses on building a modular UI system that's easy to implement in a new project. The end goal is to also implement and export from an editor as JSON. It is going to use nlohmann to load these files and create the entire UI structure at runtime.</p>
    <h3>🔧 Key Features Already Implemented</h3>
    <ul>
      <li><strong>State-Based UI Flow:</strong> Manages UI menus using a state stack (e.g., Main Menu, Settings, Pause), with <code>PushState</code>, <code>PopState</code>, and <code>PushStateAndPop</code> for seamless transitions.</li>
      <li><strong>Modular Components:</strong> Easily build interfaces with reusable elements like buttons, sliders, containers, and text. Each is a separate class with helper functions for setup.</li>
      <li><strong>Interactive & Event-Driven:</strong> Supports event callbacks for hover, click, and drag using <code>std::function</code>. Input is handled centrally in the UIManager.</li>
      <li><strong>Rendering System:</strong> Elements are added to a prioritized render list to maintain proper visual layering and efficient rendering.</li>
      <li><strong>Responsive Design:</strong> Automatically scales UI elements to screen resolution using a layout update function for different devices and aspect ratios.</li>
    </ul>
    <img src="{{ '/assets/images/spite1.gif' | relative_url }}" alt="menu">
  <figcaption><i>UI adapted to our game Spite: The Infernal Oath</i></figcaption>
    <h3>🌱 Future Improvements</h3>
    <ul>
      <li><strong>Visual UI Editor Tool:</strong> Drag-and-drop editor for building UI layouts visually.</li>
      <li><strong>Live Preview:</strong> Real-time preview of changes inside the editor.</li>
      <li><strong>Dynamic Text:</strong> Support for localization, font scaling, and multi-language UI.</li>
    </ul>
    <img src="{{ '/assets/images/intro.gif' | relative_url }}" alt="intro">
  <figcaption><i>Intro adapted to our game A.I Quit using Modular UI</i></figcaption>
  </div>
</div>

<!-- Modal 2 -->
<div class="modal" id="modal2">
  <div class="modal-content">
    <span class="close-button" onclick="closeModal('modal2')">&times;</span>
    <h2>DX11 Engine</h2><a href="https://github.com/CaptainMeehan/dx11enginebase/" target="_blank">View on GitHub</a>
    <img src="{{ '/assets/images/meehan.gif' | relative_url }}" alt="menu">
  <figcaption><i>Flying around with keyboard in engine testing out some reflection algorithms</i></figcaption>
    <p>This project focuses on building a modular UI system that's easy to implement in a new project. The end goal is to also implement and export from an editor as JSON. It is going to use nlohmann to load these files and create the entire UI structure at runtime.</p>
    <h3>🔧 Key Features Already Implemented</h3>
    <ul>
      <li><strong>State-Based UI Flow:</strong> Manages UI menus using a state stack (e.g., Main Menu, Settings, Pause), with <code>PushState</code>, <code>PopState</code>, and <code>PushStateAndPop</code> for seamless transitions.</li>
      <li><strong>Modular Components:</strong> Easily build interfaces with reusable elements like buttons, sliders, containers, and text. Each is a separate class with helper functions for setup.</li>
      <li><strong>Interactive & Event-Driven:</strong> Supports event callbacks for hover, click, and drag using <code>std::function</code>. Input is handled centrally in the UIManager.</li>
      <li><strong>Rendering System:</strong> Elements are added to a prioritized render list to maintain proper visual layering and efficient rendering.</li>
      <li><strong>Responsive Design:</strong> Automatically scales UI elements to screen resolution using a layout update function for different devices and aspect ratios.</li>
    </ul>
    <img src="{{ '/assets/images/spite1.gif' | relative_url }}" alt="menu">
  <figcaption><i>UI adapted to our game Spite: The Infernal Oath</i></figcaption>
    <h3>🌱 Future Improvements</h3>
    <ul>
      <li><strong>Visual UI Editor Tool:</strong> Drag-and-drop editor for building UI layouts visually.</li>
      <li><strong>Live Preview:</strong> Real-time preview of changes inside the editor.</li>
      <li><strong>Dynamic Text:</strong> Support for localization, font scaling, and multi-language UI.</li>
    </ul>
    <img src="{{ '/assets/images/intro.gif' | relative_url }}" alt="intro">
  <figcaption><i>Intro adapted to our game A.I Quit using Modular UI</i></figcaption>
  </div>
</div>
