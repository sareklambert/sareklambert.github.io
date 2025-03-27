---
title: Repeat After Me
author: Sarek
layout: page
---
[![Unity-tested](https://img.shields.io/badge/Made%20with-Unity%20-%23000000.svg?&logo=unity)](https://unity.com)

<iframe src="https://www.youtube.com/embed/Dwql-KgXfdE?si=jU_M9EeAFab1Xar4" allow="autoplay; encrypted-media; fullscreen;"></iframe>
<br>

### Description
<div class="blockText"> {{"
**Repeat After Me** is one of the projects I developed **during my studies** as part of a larger student **team**.
It’s a **3D puzzle platformer** centered around a unique **cloning**, **recording**, and **replaying** mechanic, enabling
a **single player** to **solve puzzles designed for multiple people**. The game gained significant traction during our
semester, leading to an **exhibition** in the indie area at **Gamescom** and the later release of our demo on **Steam**.
"| markdownify }} </div>

<div class="screenshots">
    <img src="../../../assets/images/ram/screenshot1.png">
    <img src="../../../assets/images/ram/screenshot2.png">
    <img src="../../../assets/images/ram/screenshot3.png">
</div>
<br>

### Development process
<div class="blockText"> {{"
As the **main programmer** for this project, I was responsible for **implementing** the **character’s functionality**, **animation**,
and **game managers**. Additionally, I handled **lighting**, **shaders**, and **post-processing**, ensuring they aligned with the **style
guide** set by our vision keeper.

Following our team role assignments and **kick-off meeting** with the professors, I began setting up the project’s
**basic infrastructure**. In the first few weeks, we worked closely with our **game designer** to define the **character's
specifications** and **interactions**. These details were compiled into our **game design document** on **Confluence**. Meanwhile,
another team member established our **CI pipeline** and **version control system** using **Perforce**, while our project manager
set up **task tracking** in **Jira**.

With the game design document as a reference, I implemented the **core features**, allowing our game designer to **test new
builds** and coordinate **feedback sessions**. Perforce enabled thorough **code reviews**, fostering a strong learning
environment. To keep our game systems **decoupled**, I implemented an **event bus**, allowing **parallel development** across the
team. The character controller was designed with the single responsibility principle in mind, with distinct
**subcomponents** for **input**, **physics**, **animation**, and **recording**. For the recording mechanic, inputs were stored in an **input
snapshot struct** and **timestamped** for later **playback**. Once the project was **feature-complete**, I focused on **optimizing** memory
management through **preallocating lists**, **object pooling**, etc.

We **presented** the project **on campus**, conducting **playtesting sessions** with other students. Their feedback provided a
list of **refinements** and **additional features**, which we implemented over the semester break. Finally, we **exhibited** our
game at **Gamescom**, showcasing our work to a **wider audience**.
"| markdownify }} </div>

### Project structure
<div class="structure">
    <img src="../../../assets/images/ram/structure.png">
</div>
<br>

### Source
* [Github repo](https://github.com/sareklambert/repeat-after-me)
* [Steam](https://store.steampowered.com/app/2470830/Repeat_After_Me/)