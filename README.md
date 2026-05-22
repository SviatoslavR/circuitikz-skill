# Circuitikz-Skill

An engineering-grade protocol and workflow for AI-assisted circuit schematic reconstruction using LaTeX and `circuitikz`.

## Overview

This repository provides a rigorous **system instruction (SKILL.md)** designed to guide LLMs in transforming technical circuit schematics (e.g., IEEE paper screenshots) into high-quality, professional, and editable LaTeX/Circuitikz code.

It solves the common pitfalls of AI-generated schematics, such as logical layout errors, and component overlap.

## Why this protocol?

- **Robustness:** Eliminates common AI hallucinations in circuit connectivity.
- **Maintainability:** Enforces a three-phase code architecture (Placement → Connectivity → Labeling).
- **IEEE Compliance:** Standardizes component styling, VDD/GND notations, and wire routing for academic publications.

## Key Features

- **Terminal Integrity Protocol:** A critical check-gate that forces the AI to verify the Drain/Source orientation before generating connection code.
- **Grid-Based Planning:** Pre-compilation analysis for component layout to ensure optimal spacing.
- **Modular Documentation:** Every line of code is commented, turning the generated schematic into a maintainable "tutor" for the user.

## Workflow

1. **Analyze:** Extract components and topology from the input image.
2. **Plan:** Calculate coordinate grids and component spacing.
3. **Verify:** Check and eliminate errors.
4. **Generate:** Produce modular, heavily commented LaTeX code.

## Structure

- `SKILL.md`: The core system instruction. Feed this to any LLM as a System Prompt.
- `examples/`: A showcase of reconstructed schematics (e.g., 9T SRAM) with source code and PDF output.

## Quick Start

1. Copy the contents of `SKILL.md` into your AI's system prompt or context.
2. Provide your circuit screenshot and request reconstruction.
3. Fine-tune using the generated coordinate variables to adjust spacing or labels.

---

*Maintained for academic circuit diagram reproduction.*
