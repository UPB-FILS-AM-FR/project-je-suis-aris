<p align="center">
  <img src="logo.png" alt="Néto BOT Logo" width="180">
</p>

<h1 align="center"><strong>Néto BOT</strong></h1>
<h3 align="center" style="color: gray; font-weight: normal;">robot de nettoyage autonome</h3>

<p align="center">
  <strong>Auteur :</strong> Aris-Georgian ILIE &nbsp;|&nbsp; 
  <strong>Faculté :</strong> Faculté d'Ingénierie en Langues Étrangères &nbsp;|&nbsp;
  <strong>Groupe :</strong> 1220 FA
</p>

---

## TABLE DES MATIÈRES

- [DESCRIPTION](#description)
- [MOTIVATION](#motivation)
- [ARCHITECTURE](#architecture)
  - [DIAGRAMME FONCTIONNEL](#diagramme-fonctionnel)
  - [SCHÉMA ÉLECTRIQUE](#schéma-électrique)
- [COMPOSANTS](#composants)
- [BIBLIOTHÈQUES](#bibliothèques)
- [JOURNAL DE DÉVELOPPEMENT](#journal-de-développement)
- [LIENS UTILES](#liens-utiles)

---

## <span style="color:gray;">DESCRIPTION</span>

<p align="justify">
Néto BOT est un robot autonome conçu pour détecter les obstacles et effectuer le nettoyage de surfaces planes. Il utilise des capteurs à ultrasons, un système de pulvérisation d’eau, et une structure motorisée commandée par microcontrôleur.
</p>

---

## <span style="color:gray;">MOTIVATION</span>

<p align="justify">
Ce projet combine électronique embarquée, programmation Arduino et robotique pratique, pour créer un robot utile, efficace et éducatif, tout en explorant les défis liés à l’automatisation mobile.
</p>

---

## <span style="color:gray;">ARCHITECTURE</span>

### DIAGRAMME FONCTIONNEL

<p align="center">
  <img src="schematics/block_diagram.png" alt="Diagramme fonctionnel" width="600">
</p>

### SCHÉMA ÉLECTRIQUE

<p align="center">
  <img src="schematics/kicad_schematic.png" alt="Schéma électrique" width="600">
</p>

---

## <span style="color:gray;">COMPOSANTS</span>

<div align="center">

<table>
  <thead>
    <tr>
      <th><strong>Produit</strong></th>
      <th><strong>Quantité</strong></th>
      <th><strong>Prix unitaire (RON)</strong></th>
      <th><strong>Prix total (RON)</strong></th>
      <th><strong>Utilisation</strong></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center"><a href="https://www.optimusdigital.ro/ro/audio-buzzere/635-buzzer-activ-de-3-v.html">Buzzer actif</a></td>
      <td align="center">1</td>
      <td align="center">1.5</td>
      <td align="center">1.5</td>
      <td align="justify">Signal sonore utilisé pour alerter les utilisateurs en cas d’obstacle détecté.</td>
    </tr>
    <tr>
      <td align="center"><a href="https://www.optimusdigital.ro/ro/butoane-i-comutatoare/1119-buton-6x6x6.html">Bouton-poussoir</a></td>
      <td align="center">1</td>
      <td align="center">1</td>
      <td align="center">1</td>
      <td align="justify">Permet un démarrage manuel du robot ou un reset en cas de problème.</td>
    </tr>
    <tr>
      <td align="center"><a href="https://www.optimusdigital.ro/ro/fire-fire-mufate/884-set-fire-tata-tata-40p-10-cm.html">Fils Dupont</a></td>
      <td align="center">1 set</td>
      <td align="center">7</td>
      <td align="center">7</td>
      <td align="justify">Connexion entre les composants électroniques (capteurs, contrôleur, moteurs).</td>
    </tr>
    <tr>
      <td align="center"><a href="https://www.optimusdigital.ro/ro/prototipare-breadboard-uri/8-breadboard-830-points.html">Breadboard</a></td>
      <td align="center">1</td>
      <td align="center">10</td>
      <td align="center">10</td>
      <td align="justify">Support de prototypage sans soudure pour tester les circuits du robot.</td>
    </tr>
    <tr>
      <td align="center"><a href="https://www.optimusdigital.ro/ro/acumulatori-si-accesorii/1816-acumulator-18650-li-ion-3-7v-2600mah-samsung.html">Batterie Li-ion 18650</a></td>
      <td align="center">2</td>
      <td align="center">18</td>
      <td align="center">36</td>
      <td align="justify">Alimente électriquement le système embarqué et les moteurs.</td>
    </tr>
    <tr>
      <td align="right" colspan="3"><strong>Total général</strong></td>
      <td align="center"><strong>55.5</strong></td>
      <td></td>
    </tr>
  </tbody>
</table>

</div>

---

## <span style="color:gray;">BIBLIOTHÈQUES</span>

<div align="center">

<table>
  <thead>
    <tr>
      <th><strong>Bibliothèque</strong></th>
      <th><strong>Description</strong></th>
      <th><strong>Utilisation</strong></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center"><a href="https://bitbucket.org/teckel12/arduino-new-ping/wiki/Home">NewPing</a></td>
      <td align="justify">Bibliothèque légère et rapide permettant d’utiliser efficacement les capteurs à ultrasons HC-SR04 sans bloquer le microcontrôleur.</td>
      <td align="justify">Mesure précise des distances à l’aide des capteurs à ultrasons, utilisée pour la détection d’obstacles et la navigation autonome.</td>
    </tr>
    <tr>
      <td align="center"><a href="https://www.arduino.cc/en/Reference/LiquidCrystal">LiquidCrystal</a></td>
      <td align="justify">Bibliothèque native Arduino permettant le contrôle des écrans LCD alphanumériques 16x2 ou 20x4 à base de contrôleur HD44780.</td>
      <td align="justify">Affichage en temps réel des messages, alertes et états internes du robot (par exemple : niveau de batterie, détection d'obstacle).</td>
    </tr>
  </tbody>
</table>

</div>

---

## <span style="color:gray;">JOURNAL DE DÉVELOPPEMENT</span>

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

## <span style="color:gray;">LIENS UTILES</span>

- [Tutoriel capteurs – Ben Eater](https://www.youtube.com/watch?v=wdgULBpRoXk)
- [Article sur les moteurs – ExplainThatStuff](https://www.explainthatstuff.com/induction-motors.html)
- [Arduino Project Hub](https://projecthub.arduino.cc/)
