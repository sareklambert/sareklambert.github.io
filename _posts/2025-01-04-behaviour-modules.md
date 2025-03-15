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
Behaviour Modules is a simple, yet effective system for **managing AI agents**.
An agent defines a list of **states**. A state defines its own lists of **behaviours** and **state change conditions**.
When the agent enters a state, it chooses one of the behaviours depending on the associated **weight**.
Even two agents with the same behaviours can have a distinct **"personality"**. For example a big lazy ogre will be likely
to choose the wait behaviour and only occasionally wander around. On the other hand, a restless goblin will wander around
without frequent stops.

By implementing the system in a modular way, we can **keep behaviour blocks simple** and assemble **complex**, **distinct** agent
behaviour while ensuring **maintainability** for the individual modules.

Originally, I've implemented the system in **GameMaker**, and translated it to **Unity** and **C++**. The Unity implementation
contains a custom **editor script**, allowing a game designer to quickly wire together behaviour in the **inspector** without having to touch code.

<div style="display: flex; justify-content: space-between; gap: 10px;">
    <img src="../../../assets/images/behaviour modules/screenshot1.png" style="width: 32%; height: auto;">
    <img src="../../../assets/images/behaviour modules/screenshot2.png" style="width: 32%; height: auto;">
    <img src="../../../assets/images/behaviour modules/screenshot3.png" style="width: 32%; height: auto;">
</div>

<br>

### Project structure
<img src="../../../assets/images/behaviour modules/structure.png" style="width: 100%; height: auto;">

### Why it’s in my portfolio
I've developed many of my more advanced systems for Tainted Gun, my Gamemaker project. With this piece I wanted
to demonstrate, how I'd translate one of the simpler systems of that project to Unity or another language like C++.

### Source
* [Github repo](https://github.com/sareklambert/behaviourModules)
