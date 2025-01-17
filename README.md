# MOS Differential Amplifier

## Overview
This project involves the design and simulation of a **current mirror-based differential amplifier** using the **180 nm CMOS process technology**. It explores critical analog design concepts such as gain, phase margin, slew rate, and common-mode rejection ratio (CMRR). The design specifications are tailored to meet the requirements of modern analog circuits while using systematic simulation techniques.

---

## Specifications

- **Technology**: 180 nm CMOS process
- **Power Supply**: 1.8 V
- **Input Common-Mode Voltage**: 900 mV
- **VDS,sat for Input Transistors**: 200–300 mV
- **VDS,sat for Other Transistors**: 100–200 mV
- **Tail Current**: Derived from a 20 µA current source via a current mirror

### Performance Metrics
- **DC Gain**: ≥ 35 dB
- **Phase Margin**: ≥ 60º
- **Slew Rate**: ≥ 40 V/µs (with a 1 pF load capacitance)

---

## Design Tasks

1. **Frequency Response**:
   - Plot the frequency response showing DC gain, Unity Gain Bandwidth (UGB), and phase margin.

2. **Specifications Validation**:
   - Ensure the design meets all performance specifications.

3. **CMRR Calculation**:
   - Perform AC analysis to compute the differential and common-mode gain.

4. **Voltage Follower Test**:
   - Use the OTA as a voltage follower for a 100 mV peak-to-peak, 1 kHz sine wave. Analyze gain deviations.

5. **Inverting Schmitt Trigger**:
   - Design using the OTA for:
     - UTP = 1 V
     - LTP = 0.8 V
     - Feedback resistors limit current to 10% of the tail current.
   - Test with an input: **0.9 V + 0.9 sin(2000πt)**.

---

## Key Insights

- The design avoids the use of transistor current or gm equations due to their approximations.
- Practical considerations include current mirrors, feedback networks, and proper tail current allocation.

---

## Tools & Resources

- **Simulation Software**: Use industry-standard tools such as Cadence Virtuoso, NGSpice, or LTSpice for simulation and analysis.
- **Documentation**: Detailed reports and plots included in the repository for reproducibility.
- **Process Node**: Based on 180 nm CMOS technology for compatibility with educational and research environments.

---

## Future Improvements

- Extend the design to multi-stage amplifiers.
- Experiment with other CMOS technologies (e.g., 65 nm, 28 nm).
- Incorporate noise analysis and layout optimization.

---

## How to Get Started

1. Clone the repository:
   ```bash
   git clone https://github.com/being-satyam/MOS_Differential_Amplifier.git
   ```
2. Open the design files in your preferred simulation tool.
3. Follow the documentation in the repository to replicate the results.

---

## Contributors

- **Satyam Kumar**
  - [GitHub](https://github.com/being-satyam)
  

Feel free to contribute by submitting issues or pull requests!
