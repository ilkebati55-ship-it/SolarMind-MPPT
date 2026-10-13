# SolarMind-MPPT
Firmware code, circuit schematics, and experimental datasets for SolarMind smart solar optimizer.
# SolarMind-MPPT ☀️🔋

Microcontroller-based Maximum Power Point Tracking (MPPT) firmware and experimental analysis framework designed to optimize solar panel efficiency under dynamic partial-shading conditions.

---

## 📋 Project Overview
SolarMind is developed as a low-cost, high-efficiency smart solar power optimizer targeted for high school research competitions (such as TÜBİTAK 2204-A). This repository contains the firmware, sensor calibration scripts, and data collection pipelines.

- **Research Question:** Can a low-cost microcontroller-based MPPT controller significantly improve power output from a small solar panel under rapidly changing partial-shading conditions compared to a baseline fixed operating point?
- **Field:** Electrical Engineering / Power Electronics / Renewable Energy

---

## 🛠 Hardware Architecture & Components
- **Microcontroller:** ESP32 / Arduino development board
- **Solar Panel:** 10W–20W monocrystalline photovoltaic panel
- **Current/Voltage Sensors:** INA219 / INA226 high-precision bi-directional current/power monitors
- **Power Electronics:** Custom DC-DC converter topology with adjustable duty cycle PWM control
- **Environmental Sensors:** Light intensity and temperature sensors

---

## 💻 Software & Algorithms
- **Firmware Language:** C / C++ (Arduino IDE / PlatformIO)
- **Control Algorithm:** Perturb & Observe (P&O) MPPT algorithm combined with adaptive step-size tracking.
- **Data Logging:** Real-time serial data streaming formatted for automated logging during experimental trials.

---

## 📊 Experimental Methodology
1. **Controlled Testing:** Performed 200+ controlled trials under 5–10 distinct partial-shading configurations.
2. **Data Metrics Captured:** Voltage, current, instantaneous power, panel temperature, convergence time, and total cumulative energy yield.
3. **Statistical Analysis:** Python scripts utilizing `Pandas` and `Matplotlib` for comparative performance visualization and error analysis.

---

## 📂 Repository Structure
- `/firmware` -> C/C++ source code for MPPT control and sensor polling
- `/data` -> Experimental CSV datasets and performance logs
- `/analysis` -> Python analysis scripts and generated graphs
- `/schematics` -> Circuit diagrams and hardware connection layouts
