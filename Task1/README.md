# **Summary of the video given in week 0**

The System-on-Chip (SoC) design process starts with chip modeling. In this stage, hardware functionality is defined using a C-model. This early phase, often called O0/O1, uses the GCC compiler to build and run the software model. The design is verified against a C-based testbench to make sure it meets the intended functionality.

After the design specifications are confirmed, the process moves to RTL development (O2). Here, hardware is described in Register Transfer Level (RTL) using Verilog. The processor and peripheral IPs are implemented in RTL and verified again with the same C-language testbench to keep everything consistent and correct.

Once RTL verification is done, the design is converted into a gate-level netlist. At this stage, analog IPs and pre-designed macros are integrated. This leads into the SoC integration stage (O3), where all components—including the processor, peripherals, analog IPs, and macros—are put together into a complete SoC.

After integration, the physical design phase starts. This phase includes important steps like floorplanning, placement, clock tree synthesis, and routing. The process then moves into the RTL-to-GDSII (RTL2GDS) phase, which includes signoff checks such as Design Rule Checking (DRC) and Layout Versus Schematic (LVS) to ensure the final layout is free of errors and ready for fabrication.

Throughout the whole process, a consistent verification method is used with the same C-based testbench. This ensures smooth continuity from the initial specification, through RTL development, to the final chip implementation.
