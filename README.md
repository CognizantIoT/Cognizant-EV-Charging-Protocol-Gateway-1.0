# Cognizant-EV-Charging-Protocol-Gateway-1.0
Cognizant EV Charging Protocol Gateway translates data/commands generated by EV Charger implementing OCPP protocol into a protocol supported by Azure IoT Hub (AMQP). Thus is greatly simplifies development of EV Charge Management solution using Azure IoT services without having intricate knowledge of OCPP.
# Background: 
The Open Charge Point Protocol (OCPP) is an open standard application protocol for communication between Electric vehicle chargers (EVSE) and OCPP Central System. The standard elaborates several common operations to enable standardized communication between EVSE & Central System. 
Central System receives OCPP commands from EV Charger. It then communicates with the EV Charge Management system, typically over REST APIs, for getting response of OCPP commands. EV Charge Management system is responsible for processing OCPP commands, Charge Management, EV User Management, Booking Management, Payments etc. OCPP Central System then sends back the response to EV Charger.
![alt text](https://github.com/CognizantIoT/Cognizant-EV-Charging-Protocol-Gateway-1.0/blob/main/Without%20Gateway.png)
# Challenge: 
Azure IoT Hub is a Microsoft Azure based service to develop IoT solutions like EV Charge Management that interfaces things / devices like EV Charger and supports popular protocols like AMQP, MQTT, HTTP. It provides a lot of specialized features for IoT solutions including device management and high scale telemetry data ingestion. However, OCPP being a specialized protocol for EV Chargers is not supported by Azure IoT Hub. Hence, there is no easy way to develop an EV Charge Management solution using Azure IoT Hub.
# Solution:
Cognizant EV Charging Protocol Gateway addresses this challenge by translating OCPP protocol into protocol supported by Azure IoT Hub like AMQP. Using this Gateway, EV Chargers data can be routed to Azure IoT Hub to fully utilize Azure IoT Hub capabilities. Thus, it allows the developers to develop EV Charge Management solution with familiar and powerful Azure IoT services.
![alt text](https://github.com/CognizantIoT/Cognizant-EV-Charging-Protocol-Gateway-1.0/blob/main/With%20Gateway.png)
For more details, please refer the Technical Design Document.
# Cognizant EV Charge Management Solution: 
Cognizant has also developed its own EV Charge Management Solution using Azure IoT services that leverages this Cognizant EV Charging Protocol Gateway and implements use cases like Charging Schedule Management, Pricing Management, Automatic Demand Response, Smart Charge Management, etc.
# Contact us: 
For more information on Cognizant EV Charging Protocol gateway and EV Charge Management solution, please email us: iotmsft@cognizant.com 
  
