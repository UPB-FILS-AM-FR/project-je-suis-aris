<p align="center">
  <img src="logo.png" alt="Néto BOT Logo" width="180">
</p>

<h1 align="center"><strong>Néto BOT</strong></h1>
<h3 align="center" style="color: gray; font-weight: normal;">- système de nettoyage intelligent à navigation autonome -</h3>

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
Néto BOT est un robot aspirateur autonome contrôlé par un microcontrôleur ESP32. Il est conçu pour détecter les obstacles à l’aide d’un capteur à ultrasons monté sur un servomoteur, et contourner automatiquement ces obstacles en adaptant sa trajectoire. Il est équipé d’un système de ventilation assurant l’aspiration des poussières et peut être commandé soit en mode automatique, soit manuellement via une interface Wi-Fi. Tous les composants matériels - L298N, moteurs, ventilateurs, batteries - sont intégrés sur une structure mobile légère et modulaire, optimisée pour les surfaces planes intérieures.
</p>

---

## <span style="color:gray;">MOTIVATION</span>

<p align="justify">
Le projet s’inscrit dans une démarche d’apprentissage appliqué de la robotique domestique et de l’IoT. Il vise à reproduire à moindre coût le fonctionnement des robots aspirateurs commerciaux, en utilisant des composants standards accessibles. Ce robot permet d’explorer la logique de navigation autonome, les systèmes embarqués et la communication Wi-Fi en vue d’un pilotage ou d’un retour d’état à distance. C’est un projet éducatif polyvalent, à forte valeur d’expérimentation.
</p>

---

## <span style="color:gray;">ARCHITECTURE</span>

### DIAGRAMME FONCTIONNEL

<p align="center">
  <img src="schematic_block.png" alt="Diagramme fonctionnel" width="600">
</p>

<p align="justify">
Le <strong>diagramme fonctionnel</strong> illustre de manière abstraite l'organisation logique du système. Il met en évidence les principales fonctions du robot ainsi que les flux d'information entre les composants. Ce schéma est essentiel pour comprendre la répartition des rôles au sein du robot et la manière dont les différents modules interagissent pour remplir la tâche de nettoyage autonome.
</p>

---

### SCHÉMA ÉLECTRIQUE

<p align="center">
  <img src="schematic_Neto_BOT.png" alt="Schéma électrique" width="600">
</p>

<p align="justify">
Le <strong>schéma électrique</strong> représente le câblage réel de l’ensemble des composants du robot, incluant les connexions entre l’ESP32, les moteurs, le module L298N, les capteurs, les alimentations et les ventilateurs. Il permet de visualiser avec précision comment les signaux et l’énergie circulent dans le circuit. Ce schéma est fondamental pour le montage physique du robot et sert de référence lors du prototypage, du dépannage ou de la reproduction du projet.
</p>


---

## <span style="color:gray;">COMPOSANTS</span>

<div align="center">

<div align="center">

