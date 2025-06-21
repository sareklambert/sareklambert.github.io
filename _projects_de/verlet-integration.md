---
title: Verlet Integration
layout: page
lang: de
permalink: /de/projects/verlet-integration/
order: 4
icon: fa-bowling-ball
---

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/sareklambert/gms-verlet-integration/blob/main/LICENSE)
[![Gamemaker-tested](https://img.shields.io/badge/GameMaker-orange?style=flat&logo=gamemaker&label=Made%20with)](https://gamemaker.io)

<iframe src="https://www.youtube.com/embed/Qcp4IX7KipI?si=X_U88j1Y7RCK9FOX" allow="autoplay; encrypted-media; fullscreen;"></iframe>
<br>

### Beschreibung
<div class="blockText"> {{"
**Verlet Integration** ist ein Verfahren zur **Physiksimulation**, das häufig für **Softbody-Dynamik**, **Seil-** und
**Stoffsimulationen** verwendet wird.
Ich habe diese Technik in GameMaker umgesetzt, indem ich eine 2D Physics **Library** entwickelt habe, die
das Einrichten solcher Simulationen deutlich vereinfacht.
Die Library enthält erweiterbare Klassen für grundlegende Objekte, Hilfsklassen für **Kraftfelder** und
**Verbindungen**, eine Beispielimplementierung sowie einen **Wireframe Modus** zum Debuggen.
Durch das Verketten mehrerer simulierten Objekte lassen sich dynamische und visuell interessante Strukturen
erstellen – etwa als Deko-Elemente oder spielerische Features.
"| markdownify }} </div>

<div class="screenshots">
    <img src="{{ site.baseurl | append: '/assets/images/verlet integration/screenshot1.png' }}">
    <img src="{{ site.baseurl | append: '/assets/images/verlet integration/screenshot2.png' }}">
    <img src="{{ site.baseurl | append: '/assets/images/verlet integration/screenshot3.png' }}">
</div>
<br>

### Entwicklungsprozess
<div class="blockText"> {{"
Ursprünglich habe ich diese Library im Rahmen eines kleinen Game-Projekts entwickelt, mich später jedoch dazu
entschieden, sie **öffentlich auf itch.io** zu veröffentlichen, wo sie schnell an Popularität gewann. Aufgrund des
Interesses anderer Entwickler habe ich den Code refactored, um die **Struktur**, **Lesbarkeit** und **Wartbarkeit** zu
verbessern. Gleichzeitig habe ich die Dokumentation und die Beispiele erweitert.

Die überarbeitete Library enthält nun zusätzliche **Hilfsfunktionen** für Features wie **Kraftfelder** sowie **textured
cloth / ropes**, was sie vielseitiger und **benutzerfreundlicher** macht. Um Zusammenarbeit und Weiterentwicklung zu
fördern, habe ich das Projekt als **Open-Source** auf **GitHub** veröffentlicht, sodass jeder dazu beitragen und es
erweitern kann.

Ich habe dieses Projekt in mein Portfolio aufgenommen, um zu zeigen, wie ich die Entwicklung einer Open-Source-Library
für andere Entwickler angehe. Sie folgt einer klaren Struktur, ist gut dokumentiert und enthält eine
Beispielimplementierung.
"| markdownify }} </div>

### Links
* [Github repo](https://github.com/sareklambert/gms-verlet-integration)
* [Public download](https://jamjamteam.itch.io/verlet-integration-gamemake-studio-2)

<div style="text-align: center;">
<a href="{{ site.baseurl | append: '/de/projects/lizbox/index.html' }}" class="button scrolly">Nächstes Projekt</a>
</div>
