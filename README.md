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

---

## 📁 Day 3 Tasks & Labs

### 🚀 Dataflow Programming Models & Execution Concurrency
* **Source File:** `Understanding DataFlow.vi`
* **Objective:** Map structural node execution, trace independent thread processing, and eliminate structural Flat Sequence boxes using pure wire data dependency tracking and functional selection gates.

#### 🎥 Video Knowledge Validation:
* **Fahrenheit to Celsius Study Tool:** Pre-lab diagnostic exploration verifying baseline data packet routing pipelines.
  * **System Visualization:** ![Fahrenheit to Celsius Practice](Spectragaze_Task_Screenshots/DataFlow_1.png)

---

### 🚀 Task 1: Arithmetic Primitive Chaining & Flow Logic
* **Objective:** Map multi-stage mathematical expression chains to analyze how downstream computational nodes dynamically lock until initial wire inputs are completely satisfied.

#### System Execution Layouts:

| Front Panel User Interface | Backend Block Diagram Dataflow |
| :---: | :---: |
| ![Arithmetic Chaining Panel](Spectragaze_Task_Screenshots/Arithmetic_Primitive_Chaining_Front_Panel.png) | ![Arithmetic Chaining Diagram](Spectragaze_Task_Screenshots/Arithmetic_Primitive_Chaining_Block_Diagram.png) |

---

### 🚀 Task 2: Asynchronous Parallel Branches & Concurrency
* **Objective:** Deploy isolated calculation networks running side-by-side to demonstrate automatic compiler hardware multi-threading across separate CPU cores without manual thread handling routines.

#### System Execution Layouts:

| Front Panel User Interface | Backend Block Diagram Dataflow |
| :---: | :---: |
| ![Independent Branch Panel](Spectragaze_Task_Screenshots/Independent_Branch_Front_Panel.png) | ![Independent Branch Diagram](Spectragaze_Task_Screenshots/Independent_Branch_Block_Diagram.png) |

---

### 🚀 Task 3: Sequence Structure Refactoring & Optimization
* **Objective:** Model how text-based programmers artificially force timing controls using flat film-reel frames, and subsequently refactor the logic to run purely on data dependency constraints.

#### 1. Flat Sequence Architecture Framework (Baseline)
* **Execution Behavior:** Enforces sequential step logic by restricting frame execution chronologically from left to right. Frame 1 stays completely frozen and grayed out while data bubbles travel through Frame 0.

| Flat Sequence Panel Interface | Sequence Frame 1 Block View |
| :---: | :---: |
| ![Sequence Front Panel](Spectragaze_Task_Screenshots/Sequence_Structure_Front_Panel.png) | ![Sequence Frame 2](Spectragaze_Task_Screenshots/Sequence_Structure_2.png) |

#### 2. Advanced Refactored Non-Destructive Pipelines
* **Execution Tracking Phase 1:** Demonstrates data flow monitoring under highlighted bubble routing paths.
  * **System Visualization:** ![Execution Tracking 1](Spectragaze_Task_Screenshots/Execution_tracking_1.png)
* **Execution Tracking Phase 2 (Selector Gate Function):** Utilizes a Select function block locked to an absolute **True** constant. The operational logic forces the system to freeze downstream multiplication steps until the asynchronous division data bubble finishes processing and arrives at the gate's lower terminal, preserving 100% mathematical integrity.
  * **System Visualization:** ![Execution Tracking 2 Selector Gate](Spectragaze_Task_Screenshots/Execution_tracking_2_Selector.png)

---

## 📁 Day 4: Core Environment Diagnostics & Subsystem Validation

### 🚀 Advanced Debugging Methodologies, Trace-Point Probing & Modular Engineering
* **Source Files:** Custom Sub-VI Geometry Module and Master Diagnostic Interface Canvas
* **Objective:** Master professional environment instrumentation, runtime thread interrogation, and multi-point parameter tracking by diagnosing compile-time syntax faults and correcting hidden semantic logic errors within a multi-VI application.

#### Detailed Architectural Implementations & Technical Milestones:

1. **Modular Sub-VI Architecture & Connector Mapping:**
   * Engineered a standalone geometric subsystem utilizing multi-input resizable calculation nodes to streamline block diagram workspace efficiency.
   * Mapped internal controls and indicators directly to the upper-right **Connector Pane Grid**, creating functional, external hardware terminals. This enables the top-level script to cleanly call and pass parameters to the module as a reusable function block.

2. **Real-Time Parameter Probing & Dynamic Value Logging:**
   * Configured floating **Wire Probes** across separate data buses on the block diagram, serving as virtual digital multimeters.
   * Utilized **Highlight Execution** to visually track the speed and path of data packets flowing through the circuits.
   * Activated **Retain Wire Values** mode to preserve system memory maps after program completion. Verified that the diagnostic window logged precise parameter values (`24`, `25`, and `3061.2`) along the wire paths during full-speed runtime.

3. **Execution Thread Control via Context Breakpoints:**
   * Deployed structural **Breakpoints** directly onto the called sub-VI icon node, establishing a physical thread-freeze boundary.
   * Verified that the breakpoint successfully halts background CPU execution the millisecond input data arrives, triggering a flashing red pause state on the toolbar ribbon. This allows developers to inspect static intermediate memory states calmly before the application proceeds.
   * Practiced micro-stepping execution commands (**Step Into**, **Step Over**, and **Step Out**) to advance data packets through the logic nodes one bubble at a time.

4. **Syntax & Semantic Bug Remediation:**
   * **Syntax Layer:** Analyzed compiler failures via the three-pane **Error List** window to instantly auto-locate an uncompiled, unwired pin on the sub-VI's division node. Fixed by linking a hardcoded constant denominator.
   * **Semantic Layer:** Troubleshooted a hidden runtime logic error where a side-length validation circuit permanently failed. Used wire probes to find that a Less Than (`<0`) comparator was incorrectly used instead of a Greater Than (`>0`) block. Swapping the operator allowed the resizable 3-input **AND** gate to fire the front-panel safety status LED perfectly.

#### Verified Implementation Workspaces:

| Active Trace-Point Probe Analysis | Execution Thread Boundary Interrogation |
| :---: | :---: |
| ![Probes Log Display](Day%204%20Screenshots/Debugging_Tools_Verification.png) | ![Breakpoint Thread Halt](Day%204%20Screenshots/Breakpoint_Pause_Verification.png) |

| Trace-Point Probes under Highlight Execution | Validation Status Optimization |
| :---: | :---: |
| ![Highlighted Data Flow](Day%204%20Screenshots/Debugging_Tools_Verification_Highlight_Execution.png) | ![Resolved System Assembly](Day%204%20Screenshots/Breakpoint_Pause_Verification_1.png) |
