---
title: Tainted Gun
layout: page
lang: de
permalink: /de/projects/tainted-gun/
order: 0
icon: fa-space-shuttle
---

[![Gamemaker-tested](https://img.shields.io/badge/GameMaker-orange?style=flat&logo=gamemaker&label=Made%20with)](https://gamemaker.io)

<iframe src="https://www.youtube.com/embed/LcZ-spIuBZ0?si=cvgeyEmwaPGClQUd" allow="autoplay; encrypted-media; fullscreen;"></iframe>
<br>
### Beschreibung
<div class="blockText"> {{"
**Tainted Gun** ist ein 2D Rogue-lite Platformer mit vollständig zerstörbarer Umgebung und **per-Pixel** Terrain Deformation.
Im Zentrum des Gameplays stehen Waffen, die neonfarbene Flüssigkeit verschießen – so kann der Spieler **eigene Lichtquellen setzen**,
um dunkle Höhlensysteme zu erkunden. Ein sekundärer Mining Laser ermöglicht es, Ressourcen aus dem Terrain zu extrahieren,
die wiederum für das **Crafting** von Ausrüstung genutzt werden. Das Spiel verwendet **pseudozufällige Levelgenerierung**
mithilfe **interner Mapeditoren** sowie ein dynamisches **Global Illumination System**, das **unendlich viele Lichtquellen** unterstützt.
"| markdownify }} </div>

<div class="screenshots">
    <img src="{{ site.baseurl | append: '/assets/images/tainted gun/screenshot1.png' }}">
    <img src="{{ site.baseurl | append: '/assets/images/tainted gun/screenshot2.png' }}">
    <img src="{{ site.baseurl | append: '/assets/images/tainted gun/screenshot3.png' }}">
</div>
<br>

### Entwicklungsprozess
<div class="blockText"> {{"
**Tainted Gun** begann als eine einfache Idee in einem kleinen **Game Jam Projekt**, das letztlich nie veröffentlicht wurde.
Das Konzept war ein **Puzzle Spiel**, in dem der Spieler nur eine begrenzte Anzahl von **Lichtquellen** setzen konnte,
um sich durch ein Level zu navigieren. Obwohl dieses Projekt verworfen wurde, ließ mich die Grundidee nicht los.

Jahre später nahm ich an einem weiteren Game Jam teil, diesmal mit dem Thema **„Neon“**. Ich erinnerte mich an mein
altes Konzept und dachte es neu: als Shoot 'em up Platformer mit einem besonderen Twist – die Waffe des Spielers
verursachte nicht nur Schaden, sondern beleuchtete die Welt durch leuchtende **Neonflüssigkeit**. Dieser Prototyp
hatte Potenzial, also entschied ich mich, daraus ein vollständiges Spiel zu entwickeln.

#### Weiterentwicklung des Beleuchtungssystems
Das Beleuchtungssystem hat mehrere Iterationen durchlaufen:

* Version 1: Zunächst verwendete ich einen einfachen **Blur Shader**, der auf die Neonflüssigkeit angewendet und
dann ins Spiel eingeblendet wurde, um **Licht zu simulieren**.
* Version 2: Um realistischere Effekte zu erzielen, habe ich ein System entwickelt, das an jeder Stelle,
an der die Flüssigkeit Oberflächen berührte, **raytraced Light Sources** spawnt. Dadurch entstanden **echte Schatten**
– allerdings **auf Kosten der Performance**, da der Spieler **unendlich viele Lichtquellen** setzen konnte.
* Version 3 (aktuell): Ich implementierte ein 2D **Global Illumination System**, das für jeden Pixel auf dem Bildschirm
das einfallende Licht berechnet. Die **Anzahl der Lichtquellen** hat dadurch **keinen Einfluss** mehr auf die Performance
– das Ergebnis ist ein **stabiles**, optisch ansprechendes und **effizientes** Beleuchtungssystem.

#### Zerstörbare Umgebungen & prozedurale Generierung
Ein Feature, das ich schon immer umsetzen wollte, waren **vollständig zerstörbare Level** – und zwar auf **Pixel-
statt Tile-Basis**, wie es in vielen 2D Sandbox Spielen üblich ist. Da mein Lighting System bereits dynamisch
war und **keine vordefinierte Geometrie voraussetzte**, bot sich hier die perfekte Gelegenheit, diese Idee umzusetzen.

Für die Level-Generierung wählte ich einen hybriden Ansatz: Statt komplett zufälliger Level habe ich **handgefertigte
Räume** gestaltet, die bestimmten Mustern folgen. Der Generator **setzt diese Räume prozedural zusammen** – so entsteht
**kontrollierte Zufälligkeit** bei gleichzeitig interessanten Layouts.
Die Höhlenwände werden **als Texturen gerendert** und mithilfe folgender Techniken weiter verfeinert:

* Polygonale Formgebung für **organischere Kanten**
* **Noise Shader** zur Platzierung von Erzen
* Thickness-basierte Shader zur dynamischen Generierung von **Albedo- und Normalmaps**

#### Eigenes UI Framework & Ausblick
Da die verwendete Engine kein eingebautes UI System bietet, habe ich mein **eigenes UI Framework** entwickelt
– ursprünglich für ein anderes Projekt (Lizbox). Damit konnte ich eigene **Ingame Mapeditoren** bauen,
die Leveldesign und Testing deutlich effizienter machen.

Tainted Gun ist noch weit von der Fertigstellung entfernt, aber die Kernmechaniken stehen. Immer wenn ich
Zeit finde, arbeite ich weiter an diesem Projekt – verbessere das Gameplay, optimiere die Performance
und füge neue Features hinzu.
"| markdownify }} </div>

### Links
* [Github repo](https://github.com/sareklambert/tainted-gun-public)

<div style="text-align: center;">
<a href="{{ site.baseurl | append: '/de/projects/repeat-after-me/index.html' }}" class="button scrolly">Nächstes Projekt</a>
</div>
