# WORK BREAKDOWN STRUCTURE

A work breakdown structure has been created to identify and correctly estimate the time and cost of each possible task in the proposal. Most of task do depend on the progress of each other so they need to be executed in a serial Top-Down approach.
 
## Task Duration
To estimate the time of each task, the beta distribution formula was used, shown below. This formula allows to base the estimated time more on the average time a task may require, giving a more accurate estimation of the time needed to finish a task.

𝐸𝑠𝑡𝑖𝑚𝑎𝑡𝑒𝑑 𝑡𝑖𝑚𝑒 = (𝑜𝑝𝑡𝑖𝑚𝑖𝑠𝑡𝑖𝑐 𝑡𝑖𝑚𝑒 + 4 ∗ 𝑎𝑣𝑒𝑟𝑎𝑔𝑒 𝑡𝑖𝑚𝑒 + 𝑝𝑒𝑠𝑠𝑖𝑚𝑖𝑠𝑡𝑖𝑐 𝑡𝑖𝑚𝑒) / 6 

Each task completion is considered as a Major or Minor Milestone to help us break down the overall Project duration into smaller sprints which reduces the chance of the task falling into overtime, as well as speeding up the possible completion time.

## Milestones :
The milestones for this project have been set in a chronological order, with independent, parallelizable tasks being set at the start, and interdependent tasks being arranged in a serial order and can be done one after the other.

        * Develop the hardware: 
            ** Task: Create an opensource gateware which comprises of softcore RISC-V and peripherals like CAN and Ethernet
            ** Acceptance Criteria: Gateware can be compiled and booted up on a FPGA development board.
            ** Duration: 80 hours

        * Develop the firmware: 
            ** Task: Create opensource firmware which comprises of kernel and device drivers to bring up RISC-V soft core and peripherals like CAN and Ethernet.
            ** Acceptance Criteria: FPGA runs a RISC-V softcore with CAN bus and Ethernet bus communication working.
            ** Duration: 80 hours

        * Develop the middleware: 
            ** Task: Once the hardware and firmware development are complete, the next step is to build the middleware which can support automotive protocols like Diagnostics, Log&Trace and  Measuement&Calibration based on Autosar(AUTomotive Open System ARchitecture) specification.
            ** Acceptance Criteria: Below Automotive protocols are up to make it function like a modern automotive ECU:
                *** DoIP ( Diagnostics over Internet Protocol )
                *** DLT ( Diagnostics Log and Trace ) 
                *** XCP (Universal Measurement and Calibration Protocol ) 
            ** Duration: 80 hours

        * Manufacturing: 
            ** Task: After the prototype has been tested on a development FPGA board as working, the final product can be manufactured. This involves designing and producing the few PCBs available for evaluation by interested end users.
            ** Acceptance Criteria:
                ***  Custom PCB is available with Diagnostic Interface for end user to use the LibreCar ECU. 
                *** Documentation is available to end user how to use the LibreCar ECU with firmware, gateware and PCB design files all available as opensource.
            ** Duration: 80 hours
