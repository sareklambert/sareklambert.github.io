---
title: Behaviour Modules
author: Sarek
layout: page
---
[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![made-with-cpp](https://img.shields.io/badge/C%2B%2B17-green?style=flat&label=Made%20with)](https://learn.microsoft.com/en-us/cpp/cpp/welcome-back-to-cpp-modern-cpp)
[![Unity-tested](https://img.shields.io/badge/Made%20with-Unity%20-%23000000.svg?&logo=unity)](https://unity.com)
[![Gamemaker-tested](https://img.shields.io/badge/GameMaker-orange?style=flat&logo=gamemaker&label=Made%20with)](https://gamemaker.io)

<iframe src="https://www.youtube.com/embed/t8RM2XKsNJE?si=jzgxTqzDQPRjHGed" allow="autoplay; encrypted-media; fullscreen;"></iframe>
<br>

### Description
<div class="blockText"> {{"
**Behaviour Modules** is a **simple** yet **effective** system for **managing AI agents**. Each agent defines a set of **states**, and each
state contains its own list of **behaviours** and state change **conditions**. When an agent enters a state, it selects a
behaviour based on predefined **weights**. This allows agents with the same behaviours to exhibit unique **‘personalities’**.
For example, a large, lazy ogre might frequently choose the wait behaviour, only occasionally wandering around.
Meanwhile, a restless goblin would move constantly, stopping only briefly.

The ability to **swap behaviour modules at runtime** opens up exciting possibilities. For instance, game **difficulty** can be
**dynamically adjusted** by introducing new behaviours. In a platformer project, I implemented an enemy that would charge
at the player on sight. Initially, the attack could be easily avoided by jumping over the enemy. However, on higher
difficulty levels, the enemy gained an additional behaviour — jumping whenever the player jumped — making it a much more
menacing foe to deal with.

By designing the system in a modular way, we **keep individual behaviour blocks simple** while enabling the creation of
**complex** and **varied** agent behaviours. This approach ensures **flexibility**, **maintainability**, and **scalability** across
different AI implementations.
"| markdownify }} </div>

<div class="screenshots">
    <img src="../../../assets/images/behaviour modules/screenshot1.png">
    <img src="../../../assets/images/behaviour modules/screenshot2.png">
    <img src="../../../assets/images/behaviour modules/screenshot3.png">
</div>
<br>

### Development process
<div class="blockText"> {{"
Since many of my more advanced systems were developed for **Tainted Gun**, my GameMaker project, I wanted to showcase how
one of its simpler systems could be **translated** into **another language**. For this example, I chose my **AI agent manager**,
first converting it into **C++** and then using that version as a foundation for my **Unity implementation**.

Both the GameMaker and C++ versions **define enemy states** directly **in code**. However, in the Unity implementation,
behaviours are derived from **MonoBehaviour** and instantiated within the scene hierarchy, allowing them to **reference
scene objects**. Additionally, I created **custom editor scripts** to utilize the inspector GUI, enabling game designers
to wire behaviours together **visually** without needing to modify code.
"| markdownify }} </div>

### Project structure
<div class="structure">
    <img src="../../../assets/images/behaviour modules/structure.png">
</div>
<br>

### Source
* [Github repo](https://github.com/sareklambert/behaviourModules)
