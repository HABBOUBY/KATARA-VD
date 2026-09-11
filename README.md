<div align="center">

# KATARA-VD

### une mahcine qui ne vend pas mais elle donne


<p align="center">
  <img src="05_MEDIA/IMAGES/main image of the project.png" width="600">
</p>

<p align="center">
  <img src="05_MEDIA/IMAGES/VENDING MACHINE 4K.png" width="250">
  <img src="05_MEDIA/IMAGES/JALOUL 4K.png" width="250">
  <img src="05_MEDIA/IMAGES/PCB_KEYBOARD_4K.png" width="250">
</p>

![Raspberry Pi](https://img.shields.io/badge/Vision-Raspberry%20Pi%205-red)
![Arduino](https://img.shields.io/badge/Control-Arduino%20Mega%202560-teal)
![KiCad](https://img.shields.io/badge/PCB-KiCad-blue)
![SolidWorks](https://img.shields.io/badge/CAD-SolidWorks-orange)
![RealSense](https://img.shields.io/badge/Vision-Intel%20RealSense%20D435-lightgrey)
![Solar](https://img.shields.io/badge/Power-Solar%20Backup-yellow)
![CNC](https://img.shields.io/badge/Fabrication-CNC%20Laser--Cut%20MDF-success)
![License](https://img.shields.io/badge/License-MIT-green)

Built by **HABBOUBY EDEM**

</div>

---

## Table of Contents

- [About](#about)
- [Repository Structure](#repository-structure)
- [Scope of This Submission](#scope-of-this-submission)
- [Note on Physical Fabrication](#note-on-physical-fabrication)
- [The Story Behind KATARA-VD](#the-story-behind-katara-vd)
- [The Ecosystem: 2 Systems, 1 Mission](#the-ecosystem-2-systems-1-mission)
- [Vending Machine](#vending-machine)
  - [Part 1 — Skeleton, Shelving & Archimedean Dispensers](#part-1--skeleton-shelving--archimedean-dispensers)
  - [Part 2 — Solar Power & Access Doors](#part-2--solar-power--access-doors)
  - [Part 3 — Prescription Verification System](#part-3--prescription-verification-system)
  - [Part 4 — Coin Dispensing Mechanism ("Giving Money")](#part-4--coin-dispensing-mechanism-giving-money)
  - [Part 5 — Coin Acceptance & Storage](#part-5--coin-acceptance--storage)
  - [Part 6 — Charity Keypad PCB](#part-6--charity-keypad-pcb)
  - [Part 7 — Thermal Sensing & Voice Interaction](#part-7--thermal-sensing--voice-interaction)
- [JALOUL — The Restocking Humanoid](#jaloul--the-restocking-humanoid)
  - [Part 8 — Head & Expression System](#part-8--head--expression-system)
  - [Part 9 — Body & Shoulder Joints](#part-9--body--shoulder-joints)
  - [Part 10 — Arm Completion & 360° Gripper](#part-10--arm-completion--360-gripper)
  - [Part 11 — Mecanum Base & Vertical Lift](#part-11--mecanum-base--vertical-lift)
  - [Part 12 — Frame Reinforcement & LiDAR](#part-12--frame-reinforcement--lidar)
- [The Humanitarian Logic — How the Community Fund Works](#the-humanitarian-logic--how-the-community-fund-works)
- [Electronics & PCB](#electronics--pcb)
- [Materials & Fabrication](#materials--fabrication)
- [Fasteners](#fasteners)
- [CAD Files](#cad-files)
- [Simulations](#simulations)
- [On AI Assistance](#on-ai-assistance)
- [Future Improvements](#future-improvements)
- [License](#license)

---

## About

**Katara-vd** une machine intelligente qui donne au lieu de vendre les médiacaments pour les personnes qui ont besoin . et pour que les riches personnes ont accès à cette mahicne ils doivent payer 2 euro , accompagné d'un huamnoid robot qui permet de remplir le distributeur .


Katara-vd  est le projet principal constitué de deux mini -projet:

-le distributeur: qui a une partie pour les médicaments , de plus , ce distributeur a une partie pour les dons qui a un mécanisme de pousse pour donner de l'argent et une petite pièce pour trier les pièces de monnaie ( seulement accepte les pièces de 2 euro)

-The humanoid robot  , son nom est "JALLUL " son tache est de remplir le distributeur lorsqu'il est vide de médicament 



---

## Repository Structure

```text
KATARA-VD/
│
├── 01_3D/
│   ├── SOLIDWORKS_FILES/
│   │   ├── HUMANOID_ROBOT JALOUL/      
│   │   └── VENDING_MACHINE/            
│   ├── STEP_FILES/
│   │   ├── HUMANOID_ROBOT JALOUL/      
│   │   └── VENDING_MACHINE/         
│   └── STL/
│       ├── HUMANOID_ROBOT JALOUL/      
│       └── VENDING_MACHINE/            
│
├── 02_DXF/
│   └── VENDING_MACHINE/
│
├── 03_PCB_DESIGN/
│   ├── VENDING MACHINE PCB.kicad_sch / .kicad_pcb / .kicad_pro / .kicad_prl
│   └── CARTE ELEC MEC 07.step
│
├── 04_DOCS/
│   └── KATARA-VD_PCB_Components.xlsx   
│   └──WIRING
|
├── 05_MEDIA/
│   ├── IMAGES/
│   │   ├── main image of the project.png
│   │   ├── VENDING MACHINE 4K.png
│   │   ├── JALOUL 4K.png
│   │   ├── JALOUL in different positions.png
│   │   └── PCB_KEYBOARD_4K.png
│   └── SIMULATIONS/
│       ├── mechanism of prescription.gif
│       ├── mechanism of giving money.gif
│       ├── GIF MEC PUSHING THE MONEY INTO THE BOX.gif
│       ├── mechanism for opening and closing door.gif
│       └── translation of the robot on yy' axis.gif
│
├── LICENSE
└── README.md
```

---



## remarque pour la fabrication physique 

malheuresemnt j'ai pas accès à l'impression 3d  pour faire un petit prototype et les composants électriques car ils osnt très chères ( raspberry pi 5 and intel real sense)

Mais "KATARA" est pret pour la mettre en production réelle et le rendre fonctionel ( j'ai mis tous les dossiers nécessaires pour l'impression  3d et le découpe cnc)

- **CNC laser-cut MDF** (`02_DXF/`) 
- **3D-printable STL/STEP** (`01_3D/`) 

-une petite remarque: j'ai fait ce mixage de matière  car il y a des pièces qui sont un peu grande donc il est impossible de l'imprimer avec une printer 3D local

---

## Comment l'idée de KATARA est née
Cette idée est née du hackclub comme il est  "charitable " club , donc j'ai pensé à faire une chose qui a des bienfaits pour tous le monde .

---


# Le distributeur 

## Partie 1 : MEC CiSEAUX

<p align="center">
  <img src="05_MEDIA/IMAGES/mec cisseau.PNG" width="450">
</p>

Le distributeur a  5 principaux plateaux qui referment les médicaments .Donc pour que les plateaux soient accessibles à "JALOUL"  , doit avoir un mvt en translation donc le mec de ciseux permet les plateaux de sortir autrement dit mec ciseaux permet de  l'étirement et le raccourcissement des plateaux.Ce mec ciseaux est accompagné avec un stepper A17 de telle façon le mvt en rotation se transforme en translation

---

## Partie 2- panneau solaire et le porte intelligent 

<p align="center">
  <img src="05_MEDIA/IMAGES/VENDING MACHINE 4K.png" width="450">
</p>

AU cas ou les batteries sont vide , et n'existe pas du courant donc il le panneau solaire est un alternatif dans ce cas ( qui permet de charger un batterie et cette batterie va etre consommé au cas ou les batteries vides.
De plus , ce distributeur a une porte intelligente qui s'ouvre et se ferme avec deux vérins électriques d'un façon  à transformer le mvt linéaire en mvt rotatif .Et ça a une dualité de fonction le distributeur n'est pas accessibles aux personnes seulement au "JALLOUL"

---

## Part 3 — Scanner et vérifier l'accès pour les médicaments
<p align="center">
  <img src="05_MEDIA/SIMULATIONS/mechanism of prescription.gif" width="450">
</p>

Pour avoir un accès légal pour le distributeur , doit etre la personne accompagné avec une ordonnance.Cette etapge est guidé avec un mécanisme linéaire avec un stepper nema A 17 qui permet de translater un support qui a intérieument deux aimants magnétiques de telle façon l'ordonnace est attaché au support avec deux fixation que peut la personnes l'ouvrir et le fermer  ( aussi ces deux fixations ont à son intérieur un aimant magnétique de façon une attraction magnétique va etre crée avec le support principal ).Puis un caméra intelreal sense va détecter  le nom du médicament .Et finalement le médicament est poussé avec un spirale ( avec un moteur pas à pas petit ) puis il tombe en faisant une chute libre.

<p align="center">
  <img src="05_MEDIA/IMAGES/mec ordonnance 1.1.PNG" width="350">
  <img src="05_MEDIA/IMAGES/fixation ordonnance.PNG" width="350">
</p>

*A gauche: le mvt linéaire par le stepper et le scan avec le caméra intelreal sense * 
*A droit : le support de l'ordonnance et ses deux fixations  qui vont  l'attatacher *

---

## Part 4 — système de pousse de l'argent

<p align="center">
  <img src="05_MEDIA/SIMULATIONS/mechanism of giving money.gif" width="450">
</p>
<p align="center">
  <img src="05_MEDIA/SIMULATIONS/GIF MEC PUSHING THE MONEY INTO THE BOX.gif" width="450">
</p>

Le premier GIF  montre , le pousse de l'argent pour les donnés aux personnes qui ont besoin 
Le dexième GIF montre aussi le pousse de l'argent mais dans un box , et ce mec est pour conserver les pièces de monnaies que les riches personnes ont donné  dans le boxe  qui sont tombé de la pièce de tri de monnaie 

---

## Part 5 — LA pièce de tri de l'argent 

<p align="center">
  <img src="05_MEDIA/IMAGES/système de tri coin.PNG" width="300">
</p>

la pièce de monnaie se glisse d'un façon cette pièce permet de trier les pièces , donc comment ??
Cette pièce a un petit mur qui est oblique d'un 30 degré puis il est suivi  d'un trou  de diamètre un peu plus petit du pièce de monnaie du 2 euro donc si la pièce donné est 2euro va etre glissé  et se tombe dans le box  et il y a un capteur IR qui va détcteer qu'elle a tombé.
Si la pièce est plus petite que 2 euro donc elle va tomber au trou et sort et si elle est plus  grande que 2 euro au début il ne peut pas entrer à cette pièce

regardez l'imagez pour mieux comprendre

---

## Part 6 — Charity Keypad PCB

<p align="center">
  <img src="05_MEDIA/IMAGES/PCB_KEYBOARD_4K.png" width="450">
</p>

The identification and donation-amount interface runs on a custom **KiCad PCB** — a double-sided board with **0.5 mm copper traces** throughout, since the board carries no significant power or current. An **OLED display** handles animations and shows each resident's ID code, since every person in the community has a unique identifier used to validate which function (receiving or giving) they're authorized to access. Full BOM with sourcing links: [`04_DOCS/KATARA-VD_PCB_Components.xlsx`](04_DOCS/KATARA-VD_PCB_Components.xlsx).

---

## Part 7 — Thermal Sensing & Voice Interaction

An infrared thermal camera reads the person standing in front of the machine — not to identify them, but to catch visible signs that something is wrong: distress, sadness, or a physical state serious enough to count as a medical emergency. Paired with a small onboard speaker, the machine can respond dynamically rather than just process a transaction, making the interaction feel less like a vending machine and more like something that's actually paying attention.

---

# JALOUL — The Restocking Humanoid

## Part 8 — Head & Expression System

<p align="center">
  <img src="05_MEDIA/IMAGES/JALOUL 4K.png" width="450">
</p>

JALOUL's head carries an **Intel RealSense** camera for vision and a **Raspberry Pi 5** for onboard data processing. A servo-driven **mouth mechanism** — a driver/follower pulley pair guided at both ends by matched M3 screws and nuts, same module and diameter for symmetric motion — opens and closes as if the robot is speaking, giving it a more expressive, approachable presence.

---

## Part 9 — Body & Shoulder Joints

After the head, the neck and body were completed, followed by the first two shoulder joints. The first joint's axis runs perpendicular to the robot's body, tracing a circle tangent to the head's median plane; the second joint moves in a plane perpendicular to the first. Together they formed a first half-arm, mirrored across the body to create the second.

---

## Part 10 — Arm Completion & 360° Gripper

<p align="center">
  <img src="05_MEDIA/IMAGES/JALOUL in different positions.png" width="450">
</p>

The half-arm alone didn't give a good enough range of motion, so **3 additional joints** were added — two to complete the arm and let it reach in closer toward the body, and a third dedicated to the gripper, letting it spin a full **360°** around the arm's axis. That's **5 joints per arm, 10 total** across both. The gripper itself runs on a dual-pinion system driven by an **MG995 servo**, and the overall body shape was refined to look more presentable and cohesive. The image above shows both arms swept across several positions, illustrating the reach this extra range of motion unlocks.

---
### Medication Tray Design
<p align="center">
  <img width="300" height="200" alt="medication-tray-isometric-view png" src="https://github.com/user-attachments/assets/37e8b059-3b52-4097-b8ed-f77eeaf53c0b" />
  <img width="300" height="200" alt="medication-tray-spacing-topview png" src="https://github.com/user-attachments/assets/d1b10d59-b2a3-4ea6-948e-78fdb3621509" />
</p>



The medication tray is designed with precisely spaced compartments, allowing JALOUL's
gripper to reliably grab, lift, and place each medication box during the restocking process.
## Part 11 — Mecanum Base & Vertical Lift

<p align="center">
  <img src="05_MEDIA/SIMULATIONS/translation of the robot on yy' axis.gif" width="450">
</p>

JALOUL moves on a **4-wheel mecanum differential base**, giving it 5 distinct movements — forward, backward, left, right, and rotation around its own center of inertia (deliberately aligned with its center of mass for stable motion). Four **NEMA 23 stepper motors** drive the wheels. A storage backpack rides up and down along the robot's Y-Y′ axis via a **lead screw–nut system**, powered by a fifth NEMA 23 stepper and guided by two **M8 smooth rods** with linear bearings.

---

## Part 12 — Frame Reinforcement & LiDAR

The lead screw system was finished off with a protective cover, and **aluminum extrusion profiles** were added throughout the frame for rigidity and long-term structural stability. Finally, an **RPLiDAR** sensor was integrated for obstacle detection and environment mapping, letting JALOUL navigate around the vending machine safely.

---

## The Humanitarian Logic — How the Community Fund Works

KATARA-VD doesn't rely on outside donations to stay running — the fund lives inside the machine itself, managed through the two keypads described in [Part 4](#part-4--coin-dispensing-mechanism-giving-money) and [Part 5](#part-5--coin-acceptance--storage).

- **Every person has a personal ID code**, entered on either keypad, that tells the machine exactly what they're authorized to do.
- **Requesting help:** a family in need enters their ID and the amount they need on the "receiving" keypad. Each family is capped at **€10 each day** — enough to help them get by, not a blank check.
- **Giving back:** someone whose financial situation is stable is expected to contribute through the "giving" keypad — exactly **€2 per day**. The coin acceptor is built to reject anything above or below that amount.
- **Accountability:** if a contributor misses their daily donation for **10 days within a single month**, they lose access to free medication from the machine until their participation resumes.
- **The loop closes automatically:** every euro accepted through the donation side feeds directly into the coin-dispensing mechanism on the receiving side — the community funds itself.

This logic is what turns KATARA-VD from a simple vending machine into a small, self-sustaining mutual-aid system.

---

## Electronics & PCB

- **Raspberry Pi 5** — vision and analysis layer: processes the Intel RealSense prescription scans and the thermal camera readings.
- **Arduino Mega 2560** — command layer: drives the machine's motors, servos, solenoids, and sensors.
- **Custom KiCad PCB** (`03_PCB_DESIGN/`) — the charity keypad module: double-sided, 0.5 mm traces, OLED display, ID validation circuitry.

Full BOM with Amazon sourcing links: [`04_DOCS/KATARA-VD_PCB_Components.xlsx`](04_DOCS/KATARA-VD_PCB_Components.xlsx).

---

## Materials & Fabrication

| Part type | Material | Fabrication |
|---|---|---|
| Large flat panels (walls, base, shelves) | MDF | CNC laser cutting (`02_DXF/`) |
| Mechanisms & structural parts | ABS | FDM 3D printing |
| Covers & lightweight parts | PLA | FDM 3D printing |

| Setting | Value |
|---------|------|
| Layer Height | 0.20 mm |
| Nozzle | 0.4 mm |
| Infill | 20% |
| Walls | 3 |
| Supports | Only where needed |

---

## Fasteners

| Screw | Length | Quantity |
|-------|-------:|---------:|
| M3 | 20 mm | 40 |
| M3 | 30 mm | 40 |

**Total: to be finalized** — final counts will be filled in once the last assemblies are locked.

---

## CAD Files

Per subsystem: **native SolidWorks** source, **STEP** (any CAD tool), and **STL** (slicer-ready) under `01_3D/`, plus **DXF** flat-panel files for CNC laser cutting under `02_DXF/`.

---

## Simulations

<table>
<tr>
<td width="33%" align="center">

**Prescription mechanism**

<img src="05_MEDIA/SIMULATIONS/mechanism of prescription.gif" width="250">

Rotary-to-linear extension that presents the prescription to the RealSense camera.

</td>
<td width="33%" align="center">

**Giving money mechanism**

<img src="05_MEDIA/SIMULATIONS/mechanism of giving money.gif" width="250">

Rack-and-pinion coin ejection, sized to a 1-euro coin.

</td>
<td width="33%" align="center">

**Coin storage**

<img src="05_MEDIA/SIMULATIONS/GIF MEC PUSHING THE MONEY INTO THE BOX.gif" width="250">

Donated coins pushed securely into the storage box.

</td>
</tr>
<tr>
<td width="33%" align="center">

**Door actuation**

<img src="05_MEDIA/SIMULATIONS/mechanism for opening and closing door.gif" width="250">

Dual-actuator, hinge-guided access doors.

</td>
<td width="33%" align="center">

**JALOUL — Y-axis translation**

<img src="05_MEDIA/SIMULATIONS/translation of the robot on yy' axis.gif" width="250">

The backpack lift traveling along the Y-Y′ axis via lead screw.

</td>
<td width="33%" align="center">

**JALOUL — arm reach**

<img src="05_MEDIA/IMAGES/JALOUL in different positions.png" width="250">

Both arms swept across multiple positions, showing the range unlocked by the extra joints.

</td>
</tr>
</table>

---

## Future Improvements

-Faire un assemblage et imprimer les pièces  pour faire un petit prototype 
-ajoutez un drone pour transporter les médicaments du l'usine lorsque le stockage est vide

---

## License

**MIT License**.
