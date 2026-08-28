# FPGA-Based Adaptive Voltage Window Protection System

A VHDL-based digital voltage protection system implemented on the
Artix-7 XC7A100T FPGA (Nexys A7-100T).

The system monitors an 8-bit voltage sample and classifies it into
three operating states: NORMAL, OVER, and UNDER. Comparator logic
generates the threshold conditions, while a synchronous Moore FSM
controls the system state.

A Freeze-on-Fault mechanism prevents reference/threshold updates
during abnormal conditions, providing stable and deterministic
recovery.

## Key Features

- VHDL-based RTL design
- Artix-7 XC7A100T FPGA implementation
- Comparator-based voltage window detection
- Synchronous Moore FSM
- NORMAL / OVER / UNDER states
- Freeze-on-Fault mechanism
- 100 MHz clock operation
- 8-bit voltage input
- LED-based fault indication
- Vivado XSIM simulation
- RTL schematic analysis
- FPGA floorplanning

## Implementation Results

- FPGA: Artix-7 XC7A100T
- Board: Nexys A7-100T
- Clock: 100 MHz
- Total on-chip power: 0.349 W
- Dynamic power: 0.257 W
- Static power: 0.092 W
- Junction temperature: 26.6 °C

The design was successfully synthesized, simulated, implemented,
and programmed onto the FPGA. Hardware behavior matched the
simulation results.
- On-chip power analysis
- Hardware implementation and validation
