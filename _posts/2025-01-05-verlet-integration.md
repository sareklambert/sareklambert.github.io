---
title: Verlet Integration
author: Sarek
layout: page
---
[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/sareklambert/gms-verlet-integration/blob/main/LICENSE)
[![Gamemaker-tested](https://img.shields.io/badge/GameMaker-orange?style=flat&logo=gamemaker&label=Made%20with)](https://gamemaker.io)

<iframe src="https://www.youtube.com/embed/Qcp4IX7KipI?si=X_U88j1Y7RCK9FOX" allow="autoplay; encrypted-media; fullscreen;"></iframe>
<br>

### Description
<div class="blockText"> {{"
Verlet Integration is a **physics simulation** method used for **soft-body dynamics**, **ropes**, and **cloth simulation**.
I've implemented this technique in **GameMaker**, creating a **2D physics library** that allows for an easy setup of these
simulations. The library contains expandable classes for basic objects, helper classes for **force fields** and **connectors**,
an example **implementation**, and a **wireframe** mode for debugging. By **chaining together** multiple simulated objects,
interesting structures for **decoration** can be created.
"| markdownify }} </div>

<div class="screenshots">
    <img src="../../../assets/images/verlet integration/screenshot1.png">
    <img src="../../../assets/images/verlet integration/screenshot2.png">
    <img src="../../../assets/images/verlet integration/screenshot3.png">
</div>
<br>

### Development process
<div class="blockText"> {{"
I've originally developed this library as part of a smaller game project and later decided to release it **publicly on
itch.io**, where it gained significant traction. Noticing other devs interest in it, I decided to refactor the code,
improving its **structure**, **readability**, and **maintainability** while adding better **documentation** and examples.
The library now includes helper functions for features like **force fields** and **textured cloth / ropes**, making it more
versatile and **user-friendly**. To encourage collaboration and further improvements, I made the project **open-source
on GitHub**, allowing anyone to contribute and expand on the project.

I've included this piece to demonstrate how I would implement an open-source library for other developers.
The library follows a clear structure, is documented and includes an example implementation.
"| markdownify }} </div>

### Project structure
<div class="structure">
    <img src="../../../assets/images/verlet integration/structure.png">
</div>
<br>

### Source
* [Github repo](https://github.com/sareklambert/gms-verlet-integration)
* [Public download](https://jamjamteam.itch.io/verlet-integration-gamemake-studio-2)
