# Shared Resource
This project is an implementation of a system based on STM32 that analyze contetion problems when tasks accessing shared resource function in a multitasking system.

## Description
This project provides practical examples to understand how contention can occur and why they can become problematic. There are two tasks accessing the AccessSharedData function. One task has higher priority. When the lower-priority task accesses the function (StartFlag = 0) and is performing a write or read operation, the higher-priority task also accesses the same function. This leads to contention. As a result, the previous task cannot complete its work and returns to its initial state to start its task again.

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
   - Check StartFlag
   - If StartFlag up (1), put it down (0)
   - Else show an alert
   - Simulate read/write operation
   - Set back StartFlag up

## Hardware Used
- STM32 Microcontroller
- LED
- Resistor

## Demo Video
