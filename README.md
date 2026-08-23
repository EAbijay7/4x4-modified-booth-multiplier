# 4×4 Modified Booth Multiplier Design

Transistor-level design and hierarchical schematic implementation of a **4×4 Modified Booth (Radix-4) multiplier** using **Cadence Virtuoso** and **GPDK90** technology.

> **Project status:** Documentation skeleton created. Cadence schematics, hierarchy, and verification evidence will be added from the project screenshots.

## Overview

This project focuses exclusively on the implementation of a 4×4 Modified Booth multiplier at the transistor level. The design was developed in Cadence Virtuoso using the GPDK90 technology library. Individual circuit modules were designed as reusable schematic blocks and integrated hierarchically to construct the complete multiplier architecture.

The project emphasizes circuit-level implementation of the Modified Booth multiplication architecture rather than RTL or Verilog implementation.

## Objectives

- Implement a 4×4 Modified Booth multiplier architecture.
- Translate the Modified Booth algorithm into transistor-level circuit blocks.
- Develop reusable schematic symbols for individual modules.
- Integrate the modules using hierarchical schematic design.
- Verify circuit connectivity and the resulting multiplier architecture in Cadence Virtuoso.

## Design Environment

| Category | Details |
|---|---|
| EDA Tool | Cadence Virtuoso |
| Technology | GPDK90 |
| Design Level | Transistor-level schematic |
| Architecture | Modified Booth / Radix-4 |
| Operand Size | 4×4 bits |
| Design Method | Hierarchical schematic design |

## Modified Booth Architecture

The Modified Booth algorithm recodes the multiplier into signed digits from the set:

`{−2, −1, 0, +1, +2}`

For a 4-bit multiplier, overlapping groups of three bits are examined to generate the required partial-product operations. The resulting partial products are then combined to obtain the final multiplication result.

The circuit implementation follows this algorithm at the schematic level using transistor-level building blocks and reusable symbols.

## Booth Encoding Table

| Group | Operation |
|---|---|
| 000 | 0 |
| 001 | +M |
| 010 | +M |
| 011 | +2M |
| 100 | −2M |
| 101 | −M |
| 110 | −M |
| 111 | 0 |

## Hierarchical Design

The multiplier is organized hierarchically. Individual circuit modules are first implemented and represented using reusable schematic symbols. These symbols are then connected at higher levels to construct the complete 4×4 Modified Booth multiplier.

Detailed hierarchy and module descriptions will be documented here after the Cadence screenshots are added.

## Circuit Implementation

The project was implemented using transistor-level schematics in Cadence Virtuoso with the GPDK90 technology. The repository will document the actual schematic hierarchy, reusable symbols, and module-level implementation using screenshots from the completed design.

## Verification

Circuit connectivity and design integration were verified within the Cadence design environment. Detailed verification evidence will be added to the repository once the corresponding project screenshots and results are available.

## Repository Structure

```text
4x4-modified-booth-multiplier/
│
├── README.md
├── LICENSE
├── .gitignore
│
├── docs/
│   ├── architecture/
│   └── algorithm/
│
├── cadence/
│   └── README.md
│
├── screenshots/
│   └── README.md
│
└── results/
    └── README.md
```

## Planned Documentation

- Modified Booth algorithm explanation
- Architecture overview
- Cadence Virtuoso schematic hierarchy
- Reusable schematic symbols
- Transistor-level module screenshots
- Connectivity and verification evidence
- Final design results

## Tools & Technologies

- Cadence Virtuoso
- GPDK90
- Transistor-level circuit design
- Schematic capture
- Hierarchical design
- Modified Booth multiplication

## Author

**E. Abijay**  
Electronics and Communication Engineering
