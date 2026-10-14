<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:4cc9f0,100:06d6a0&height=140&section=header&text=Hey,%20I'm%20Ayush&fontSize=36&fontColor=ffffff&fontAlignY=38" width="100%"/>

<img src="./space-invaders.svg" alt="Space Invaders" width="720"/>

<a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=18&duration=3200&pause=1000&color=06D6A0&center=true&vCenter=true&width=640&lines=Computer+Engineering+%40+Toronto+Metropolitan+University;Embedded+firmware+%7C+FPGA+%7C+Robotics+%7C+Test+automation;I+build+things+that+run+on+real+hardware" alt="Typing SVG" /></a>

<br>

[![Email](https://img.shields.io/badge/Email-sehijpalayush%40gmail.com-0b0f1a?style=for-the-badge&logo=gmail&logoColor=4cc9f0)](mailto:sehijpalayush@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Ayush%20Sehijpal-0b0f1a?style=for-the-badge&logo=linkedin&logoColor=4cc9f0)](https://www.linkedin.com/in/ayush-sehijpal)

</div>

<br>

## About me

I'm a Computer Engineering student at **TMU** (graduating May 2028) who likes working close to the metal: writing firmware, designing CPUs in Verilog, and making sensors, rovers and receivers behave in the real world. Most of my work sits where hardware meets software, and I care about making it **verified, reliable and repeatable**.

- 🛰️ **Now:** Software Engineer Intern at **Trimble (Applanix)**, building hardware-in-the-loop validation for high-precision GNSS/INS receivers
- 🚀 **Also:** Avionics firmware at **MetRocketry** and autonomous systems at **T.A.S.C.**
- 🔧 **Tinkering with:** RISC-V, SoC design, sensor fusion, ROS 2, and CI for embedded systems
- 📍 Toronto, ON

<br>

## What I'm working on

| Where | Role | What I do |
|---|---|---|
| **Trimble (Applanix)** | Software Engineer Intern, Embedded Hardware Validation | Python hardware-in-the-loop framework that streams every GNSS/INS sensor-output message over TCP at 1 Hz and reports PASS/FAIL/SKIP to GitLab CI. Built a YAML-backed test-applicability engine covering **224 test IDs and 896 configuration decisions**, and root-caused a binary-protocol framing bug that misdecoded stale packets as valid responses. |
| **MetRocketry** | Software Engineer, Avionics & Firmware | Real-time C++ on a **Teensy 4.0** fusing IMU, barometer, GPS and current sensing across 4 concurrent SPI/I2C streams. Extended Kalman Filter with all matrix math written from scratch, and a fault-tolerant logger that kept **100% of telemetry** across test launches. |
| **T.A.S.C.** | Software Developer, Autonomous Systems | ROS 2 perception and GPS nodes on an **NVIDIA Jetson** rover, tested at **CIRC 2026**. Took a vision pipeline from ~3 FPS to **30 FPS** with a lock-protected multithreaded frame grabber. |

<br>

## Featured projects

### 🕹️ RV32I Starflight: RISC-V SoC and a playable VGA game on FPGA
`Verilog` `C` `Quartus` `Questa` `SDC` `Intel MAX 10`

A single-cycle **RV32I CPU** designed in Verilog (25+ instructions) inside a 9-region memory-mapped SoC, with bare-metal C firmware driving a framebuffer-free 640×480 VGA renderer and an SPI accelerometer for tilt controls. Runs on a physical DE10-Lite board.

| Metric | Result |
|---|---|
| Timing | **80.19 MHz Fmax** vs. a 50 MHz constraint (+7.53 ns setup / +0.34 ns hold) |
| Area | 1,885 logic elements (**3.8%** of a MAX 10 10M50), 191 registers, 1 PLL |
| Verification | Self-checking Questa testbenches (CPU regression + VGA), **0 errors, 0 warnings** |
| Build | PowerShell flows driving `quartus_sh`, checking exit codes and confirming `.sof` generation |

### 🛰️ MARS Rocket Avionics PCB
`KiCad` `ESP32` `C++` `I2C/UART` `MATLAB`

A full flight avionics board in KiCad: an ESP32 with MPU6050 IMU, BN-220 GPS, BME280 barometer and BH1750 light sensor. Custom C++ firmware, a live 3D rocket-position visualization on OpenStreetMap terrain, and MATLAB nosecone drag optimization (`fminbnd` across elliptical, ogive, parabolic and Haack profiles).

### 🧠 8-bit Microcoded Processor
`Verilog` `VHDL` `Altera FPGA`

An 8-bit CPU built from scratch: 16-operation ALU, 4×16 decoder, register file, microcoded control and a 9-state FSM. Verified with Quartus waveforms and on-board testing.

### 💊 Prescription Tracker
`Python` `PyTorch` `YOLOv8` `OpenCV` `Django` `MySQL` `OpenAI API`

A YOLOv8 model trained from scratch in PyTorch with custom OpenCV preprocessing, reaching **95% extraction accuracy** on unstructured image/PDF inputs. Includes an LLM query layer behind a Django REST API.

### 🏆 More
- 🥇 [**Fair Game**](https://github.com/SourCream206/FairGame---Solution-Hacks): student-mentor matching platform (React, Node.js, Supabase). **1st place at Lunaris Hacks**, built in 24 hours.
- ✈️ [**Bon Voyage**](https://github.com/SourCream206/BonVoyage---McHacks12): LLM-powered travel planner (McHacks 12).
- 🤖 [**jojoBot**](https://github.com/SourCream206/jojoBot): event-driven Discord RPG in Python with Supabase persistence, 50+ commits.
- 🌍 [**Terrahacks 2024**](https://github.com/t4ttc/terrahacks): hackathon project (JavaScript).

<br>

## Tech stack

**Digital design and verification**

![Verilog](https://img.shields.io/badge/Verilog-0b0f1a?style=flat-square&logo=v&logoColor=4cc9f0)
![VHDL](https://img.shields.io/badge/VHDL-0b0f1a?style=flat-square&logoColor=4cc9f0)
![RISC-V](https://img.shields.io/badge/RISC--V-0b0f1a?style=flat-square&logo=riscv&logoColor=4cc9f0)
![Quartus](https://img.shields.io/badge/Quartus-0b0f1a?style=flat-square&logo=intel&logoColor=4cc9f0)
![Questa](https://img.shields.io/badge/Questa%20%2F%20ModelSim-0b0f1a?style=flat-square&logoColor=4cc9f0)
![STA](https://img.shields.io/badge/Static%20Timing%20Analysis-0b0f1a?style=flat-square&logoColor=4cc9f0)

**Embedded and hardware**

![C](https://img.shields.io/badge/C-0b0f1a?style=flat-square&logo=c&logoColor=4cc9f0)
![C++](https://img.shields.io/badge/C++-0b0f1a?style=flat-square&logo=cplusplus&logoColor=4cc9f0)
![Teensy](https://img.shields.io/badge/Teensy%204.0-0b0f1a?style=flat-square&logo=arduino&logoColor=4cc9f0)
![ESP32](https://img.shields.io/badge/ESP32-0b0f1a?style=flat-square&logo=espressif&logoColor=4cc9f0)
![KiCad](https://img.shields.io/badge/KiCad-0b0f1a?style=flat-square&logo=kicad&logoColor=4cc9f0)
![SPI/I2C/UART](https://img.shields.io/badge/SPI%20%7C%20I2C%20%7C%20UART-0b0f1a?style=flat-square&logoColor=4cc9f0)

**Robotics, test automation and tooling**

![Python](https://img.shields.io/badge/Python-0b0f1a?style=flat-square&logo=python&logoColor=4cc9f0)
![ROS 2](https://img.shields.io/badge/ROS%202-0b0f1a?style=flat-square&logo=ros&logoColor=4cc9f0)
![Jetson](https://img.shields.io/badge/NVIDIA%20Jetson-0b0f1a?style=flat-square&logo=nvidia&logoColor=4cc9f0)
![OpenCV](https://img.shields.io/badge/OpenCV-0b0f1a?style=flat-square&logo=opencv&logoColor=4cc9f0)
![PyTorch](https://img.shields.io/badge/PyTorch-0b0f1a?style=flat-square&logo=pytorch&logoColor=4cc9f0)
![GitLab CI](https://img.shields.io/badge/GitLab%20CI-0b0f1a?style=flat-square&logo=gitlab&logoColor=4cc9f0)
![Docker](https://img.shields.io/badge/Docker-0b0f1a?style=flat-square&logo=docker&logoColor=4cc9f0)
![Linux](https://img.shields.io/badge/Linux-0b0f1a?style=flat-square&logo=linux&logoColor=4cc9f0)
![Bash](https://img.shields.io/badge/Bash%20%7C%20PowerShell-0b0f1a?style=flat-square&logo=gnubash&logoColor=4cc9f0)

**Web and data (when the project needs it)**

![React](https://img.shields.io/badge/React-0b0f1a?style=flat-square&logo=react&logoColor=4cc9f0)
![Node](https://img.shields.io/badge/Node.js-0b0f1a?style=flat-square&logo=nodedotjs&logoColor=4cc9f0)
![Django](https://img.shields.io/badge/Django-0b0f1a?style=flat-square&logo=django&logoColor=4cc9f0)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-0b0f1a?style=flat-square&logo=postgresql&logoColor=4cc9f0)
![MySQL](https://img.shields.io/badge/MySQL-0b0f1a?style=flat-square&logo=mysql&logoColor=4cc9f0)

<br>

## GitHub stats

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=SourCream206&show_icons=true&theme=onedark&hide_border=true&bg_color=0b0f1a&title_color=4cc9f0&icon_color=06d6a0&count_private=true" />
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=SourCream206&theme=onedark&hide_border=true&bg_color=0b0f1a&title_color=4cc9f0&layout=compact&count_private=true" />

</div>

<br>

<div align="center">

*Currently looking for opportunities in embedded systems, firmware, FPGA/digital design and robotics.*

[![Email](https://img.shields.io/badge/Say%20hi-sehijpalayush%40gmail.com-0b0f1a?style=for-the-badge&logo=gmail&logoColor=06d6a0)](mailto:sehijpalayush@gmail.com)

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:06d6a0,100:4cc9f0&height=100&section=footer" width="100%"/>

</div>
