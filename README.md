# FoodComputer_v1.4.2
includes vent control , humidifier control 


Version Control 

For Version 1.1-
Displays temperature read from DS18B20 via ONE WIRE COMMUNICATION at PIN 12 and
Percentage value of Heater ON (PWM at PIN 3).

Setpoint 25 for PID Control
Input For PID is Temperature ( read from DS18B20 )
Output is PWM at pin 3 ( for controlling the heater )

Sample Rate is set for 25 
Default : 100 !

For reference https://github.com/br3ttb/Arduino-PID-Library/blob/master/PID_v1.h


For Version 1.2-
Displays temperature read from DS18B20 via ONE WIRE COMMUNICATION at PIN 12 and
Percentage value of Heater ON (PWM at PIN 3).

Setpoint 25 for PID Control
Input For PID is Temperature ( read from DS18B20 )
Output is PWM at pin 3 ( for controlling the heater )

Prints Intermediate Heater Temperature read from EPCOS Thermistor.


--> Version 1.2.1
Displays temperature read from DS18B20 via ONE WIRE COMMUNICATION at PIN 12 and also from Humidity data from DHT22 at pin 13 
Percentage value of Heater ON (PWM at PIN 3).

Setpoint 31 for PID Control
Input For PID is Temperature ( read from DS18B20 )
Output is PWM at pin 3 ( for controlling the heater )

Prints Intermediate Heater Temperature read from EPCOS Thermistor.

( To make the circuit check the reference Image ! Name : Thermistor_connection_)


--> Version 1.2.2
Displays temperature read from DS18B20 via ONE WIRE COMMUNICATION at PIN 12 and also from Humidity data from DHT22 at pin 13 
Percentage value of Heater ON (PWM at PIN 3).

Setpoint 31 for PID Control
Input For PID is Temperature ( read from DS18B20 )
Output is PWM at pin 3 ( for controlling the heater )

Prints Intermediate Heater Temperature read from EPCOS Thermistor.

2nd Thermistor and Heater included

( To make the circuit check the reference Image ! Name : Thermistor_connection_)

--> Version 1.2.2_ peltier

Runs on previous version too.
Peltier control and fan protection control included by reading tacho input from both the fans ( kept for cold and hot side ) at pin 4 & pin 8.

Peltier relay control at pin 7 and fan relay at 9.


--> Version 1.2.3

Version 1.2.2_peltier + TSL2561 reading ( Luminosity sensor or LIGHT sensor )
and 
decides when to switch on peltier or heater


--> Version 1.2.4

Version 1.2.3 + and 
decides when to switch on peltier or heater

ie when internal temperature is less than set environment temperature (31) then Heater On
and 
when internal temperature is greater than set environment temperature then Peltier cooling system On

this action is decided after 15 seconds reading temperature from dallas temperature sensor placed inside
( allowed 15 seconds for temperature settlement )

For Version 1.3 (mist control using pressure sensors) !! DIDNT WORK !!
V1.2.3 included + readPressure using bmp280(internal pressure) and bme280(external pressure) to determine the water level
at the bottom water tank.

For Version 1.4 (mist control using ultrasonic sensors) !! worked !!
V1.2.3 included + read Waterlevel using Ultrasonic sensor 


--> Version 1.4.x --
1) includes Humidifier ON/OFF CONTROL
2) includes Vent ON/OFF Control

Sooner all the version will be uploaded.. 
