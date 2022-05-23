**GROUP 34**

Getting Started with Temperature Sensor version5.1 and STM32CubeID

**Introduction**
_________________________________________________________________________________

In this simple getting started how to document, we will be building a simple STM32CUBEID project (code) on a simple Temperature and Humidity Sensor uHAT. At its simplest/basic level the whole process of deploying  a code to the Temperature and Humidity Sensor PCB Version 5.1 consists of two “must do'' steps:

→ You would need to set your Temperature and Humidity Sensor with Group34OS, the  host OS which is responsible for  communication with the UCTCloud and also runs the core operations of the device

→  You need to also push your STM32CUBEID project image builder, which is responsible for pulling in all the important   
   dependencies and makes a container image for your fleet.
   
A completion of these steps implies that your Temperature and humidity Sensor Ver 5.1 will start to download the container image, begin your application, and start sending logs to your Group34 dashboard. This has got you at least a step towards success!


**What will you need?**
__________________________________________________________________________________
Hardware:


→ A Temperature and Humidity Sensor uHAT Ver5.1. You can also visit or GitHub repo and check out similar or related
                models.
→  18650-5V Li-ion battery for Power supply(optional) .
→ A simple micro USB mini cable for access to the CH340G transceiver and debugging
→ The micro USB can also be used for power supply.
→ Female connectors 

→ A syringe for water drops to acknowledge and appreciate the functionality of the sensors.
→ The STM32F051 UCT discovery board for the Cortex-M0 microcontroller interfacing.
→ A Group34 account/ link
→ Github account   


Software :
    →  STM32CUBEIDE
     →   Atollic and C are also alternatives but STM32CUBE IDE are strongly recommended

Setting up the Temperature and Humidity Sensor
 _________________________________________________________

Step1: Getting the overall view of the board

The overall view of the PCB is pretty much self explanatory, with the USB connector at the top and extended layer for the battery holder. On either side of the board there are 33x2 connectors, the first ones are female connectors  for mounting the uHAT on the UCT STM32F051 discovery board. The second are for debugging the board itself in a case of damaged pins. In Between the connectors there is a range of peripherals which include the two analog and digital sensors.

Overall View
![image](https://user-images.githubusercontent.com/104798529/169913284-c4d1d511-424b-46f6-9c91-e4e7bc53d049.png)




