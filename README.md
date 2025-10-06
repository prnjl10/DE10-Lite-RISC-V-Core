This project implements a custom 32-bit RISC-V RV32I CPU core with a 4-stage pipeline (IF, ID, EX, MEM+WB), optimized for deployment on the Intel MAX10 FPGA (DE10-Lite board). The design features a modular, single-issue, in-order pipeline capable of executing RISC-V integer workloads.

Features Implemented:

4-stage pipelined RV32I core: Instruction Fetch, Decode, Execute, and MEM+Writeback stages

Modular design: ALU, register file, control unit, and immediate generator

Branch handling with BNE support

Dual-port data and instruction memory

Memory-mapped UART-TX logic (designed but not yet verified on hardware)

Successfully synthesized and deployed to DE10-Lite

Benchmark programs loaded into instruction memory for testing

Work in Progress:

UART output over USB-Serial (CP2102) is integrated in design but not yet successfully verified due to driver/connection issues.

Real-time benchmark result capture is pending hardware serial communication debug.

Testbench verification of the RISC-V Core
