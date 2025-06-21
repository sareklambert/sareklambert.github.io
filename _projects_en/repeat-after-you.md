---
title: Repeat After You
layout: page
lang: en
permalink: /en/projects/repeat-after-you/
order: 2
icon: fa-edit
---

[![Unity-tested](https://img.shields.io/badge/Made%20with-Unity%20-%23000000.svg?&logo=unity)](https://unity.com)

<iframe src="https://www.youtube.com/embed/UfmWDT9p7yo?si=vFIVl7djQLLdHUQi" allow="autoplay; encrypted-media; fullscreen;"></iframe>
<br>

### Description
<div class="blockText"> {{"
**Repeat after You** expands on last semester’s project, *Repeat after Me*, by introducing a **level editor**
that lets players create and share their own puzzles. Featuring a **custom serialization system**, puzzle objects and
logic gates can be interconnected seamlessly, with levels saved as **JSON** files for easy sharing. The project transforms
the original game into a dynamic, community-driven experience, giving players the tools to craft and challenge each
other with custom levels.
"| markdownify }} </div>

<div class="screenshots">
    <img src="{{ site.baseurl | append: '/assets/images/ray/screenshot1.png' }}">
    <img src="{{ site.baseurl | append: '/assets/images/ray/screenshot2.png' }}">
    <img src="{{ site.baseurl | append: '/assets/images/ray/screenshot3.png' }}">
</div>
<br>

### Development process
<div class="blockText"> {{"
Following the success of our previous semester’s project, *Repeat after Me*, our team set out to expand the
experience by developing a full-fledged **level editor**. While university guidelines initially required students
to create an entirely new game each semester, we successfully made the case — with the support of our professors — that
a level editor constituted a **new and distinct technical challenge**. This made us the **first student team** permitted to
continue a previous project, ultimately leading to a policy change at our university that now allows other teams to
extend their work under special circumstances.

We reassembled our original team, adding two more artists, one of whom focused specifically on UI design. This
continuity allowed us to **retain the existing infrastructure** from the previous semester, including our **CI pipeline**,
**version control system**, and **code review workflow** using **Perforce**.

As the **core programmer**, my responsibilities centered around implementing the **serialization and file handling
backend**, along with the **main architecture** for the level editor’s **controller system**. I began by creating a
system for managing **platform IDs**, **prop IDs**, and **connectable IDs**, used to uniquely identifying the position and
type of objects to be placed in the level. This system served as the backbone for **loading**, **saving**, and **placing**
elements accurately in the scene.

To support extensibility, I developed **generic base classes** for **editor objects**, **platforms**, and **props**, which our
second programmer used to create specific puzzle components. He also implemented a **connection system**, allowing
our game designer to link puzzle elements using logic gates and other mechanics.

I structured the main scene and editor controller into **modular manager components**, each responsible for a specific
editor subsystem. In addition, I implemented a **camera system** and an **onion skinning feature** to enhance level navigation
and iteration. To support level composition, I also created a **custom grid shader** for improved spatial clarity.
Finally, I developed the **JSON-based save/load system**, enabling seamless export and import of user-created levels.

Once the editor reached **feature-complete status**, I focused on **performance optimization**, **memory management**, and
**codebase cleanup**. I also supported our UI artist by **integrating UI functionality on the code side**, ensuring a
smooth and intuitive user experience.
"| markdownify }} </div>

### Source
* [Github repo](https://github.com/sareklambert/repeat-after-you)

<div style="text-align: center;">
<a href="{{ site.baseurl | append: '/en/projects/behaviour-modules/index.html' }}" class="button scrolly">Next project</a>
</div>
