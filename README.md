**GROUP 34**
Introduction

TheTemperature-Light sensor is a system that monitors and records
the temperature and light of a room or any place under consideration such that if the
temperature and the light are higher than required, the system displays it on the
computer. Similarly, if the temperature and the light are lower, the system displays it.
This System can also be connected to external Temperature/Light controllers.
Temperature/Light controller can be manual or automatic. The former requires full
human intervention to operate, while the latter requires little or not at all.
Furthermore, most temperature/light controller and related systems designed make
used of discrete components design such as timers, counters, decoder drivers and
thermistor temperature sensor and some use microcontrollers with external analogue
to digital converter (ADC) which is recommended for this system.
This system is powerful and very easy-to-program. It has 33-pins, and it has a
memory of 256-KB I2C of EEPROM data memory, self-programming.
Operating voltage range between 2V to 5V

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


Step2: Soldier and connect the female connectors on the board, These female connectors enable the PCB to be logged on the STM32f051 discovery board.
If soldered and connected correctly you have something like this: 

![image](https://user-images.githubusercontent.com/104798529/169913581-71daf7d9-c91e-494c-8bae-068c3ef2a72a.png)


Step 3: Plugging the board to a power source.

This step is a 2 in 1 where we will be powering the PCB using the micro USB and deploying a code for the board to be able send information to the microcontroller.

Plugged board:

![image](https://user-images.githubusercontent.com/104798529/169913617-b8e48cdd-e321-4dad-9b34-6c83d0465e83.png)


OPTIONAL:
The uHAT uses two sources of power, the USB and the Battery. You can also use the 5V Li-ion battery(18650)  but this step is optional because you would still need to connect the USB cable to send and receive information to the microcontroller. 

DEPLOYING THE CODE
________________________________________________________________________________________________________

This section covers the codes that are supposed to be written on the STM32CUBE IDE which sends this information (code) to the microcontroller, 

Step4 : Run the STM32CUBE IDE
Open and run the Stm32cube ide and copy and paste the following code on the references.
1.  

![image](https://user-images.githubusercontent.com/104798529/169913675-653ad4cf-55d7-4585-ab35-4ec0b90a3e93.png)

2.

![image](https://user-images.githubusercontent.com/104798529/169913738-c7c8b4e0-acc4-4bdf-848a-bd47e93eebc3.png)

3.

![image](https://user-images.githubusercontent.com/104798529/169913753-b95e6fff-f8db-4e82-b0e8-e606707c8348.png)

CONGRATULATIONS🥳, the Temperature and Humidity sensor is now fully functional, you can proceed to test the functionality of the board, we are looking forward to seeing you on version 6.


