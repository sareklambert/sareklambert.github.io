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
Behaviour Modules is a **simple**, yet **effective**, **system** for **managing AI agents**.
An agent defines a list of **states**. A state defines its own lists of **behaviours** and **state change conditions**.
When the agent enters a state, it chooses one of the behaviours depending on the associated **weight**.
That way, two agents with the same behaviours can still have a distinct **'personality'**. For example a big lazy ogre
will be likely to choose the wait behaviour and only occasionally wander around. On the other hand, a restless goblin
will wander around without frequent stops.

The ability to **swap out** different behaviour modules **at runtime** opens up other interesting possibilities as well.
The games **difficulty** level may be **dynamically** increased by **inserting new behaviours**. In a platformer game project I've
added an enemy which would **charge** the player on sight. The attack could be easily avoided by jumping over the incoming
enemy. However, when choosing a harder difficulty the enemy would have an **additional trigger** which caused it to **jump
whenever the player jumped**, making it a very menacing foe to deal with.

By implementing the system in a modular way, we can **keep behaviour blocks simple** and assemble **complex**, **distinct** agent
behaviour while ensuring **maintainability** for the individual modules.
"| markdownify }} </div>

<div class="screenshots">
    <img src="../../../assets/images/behaviour modules/screenshot1.png">
    <img src="../../../assets/images/behaviour modules/screenshot2.png">
    <img src="../../../assets/images/behaviour modules/screenshot3.png">
</div>
<br>

### Development process
<div class="blockText"> {{"
As I've developed many of my more advanced systems for **Tainted Gun**, my GameMaker project, I wanted to demonstrate how
I'd translate one of the simpler systems of that project to another language. For this example I picked my AI agent
manager and first translated it into **C++**. After, that I used that translation as a base for my **Unity** version.

Both, the GameMaker and the C++ version **define enemy states in code**. In the Unity implementation behaviours are derived
from **monobehaviour** and instantiated in the scene hierarchy, so they can **hold references to scene objects**. I've also added
a couple of custom **editor scripts** to utilize the inspector GUI, allowing a game designer to quickly wire together
behaviour in the **inspector** without having to touch code.
"| markdownify }} </div>

### Project structure
<div class="structure">
    <img src="../../../assets/images/behaviour modules/structure.png">
</div>
<br>

### Source
* [Github repo](https://github.com/sareklambert/behaviourModules)
