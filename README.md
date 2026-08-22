# RISC-V Processor in Verilog

## Overview

This repository contains the Verilog implementation of a basic **RISC-V processor**. The project is designed to demonstrate the fundamental architecture and operation of a RISC-V CPU, including instruction execution, arithmetic and logical operations, memory access, and control flow.

## Features

* Verilog implementation of a basic RISC-V processor
* Modular design for easy understanding and debugging
* Supports core RISC-V instructions
* Synthesizable and simulation-friendly design
* Well-commented source code

## Components

The project consists of the following modules:

* **Program Counter (PC)** – Holds the address of the current instruction.
* **Instruction Memory** – Stores program instructions.
* **Control Unit** – Generates control signals based on the opcode.
* **Register File** – Contains 32 general-purpose registers.
* **Immediate Generator** – Extracts and extends immediate values.
* **ALU (Arithmetic Logic Unit)** – Performs arithmetic and logical operations.
* **ALU Control** – Determines the ALU operation.
* **Data Memory** – Handles load and store instructions.
* **Multiplexers (MUXes)** – Select appropriate data paths.
* **Adder Units** – Compute PC+4 and branch target addresses.
* **Top Module** – Integrates all processor components.

## Code Structure

```text
RISC-V/
│── rtl/
│   ├── program_counter.v
│   ├── instruction_memory.v
│   ├── control_unit.v
│   ├── register_file.v
│   ├── immediate_generator.v
│   ├── alu.v
│   ├── alu_control.v
│   ├── data_memory.v
│   ├── mux.v
│   ├── top.v
│
│── testbench/
│   └── processor_tb.v
│
└── README.md
```

## Tools Used

* Verilog HDL
* ModelSim / Vivado Simulator / Icarus Verilog (or any Verilog simulator)

## Resources

* RISC-V Unprivileged ISA Specification
* *Computer Organization and Design: RISC-V Edition* by Patterson & Hennessy
* Digital Design and Computer Architecture (RISC-V Edition)

## Future Improvements

* Five-stage pipelined processor
* Hazard detection and forwarding
* Branch prediction
* Instruction and data caches
* Support for additional RISC-V instructions

## Author

**Karthik Reddy**

## License

This project is provided for educational purposes. Feel free to use, modify, and extend the design for learning and research.
