# Introduction

The ECU is a microprocessor-based system that receives input from various sensors, analyzes the data, and controls various driving functions based on the input. LibreCar is a small and affordable Engine Control Unit (ECU), an electronic control module that manages control of an automotive vehicle. 

LibreCar comprises of:
* opensource hardware
    * Opensource softcore of RISC-V
    * Digital peripheral IPs for CAN and Ethernet
* opensource software
    * Device drivers for CAN and Ethernet
    * Middleware based on AUTOSAR specification for Automotive protocols

LibreCar embodies both CAN Bus (Controller Area Network) or over Automotive Ethernet Bus, a switched network used in the automotive field to enable supporting modern automotive protocols listed below: 
* DoIP ( Diagnostics over Internet Protocol )
* DLT ( Diagnostics Log and Trace ) 
* XCP ( Universal Measurement and Calibration Protocol ) 

