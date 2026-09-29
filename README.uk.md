<p align="center">
  <a href="https://www.softeralab.com/">
    <img src="docs/assets/images/uk/logo.png" alt="Softera Lab" width="96">
  </a>
</p>

<h1 align="center">Tiny Light · SK-10</h1>

<p align="center"><strong>Набір Softera Lab — кишеньковий LED-ліхтарик · зарядка USB-C · CR2032</strong></p>

<p align="center">
  <a href="README.md"><img alt="EN" src="https://img.shields.io/badge/EN-README.md-F97316?style=flat-square"></a>
  <a href="https://www.softeralab.com/"><img alt="Сайт" src="https://img.shields.io/badge/softeralab.com-09090B?style=flat-square&labelColor=18181B"></a>
  <a href="https://www.instagram.com/softeralab/"><img alt="Instagram" src="https://img.shields.io/badge/Instagram-09090B?style=flat-square&labelColor=18181B"></a>
  <a href="https://www.youtube.com/@SofteraLab"><img alt="YouTube" src="https://img.shields.io/badge/YouTube-09090B?style=flat-square&labelColor=18181B"></a>
  <img alt="USB-C" src="https://img.shields.io/badge/USB--C-зарядка-09090B?style=flat-square&labelColor=F97316">
</p>

<p align="center"><strong>Мови:</strong> <a href="README.md">English</a> · Українська (ця сторінка)</p>

<p align="center">
  <img src="docs/assets/images/uk/banner.png" alt="Tiny Light SK-10" width="720">
</p>

**Tiny Light · SK-10** — компактний набір Softera Lab для пайки: після збірки отримуєте маленький LED-ліхтарик із портом **USB-C**, зарядним контролером **TP4054**, вимикачем **Switch**, кнопкою **Light** і світлодіодом **5 мм**.

Може працювати від **трьох джерел живлення**: **USB-C**, батарейки **CR2032** (у комплекті) або **акумулятора Li-ion / LiPo** на площадках **B(+) / B(−)**.

Це **сторінка продукту та інструкція**. Це **не open-source hardware** — Gerber і виробничі файли публічно не викладаються.

> © Softera Lab. All rights reserved.

## Як працює

<p align="center">
  <img src="docs/assets/images/uk/how-it-works.png" alt="Як працює Tiny Light" width="720">
</p>

1. **USB-C** — живлення від кабелю та шлях зарядки через **TP4054 (U1)**; індикатор **CHARGE**  
2. **CR2032** — батарейка (у комплекті) у тримачі на тилі  
3. **Li-ion / LiPo** — опційний акумулятор на **B(+) / B(−)**  
4. **Switch** — увімкнення / вимкнення  
5. Кнопка **Light** — керування основним LED  
6. **LED (+ / −)** — наскрізний **5 мм** (слідкуйте за полярністю)  

<p align="center">
  <img src="docs/assets/images/uk/ready.png" alt="Зібраний Tiny Light" width="720">
</p>

## Захист живлення

<p align="center">
  <img src="docs/assets/images/uk/protection.png" alt="Захист USB-C · діоди · CR2032" width="720">
</p>

Захисні діоди (**D1 / D2**, Schottky **SS14**) утворюють **Power-OR**: ліхтарик може брати живлення від **USB-C**, батарейки **CR2032** або **акумулятора Li-ion**, зі захистом від зворотного струму — щоб джерела працювали безпечно разом.

<p align="center">
  <img src="docs/assets/images/uk/schematic-block.png" alt="Фрагмент схеми — зарядка і захист" width="720">
</p>

Фрагмент схеми: **USB-C → D1/D2 → TP4054 → батарея**, плюс **Switch / Light** і основний LED з **R1 220 Ω**.

## Про набір

| Зона | Що отримуєте |
| --- | --- |
| **Світло** | Площадки LED **5 мм** з **+ / −** · обмежувач **R1 220 Ω** (221) |
| **Керування** | Слайдер **Switch** · тактова кнопка **Light** |
| **Зарядка** | **USB-C** · **U1 TP4054** · **CHARGE** · **R2 1 кОм** · **R3 3 кОм** · **C1/C2 1 µF** |
| **Живлення** | **USB-C** · **CR2032** (у наборі) · опційний **Li-ion** на **B(+) / B(−)** |
| **Практика** | SMD-пасиви, зарядний IC, USB-C, кнопка, вимикач, THT LED |

**Мікроконтролера немає** — дискретна схема зарядки + вимикач + LED.

