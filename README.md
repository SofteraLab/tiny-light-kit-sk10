<p align="center">
  <a href="https://www.softeralab.com/">
    <img src="docs/assets/images/en/logo.png" alt="Softera Lab" width="96">
  </a>
</p>

<h1 align="center">Tiny Light · SK-10</h1>

<p align="center"><strong>Softera Lab soldering kit — pocket LED light · USB-C charge · CR2032</strong></p>

<p align="center">
  <a href="README.uk.md"><img alt="UA" src="https://img.shields.io/badge/UA-README.uk.md-F97316?style=flat-square"></a>
  <a href="https://www.softeralab.com/"><img alt="Website" src="https://img.shields.io/badge/softeralab.com-09090B?style=flat-square&labelColor=18181B"></a>
  <a href="https://www.instagram.com/softeralab/"><img alt="Instagram" src="https://img.shields.io/badge/Instagram-09090B?style=flat-square&labelColor=18181B"></a>
  <a href="https://www.youtube.com/@SofteraLab"><img alt="YouTube" src="https://img.shields.io/badge/YouTube-09090B?style=flat-square&labelColor=18181B"></a>
  <img alt="USB-C" src="https://img.shields.io/badge/USB--C-charge-09090B?style=flat-square&labelColor=F97316">
</p>

<p align="center"><strong>Languages:</strong> English (this page) · <a href="README.uk.md">Українська</a></p>

<p align="center">
  <img src="docs/assets/images/en/banner.png" alt="Tiny Light SK-10" width="720">
</p>

**Tiny Light · SK-10** is a compact Softera Lab soldering kit: after assembly you get a small LED light with a **USB-C** charge port, **TP4054** charge IC, power **Switch**, **Light** button, and a **5 mm** LED.

It can run from **three power sources**: **USB-C**, a **CR2032** coin cell (included), or a **Li-ion / LiPo** pack on pads **B(+) / B(−)**.

This repository is a **product page and assembly guide**. It is **not open-source hardware** — Gerbers and manufacturing files are not published.

> © Softera Lab. All rights reserved.

## How it works

<p align="center">
  <img src="docs/assets/images/en/how-it-works.png" alt="How Tiny Light works" width="720">
</p>

1. **USB-C** — power from the cable and charge path via **TP4054 (U1)**; **CHARGE** LED shows charging  
2. **CR2032** — coin cell (included) in the back holder  
3. **Li-ion / LiPo** — optional pack on **B(+) / B(−)**  
4. **Switch** — power on / off  
5. **Light** button — control the main LED  
6. **LED (+ / −)** — through-hole **5 mm** lamp (observe polarity)  

<p align="center">
  <img src="docs/assets/images/en/ready.png" alt="Assembled Tiny Light" width="720">
</p>

## Power protection

<p align="center">
  <img src="docs/assets/images/en/protection.png" alt="USB-C diodes CR2032 protection" width="720">
</p>

Protection diodes (**D1 / D2**, Schottky **SS14**) form a **Power-OR**: the light can take power from **USB-C**, the **CR2032** cell, or a **Li-ion** pack, with reverse-current protection so the sources stay safe together.

<p align="center">
  <img src="docs/assets/images/en/schematic-block.png" alt="Schematic snippet — charge and protection" width="720">
</p>

Schematic snippet: **USB-C → D1/D2 → TP4054 → battery**, plus **Switch / Light** and the main LED with **R1 220 Ω**.

## About the kit

| Zone | What you get |
| --- | --- |
| **Light** | 5 mm LED pads with **+ / −** · current limit **R1 220 Ω** (221) |
| **Controls** | Slide **Switch** · tactile **Light** button |
| **Charge** | **USB-C** · **U1 TP4054** · **CHARGE** · **R2 1 kΩ** · **R3 3 kΩ** · **C1/C2 1 µF** |
| **Power** | **USB-C** · **CR2032** (kit) · optional **Li-ion** on **B(+) / B(−)** |
| **Practice** | Mix of SMD passives, charge IC, USB-C, button, switch, THT LED |

There is **no microcontroller** — discrete charge + switch + LED circuit.

Step-by-step: [`docs/en/`](docs/en/).

