# User Interface

## Diagnostic Interface
The user has On-Board Diagnostics version 2 (OBD-II) as an interface to the Diagnosis Bus of the LibreCar ECU.
Below steps are used to send a signal:

* **Establish a connection**: First, you need to establish a connection between the LibreCar OBD-II module and the diagnostic tool. This can be done using a wired or wireless connection. For example, you can connect the LibreCar OBD-II module to a Wi-Fi access point and use a diagnostic tool connected to the same network to communicate with it.

* **Set up LibreCar OBD-II module**: Once the connection is established, you need to configure the LibreCar OBD-II module to communicate over IP. This can be done by setting the IP address and other network parameters.

* **Identify the OBD-II commands**: The OBD-II standard defines a set of commands that can be used to communicate with the different ECUs in the vehicle. You need to identify the OBD-II commands that are relevant to the diagnostic data you are trying to retrieve.

* **Send the OBD-II commands over IP**: Once you have identified the relevant OBD-II commands, you can send them over IP to the OBD-II device. You can use a diagnostic tool or a custom application to send the OBD-II commands.

* **Receive the response**: Once the OBD-II commands are sent,  LibreCar OBD-II module will respond with the diagnostic data in the form of a response message. You can then parse the response message to extract the diagnostic data you need.

## REST API Interface

The user also has REST APIs availble over http to directly talk to services in the LibreCar ECU:

# Core APIs
  +  HelloWorldPublisher - Publish a message from a node to the Vehicle bus.
  +  HelloWorldSubscriber - Subscribe a node to messages on the Vehicle bus.
  +  Publish & Subscribe - Use publish/subscribe routines.
  +  Sample Application - Create an application node.
# Device APIs
  +  Ethernet Reader - Read data from a network device.
  +  Ethernet Writer - Write data to a network device.
  +  CAN Reader - Read data from a CAN device.
  +  CAN Writer - Write data to a CAN device.
