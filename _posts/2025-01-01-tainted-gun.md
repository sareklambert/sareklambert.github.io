---
title: Tainted Gun
author: Sarek
layout: page
---
[![Gamemaker-tested](https://img.shields.io/badge/GameMaker-orange?style=flat&logo=gamemaker&label=Made%20with)](https://gamemaker.io)

<iframe src="https://www.youtube.com/embed/LcZ-spIuBZ0?si=cvgeyEmwaPGClQUd" allow="autoplay; encrypted-media; fullscreen;"></iframe>
<br>
### Description
<div class="blockText"> {{"
**Tainted Gun** is a 2D rogue-lite platformer, featuring a **fully destructible environment** with **per-pixel** terrain
deformation. The game's core mechanics revolve around guns that fire neon liquid, allowing the player to **manually
place light sources** in order to explore dark cave systems. A secondary mining laser allows players to extract resources
from the terrain, which are used for equipment **crafting**. The game incorporates **pseudo random level generation** using
**ingame map editors** and a dynamic **global illumination** system for **infinite light sources**.
"| markdownify }} </div>

<div class="screenshots">
    <img src="../../../assets/images/tainted gun/screenshot1.png">
    <img src="../../../assets/images/tainted gun/screenshot2.png">
    <img src="../../../assets/images/tainted gun/screenshot3.png">
</div>
<br>

### Development process
<div class="blockText"> {{"
**Tainted Gun** started as a simple idea in a small **game jam** project that never saw the light of day. The concept was a
**puzzle game** where the player had a limited number of **light sources** they could place to navigate the level. Though
that project was abandoned, the idea stuck with me.

Years later, I participated in another game jam with the theme **'Neon'**. Remembering my old concept, I reimagined it as a
shoot 'em up platformer with a unique twist — the player’s gun not only dealt damage but also illuminated the world using
**glowing neon liquid**. This new prototype had potential, and I decided to expand it into a full game.

#### Evolving the Lighting Engine
The lighting system has gone through several iterations:

* Version 1: Initially, I used a simple approach — applying a **blur shader** to the neon liquid texture and blending it
into the game to **simulate lighting**.
* Version 2: To improve realism, I added a system that spawned **raytraced light sources** wherever the neon liquid
touched surfaces. This created **proper shadows** but quickly became a **performance nightmare**, as players could
place **infinite light sources**.
* Version 3 (Current): I implemented a 2D **global illumination** system, calculating incoming light for every pixel
on the screen. This means **the number of light sources no longer affects performance**, resulting in a **stable**,
**visually appealing**, and **efficient** lighting system.

#### Destructible Environments & Procedural Generation
Another feature I had always wanted to implement were **fully destructible levels** on a **per-pixel** basis, instead
of using the traditional **tile-based** approach seen in most 2D sandbox games. Since my lighting system was already
dynamic and **independent of predictable geometry**, it was the perfect opportunity to bring this idea to life.

For map generation, I opted for a hybrid approach — rather than fully random worlds, I designed **handcrafted rooms**
that follow specific **patterns**. The generator **assembles** these rooms **procedurally**, allowing for **controlled randomness**
while maintaining interesting level layouts. The cave walls are **rendered** as textures, then further refined using:

* Polygonal shaping for more **organic edges**
* Noise shaders for ore placement
* Thickness-based shaders to generate **albedo** and **normal maps** dynamically

#### Custom UI Framework & Future Plans
Since the engine I’m using lacks built-in UI support, I implemented my own **custom UI framework**, originally created
for another project (Lizbox). This enabled me to build in-game **map editors**, making level design and testing far
more efficient.

Tainted Gun is still far from completion, but the core mechanics are in place. Whenever I find the time, I continue
tinkering with this passion project — refining the gameplay, improving performance, and adding new features.
"| markdownify }} </div>

### Source
* [Github repo](https://github.com/sareklambert/tainted-gun-public)

<div style="text-align: center;">
<a href="../../../2025/01/02/repeat-after-me.html" class="button scrolly">Next project</a>
</div>