<p align="center">
  <img src="docs/assets/images/en/board-front.png" alt="Front — Tiny Light footprints" width="720">
</p>

<p align="center">
  <img src="docs/assets/images/en/board-back.png" alt="Back — CR2032 and SofteraLab" width="720">
</p>

## Specifications

| Parameter | Value |
| --- | --- |
| Product | Tiny Light · **SK-10** |
| Charge port | **USB-C** only |
| Charge IC | **TP4054** (U1) |
| Protection | **D1 / D2** SS14 Schottky (Power-OR) |
| Power sources | **USB-C** · **CR2032** · **Li-ion / LiPo** on **B(+) / B(−)** |
| Battery in kit | **CR2032** |
| Main LED | Through-hole **5 mm** |
| Controls | Slide switch + push button |
| MCU | None |

## What's in the kit

<p align="center">
  <img src="docs/assets/images/en/kit-contents.png" alt="Kit contents" width="720">
</p>

**14 parts** + **5 LEDs of different types** (practice / spare).

Includes among the 14:

1. Tiny Light PCB (**SK-10**)  
2. **USB-C** connector  
3. Charge IC **TP4054** (U1)  
4. Resistors **R1 220 Ω** · **R2 1 kΩ** · **R3 3 kΩ** (codes 221 / 102 / 302)  
5. Capacitors **C1 · C2** — **1 µF** each  
6. **CHARGE** indicator LED  
7. Slide **Switch**  
8. Tactile **Light** button  
9. **CR2032** holder  
10. **CR2032** cell  
11. Main **5 mm** LED and the rest of the packed **14-piece** set  

Plus **5 different LEDs** for experiments and polarity practice.

## Assembly (short)

1. Solder SMD passives **R1–R3**, **C1**, **C2**  
2. Solder **U1 TP4054** and **CHARGE** LED  
3. Solder **USB-C**  
4. Solder **Switch** and **Light** button  
5. Solder the main **5 mm** LED (**+ / −**)  
6. Mount **CR2032** holder on the back · insert cell  
7. Power **Switch** on → press **Light** → LED on  

Full order: [docs/en/02-getting-started.md](docs/en/02-getting-started.md).

## Learning cards

<p align="center">
  <img src="docs/assets/images/en/component-map-clean-v1.png" alt="Component map" width="720">
</p>

<p align="center">
  <img src="docs/assets/images/en/tp4054-diodes.png" alt="TP4054 and diodes D1/D2" width="720">
</p>

<p align="center">
  <img src="docs/assets/images/en/power-sources.png" alt="Power sources" width="720">
</p>

<p align="center">
  <img src="docs/assets/images/en/what-is-diode.png" alt="What is a diode" width="720">
</p>

<p align="center">
  <img src="docs/assets/images/en/two-modes.png" alt="Two operating modes" width="720">
</p>

<p align="center">
  <img src="docs/assets/images/en/usb-solder.png" alt="Soldering USB-C" width="720">
</p>

<p align="center">
  <img src="docs/assets/images/en/battery-wiring-fixed.png" alt="Battery wiring" width="720">
</p>

## Guides

| Guide | Link |
| --- | --- |
| Hardware overview | [docs/en/01-hardware-overview.md](docs/en/01-hardware-overview.md) |
| Getting started | [docs/en/02-getting-started.md](docs/en/02-getting-started.md) |
| Soldering | [docs/en/03-soldering.md](docs/en/03-soldering.md) |
| Troubleshooting | [docs/en/04-troubleshooting.md](docs/en/04-troubleshooting.md) |

## Links

| | |
| --- | --- |
| Website | [softeralab.com](https://www.softeralab.com/) |
| Soldering course | [course page](https://www.softeralab.com/course-basic-soldering/) |
| Contact | [Contacts](https://www.softeralab.com/our-contacts/) · support@softeralab.com |
| Instagram | [instagram.com/softeralab](https://www.instagram.com/softeralab/) |
| YouTube | [YouTube @SofteraLab](https://www.youtube.com/@SofteraLab) |

---

© Softera Lab. All rights reserved. See [COPYRIGHT.md](COPYRIGHT.md).
