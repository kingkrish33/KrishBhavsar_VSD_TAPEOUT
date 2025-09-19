# KrishBhavsar_VSD_TAPEOUT

# VSD-SoC-Design-Program-Day0

## Day0_Setup_Yosys_IcarusVerilog_GTKWave

Welcome to **Day 0** of the VSD SoC Design and Physical Design program.  
On this day, we focus on setting up the open-source tools that will be used throughout the course: **Yosys**, **Icarus Verilog (iverilog)**, and **GTKWave**.

To ensure a stable and controlled development environment, we first set up a virtualized Linux system:

* Installed **Oracle VirtualBox** as the hypervisor.
* Created a dedicated **Ubuntu 20.04 LTS** virtual machine.
* Provisioned the VM with **6 GB of RAM** and **4 virtual CPUs**, ensuring sufficient resources for compute-intensive EDA tasks.
* Once Ubuntu was running, we accessed the **Linux terminal** to begin tool installation and environment configuration.

---

## Theory and Background

### 🔹 Yosys – RTL Synthesis Engine

Yosys is a powerful open-source **RTL synthesis framework** that transforms **Verilog RTL code** into an optimized **gate-level netlist**. It integrates with standard cell libraries (e.g., **Sky130 PDK**) to map RTL designs into real hardware primitives.

* **Role in Flow:** RTL → Gate-Level Netlist
* **Capabilities:** logic optimization, technology mapping, design hierarchy handling, synthesis reports.
* **Why Yosys?** It forms the backbone of open-source digital synthesis and is compatible with OpenLANE for complete RTL-to-GDSII flows.

### 🔹 Icarus Verilog (iverilog) – Simulation Engine

Icarus Verilog is an open-source **HDL simulation and compilation tool**. It validates design functionality **before synthesis** by simulating RTL.

* **Role in Flow:** Functional simulation & verification of Verilog RTL.
* **Outputs:** Generates executable simulation files (`.vvp`) and waveform dump files (`.vcd`).
* **Importance:** Detects design bugs early, reducing synthesis-debug cycles.

### 🔹 GTKWave – Waveform Analysis Tool

GTKWave is a **waveform viewer** that visualizes simulation outputs from `.vcd` or `.fst` files. It enables signal-level debugging by showing how inputs and outputs evolve over time.

* **Role in Flow:** Debugging and waveform inspection.
* **Features:** zooming, signal grouping, cursor-based measurement, and hierarchical viewing.
* **Use Case:** Essential for confirming functional correctness and validating timing behavior.

---

## Key Objectives for Day 0

1. **Prepare Environment**

   * Configure Oracle VirtualBox and Ubuntu 20.04 VM.
   * Allocate sufficient resources (≥6 GB RAM, ≥4 vCPUs).

2. **Install Core Tools**

   * Install and build Yosys from source.
   * Install Icarus Verilog via package manager.
   * Install GTKWave for waveform visualization.

3. **Validate Setup**

   * Run version checks (`yosys`, `iverilog -v`, `gtkwave`) to confirm successful installation.
   * Prepare environment for Day 1
   


