<p align="left"><img alt="OSPTEK" src="./images/logo.png" width="200" /></p>

<h1 align="center">OSPTEK 10.1″ TFT 800×1280 (JD9366 · MIPI)</h1>

<p align="center"><b>Touch TFT module · MIPI DSI · JD9366</b></p>

<p align="center"><a href="./README.md">简体中文</a> | English · <a href="../../README_EN.md">Family index</a></p>

<p align="center">
  <img alt="Size: 10.1 inch" src="https://img.shields.io/badge/Size-10.1%22-3498DB?style=flat-square" />
  <img alt="Resolution: 800x1280" src="https://img.shields.io/badge/Resolution-800%C3%971280-8E44AD?style=flat-square" />
  <img alt="Interface: MIPI" src="https://img.shields.io/badge/Interface-MIPI-27AE60?style=flat-square" />
  <img alt="Driver: JD9366" src="https://img.shields.io/badge/Driver-JD9366-E7352C?style=flat-square" />
</p>

## Contents

- [Overview](#overview)
- [Specifications](#specifications)
- [Sample projects](#sample-projects)
- [Repository layout](#repository-layout)
- [Resources](#resources)
- [Buy](#buy)
- [Support](#support)

---

## Overview

OSPTEK **10.1″ 800×1280 TFT** is an **IPS** color display module with **MIPI DSI**, driven by **JD9366**. The FPC exposes capacitive-touch I2C (TP-SCL / TP-SDA / TP-INT / TP-RST); the datasheet does not name the touch IC.

Spec ID (repository name): `tft-10.1-800x1280-mipi-jd9366`

Current module version: **YDP1010BT003-V1**. Electrical and mechanical details follow [`docs/YDP1010BT003-V1.pdf`](./docs/YDP1010BT003-V1.pdf).

## Specifications

| Item | Spec |
| ---- | ---- |
| Size | 10.1 inch |
| Type | TFT / IPS (color) |
| Resolution | 800×1280 |
| Interface | MIPI DSI |
| Driver IC | JD9366 |
| Touch | Capacitive (I2C; IC not named in the datasheet) |
| FPC | 45-pin |
| Module size | 140.36 × 226.96 × 2.37 mm |
| Active area | 135.36 × 216.58 mm |
| Luminance | 350 cd/m² (typ.) |
| Contrast | 1500 |
| Operating temperature | −10 ~ +50 ℃ |

> Full outline, FPC definition, power, and timing follow the product datasheet / driver IC datasheet.

## Sample projects

These samples are shared with family SKU **YDP1010BT006-V1**.

| Description | Path |
| ---- | ---- |
| ESP32-P4 · JD9366 MIPI + esp-lvgl-port / LVGL9 | [`examples/esp32p4-idf5_jd9366-mipi_esp-lvgl-port_lvgl9/`](./examples/esp32p4-idf5_jd9366-mipi_esp-lvgl-port_lvgl9/) |
| ESP32-P4 · JD9366 MIPI + PPA landscape / LVGL9 | [`examples/esp32p4-idf5_jd9366-mipi_esp-lvgl-port_lvgl9_ppa/`](./examples/esp32p4-idf5_jd9366-mipi_esp-lvgl-port_lvgl9_ppa/) |
| ESP32-P4 v3.2 · ESP-IDF 6.1 · JD9366 MIPI + LVGL 9 | [`examples/esp32p4-idf6_jd9366-mipi_esp-lvgl-port_lvgl9/`](./examples/esp32p4-idf6_jd9366-mipi_esp-lvgl-port_lvgl9/) |
| ESP32-P4 v3.2 · ESP-IDF 6.1 · JD9366 MIPI + PPA landscape / LVGL 9 | [`examples/esp32p4-idf6_jd9366-mipi_esp-lvgl-port_lvgl9_ppa/`](./examples/esp32p4-idf6_jd9366-mipi_esp-lvgl-port_lvgl9_ppa/) |
| Raspberry Pi 5 · JD9366 800×1280 panel / DT overlay (display only) | [`examples/rpi5-panel-jd9366-800x1280/`](./examples/rpi5-panel-jd9366-800x1280/) |
| Raspberry Pi 5 · JD9366 display + touch / DT overlay | [`examples/rpi5-panel-jd9366-touch-800x1280/`](./examples/rpi5-panel-jd9366-touch-800x1280/) |
| Raspberry Pi 5 · JD9366 display + touch · LVGL (DRM + EVDEV) | [`examples/rpi5-lvgl-jd9366-touch-800x1280/`](./examples/rpi5-lvgl-jd9366-touch-800x1280/) |

## Repository layout

```text
tft-10.1-800x1280-mipi-jd9366/                                # repo root (nav: ../../README_EN.md)
└── versions/
    └── YDP1010BT003-V1/                                # full materials for this part number
        ├── README.md
        ├── README_EN.md
        ├── images/
        ├── docs/
        └── examples/
```

## Resources

### Product materials

| Document | Link |
| -------- | ---- |
| Product datasheet (YDP1010BT003-V1) | [`docs/YDP1010BT003-V1.pdf`](./docs/YDP1010BT003-V1.pdf) |
| Driver IC datasheet (JD9366) | [`docs/JD9366TC_DS_V0.01_20220426.pdf`](./docs/JD9366TC_DS_V0.01_20220426.pdf) |

### Sample projects

- [ESP32-P4 JD9366 MIPI + LVGL9](./examples/esp32p4-idf5_jd9366-mipi_esp-lvgl-port_lvgl9/)
- [ESP32-P4 JD9366 MIPI + PPA landscape / LVGL9](./examples/esp32p4-idf5_jd9366-mipi_esp-lvgl-port_lvgl9_ppa/)
- [ESP32-P4 v3.2 · ESP-IDF 6.1 · JD9366 MIPI + LVGL 9](./examples/esp32p4-idf6_jd9366-mipi_esp-lvgl-port_lvgl9/)
- [ESP32-P4 v3.2 · ESP-IDF 6.1 · JD9366 MIPI + PPA landscape / LVGL 9](./examples/esp32p4-idf6_jd9366-mipi_esp-lvgl-port_lvgl9_ppa/)
- [Raspberry Pi 5 JD9366 panel (display only)](./examples/rpi5-panel-jd9366-800x1280/)
- [Raspberry Pi 5 JD9366 display + touch](./examples/rpi5-panel-jd9366-touch-800x1280/)
- [Raspberry Pi 5 JD9366 display + touch · LVGL](./examples/rpi5-lvgl-jd9366-touch-800x1280/)

## Buy

<p align="center">
  <a href="https://www.aliexpress.com/store/1105701619"><img alt="AliExpress Official Store" src="https://img.shields.io/badge/AliExpress-Official_Store-E62E04?style=for-the-badge&logo=aliexpress&logoColor=white" /></a>
  &nbsp;&nbsp;
  <a href="https://shop110742373.taobao.com/"><img alt="Taobao Official Store" src="https://img.shields.io/badge/Taobao-Official_Store-FF6A00?style=for-the-badge" /></a>
</p>

**International (AliExpress)**

- Store: [OSPTEK Official Store](https://www.aliexpress.com/store/1105701619)

**China (Taobao)**

- Store: [鱼鹰光电工厂店](https://shop110742373.taobao.com/)

## Support

- Technical Support / Sales: <luyu@osptek.com>
- QQ Technical Group: **985881096**
- Website: <https://osptek.com/>
- Feel free to open an Issue in this repository if you have any questions

---

<p align="center"><sub>© 2026 OSPTEK · Licensed under CC BY 4.0</sub></p>
