# Router_1X3
**README.md**

**1x3 Router Design**

**Overview**

This repository contains the Verilog HDL implementation of a 1x3 router for FPGA. The router is a fundamental building block in Network-on-Chip (NoC) architectures, responsible for directing data packets to their intended destinations. This specific design can receive data from a single input port and route it to one of three output ports.

**Key Components and Functionality**

* **FIFO Module:** Stores incoming data packets temporarily.
* **FSM Module:** Controls the overall operation of the router.
* **Register Module:** Stores intermediate data and control signals.
* **Synchronization Module:** Handles clock domain crossing (CDC) issues.
* **Top Module:** Integrates all modules to form the complete router system.

**Design Methodology**

1. **RTL Design:** Verilog HDL is used to describe the hardware behavior of each module.
2. **Testbench Development:** Testbenches are created to verify the functionality of each module and the entire router system.
3. **Synthesis and Implementation:** Xilinx Vivado is used to synthesize and implement the design onto a target FPGA.
4. **Verification:** Simulation and hardware testing are performed to ensure correct functionality and timing.

**Project Structure**

```
1x3_router/
├── src/
│   ├── fifo.v
│   ├── fsm.v
│   ├── register.v
│   ├── sync.v
│   └── top.v
└── testbench/
    ├── fifo_tb.v
    ├── fsm_tb.v
    ├── register_tb.v
    ├── sync_tb.v
    └── top_tb.v
```

**Usage**

1. **Simulation:** Use a Verilog simulator (e.g., ModelSim, Vivado Simulator) to simulate the design and testbenches.
2. **Synthesis and Implementation:** Use Xilinx Vivado to synthesize the design and implement it onto a target FPGA.
3. **Hardware Testing:** Download the bitstream to the FPGA and test the router's functionality using a hardware testbench or a software test environment.

**Additional Notes**

* **Timing Constraints:** Ensure proper timing constraints are defined in the Xilinx project to meet the desired performance.
* **Power Optimization:** Consider low-power design techniques to reduce power consumption.
* **Area Optimization:** Optimize the design for area efficiency to fit the target FPGA.
* **Error Handling:** Implement error detection and recovery mechanisms to handle potential issues.

**Future Work**

* Explore advanced routing algorithms for improved performance and flexibility.
* Implement support for different packet formats and priorities.
* Investigate the use of formal verification techniques to increase design confidence.

**For further inquiries or support, please contact:**
* Neeraj Goud Nagunoori => neerajnagunoori12@gmail.com


