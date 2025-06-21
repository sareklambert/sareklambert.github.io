---
title: Repeat After Me
layout: page
lang: de
permalink: /de/projects/repeat-after-me/
order: 1
icon: fa-walking
---

[![Unity-tested](https://img.shields.io/badge/Made%20with-Unity%20-%23000000.svg?&logo=unity)](https://unity.com)

<iframe src="https://www.youtube.com/embed/Dwql-KgXfdE?si=jU_M9EeAFab1Xar4" allow="autoplay; encrypted-media; fullscreen;"></iframe>
<br>

### Beschreibung
<div class="blockText"> {{"
**Repeat After Me** ist eines der Projekte, das ich **während meines Studiums** im Rahmen eines **größeren Studententeams**
entwickelt habe. Es handelt sich um einen **3D Puzzle Platformer** mit einem einzigartigen **Klon-**, **Aufnahme-** und
**Wiedergabemechanik**, die es einem einzelnen Spieler ermöglicht, Rätsel zu lösen, die eigentlich für mehrere
Personen ausgelegt sind. Das Spiel erregte während des Semesters viel Aufmerksamkeit und wurde unter anderem
auf den **German Dev Days** sowie im Indie Bereich der **Gamescom** **ausgestellt**. Später veröffentlichten wir auch eine
Demoversion auf **Steam**.
"| markdownify }} </div>

<div class="screenshots">
    <img src="{{ site.baseurl | append: '/assets/images/ram/screenshot1.png' }}">
    <img src="{{ site.baseurl | append: '/assets/images/ram/screenshot2.png' }}">
    <img src="{{ site.baseurl | append: '/assets/images/ram/screenshot3.png' }}">
</div>
<br>

### Entwicklungsprozess
<div class="blockText"> {{"
Als **Hauptprogrammierer** dieses Projekts war ich für die **Implementierung** des **Characters**, seiner **Animationen**
sowie den **Game Manager** zuständig. Außerdem habe ich das **Lighting**, **Shader** und **Post-Processing** übernommen –
alles in Abstimmung mit dem **Styleguide**, den unser Vision Keeper vorgegeben hatte.

Nach der Aufgabenverteilung im Team und dem Kick-off Meeting mit unseren Professor*innen begann ich mit dem
Aufbau der grundlegenden Projektstruktur. In den ersten Wochen arbeiteten wir eng mit unserem Game Designer
zusammen, um die **Spezifikationen** und **Interaktionen der Spielfigur** festzulegen. Diese Informationen wurden in
unserem **Game Design Document** auf **Confluence** dokumentiert. Parallel dazu richtete ein anderes Teammitglied unsere
**CI-Pipeline** und **Versionskontrolle** mit **Perforce** ein, während unser Project Manager die **Aufgabenverwaltung**
in **Jira** aufsetzte.

Basierend auf dem Game Design Document implementierte ich die **zentralen Spielfunktionen**. So konnte der Gamedesigner
neue Builds testen und gezielt Feedback sessions organisieren. Dank Perforce waren detaillierte **Code Reviews** möglich,
was ein starkes Lernumfeld förderte. Um die einzelnen Systeme möglichst **entkoppelt** zu halten, implementierte ich
einen **Event Bus**, der eine **parallele Entwicklung** im Team ermöglichte. Der Character Controller folgte dem Single
Responsibility Principle und bestand aus **klar getrennten Komponenten** für **Input**, **Physik**, **Animation** und **Recording**.
Für die Aufnahme-Mechanik wurden Eingaben in einem **Input Snapshot Struct** gespeichert und mit **Timestamps** versehen,
um sie später abspielen zu können. Nach der **Feature Complete Phase** konzentrierte ich mich auf **Optimierungen** im
**Memory Management** – z.B. durch **preallocation von datastructures** und **Object Pooling**.

Wir **präsentierten** das Projekt **auf dem Campus** und führten **Playtesting Sessions** mit anderen Studierenden durch.
Das gesammelte Feedback diente uns als Grundlage für weitere **Verbesserungen** und **neue Features**, die wir in der
Semesterpause umsetzten. Schließlich **stellten wir unser Spiel** zuerst auf den **German Dev Days** und später im
**Indie-Bereich der Gamescom aus** – und konnten dort einem größeren Publikum unsere Arbeit zeigen.
"| markdownify }} </div>

### Links
* [Github repo](https://github.com/sareklambert/repeat-after-me)
* [Steam](https://store.steampowered.com/app/2470830/Repeat_After_Me/)

<div style="text-align: center;">
<a href="{{ site.baseurl | append: '/de/projects/repeat-after-you/index.html' }}" class="button scrolly">Nächstes Projekt</a>
</div>
