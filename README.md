# Edge Triggered Flip-Flop Implementation in Cadence Virtuoso

## Overview
This project demonstrates the design and simulation of an **Edge-Triggered Flip-Flop** implemented using **SR and D Flip-Flops** in **Cadence Virtuoso**.  
All fundamental digital blocks used in the design were created from **transistor-level CMOS circuits**, including **NAND gates and inverters**, and later converted into reusable **symbols**.

The project highlights a **hierarchical VLSI design approach**, where basic logic gates are used to construct sequential circuits and ultimately form an **edge-triggered flip-flop**.

---

## Design Methodology

The design was implemented using a **bottom-up design approach**.

### 1. CMOS Inverter
- Designed using **PMOS and NMOS transistors**
- Used as a fundamental building block in the circuit.

### 2. CMOS NAND Gate
- Implemented using **CMOS transistor-level logic**
- Converted into a **symbol for hierarchical design**

### 3. SR Flip-Flop
- Constructed using **cross-coupled NAND gates**
- Verified correct **Set and Reset functionality**

### 4. D Flip-Flop
- Designed using logic gates and feedback structure
- Ensures output follows the input based on the **clock signal**

### 5. Edge Triggered Flip-Flop
- Implemented by combining **D Flip-Flop and SR Flip-Flop**
- Stores data only during the **clock edge**

---

## Schematic Components

### Logic Blocks
- CMOS Inverter
- CMOS NAND Gate

### Sequential Blocks
- SR Flip-Flop
- D Flip-Flop

### Final Module
- Edge Triggered Flip-Flop

### Power Supply
- **VDD = 1.8 V**

### Inputs
- **Clock Signal**
- **Data Input (D)**

### Outputs
- **Q**
- **Q̅ (Complement Output)**

---

## Simulation Details

**EDA Tool:** Cadence Virtuoso  
**Simulator:** Spectre  
**Simulation Type:** Transient Analysis

### Observed Signals
- Input Data (D)
- Clock Signal (CLK)
- Output (Q)
- Complement Output (Q̅)

### Expected Behavior
- Output changes **only at the clock edge**
- Output remains **stable between clock transitions**
- **Q and Q̅ remain complementary**

---

## How to Run the Simulation

1. Open **Cadence Virtuoso**
2. Load the project library
3. Open the **edge_triggered_flip_flop schematic**
4. Launch **ADE Explorer / ADE L**
5. Configure **Transient Analysis**
6. Select signals to observe:
   - D
   - CLK
   - Q
   - Q̅
7. Run the simulation
8. Observe waveforms in the **Cadence waveform viewer**

---

## Design Highlights

- Transistor-level CMOS implementation
- Custom design of **NAND gates and inverters**
- Hierarchical circuit design
- Functional verification using **Cadence Spectre**

---

## Applications

Edge-triggered flip-flops are widely used in:

- Registers
- Counters
- Shift Registers
- Memory Elements
- Synchronous Digital Systems

---

## Tools Used

- Cadence Virtuoso
- Spectre Simulator
