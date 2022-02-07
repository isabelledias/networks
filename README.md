# networks
## Network assignment for Supervisory Control and PLC simulation
Frameworks used:
  - AWS
  - Node-RED
  - ScadaBR

We used AWS Educate to create two virtual machines, one for the supervision system and another representing a PLC. In the supervision VM we installed ScadaBR, and the PLC was simulated using Node-RED.

To know how to install ScadaBR please refer to: http://forum.scadabr.com.br/t/scadabr-1-2-instalando-no-linux/3825

To install Node-RED on your AWS instance please refer to: https://nodered.org/docs/getting-started/aws#running-on-aws-ec2-with-ubuntu

OBS: Please remember to configure a port in your node-RED VM that will connect via Modbus to our Supervisory System, in my example, I used port 10502.

Presentation Link (in Portuguese): https://www.youtube.com/watch?v=8tHapLZrnW4

## AWS Config
Security rules for our PLC (Node-RED Machine):

![image](https://user-images.githubusercontent.com/53828752/152714649-7f0d6772-3e14-4727-b72a-69b568fa1421.png)

Security rules for the Supervisory Control (ScadaBR Machine):
![image](https://user-images.githubusercontent.com/53828752/152714724-1c5473c6-ce52-4ae2-995f-e0469fcbd2dd.png)

## Node-RED Flow
![image](https://user-images.githubusercontent.com/53828752/152714910-17c07d8d-b96b-45e9-aa58-ec2abb13f11a.png)

![image](https://user-images.githubusercontent.com/53828752/152714894-ed67a7e5-de94-4e1e-9073-09cd7a7da175.png)

## ScadaBR
Graphic Interface:
![Captura de tela 2022-02-06 225406](https://user-images.githubusercontent.com/53828752/152715024-23a15a1a-8921-4dc8-9a9e-e65b516109f8.png)

Data Source and Data Points Config:

![image](https://user-images.githubusercontent.com/53828752/152715071-395638da-fdc0-44da-bb7a-d86f1a88af5f.png)
![image](https://user-images.githubusercontent.com/53828752/152715077-77311a87-f8b7-4223-bd8c-40a0aa16bb63.png)

