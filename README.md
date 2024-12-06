# Access Contention Problems When Using Shared Resource in a Multitasking System
This project is an implementation of a system based on STM32 that analyze contetion problems when tasks accessing shared resource function in a multitasking system.

## Description
This project provides a practical example to understanding about how contention can occure and why it can be a problem. There are two tasks that access the AccessSharedData function. One of the tasks has a higher priority. When 

## Task Overflow
1. **Initialization**
   - Configure GPIO of LED
   - Create tasks, with red LED task having highest priority
3. **Start Green Flashing Task**
   - Turn the Green LED ON
   - Accessing shared data function
   - Turn the Green LED OFF
   - Delay for 0.5 seconds
5. **Start Red Flashing Task**
   - Turn the Red LED ON
   - Accessing shared data function
   - Turn the Red LED OFF
   - Delay for 0.1 seconds
7. **Access Shared Data**
   - 

## Hardware Used
- STM32 Microcontroller
- LED
- Resistor

## Demo Video
