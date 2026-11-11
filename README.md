# Hi, I'm Tristan Dobrowney 👋

**Systems Engineer | Embedded Linux & Firmware | Hardware-Software Integration**

Computer Engineer (B.Sc., With Distinction, University of Manitoba, 2026) working on autonomous agricultural machinery at PTx Trimble, where I'm a Systems Engineer on the OutRun intelligence platform. I like owning a system end to end: schematic and board, microcontroller firmware, the Linux kernel and user space on top, and the tooling that ships it to a fleet.

Dual UK and Canadian citizen.

## 🔧 What I work on

- **Systems integration** of sensors, vision hardware, controllers and compute across harnessing, firmware, embedded Linux and ROS2
- **Embedded Linux** on NVIDIA Jetson: custom kernels, Kconfig, U-Boot/UEFI, systemd, SocketCAN, NetworkManager, Debian packaging and fleet updates
- **Firmware** for STM32 (Cortex-M) in C: USB drivers, interrupt-driven peripherals, FreeRTOS and bare metal
- **Vehicle networks**: CAN, J1939, ISOBUS, automotive Ethernet; DBC authoring in Vector CANdb++
- **Hardware design**: KiCad schematics and layouts, from power regulation to precision analog front ends
- **Developer tooling**: GitHub Actions CI with self-hosted and ephemeral runners, Docker, unit-test frameworks, hardware-in-the-loop test rigs
- **Agentic development**: daily use of Claude Code with multi-agent workflows, custom skills and MCP servers

## 🛠️ Skills

**Languages**: C • C++ • Python • C# • TypeScript/JavaScript • Verilog • Lua • Bash • SQL

**Embedded**: STM32, FreeRTOS, RP2350 (Pico 2), Arduino, NVIDIA Jetson, Raspberry Pi, FPGA (Altera DE-2, DE-10)

**Linux**: kernel configuration and builds, U-Boot/UEFI, systemd, Debian packaging, apt repositories, Docker, nginx, VPS administration

**Protocols**: CAN • J1939 • ISOBUS • Automotive Ethernet • USB • SPI • I2C • UART • MQTT

**Robotics & tooling**: ROS2 (Humble, Jazzy, ros2_control), MATLAB/Simulink, Vector CANdb++, KiCad, Altium, LaTeX

**Web & data**: Node.js (Express, Fastify, WebSockets), React/Vite, FastAPI, PostgreSQL, MariaDB, SQLite

## 🚀 Projects

### [Bot-Hoven](https://github.com/bot-hoven) - autonomous piano-playing robot
*Capstone project, IEEE Winnipeg Section 2nd Prize (2025)*

Wrote the ros2_control hardware-interface layer in C++: an I2C bus manager and SPI peripheral over Linux character devices, with PCA9685 servo, MCP23017 solenoid and CL42T stepper plugins driving 20+ actuators with sub-millisecond timing. Also the Raspberry Pi bring-up and the Pico 2 SPI-slave stepper firmware (one core per motor, PID). Batched I2C transactions cut bus overhead by 60%.

**Stack**: ROS2 Jazzy, ros2_control, C++17, Pico SDK, CMake, Docker on arm64

### Magnetic-field sensor data acquisition
*Undergraduate research, UManitoba Electromagnetic Imaging Lab (2025)*

Designed a four-board KiCad system for a three-channel research magnetometer: power regulation (±12 V, 5 V, 3.3 V, 1 V rails), stacked signal-conditioning boards with DAC-driven DC nulling and I2C-controlled gain, a MAX11040K ADC breakout (3 × 24 kSPS over SPI, GPS PPS sync), and a Raspberry Pi 5 carrier. Wrote the C++ acquisition code for the ADC, DAC, accelerometer and GPS.

**Stack**: KiCad, C++, SPI/I2C/UART, Raspberry Pi 5

### [TeaMate](https://github.com/DobrowneyT/teamate) - autonomous tea-making robot

A 3-DOF arm with inverse kinematics and PID control on an Arduino Mega 2560, sub-millimetre positioning from encoder feedback and auto-calibration, and five sensor types for a safe, collision-aware brewing sequence.

**Stack**: C++, Arduino

### [pagefetch](https://github.com/DobrowneyT/pagefetch) - browser-backed fetch service for agents

Self-hosted Chromium-in-Docker service that fetches pages plain HTTP can't, exposed over MCP and plain HTTP, with robots.txt enforced by default, a SQLite cache and server-side politeness caps. Specified as a PRD first; built with Claude Code.

**Stack**: TypeScript, Docker, MCP, SQLite

### [Faction dashboard](https://github.com/DobrowneyT/torn-dashboard) for an online game community

A multi-tenant web app I run for several player groups: Fastify API, WebSocket live updates, PostgreSQL with one database per tenant, and a Docker Compose stack on a VPS I administer. About 320 test files, CI on a self-hosted runner with changelog and lint gates. AI-assisted with Claude Code; I own the architecture, reviews and tests.

**Stack**: TypeScript, Node.js, React, PostgreSQL 17, Docker, nginx, systemd

### CAN trace plotter
*Internal tool, MacDon Industries*

PyQt6 desktop app that parses .trc/.asc/.bfl/.csv traces with DBC decoding, four simultaneous plots and statistics; shipped as an executable to the controls team.

**Stack**: Python, PyQt6

### 16-bit RISC processor
Parametrised single-cycle CPU in Verilog on an Altera DE-10 FPGA: full fetch/decode/execute/memory/write-back datapath with condition-code branching, with ALU, register file and memory widths set from one parameter.

## 🎯 Where I'm heading

Kernel development, and eventually computer architecture and instruction-set design. The processor project above is where that started.

## 🏆 Recognition

- IEEE Winnipeg Section 2nd Prize, capstone project (2025)
- Faculty of Engineering Undergraduate Research Award (2025)
- NSERC Undergraduate Student Research Award (2022)
- Dean's Honour List every term; graduated With Distinction (2026)

## 💡 Before engineering

I spent eight years as a professional dancer, including Soloist with Canada's Royal Winnipeg Ballet and Principal Dancer at the Lviv National Opera and Ballet, and eight years as the elected union representative for the RWB dancers. Touring taught me to debug under pressure and to keep the show running.

## 📫 Contact

- **Email**: dobrownt@myumanitoba.ca
- **LinkedIn**: [tristandobrowney](https://www.linkedin.com/in/tristandobrowney-68b3ba161)
- **Location**: Winnipeg, Canada