<table>
  <thead>
    <tr>
      <th><strong>Produit</strong></th>
      <th><strong>Quantité</strong></th>
      <th><strong>Prix unitaire</strong></th>
      <th><strong>Prix total</strong></th>
      <th><strong>Utilisation</strong></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center"><a href="https://www.optimusdigital.ro/ro/componente-electronice-altele/4359-mufa-dc-pentru-carcasa-interior-de-55-mm-pin-de-21-mm.html?search_query=Mufa+DC+pentru+Carcasa+%28Interior+de+5.5+mm%2C+Pin+de+2.1+mm%29+&results=1">Connecteur DC pour boîtier</a></td>
      <td align="center">2</td>
      <td align="center">0,87 lei</td>
      <td align="center">1,74 lei</td>
      <td align="justify">Interface d’alimentation externe sécurisée.</td>
    </tr>
    <tr>
      <td align="center"><a href="https://www.optimusdigital.ro/ro/prototipare-breadboard-uri/44-breadboard-400-points.html?search_query=Breadboard+HQ+%28400+Points%29+&results=1">Breadboard HQ (400 points)</a></td>
      <td align="center">1</td>
      <td align="center">4,56 lei</td>
      <td align="center">4,56 lei</td>
      <td align="justify">Prototypage sans soudure des circuits électroniques.</td>
    </tr>
    <tr>
      <td align="center"><a href="https://www.optimusdigital.ro/ro/fire-fire-mufate/884-set-fire-tata-tata-40p-10-cm.html?search_query=Fire+Colorate+Tata-Tata+%2840p%2C+10+cm%29+&results=10">Fils Dupont Mâle-Mâle (40p, 10 cm)</a></td>
      <td align="center">1</td>
      <td align="center">4,99 lei</td>
      <td align="center">4,99 lei</td>
      <td align="justify">Connexion directe entre broches GPIO.</td>
    </tr>
    <tr>
      <td align="center"><a href="https://sigmanortec.ro/Suport-Baterii-4AA-cu-Mufa-p148578749">Support pour 4 piles AA avec connecteur</a></td>
      <td align="center">1</td>
      <td align="center">5,34 lei</td>
      <td align="center">5,34 lei</td>
      <td align="justify">Support d’alimentation portable à 6V.</td>
    </tr>
    <tr>
      <td align="center"><a href="https://www.optimusdigital.ro/ro/fire-fire-mufate/881-set-fire-mama-mama-40p-15-cm.html?search_query=Fire+Colorate+Mama-Mama+%2840p%2C+15+cm%29+&results=10">Fils Dupont Femelle-Femelle (40p, 15 cm)</a></td>
      <td align="center">1</td>
      <td align="center">6,99 lei</td>
      <td align="center">6,99 lei</td>
      <td align="justify">Connexion entre modules ou capteurs femelles.</td>
    </tr>
    <tr>
      <td align="center"><a href="https://www.optimusdigital.ro/ro/fire-fire-mufate/878-set-fire-mama-tata-40p-30-cm.html?search_query=Fire+Colorate+Mama-Tata+%2840p%2C+30+cm%29+&results=5">Fils Dupont Mâle-Femelle (40p, 30 cm)</a></td>
      <td align="center">2</td>
      <td align="center">4,81 lei</td>
      <td align="center">9,62 lei</td>
      <td align="justify">Interconnexion flexible entre cartes et modules.</td>
    </tr>
    <tr>
      <td align="center"><a href="https://www.optimusdigital.ro/ro/motoare-servomotoare/2261-micro-servo-motor-sg90-180.html?search_query=Micro+Servomotor+SG90+180%C2%B0+&results=2">Micro Servomoteur SG90 180°</a></td>
      <td align="center">1</td>
      <td align="center">11,99 lei</td>
      <td align="center">11,99 lei</td>
      <td align="justify">Permet l’orientation du capteur à ultrasons (balayage angulaire).</td>
    </tr>
    <tr>
      <td align="center"><a href="https://www.emag.ro/cablu-date-si-incarcare-baseus-cafule-camklf-bg1-usb-la-microusb-1m-2-4a-negru-gri-6953156280335/pd/DNXNN8MBM/">Câble USB à MicroUSB (CAMKLF-BG1)</a></td>
      <td align="center">1</td>
      <td align="center">13,48 lei</td>
      <td align="center">13,48 lei</td>
      <td align="justify">Utilisé pour alimenter et programmer la carte ESP32 via USB.</td>
    </tr>
    <tr>
      <td align="center"><a href="https://www.optimusdigital.ro/ro/suporturi-de-baterii/12571-suport-pentru-6-baterii-aa-fara-capac.html?search_query=Suport+pentru+6+baterii+AA+fara+capac+&results=1">Support pour 6 piles AA</a></td>
      <td align="center">1</td>
      <td align="center">8,98 lei</td>
      <td align="center">8,98 lei</td>
      <td align="justify">Alimentation modulaire de 9V pour moteurs.</td>
    </tr>
    <tr>
      <td align="center"><a href="https://www.optimusdigital.ro/ro/accesorii-altele/7962-ventilator-cy205a-12-v-80x80x25-mm.html?search_query=Ventilator+CY205%2FA+12+V+80x80x25+mm+&results=1">Ventilateur CY205/A 12 V 80×80×25 mm</a></td>
      <td align="center">2</td>
      <td align="center">8,99 lei</td>
      <td align="center">17,98 lei</td>
      <td align="justify">Génère une aspiration d’air pour la fonction de nettoyage par succion.</td>
    </tr>
    <tr>
      <td align="center"><a href="https://www.optimusdigital.ro/ro/drivere-de-motoare-cu-perii/145-driver-de-motoare-dual-l298n.html?search_query=Modul+cu+Driver+de+Motoare+Dual+L298N+Rosu+&results=1">Module avec Driver de Moteurs Double L298N</a></td>
      <td align="center">3</td>
      <td align="center">10,99 lei</td>
      <td align="center">32,97 lei</td>
      <td align="justify">Contrôle indépendant de deux moteurs DC par module.</td>
    </tr>
    <tr>
      <td align="center"><a href="https://altex.ro/baterii-alcaline-basic-duracell-aa-6-bucati/cpd/BATBASICAAK6/">Piles AA</a></td>
      <td align="center">10</td>
      <td align="center">3,60 lei</td>
      <td align="center">36,00 lei</td>
      <td align="justify">Source d’énergie autonome pour modules électroniques.</td>
    </tr>
    <tr>
      <td align="center"><a href="https://www.emag.ro/placa-esp32-cu-esp-wroom-32-38-pini-cu-cip-cp2102-multicolor-esp32-cp2102/pd/D7R798MBM/?ref=history-shopping_416932438_112784_1">Carte ESP32 avec module ESP-WROOM-32</a></td>
      <td align="center">1</td>
      <td align="center">57,96 lei</td>
      <td align="center">57,96 lei</td>
      <td align="justify">Microcontrôleur central assurant la logique, les capteurs et la connectivité Wi-Fi/Bluetooth.</td>
    </tr>
    <tr>
      <td align="center"><a href="https://www.optimusdigital.ro/ro/motoare-altele/139-motor-cu-reductor-si-roata.html?search_query=Motor+cu+reductor+si+roata+&results=18">Moteur avec réducteur et roue</a></td>
      <td align="center">4</td>
      <td align="center">14,99 lei</td>
      <td align="center">59,96 lei</td>
      <td align="justify">Permet la mobilité du robot avec force de traction suffisante.</td>
    </tr>
    <tr>
      <td colspan="3" align="right"><strong>Total général</strong></td>
      <td align="center"><strong>328,12 lei</strong></td>
      <td></td>
    </tr>
  </tbody>
