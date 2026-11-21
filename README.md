# FPGA-Lab

Notes on the digital design and FPGA/SoC lab I am studying: Verilog, two boards, Vivado and Vitis.

This repository is about FPGA design only. The lab runs 17 weeks, 4 hours a week (about 68 contact hours), from 7 July to 31 October 2026.

## Boards and tools

| Item | Details |
| --- | --- |
| RealDigital Boolean Board | AMD/Xilinx Spartan-7 (xc7s50). 16 slide switches, 4 pushbuttons, 16 LEDs, 2 RGB LEDs, two 4-digit seven-segment displays, 100 MHz oscillator, USB, PMOD. Weeks 1 to 9. |
| Digilent Zybo | Xilinx Zynq-7000 SoC: dual-core ARM Cortex-A9 Processing System plus Artix-7 Programmable Logic. Weeks 10 to 16. |
| Vivado | HDL entry, simulation, IP Integrator, synthesis, implementation, bitstream, hardware programming. |
| Vitis | Bare-metal C/C++ for the Zynq Processing System. |
| Serial terminal | 115200 baud for UART exercises. |

## How each exercise is organised

1. **Verilog simulation and synthesis.** Testbench, waveform, then synthesis with utilization and timing reports.
2. **Boolean Board (PL only).** The same design on real hardware: switches, LEDs, seven-segment display.
3. **Zybo (PS and PL).** From week 10, three cumulative exercises: GPIO, a custom arithmetic IP over UART, and an AXI-Stream/DMA data path.

## Part A: Boolean Board (weeks 1 to 9)

| Week | Topic |
| --- | --- |
| 1 | Tool setup, first simulation and first bitstream. 2-input AND/OR/XOR module, LED blink counter, XDC constraints. |
| 2 | Decoders, multiplexers and code converters. 3-to-8 decoder, 4-to-1 mux, binary-to-BCD or Gray converter. Dataflow versus case style. |
| 3 | Counters and shift registers. Up/down 16-bit counter, 8-bit universal shift register. |
| 4 | FSM design: two-way traffic-light controller with a pedestrian request. |
| 5 | Arithmetic circuits: 4-bit ripple-carry adder and a one-digit BCD adder. |
| 6 | Memory and logic arrays: 16x4 memory used as a lookup-table function unit. |
| 7 | Top-down design: 8x8 shift-add multiplier and restoring divider, datapath plus control FSM. |
| 8 | FPGA fabric study, switch debouncer and 2-flip-flop synchronizer. |
| 9 | UART transmitter and receiver FSM at 115200 baud. |

## Part B: Zybo (weeks 10 to 16)

| Week | Topic |
| --- | --- |
| 10 | Zynq and AXI overview. PS-PL exercise 1: LED and switch through an AXI GPIO IP in an IP Integrator block design. |
| 11 | PS-PL exercise 1: Vitis bare-metal application with UART output. |
| 12 | Custom AXI4-Lite arithmetic IP: design and packaging. |
| 13 | PS-PL exercise 2: UART command console driving the arithmetic IP. |
| 14 to 16 | AXI4-Stream and DMA. PS-PL exercise 3: custom stream IP with AXI DMA, DDR to stream to DDR, PASS/FAIL over UART. |

## Course modules

M1 digital building blocks, M2 digital system design, M3 programmable devices, M4 FPGA SoCs, M5 embedded system design using FPGAs.

## Status

This repository only lists what the lab covers. My own source files and reports will be added later.
