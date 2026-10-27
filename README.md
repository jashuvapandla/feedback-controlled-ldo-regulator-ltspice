# feedback-controlled-ldo-regulator-ltspice
# ⚡ Feedback-Controlled LDO Voltage Regulator
### Analog Electronics | Power Management | LTspice Simulation

<p align="center">
  <img src="https://img.shields.io/badge/Domain-Analog%20Electronics-blue?style=for-the-badge" alt="Analog Electronics" />
  <img src="https://img.shields.io/badge/Tool-LTspice-orange?style=for-the-badge" alt="LTspice" />
  <img src="https://img.shields.io/badge/Status-In%20Progress-yellow?style=for-the-badge" alt="In Progress" />
</p>

## 🚀 Overview

A stable power supply is essential for electronic circuits. Changes in input voltage and load current can cause unwanted variations in the output voltage.

This project explores the design and simulation of a **feedback-controlled Low-Dropout (LDO) voltage regulator** using LTspice. The circuit uses a reference voltage, feedback network, error amplifier, and pass transistor to regulate its output.

## 🎯 Project Objectives

- Design a closed-loop voltage regulation circuit.
- Understand negative feedback and error-amplifier operation.
- Analyse output voltage under changing input conditions.
- Evaluate load regulation and transient response.
- Investigate the influence of output capacitance and feedback components.
- Document simulation results and compare them with theoretical expectations.

## 🏗️ Proposed Architecture

```text
       Input Supply (Vin)
              │
              ▼
       ┌─────────────┐
       │ Pass Device │
       └─────────────┘
              │
              ├──────────► Regulated Output (Vout)
              │                       │
              │                       ▼
              │                Feedback Divider
              │                       │
              ▼                       ▼
         Load Circuit          Error Amplifier
                                      ▲
                                      │
                                Reference Voltage
```

*Conceptual architecture; the final schematic and control polarity will be verified during implementation.*

## ⚙️ Initial Design Targets

| Parameter | Target |
|---|---|
| Input voltage | 5 V nominal |
| Output voltage | 3.3 V nominal |
| Load current | 10–100 mA test range |
| Pass element | PMOS transistor |
| Control method | Negative feedback |
| Simulation tool | LTspice |
| Implementation | Simulation only |

These are initial design targets, not measured results. The achievable regulation and dropout performance will depend on the selected components and verified circuit design.

## 🧪 Verification Plan

| Test | Purpose |
|---|---|
| DC operating point | Check the nominal output voltage |
| Input-voltage sweep | Evaluate line regulation |
| Load-current sweep | Evaluate load regulation |
| Transient analysis | Observe output recovery after load changes |
| Output-capacitor comparison | Study transient behaviour |
| Stability investigation | Check for oscillation or excessive ringing |

## 📊 Simulation Results

**Status: Pending implementation**

The following will be documented after simulation:

- Input and output voltage plots
- Output variation across the load range
- Transient response to load changes
- Measured regulation error
- Limitations and possible improvements

No performance results are claimed until the circuit has been simulated and checked.

## 🛠️ Tools & Concepts

**Tool:** LTspice

**Concepts:** Analog electronics, MOSFET operation, voltage references, negative feedback, error amplifiers, voltage regulation, transient analysis, and stability fundamentals.

## 🔮 Future Improvements

- Investigate different pass-transistor models.
- Compare output-capacitor values and equivalent series resistance.
- Examine dropout behaviour and power dissipation.
- Improve the amplifier model and assess feedback-loop stability.

## 👨‍💻 Author

**Pandla Jashuva**

ECE Project Portfolio | Analog Electronics 

---

*An educational, simulation-based project. Physical hardware testing has not been performed.*