</table>

</div>

---

## <span style="color:gray;">BIBLIOTHÈQUES</span>

<div align="justify">

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
      <td><a href="https://github.com/espressif/arduino-esp32">ESP32 WiFi</a></td>
      <td align="justify">Librairie officielle ESP32 pour gérer la connectivité Wi-Fi, les sockets TCP, UDP, et les serveurs HTTP.</td>
      <td align="justify">Utilisée pour établir une connexion à un réseau local et permettre la commande du robot via interface Web embarquée.</td>
    </tr>
  </tbody>
</table>

</div>

---

## <span style="color:gray;">JOURNAL DE DÉVELOPPEMENT</span>

<div align="justify">

#### Semaine 6 – 12 Mai
- Assemblage du châssis mobile  
- Installation des moteurs DC et test avec L298N  
- Implémentation du système d’alimentation à base de batteries AA

#### Semaine 7 – 19 Mai


#### Semaine 20 – 26 Mai


</div>

---

## <span style="color:gray;">LIENS UTILES</span>

<div align="justify">

##### **Vidéos de projets similaires**

- [Autonomous Vacuum Cleaner DIY Project – How It Works](https://www.youtube.com/watch?v=iOrvGC9REEE)
- [Robot Aspirateur fait maison (système complet)](https://www.youtube.com/watch?v=n8C8cyyUXuY)
- [Build an Obstacle Avoiding Robot Using Arduino and Ultrasonic](https://www.youtube.com/watch?v=UU7VVbEZulw)
- [#vacuumcleanerscienceproject (inspirations scientifiques)](https://www.youtube.com/watch?v=hHIIWpZcYNs&pp=ygUcI3ZhY2N1bWNsZWFuZXJzY2llbmNlcHJvamVjdA%3D%3D)

---

##### **Tutoriels techniques (composants)**

- [ESP32 Pinout and Configuration Guide](https://randomnerdtutorials.com/esp32-pinout-reference-gpios/)
- [How to Use the L298N Motor Driver Module](https://lastminuteengineers.com/l298n-dc-stepper-driver-arduino-tutorial/)
- [Servo Motor SG90 with Arduino](https://components101.com/motors/sg90-servo-motor)
- [Ultrasonic Sensor HC-SR04 – How it Works & How to Use](https://randomnerdtutorials.com/complete-guide-for-ultrasonic-sensor-hc-sr04/)
- [How to Power a Robot (Battery & Voltage Considerations)](https://www.robotshop.com/community/forum/t/robot-power-supplies-how-to-choose-the-right-one/13093)

---

##### **Documentation officielle & fiches techniques**

- [ESP32 Datasheet (Espressif)](https://www.espressif.com/sites/default/files/documentation/esp32_datasheet_en.pdf)
- [Arduino Reference – Digital and PWM Pins](https://www.arduino.cc/reference/en/)
- [SG90 Servo Datasheet PDF](https://cdn.sparkfun.com/datasheets/Robotics/Standard%20Servo%20-%20SG90.pdf)
- [L298N Motor Driver Datasheet](https://www.st.com/resource/en/datasheet/l298.pdf)
- [HC-SR04 Sensor Datasheet](https://cdn.sparkfun.com/datasheets/Sensors/Proximity/HCSR04.pdf)

---

##### **Articles scientifiques & applications robotiques**

- [Low-cost Autonomous Vacuum Cleaner: A Hardware Perspective – ResearchGate](https://www.researchgate.net/publication/348364379_Low-cost_Autonomous_Vacuum_Cleaner_A_Hardware_Perspective)
- [Design and Implementation of an Obstacle Avoiding Robot](https://www.ijser.org/researchpaper/Design-and-Implementation-of-Obstacle-Avoiding-Robot.pdf)
- [Smart Vacuum Cleaners in IoT Ecosystem](https://ieeexplore.ieee.org/document/9565893)
- [Embedded Systems in Robotics Applications – Overview](https://ieeexplore.ieee.org/document/8754793)

</div>
