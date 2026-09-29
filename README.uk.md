<p align="center">
  <a href="https://www.softeralab.com/">
    <img src="docs/assets/images/uk/logo.png" alt="Softera Lab" width="96">
  </a>
</p>

<h1 align="center">Tiny Light · SK-10</h1>

<p align="center"><strong>Набір Softera Lab — кишеньковий LED-ліхтарик · USB-C · CR2032</strong></p>

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

**Tiny Light · SK-10** — компактний набір Softera Lab для пайки: після збірки отримуєте кишеньковий LED-ліхтарик із сучасним портом **USB-C**, зарядним контролером **TP4054**, вимикачем **Switch**, кнопкою **Light** і світлодіодом **5 мм**.

Працює від **трьох джерел живлення**: **USB-C**, батарейки **CR2032** (у комплекті) або **акумулятора Li-ion / LiPo** на площадках **B(+) / B(−)**.

Це **сторінка продукту та інструкція**. Це **не open-source hardware** — Gerber і виробничі файли публічно не викладаються.

> © Softera Lab. All rights reserved.

## Як працює

<p align="center">
  <img src="docs/assets/images/uk/how-it-works.png" alt="Як працює Tiny Light" width="720"><br>
  <em>Шлях живлення: USB-C / батарея → Switch → кнопка Light → LED 5 мм</em>
</p>

1. **USB-C** — живлення від кабелю; зарядка через **TP4054 (U1)** з індикатором **CHARGE**  
2. **CR2032** — батарейка в тримачі на тилі (у комплекті)  
3. **Li-ion / LiPo** — опційний акумулятор на **B(+) / B(−)**  
4. **Switch** — увімкнення / вимкнення  
5. Кнопка **Light** — керування основним LED  
6. **LED (+ / −)** — наскрізний **5 мм** (слідкуйте за полярністю)  

<p align="center">
  <img src="docs/assets/images/uk/ready.png" alt="Зібраний Tiny Light" width="720"><br>
  <em>Зібраний Tiny Light із увімкненим основним LED</em>
</p>

## Джерела живлення

<p align="center">
  <img src="docs/assets/images/uk/power-sources.png" alt="Джерела живлення" width="720"><br>
  <em>USB-C · CR2032 · Li-ion — автоматичний Power-OR через діоди Шотткі D1/D2</em>
</p>

**D1 / D2** (SS14) дозволяють платі безпечно брати живлення від **USB-C**, **CR2032** або **акумулятора Li-ion** без зворотного струму між джерелами.

## Про набір

| Зона | Що отримуєте |
| --- | --- |
| **Світло** | Площадки LED **5 мм** з **+ / −** · **R1 220 Ω** (221) |
| **Керування** | Слайдер **Switch** · тактова кнопка **Light** |
| **Зарядка** | **USB-C** · **U1 TP4054** · **CHARGE** · **R2 1 кОм** · **R3 3 кОм** · **C1/C2 1 µF** |
| **Живлення** | **USB-C** · **CR2032** (у наборі) · опційний **Li-ion** на **B(+) / B(−)** |

Мікроконтролера немає — дискретна схема зарядки + вимикач + LED. Гайди: [`docs/`](docs/).

<p align="center">
  <img src="docs/assets/images/uk/board-front.png" alt="Лицьова сторона" width="720"><br>
  <em>Лицьова — USB-C, TP4054, Switch, кнопка Light, площадки LED</em>
</p>

<p align="center">
  <img src="docs/assets/images/uk/board-back.png" alt="Тильна сторона" width="720"><br>
  <em>Тильна — тримач CR2032 і маркування SofteraLab</em>
</p>

## Характеристики

| Параметр | Значення |
| --- | --- |
| Product | Tiny Light · **SK-10** |
| Порт зарядки | **USB-C** |
| Зарядний IC | **TP4054** (U1) |
| Захист | **D1 / D2** SS14 Schottky (Power-OR) |
| Джерела живлення | **USB-C** · **CR2032** · **Li-ion / LiPo** |
| Батарея в наборі | **CR2032** |
| Основний LED | Наскрізний **5 мм** |
| Керування | Слайдер + кнопка |
| МК | Немає |

## Що в наборі

<p align="center">
  <img src="docs/assets/images/uk/kit-contents.png" alt="Комплектація" width="720"><br>
  <em>14 деталей + 5 LED для практики</em>
</p>

**14 деталей** + **5 світлодіодів різних типів** (практика / запас), зокрема: плата **SK-10**, **USB-C**, **TP4054**, **R1–R3**, **C1/C2**, LED **CHARGE**, **Switch**, кнопка **Light**, тримач і елемент **CR2032**, основний LED **5 мм**.

## Збірка (коротко)

1. SMD **R1–R3**, **C1**, **C2**  
2. **U1 TP4054** і LED **CHARGE**  
3. **USB-C**  
4. **Switch** і кнопка **Light**  
5. Основний LED **5 мм** (**+ / −**)  
6. Тримач **CR2032** на тил · вставити елемент  
7. **Switch** увімк → **Light** → світить  

Повний порядок: [docs/02-getting-started.md](docs/02-getting-started.md).

## Навчальні картки

<p align="center">
  <img src="docs/assets/images/uk/component-map-clean-v1.png" alt="Карта компонентів" width="720"><br>
  <em>Карта компонентів — де що стоїть на платі</em>
</p>

<p align="center">
  <img src="docs/assets/images/uk/tp4054-diodes.png" alt="TP4054 і діоди" width="720"><br>
  <em>Розпіновка TP4054 і діоди Шотткі D1/D2 (Power-OR)</em>
</p>

<p align="center">
  <img src="docs/assets/images/uk/two-modes.png" alt="Два режими роботи" width="720"><br>
  <em>Два режими: Switch ON — постійне світло, або тримати KEY</em>
</p>

<p align="center">
  <img src="docs/assets/images/uk/usb-solder.png" alt="Пайка USB-C" width="720"><br>
  <em>Пайка роз’єму USB-C — порядок контактів</em>
</p>

<p align="center">
  <img src="docs/assets/images/uk/battery-wiring-fixed.png" alt="Підключення батареї" width="720"><br>
  <em>Підключення батареї — червоний до B(+), чорний до B(−)</em>
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