Покроково: [`docs/`](docs/).

<p align="center">
  <img src="docs/assets/images/uk/board-front.png" alt="Лицьова — площадки Tiny Light" width="720">
</p>

<p align="center">
  <img src="docs/assets/images/uk/board-back.png" alt="Тильна — CR2032 і SofteraLab" width="720">
</p>

## Характеристики

| Параметр | Значення |
| --- | --- |
| Product | Tiny Light · **SK-10** |
| Порт зарядки | лише **USB-C** |
| Зарядний IC | **TP4054** (U1) |
| Захист | **D1 / D2** SS14 Schottky (Power-OR) |
| Джерела живлення | **USB-C** · **CR2032** · **Li-ion / LiPo** на **B(+) / B(−)** |
| Батарея в наборі | **CR2032** |
| Основний LED | Наскрізний **5 мм** |
| Керування | Слайдер + кнопка |
| МК | Немає |

## Що в наборі

<p align="center">
  <img src="docs/assets/images/uk/kit-contents.png" alt="Комплектація" width="720">
</p>

**14 деталей** + **5 світлодіодів різних типів** (практика / запас).

Серед 14 позицій:

1. Плата Tiny Light (**SK-10**)  
2. Роз’єм **USB-C**  
3. Зарядний IC **TP4054** (U1)  
4. Резистори **R1 220 Ω** · **R2 1 кОм** · **R3 3 кОм** (коди 221 / 102 / 302)  
5. Конденсатори **C1 · C2** — по **1 µF**  
6. Індикатор **CHARGE**  
7. Слайдер **Switch**  
8. Кнопка **Light**  
9. Тримач **CR2032**  
10. Елемент **CR2032**  
11. Основний LED **5 мм** і решта з комплекту **14 деталей**  

Плюс у коробці **5 різних LED** для експериментів і тренування полярності.

## Збірка (коротко)

1. Припаяйте SMD **R1–R3**, **C1**, **C2**  
2. Припаяйте **U1 TP4054** і LED **CHARGE**  
3. Припаяйте **USB-C**  
4. Припаяйте **Switch** і кнопку **Light**  
5. Припаяйте основний LED **5 мм** (**+ / −**)  
6. Встановіть тримач **CR2032** на тил · вставте елемент  
7. **Switch** увімк → **Light** → світить  

Повний порядок: [docs/02-getting-started.md](docs/02-getting-started.md).

## Навчальні картки

<p align="center">
  <img src="docs/assets/images/uk/component-map-clean-v1.png" alt="Карта компонентів" width="720">
</p>

<p align="center">
  <img src="docs/assets/images/uk/tp4054-diodes.png" alt="TP4054 і діоди D1/D2" width="720">
</p>

<p align="center">
  <img src="docs/assets/images/uk/power-sources.png" alt="Джерела живлення" width="720">
</p>

<p align="center">
  <img src="docs/assets/images/uk/what-is-diode.png" alt="Що таке діод" width="720">
</p>

<p align="center">
  <img src="docs/assets/images/uk/two-modes.png" alt="Два режими роботи" width="720">
</p>

<p align="center">
  <img src="docs/assets/images/uk/usb-solder.png" alt="Пайка USB-C" width="720">
</p>

<p align="center">
  <img src="docs/assets/images/uk/battery-wiring-fixed.png" alt="Підключення батареї" width="720">
</p>

## Інструкції

| Гайд | Посилання |
| --- | --- |
| Огляд плати | [docs/01-hardware-overview.md](docs/01-hardware-overview.md) |
| Старт | [docs/02-getting-started.md](docs/02-getting-started.md) |
| Пайка | [docs/03-soldering.md](docs/03-soldering.md) |
| Пошук несправностей | [docs/04-troubleshooting.md](docs/04-troubleshooting.md) |

## Посилання

| | |
| --- | --- |
| Сайт | [softeralab.com](https://www.softeralab.com/) |
| Курс пайки | [сторінка курсу](https://www.softeralab.com/course-basic-soldering/) |
| Контакт | [Контакти](https://www.softeralab.com/our-contacts/) · support@softeralab.com |
| Instagram | [instagram.com/softeralab](https://www.instagram.com/softeralab/) |
| YouTube | [YouTube @SofteraLab](https://www.youtube.com/@SofteraLab) |

---

© Softera Lab. All rights reserved. Див. [COPYRIGHT.md](COPYRIGHT.md).
