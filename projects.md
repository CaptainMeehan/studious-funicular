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

  <!-- Project 3 -->
  <div class="project-card" onclick="openModal('modal3')">
    <img src="{{ '/assets/images/tankgame.png' | relative_url }}" alt="menu">
    <h3>Networked Tank Game</h3>
    <p>This project walks through implementing a simple networked multiplayer tank game with features like prediction, interpolation, delay compensation, and network debugging tools.</p>
  </div>

  <!-- Project 4 -->
  <div class="project-card" onclick="openModal('modal4')">
    <h3>To be added:</h3>
    <p>I will add some of my school game projects and more snippets from my programming methology soon!</p>
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
<p>For this project I worked with procedural generation, Directx11, reflection and raycasting and in general just game related math needed for engines.</p>
  </div>
</div>

<!-- Modal 3 -->
<div class="modal" id="modal3">
  <div class="modal-content">
    <span class="close-button" onclick="closeModal('modal3')">&times;</span>
    <h2>DX11 Engine</h2><a href="https://github.com/CaptainMeehan/dx11enginebase/" target="_blank">View on GitHub</a>
    <img src="{{ '/assets/images/tankgame.png' | relative_url }}" alt="menu">
  <figcaption><i>How my project structure looks right now.</i></figcaption>
  <h2>Networked Tank Game</h2>
<p>This project walks through implementing a simple networked multiplayer tank game with features like prediction, interpolation, delay compensation, and network debugging tools.</p>
<p>I am currently developing it.</p>
I am using <a href="https://sourceforge.net/projects/asio/files/asio/1.30.2%20%28Stable%29/" target="_blank">ASIO</a> for networking as it is cross platform.
<a href="https://sourceforge.net/projects/asio/files/asio/1.30.2%20%28Stable%29/" target="_blank">Jolt</a> for Physics.
<a href="https://capnproto.org/install.html" target="_blank">Cap'n Proto</a> for Serialization.
<a href="https://github.com/CaptainMeehan/dx11enginebase/" target="_blank">My Engine</a> my own graphics engine. More control
<a href="https://download.autodesk.com/us/fbx/20112/fbx_sdk_help/index.html?url=WS1a9193826455f5ff-150b16da11960d83164-6bf0.htm,topicNumber=d0e1518" target="_blank">FBXSDK</a> for model loading (later) with maybe unity or UE for model export to JSON using nlohmann.
    
<h3>🛠️ Development Process</h3>

<div class="process-section">
  <h4>🔌 Networking Basics</h4>
  <ul>
    <li>Configured a simple TCP/UDP server and client setup (authoritative or not).</li>
    <li>Established basic client-server communication.</li>
    <li>Implemented a handshake/login system.</li>
    <li>Decided on message structure and serialization format.</li>
  </ul>
</div>

<div class="process-section">
  <h4>🎮 Core Gameplay Loop</h4>
  <ul>
    <li>Built a game loop to send tank positions to the server.</li>
    <li>Implemented server-side state management (authoritative/semi-authoritative).</li>
    <li>Synchronized player movement across clients.</li>
  </ul>
</div>

<div class="process-section">
  <h4>🕹️ Prediction & Interpolation</h4>
  <ul>
    <li>Will add basic interpolation for smooth movement.</li>
    <li>Implement input prediction on the client.</li>
    <li>Handle motion delay compensation.</li>
  </ul>
</div>

<div class="process-section">
  <h4>🔫 Shooting Mechanics</h4>
  <ul>
    <li>Send input events for shooting.</li>
    <li>Handle projectiles on the server and synced them with clients.</li>
    <li>Add basic physics (custom or using a physics lib).</li>
    <li>Implement collision detection between bullets and tanks.</li>
    <li>Synchronize point/projectile positions over the network.</li>
  </ul>
</div>

<div class="process-section">
  <h4>💥 Health & Combat</h4>
  <ul>
    <li>Implement a health/damage system with notifications to clients.</li>
    <li>Enhance motion smoothing using interpolation/extrapolation.</li>
    <li>Improve hit registration using delay compensation techniques.</li>
  </ul>
</div>

<div class="process-section">
  <h4>🌐 Network Optimization</h4>
  <ul>
    <li>Simulate latency and jitter for testing.</li>
    <li>Optimize packet rate and size.</li>
    <li>Add tank explosions and death handling.</li>
    <li>Add respawn logic and a simple win condition.</li>
  </ul>
</div>

<div class="process-section">
  <h4>🧪 UI & Polish</h4>
  <ul>
    <li>Create UI elements for health and status.</li>
    <li>Add sound and visual feedback for combat.</li>
    <li>Build network debugging tools (packet logs, latency graphs).</li>
    <li>Playtest to catch bugs and edge cases.</li>
    <li>Finalize UI polish and game feel.</li>
    <li>Optimize physics and mesh code for better responsiveness.</li>
  </ul>
</div>

<!-- Modal 4 -->
<div class="modal" id="modal1">
  <div class="modal-content">
    <span class="close-button" onclick="closeModal('modal1')">&times;</span>
    <h3>To be added:</h3>
    <p>I will add some of my school game projects and more snippets from my programming methology soon!</p>
  </div>
</div>

  </div>
</div>
