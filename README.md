<p align="center">
  <img src="assets/logo.png" alt="Néto BOT Logo" width="180">
</p>

<h1 align="center">Néto BOT – Robot de nettoyage autonome</h1>

---

## Table des matières

- [Description](#description)
- [Motivation](#motivation)
- [Architecture](#architecture)
  - [Diagramme fonctionnel](#diagramme-fonctionnel)
  - [Schéma électrique](#schéma-électrique)
- [Composants](#composants)
- [Bibliothèques](#bibliothèques)
- [Journal de développement](#journal-de-développement)
- [Liens utiles](#liens-utiles)

---

## Description

Néto BOT est un robot autonome conçu pour détecter les obstacles et effectuer le nettoyage de surfaces planes. Il utilise des capteurs à ultrasons, un système de pulvérisation d’eau, et une structure motorisée commandée par microcontrôleur.

---

## Motivation

Ce projet combine électronique embarquée, programmation Arduino et robotique pratique, pour créer un robot utile, efficace et éducatif, tout en explorant les défis liés à l’automatisation mobile.

---

## Architecture

### Diagramme fonctionnel

![Diagramme fonctionnel](schematics/block_diagram.png)

### Schéma électrique

![Schéma](schematics/kicad_schematic.png)

---

## Composants

| Appareil              | Rôle                    | Prix |
|-----------------------|-------------------------|------|
| Buzzer actif          | Signal sonore           | [1.5 RON](https://www.optimusdigital.ro/ro/audio-buzzere/635-buzzer-activ-de-3-v.html) |
| Bouton-poussoir       | Commande manuelle       | [1 RON](https://www.optimusdigital.ro/ro/butoane-i-comutatoare/1119-buton-6x6x6.html) |
| Fils Dupont           | Connexions internes     | [7 RON](https://www.optimusdigital.ro/ro/fire-fire-mufate/884-set-fire-tata-tata-40p-10-cm.html) |
| Breadboard            | Support de prototypage  | [10 RON](https://www.optimusdigital.ro/ro/prototipare-breadboard-uri/8-breadboard-830-points.html) |
| Batterie Li-ion 18650 (x2) | Alimentation mobile | 18 RON × 2 |

---

## Bibliothèques

| Bibliothèque | Description                                      | Utilisation                        |
|--------------|--------------------------------------------------|------------------------------------|
| [NewPing](https://bitbucket.org/teckel12/arduino-new-ping/wiki/Home) | Bibliothèque pour capteurs HC-SR04 | Mesure de distance à ultrasons    |
| [LiquidCrystal](https://www.arduino.cc/en/Reference/LiquidCrystal) | Contrôle des écrans LCD 16x2       | Affichage d’informations          |

---

## Journal de développement

### Semaine 6 – 12 Mai
- Assemblage du châssis
- Test des moteurs avec le pilote L298N

### Semaine 7 – 19 Mai
- Intégration des capteurs à ultrasons
- Début du système de détection d’obstacles

### Semaine 20 – 26 Mai
- Calibration de la pompe à eau
- Tests en environnement réel

---

## Liens utiles

- [Tutoriel capteurs – Ben Eater](https://www.youtube.com/watch?v=wdgULBpRoXk)
- [Article sur les moteurs – ExplainThatStuff](https://www.explainthatstuff.com/induction-motors.html)
- [Arduino Project Hub](https://projecthub.arduino.cc/)
