# 4x4 Vedic Multiplier using Urdhva Tiryagbhyam Sutra (Verilog)

## Project Overview

This project involves the design and implementation of a 4x4 Vedic Multiplier using the Urdhva Tiryagbhyam Sutra from Vedic Mathematics. The multiplier is written in Verilog HDL and simulated using Xilinx Vivado. The goal is to develop a fast and area-efficient multiplier suitable for use in digital systems such as DSPs, ALUs, and microcontrollers.

## What is the Urdhva Tiryagbhyam Sutra?

"Urdhva Tiryagbhyam" is a Sanskrit phrase from Vedic Mathematics.  
It translates to **"Vertically and Crosswise"**.

### Sutra Meaning:
- **Urdhva (ऊर्ध्व)** = Vertical
- **Tiryagbhyam (तिर्यग्भ्याम्)** = Crosswise

This method performs multiplication by computing all partial products in parallel, then summing them. The method is modular and highly suitable for hardware implementation, resulting in faster computation and better area optimization compared to traditional techniques.

## Decimal Example: Multiply 12 × 13 using Urdhva Tiryagbhyam
    1  2
  
  × 1  3

Steps:
1. Multiply units digits → 2 × 3 = 6 → units place  
2. Cross-multiply and add → (1×3) + (2×1) = 5 → tens place  
3. Multiply tens digits → 1 × 1 = 1 → hundreds place  

**Final Result:** 156

This same principle is extended in binary logic for digital hardware. In this project, it is implemented using Verilog.

## Comparison with Traditional Multipliers

| Feature               | Vedic Multiplier             | Traditional Multiplier           |
|-----------------------|-------------------------------|----------------------------------|
| Speed                 | High (parallel computation)   | Moderate                         |
| Area Efficiency       | Good (fewer hardware gates)   | Higher gate count                |
| Scalability           | Modular and easy to expand    | Becomes complex with size        |
| Power Consumption     | Lower                         | Higher due to more switching     |
| Implementation        | Simple and structured         | More complex                     |

## Tools Used

- Hardware Description Language: Verilog
- Simulation and Synthesis Tool: Xilinx Vivado (WebPACK Edition)
- Behavioral Simulation: Vivado Simulator

## Project Files

- `vedic_2x2.v` – 2x2 Vedic multiplier module
- `vedic_4x4.v` – 4x4 multiplier using 2x2 units and adders
- `tb_vedic_4x4.v` – Testbench for simulation
- `README.md` – Project documentation



