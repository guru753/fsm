# 100 Mealy Sequence Detector using Verilog

## Overview

This project implements a Mealy Finite State Machine (FSM) in Verilog HDL to detect the binary sequence **100** in a serial input stream.

The detector asserts the output `det_out` whenever the sequence **100** is detected.

## State Diagram

* **idle (00):** Initial state, no bits detected.
* **s1 (01):** Sequence `1` detected.
* **s2 (10):** Sequence `10` detected.
* When the FSM is in `s2` and the next input bit is `0`, the sequence `100` is detected and `det_out` is asserted.

## Files

* `fsm_100_mealy.v` – Verilog code for the Mealy sequence detector.
* `tb.v` – Testbench for simulation and verification.

## Simulation

### Input Sequence

```text
1 ? 0 ? 0
```

### Output

```text
det_out = 1
```

## Tools Used

* Verilog HDL
* EDA Playground
* EPWave / GTKWave

## Learning Outcomes

* Finite State Machine (FSM) design
* Mealy machine implementation
* State transition and output logic
* Verilog coding and simulation
* Testbench development and waveform analysis

## Author

Guruprasad Babanna
Electronics and Communication Engineering (ECE)
Aspiring VLSI Design and Verification Engineer
