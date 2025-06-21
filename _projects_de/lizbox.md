---
title: Lizbox
layout: page
lang: de
permalink: /de/projects/lizbox/
order: 5
icon: fa-wrench
---

[![Gamemaker-tested](https://img.shields.io/badge/GameMaker-orange?style=flat&logo=gamemaker&label=Made%20with)](https://gamemaker.io)

<iframe src="https://www.youtube.com/embed/zRNpTJLAKzE?si=4N1GyI4RCSoPohNM" allow="autoplay; encrypted-media; fullscreen;"></iframe>
<br>

### Beschreibung
<div class="blockText"> {{"
**Lizbox** ist eine Sammlung spezialisierter **Pixel Art Tools**, die ich für meine Game Projekte entwickelt habe. Das
herausragendste Tool ist der **Animation Mask Editor**, mit dem sich **Gradient Texturen** erstellen lassen, die in
Kombination mit **Shadern** einzigartige **2D Animationen** ermöglichen.
Das Tool bietet unter anderem Funktionen zur **besseren Visualisierung von Gradients**, verschiedene **Zeichenwerkzeuge**,
eine Aktionen-Historie (**Protokoll**) sowie diverse Exportoptionen – leistungsstark und gleichzeitig **benutzerfreundlich**.
"| markdownify }} </div>

<div class="screenshots">
    <img src="{{ site.baseurl | append: '/assets/images/lizbox/screenshot1.png' }}">
    <img src="{{ site.baseurl | append: '/assets/images/lizbox/screenshot2.png' }}">
    <img src="{{ site.baseurl | append: '/assets/images/lizbox/screenshot3.png' }}">
</div>
<br>

### Entwicklungsprozess
<div class="blockText"> {{"
Während ich **UI-Animationen** für eines meiner Spiele erstellte, frustrierte mich, wie **zeitaufwändig** der Prozess war –
also begann ich, nach **Alternativen** zu suchen. Zuvor hatte ich **shaderbasierte Übergänge** verwendet, bei denen einfache
graue Gradient Texturen genutzt wurden, um **Zeit darzustellen** und Bilder ein- bzw. auszublenden. Diese Methode war
jedoch ungenau und konnte nur auf ganze Bilder angewendet werden.

Um **präziser** zu arbeiten, experimentierte ich damit, Gradients manuell über UI-Elemente zu zeichnen, um dynamischere
Animationen zu erzeugen. Die Ergebnisse waren vielversprechend, doch der Prozess war weiterhin mühsam, und die
feinen **Farbunterschiede** der Gradients waren mit bloßem Auge **schwer zu erkennen**. Ich brauchte ein Tool, mit dem
man quasi **„Zeit zeichnen“** konnte – und das gleichzeitig genug Kontrast zwischen den einzelnen Pixeln bietet. Doch
ein solches Tool gab es nicht.

Also habe ich es selbst gebaut – in **GameMaker**. Da die Engine kein integriertes UI-System bietet, habe ich zunächst
ein vollständiges **UI-Framework** von Grund auf entwickelt, inklusive **Fenster**, **Docking**, **Skalierung** und weiteren
Basisfunktionen. Darauf aufbauend entstand ein Zeichenwerkzeug, das automatisch durch eine benutzerdefinierte
Palette cycled und so **klare visuelle Abgrenzung** zwischen den Gradient-Schritten schafft.
Dann folgten **Quality-of-Life Features** wie Linienwerkzeug, anpassbare Pinselgrößen, Zoom, Undo-/Redo-System
(basierend auf Software-Design-Patterns, die ich im Studium gelernt habe), Exportoptionen und vieles mehr.

Dieses Projekt war eine großartige Gelegenheit, mein Verständnis für **UI Design** zu vertiefen – und ein gutes
Beispiel für die **maßgeschneiderten Tools**, die ich gelegentlich entwickle, um meinen Workflow zu optimieren.
Außerdem zeigt es einige meiner einfacheren **2D Shader** in Aktion.
"| markdownify }} </div>

### Links
* [Github repo](https://github.com/sareklambert/lizbox-public)
* [Public download](https://jamjamteam.itch.io/lizbox)

<div style="text-align: center;">
<a href="{{ '/de/' }}" class="button scrolly">Home</a>
</div>
