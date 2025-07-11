---
title: Lizbox
layout: page
lang: en
permalink: /en/projects/lizbox/
order: 5
icon: fa-wrench
---

[![Gamemaker-tested](https://img.shields.io/badge/GameMaker-orange?style=flat&logo=gamemaker&label=Made%20with)](https://gamemaker.io)

<iframe src="https://www.youtube.com/embed/zRNpTJLAKzE?si=4N1GyI4RCSoPohNM" allow="autoplay; encrypted-media; fullscreen;"></iframe>
<br>

### Description
<div class="blockText"> {{"
**Lizbox** is a collection of specialized **pixel art tools** I developed for my game projects. The most notable tool is the
**Animation Mask Editor**, which allows users to create **gradient textures** that can be used with **shaders** to produce
unique **2D animations**.
The tool includes features to **simplify gradient visualization**, various **drawing tools**, an action history (**protocol**),
and multiple export options, making it both powerful and **user-friendly**.
"| markdownify }} </div>

<div class="screenshots">
    <img src="{{ site.baseurl | append: '/assets/images/lizbox/screenshot1.png' }}">
    <img src="{{ site.baseurl | append: '/assets/images/lizbox/screenshot2.png' }}">
    <img src="{{ site.baseurl | append: '/assets/images/lizbox/screenshot3.png' }}">
</div>
<br>

### Development process
<div class="blockText"> {{"
While creating **UI animations** for one of my games, I grew frustrated with how **time-consuming** the process was and
started exploring **alternatives**. Previously, I had used **shader-based transitions** by applying simple gray gradient
textures to **encode time**, revealing and hiding images. However, this method was imprecise and could only be applied
to entire images.

To **improve precision**, I experimented with manually drawing gradients over UI elements to create more dynamic
animations. While the results were promising, the process remained slow, and the subtle gradient shades were
**difficult to distinguish** by eye. I needed a tool that could **'draw time'** onto a texture while maintaining enough
contrast between pixels — but no such tool existed.

So, I built one myself in **GameMaker**. Since the engine lacked built-in UI support, I first developed a full **UI
framework** from scratch, including **windows**, **docking**, **scaling**, and other essential features. With this foundation,
I created a drawing tool that automatically cycled through a custom palette, ensuring **clear visual separation**
between gradient steps. I then added **quality-of-life features** like line drawing, adjustable brush sizes,
zooming, an undo / redo system (using software design patterns I learned during my studies), exporting options, and more.

This project was a great opportunity to deepen my understanding of **UI design** and served as an example of the
**custom development tools** I occasionally create to **streamline** my workflow. Additionally, it showcases some of
the simpler 2D **shaders** I’ve worked on.
"| markdownify }} </div>

### Source
* [Github repo](https://github.com/sareklambert/lizbox-public)
* [Public download](https://jamjamteam.itch.io/lizbox)

<div style="text-align: center;">
<a href="{{ '/en/' }}" class="button scrolly">Home</a>
</div>
