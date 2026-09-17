# BIM-Based Design Evaluator for Structural Components (Modular Construction)

A Revit-based research tool (**BIM-DE4PB**) for evaluating the design of prefabricated/modular building components **before fabrication and installation**, so design issues are caught at the conception stage rather than on site.

## Why this exists

Modular/prefabricated construction is efficient, but poor early-stage design decisions lead to higher cost, material waste, safety issues, and construction delays. Traditional workflows give architects and engineers no coordinated platform to evaluate a prefabricated design before it moves forward. This project integrates two proven design-improvement approaches into BIM to close that gap:

- **Design for Manufacture and Assembly (DFMA)**
- **Lean construction principles**

## Objectives

1. Identify design-evaluation factors for prefabricated elements from DFMA and Lean construction principles.
2. Formulate a BIM-based design-evaluation framework from those factors.
3. Integrate and validate the framework as a working digital platform.

## How it works

1. **Literature review + industry survey** — Design factors were extracted from DFMA/Lean literature, then validated and shortlisted with input from construction industry professionals.
2. **Framework development** — The shortlisted factors were structured into an evaluation framework covering both DFMA and Lean assessment routes.
3. **Plugin development** — The framework was implemented as a Revit add-in (Ribbon panel + UI) that walks a user through evaluating a design directly inside their Revit model.
4. **Validation** — The tool was validated with industry experts via semi-structured interviews, scored on need, usability, implementability, and DFMA factor relevance.

## Tech stack

- **Autodesk Revit Architecture 2022** — BIM platform / host application
- **Revit API (.NET Framework 4.7)** — plugin logic and UI
- **JavaScript** — application logic
- **Microsoft Visual Studio** — development environment
- **SQL Server** — data storage for evaluator inputs/results

## Core features

- Ribbon-integrated add-in inside Revit — no separate application needed
- Evaluator registration with a unique, auto-generated ID per evaluation session
- Choice of evaluation method: **DFMA** or **Lean principles**, with in-app descriptions of each
- Heuristic evaluation of a design against each factor on a Likert (compliance) scale
- Exportable evaluation report (PDF) for documentation and follow-up

## Validation results (summary)

Industry experts rated the tool positively across need, usability, and implementability, and confirmed the DFMA/Lean factors used are relevant to evaluating prefabricated designs. Adoption barriers noted by experts include limited BIM knowledge in the local industry, training/equipment cost, and general resistance to new tools in traditional construction workflows.

## Limitations & future work

- Most effective when used by someone familiar with DFMA/Lean principles.
- Future improvements could add financial-benefit analysis and integrate sustainability guidelines into the evaluation framework.

## Reference

Based on the MS thesis: *"Modular Construction: Developing a BIM Based Design Evaluator for Building Components"* — Mubashir Islam, NUST (Construction Engineering & Management), 2021.
