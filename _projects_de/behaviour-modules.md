---
title: Behaviour Modules
layout: page
lang: de
permalink: /de/projects/behaviour-modules/
order: 3
icon: fa-sitemap
---

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![made-with-cpp](https://img.shields.io/badge/C%2B%2B17-green?style=flat&label=Made%20with)](https://learn.microsoft.com/en-us/cpp/cpp/welcome-back-to-cpp-modern-cpp)
[![Unity-tested](https://img.shields.io/badge/Made%20with-Unity%20-%23000000.svg?&logo=unity)](https://unity.com)
[![Gamemaker-tested](https://img.shields.io/badge/GameMaker-orange?style=flat&logo=gamemaker&label=Made%20with)](https://gamemaker.io)

<iframe src="https://www.youtube.com/embed/t8RM2XKsNJE?si=jzgxTqzDQPRjHGed" allow="autoplay; encrypted-media; fullscreen;"></iframe>
<br>

### Beschreibung
<div class="blockText"> {{"
**Behaviour Modules** ist ein simples, aber wirkungsvolles System zur **Steuerung von KI-Agenten** Jeder Agent definiert
eine Reihe von **States**, und jeder dieser States enthält eine eigene Liste an **Behaviours** sowie Bedingungen für den
**Zustandswechsel**. Betritt ein Agent einen State, wählt er anhand festgelegter **Gewichtungen** ein Behaviour aus. So
können selbst Agenten mit denselben Verhaltensbausteinen unterschiedliche **„Persönlichkeiten“** zeigen.
Ein träger Oger wählt zum Beispiel häufiger das Wait-Behaviour und schlendert nur gelegentlich umher, während ein
hibbeliger Goblin ständig in Bewegung ist und nur kurz pausiert.

Das **Austauschen von Behaviour-Modulen zur Laufzeit** eröffnet spannende Möglichkeiten. So kann etwa der
**Schwierigkeitsgrad** **dynamisch angepasst** werden, indem neue Behaviours hinzukommen. In einem Platformer-Projekt
habe ich etwa einen Gegner implementiert, der bei Sichtkontakt auf den Spieler zustürmt. Anfangs konnte man dem
Angriff leicht ausweichen, indem man über ihn sprang. Auf höheren Schwierigkeitsgraden bekam der Gegner jedoch
ein zusätzliches Behaviour: Er sprang, sobald der Spieler sprang – was ihn zu einer deutlich gefährlicheren
Bedrohung machte.

Durch den **modularen Aufbau** bleibt **jedes Behaviour simpel**, während sich trotzdem **komplexe** und **vielfältige**
Agenten-Verhalten gestalten lassen. Dieses Prinzip sorgt für **Flexibilität**, **Wartbarkeit** und **Skalierbarkeit**
– unabhängig davon, in welchem KI-Kontext das System eingesetzt wird.
"| markdownify }} </div>

<div class="screenshots">
    <img src="{{ site.baseurl | append: '/assets/images/behaviour modules/screenshot1.png' }}">
    <img src="{{ site.baseurl | append: '/assets/images/behaviour modules/screenshot2.png' }}">
    <img src="{{ site.baseurl | append: '/assets/images/behaviour modules/screenshot3.png' }}">
</div>
<br>

### Entwicklungsprozess
<div class="blockText"> {{"
Da viele meiner komplexeren Systeme im Rahmen von **Tainted Gun**, meinem GameMaker Projekt, entstanden sind, wollte ich
zeigen, wie sich eines der einfacheren Systeme **in eine andere Sprache übertragen** lässt. Für dieses Beispiel habe ich
meinen AI Agent Manager ausgewählt – zuerst wurde er **in C++ portiert**, und auf dieser Basis habe ich dann die
**Unity-Version** entwickelt.

Sowohl in GameMaker als auch in der C++ Version werden die **States** der Gegner **direkt im Code definiert**. In der
Unity-Umsetzung hingegen basieren die Behaviours auf **MonoBehaviour** und werden in der Scene-Hierarchie
instanziiert, wodurch sie direkten Zugriff auf Objekte in der Szene haben. Außerdem habe ich **eigene
Editor-Skripte** geschrieben, um das **Inspector GUI** zu nutzen. So können Game Designer die Behaviours **visuell**
miteinander verknüpfen – ganz ohne Codeänderungen.
"| markdownify }} </div>

### Links
* [Github repo](https://github.com/sareklambert/behaviourModules)

<div style="text-align: center;">
<a href="{{ site.baseurl | append: '/de/projects/verlet-integration/index.html' }}" class="button scrolly">Nächstes Projekt</a>
</div>
