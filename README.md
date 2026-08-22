# SpectraGaze Systems — Engineering Internship Portfolio

This repository hosts development deliverables, environment validations, and graphic dataflow applications completed during the engineering onboarding training track.

---

## 📁 Day 1 Tasks & Labs

### 🚀 Task 1: Onboarding & Environment Setup
* **Objective:** Install LabVIEW 2026 Q3 (Community Edition), configure NI-DAQmx and NI-VISA drivers, and verify activation in NI Package Manager.

#### Deliverables:
- Verified installation of LabVIEW + drivers
- Repo cloned successfully

---

### 🚀 Task 2: Graphic Dataflow Foundations ("Hello VI")
* **Source File:** `Hello VI.vi`
* **Objective:** Design an introductory visual pipeline to accept distinct user inputs, execute dynamic arithmetic calculations, and update front-panel indicators safely.

#### System Execution Layout:
![Hello VI Execution Layout](Spectragaze_Task_Screenshots/Hello_VI.png)

---

### 🚀 Task 3: Mathematical Function Conversions (Temperature Converter)
* **Source File:** `Celsius to Fahrenheit.vi`
* **Objective:** Implement physical formulaic scaling logic to dynamically map temperature shifts across fractional integer paths, using intuitive UI elements.

#### Logic & Layout:
- Added a **vertical slider** for Celsius input to make temperature selection more interactive.  
- Used **Multiply (×)**, **Add (+)**, and **Divide (÷)** blocks to structure the conversion formula clearly.  
- Routed the result into a Fahrenheit indicator for live display.  
- Verified correctness (e.g., 100°C → 212°F).  

#### System Execution Layout:
![Temperature Converter Logic Layout](Spectragaze_Task_Screenshots/Celsius_Converter.png)

---

## 📁 Day 2 Tasks & Labs

### 🚀 Task 1: Core Data Types & Strict Typing Exploration
* **Source File:** `Data Types Exploration.vi`
* **Objective:** Verify operational behavior across standard memory primitives and demonstrate compilation enforcement under LabVIEW's strictly typed visual architecture.

#### Architectural Implementations:
1. **Compatible Type Scaling:** Demonstrates data promotion layers running an Integer (`I32`) pipeline cleanly into a Floating-Point (`DBL`) register path.  
2. **Strict Type Enforcement:** Intentionally highlights a type-mismatch compilation block (broken wire) when attempting to route raw Integer structures into text String outputs.  
3. **Explicit Type Casting:** Implements a baseline structural converter node to cleanly serialize numeric data into active text streams safely.

#### System Execution Layouts:
- **Front Panel User Interface:** ![Front Panel Screenshot](Spectragaze_Task_Screenshots/Data%20Types%20Exploration%20Front%20Panel.png)
- **Backend Block Diagram Dataflow:** ![Block Diagram Screenshot](Spectragaze_Task_Screenshots/Data%20Types%20Exploration%20Block%20Diagram.png)

---

### 🚀 Task 2: Linear Ramp Calibration Engine
* **Source File:** `Ramp Calibration Logic.vi`
* **Objective:** Synthesize sequential loop operations, arithmetic scaling factors, and multi-branch case structures to generate a software-calibrated ramp signal with active boundary checking.

#### Architectural Implementations:
1. **Data Domain Translation:** Maps raw incremental loop indices (`I32`) down to precise fractional data bounds (`DBL`) via linear feature-scaling multipliers (`× 0.1`).
2. **Active Exception Monitoring:** Hooks a comparative boolean branch into an independent `If/Else` Case Structure framework to toggle critical front-panel warning indicators the moment boundaries cross safety limits (`> 5.0`).
3. **Resource Optimization:** Integrates a localized **Wait (ms)** block to protect the CPU from processing spikes.

#### System Execution Layout:
![Ramp Calibration Layout](Spectragaze_Task_Screenshots/Ramp_Calibration.png)
![Ramp Calibration Layout](Spectragaze_Task_Screenshots/Ramp_Calibration_2.png)

---

### 🚀 Task 3: Geometric Specification Matching (Area & Perimeter)
* **Source File:** `Area and Perimeter Calculator.vi`
* **Objective:** Recreate a specified arithmetic block diagram handling simultaneous geometric algebraic formulas based on linear user controls.

#### Layout Details:
1. **Area Pipeline:** Formulates a straight product map ($w \times h$) driven to the designated indicator node.
2. **Perimeter Pipeline:** Branches inputs into an introductory summation stage ($w + h$), passes the result downstream to a hardcoded constant multiplier factor (`2`), and updates the boundary display.

#### System Execution Layout:
![Geometry Layout](Spectragaze_Task_Screenshots/Area_and_Perimeter_Calculator.png)

---

## 📁 Day 2 Self-Paced Advanced Extensions

### 🚀 Extension 1: Continuous Operational Loops
* **Source File:** `Understanding Loops.vi`
* **Objective:** Upgrade the static calculation pipeline by wrapping it inside an execution **While Loop** framework to process user inputs continuously without manual program restarts.

#### Architectural Implementations:
- Placed an active execution container that keeps the script alive until an explicit condition is met. 
- Wired a front-panel mechanical **STOP Button** straight into the red loop conditional terminal to release CPU threads safely upon user termination.

#### System Execution Layout:
![Understanding Loops Layout](Spectragaze_Task_Screenshots/Loops.png)

---

### 🚀 Extension 2: Multi-Branch Logical Scaling
* **Source File:** `Understanding Case Structure.vi`
* **Objective:** Integrate a deep architectural branch condition using an interactive switch to toggle backend mathematical calculation paths dynamically.

#### Architectural Implementations:
- Placed a **Mechanical Toggle Switch (Boolean Control)** and routed its green signal line directly to the frame selection terminal of a **Case Structure**.
- When set to `True`, the program executes the baseline temperature formula pipeline cleanly. When toggled, alternative structural branches are activated to handle fallback logic paths safely.

#### System Execution Layout:
![Understanding Case Structure Layout](Spectragaze_Task_Screenshots/Case%20Structure.png)

---

### 🚀 Extension 3: Array Primitive Matrices & Index Interrogation
* **Source File:** `Understanding Arrays.vi`
* **Objective:** Design an advanced memory exploration canvas to verify how composite collection data paths handle bundled variables, size metrics, and localized position extractions.

#### Architectural Implementations:
1. **Parallel Type Grouping:** Grouped separate homogeneous data vectors for both **Numeric Arrays** (Orange thick wires feeding vertical graphs) and **Boolean Arrays** (Thick green wires driving multi-LED indicators).
2. **Data Extraction Nodes:** Deployed the **Array Size** function node to automatically calculate total data density (`Size = 4`) and the **Index Array** function node to scan registers and isolate a single variable item out to an independent display.

#### System Execution Layout:
![Understanding Arrays Layout](Spectragaze_Task_Screenshots/Arrays.png)
