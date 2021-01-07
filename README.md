# Cognizant-EV-Charging-Protocol-Gateway-1.0
![alt text](https://github.com/CognizantIoT/Cognizant-EV-Charging-Protocol-Gateway-1.0/blob/main/Gateway.png)
# Current process: 
The Open Charge Point Protocol (OCPP) is an open standard application protocol for communication between Electric vehicle chargers (EVSE) and OCPP Central System. The standard elaborates several standard operations to enable standardized communication between EVSE & Central System.
Central system receives OCPP commands from EV Charger. It then communicates with the Back End System for getting response of OCPP commands. Back end system is responsible for processing OCPP commands, Charge Management, EV User Management, Booking Management, Payments etc. Central System then sends back the response to EV Charger.


# The challenge and the resolution: 
Azure IoT Hub is a popular service in Azure to develop IoT solutions like EV Charge Management that interfaces things / devices like EV Charger. However, OCPP is a specialized protocol for EV Chargers and hence it is not supported by Azure IoT Hub. Cognizant EV Charging Protocol Gateway addresses this challenge by translating OCPP protocol into protocol supported by Azure IoT Hub like AMQP. Using this Gateway, developers can easily develop solutions in Azure using familiar technologies like IoT Hub.
or more details, please refer the Technical Design Document.


# Cognizant EV Charge Management Solution: 
Cognizant has also developed EV Charge Management Solution (i.e. Back End System shown in the High Level Architecture) in Azure and implemented connectivity between EV Charger and Azure messaging services using OCPP with custom development.


# Contact us: 
For more information, please email us: iotmsft@cognizant.com
  
  
