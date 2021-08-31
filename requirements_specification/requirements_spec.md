# Requirements Specification
The project name: "Auto-Fan System"

This module sends IR signals in order to automate a fan which is controlled by a set of IR signals.

In a certain hours of a day, it decides to turn on or off of a fan on a following condition.

 - If humidity or temperature of the room is "high", then the module send a signal to make a fan turn on.

Otherwise, turn off for saving energy.

 
The settings for the conditions can be configured via web server running on the module. For example,

 - Let a fan work in what hours?
 - How high the temperature or humidity is to turn on?
 
In the html page, a fan can be turned on or be changed the power manually.

It should be permanently connected the household router in order to perform the web application.

## How to use
 - Set the module in order to 

## Components
 - A NodeMCU development board
    - A Wifi module which is pre-installed on the board
 - An IR signal emitter
 - A temprature and humidity sensor module

## Constraints
 - On and off signal might be same as a fan toggles the on and off states.
 - Similarly, changing the power of a fan might be done by the same signal.
 - 5V power supply with MicroUSB is needed.
 - The number of analog inputs of the NodeMCU is only one.
 - It can not learn the IR signal so it works with one specific model.
