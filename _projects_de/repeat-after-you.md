---
title: Repeat After You
layout: page
lang: de
permalink: /de/projects/repeat-after-you/
order: 2
icon: fa-edit
---

[![Unity-tested](https://img.shields.io/badge/Made%20with-Unity%20-%23000000.svg?&logo=unity)](https://unity.com)

<iframe src="https://www.youtube.com/embed/UfmWDT9p7yo?si=vFIVl7djQLLdHUQi" allow="autoplay; encrypted-media; fullscreen;"></iframe>
<br>

### Beschreibung
<div class="blockText"> {{"
**Repeat after You** erweitert das Projekt **Repeat after Me** aus dem letzten Semester um einen Level Editor,
mit dem Spieler eigene Level erstellen und teilen können. Dank eines eigens entwickelten **Serialisierungssystems**
lassen sich Puzzle-Objekte und Logik-Gates nahtlos miteinander verbinden. Die Levels werden als **JSON-Dateien**
gespeichert, was das Teilen besonders einfach macht.
Das Projekt verwandelt das ursprüngliche Spiel in ein dynamisches, Community-getriebenes Erlebnis – und gibt den
Spielern die Werkzeuge an die Hand, um eigene Level zu gestalten und sich gegenseitig herauszufordern.
"| markdownify }} </div>

<div class="screenshots">
    <img src="{{ site.baseurl | append: '/assets/images/ray/screenshot1.png' }}">
    <img src="{{ site.baseurl | append: '/assets/images/ray/screenshot2.png' }}">
    <img src="{{ site.baseurl | append: '/assets/images/ray/screenshot3.png' }}">
</div>
<br>

### Entwicklungsprozess
<div class="blockText"> {{"
Nach dem Erfolg unseres Projekts *Repeat after Me* im vorherigen Semester setzte sich unser Team das Ziel,
das Spielerlebnis durch die Entwicklung eines vollwertigen **Level Editors** zu erweitern. Zwar verlangte die
Prüfungsordnung ursprünglich, dass Studierende jedes Semester ein komplett neues Spiel entwickeln, doch mit
Unterstützung unserer Professor*innen konnten wir erfolgreich darlegen, dass ein Level Editor eine **eigenständige
technische Herausforderung** darstellt. Damit wurden wir das **erste Studierendenteam**, das offiziell ein bestehendes
Projekt fortsetzen durfte – und sorgten so für eine Regeländerung, die es künftig auch anderen Teams ermöglicht,
unter bestimmten Voraussetzungen an früheren Projekten weiterzuarbeiten.

Wir stellten unser ursprüngliches Team wieder zusammen und nahmen zwei weitere Artists dazu, von denen sich einer
gezielt auf UI-Design konzentrierte. Durch diese Kontinuität konnten wir die **bestehende Infrastruktur** aus dem
vorherigen Semester **weiter nutzen** – inklusive **CI Pipeline**, **Versionskontrolle** und **Code Review Workflow**
mit **Perforce**.

Als **Hauptprogrammierer** war ich primär für die Implementierung des **Serialisierungs- und File Handling Backends**
verantwortlich sowie für die **Architektur des Controller Systems** im Level Editor. Ich entwickelte ein System
zur Verwaltung von **Plattform IDs**, **Prop IDs** und **Connectable IDs** – eindeutige Kennungen, die Position und Typ
der platzierten Objekte im Level eindeutig beschreiben. Dieses System bildete das Rückgrat für das **Laden**,
**Speichern** und **Platzieren** von Levelelementen.

Zur Unterstützung der Erweiterbarkeit schrieb ich **generische Basisklassen** für **Editor Objekte**, **Plattformen** und
**Props**, auf deren Grundlage unser zweiter Programmierer spezifische Puzzle Komponenten entwickelte. Er
implementierte außerdem ein **Verbindungssystem**, mit dem unser Game Designer Puzzleelemente per Logic Gates
und anderen Mechaniken verknüpfen konnte.

Die Hauptszene und den Editor Controller habe ich in **modulare Manager Komponenten** unterteilt, die jeweils ein
bestimmtes Editor Subsystem steuern. Zusätzlich entwickelte ich ein **Kamerasystem** und ein **Onion Skinning Feature**
zur besseren Navigation und Iteration beim Level Design. Für mehr räumliche Klarheit beim Platzieren von Objekten
erstellte ich zudem einen eigenen **Grid Shader**. Abschließend programmierte ich das **JSON basierte
Save-/Load System**, das den reibungslosen Export und Import benutzerdefinierter Levels ermöglicht.

Nachdem der Editor **feature-complete** war, konzentrierte ich mich auf **Performanceoptimierung**, **Memory management**
und die **Bereinigung des Codes**. Außerdem unterstützte ich unseren UI Artist bei der **technischen Umsetzung** ihrer
Designs, um eine möglichst intuitive und flüssige Nutzererfahrung zu gewährleisten.
"| markdownify }} </div>

### Links
* [Github repo](https://github.com/sareklambert/repeat-after-you)

<div style="text-align: center;">
<a href="{{ site.baseurl | append: '/de/projects/behaviour-modules/index.html' }}" class="button scrolly">Nächstes Projekt</a>
</div>
