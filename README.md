Project Overview
This project implements the core functionalities of a car black box system using a PIC microcontroller. The system continuously monitors and logs important events (such as collisions) and stores this data in EEPROM memory for post-event analysis. Designed as a foundation for vehicle monitoring systems, this project can be extended to any vehicle requiring event logging and analysis.
Features

Event Logging: Records critical vehicle events with timestamps
Collision Detection: Monitors for potential collision events
Secure Access: Password protection for accessing logged data
Real-Time Clock: Maintains accurate timestamps for each event
Data Persistence: Stores event logs in non-volatile EEPROM memory
User Interface: Character LCD display for system status and data viewing
Input Control: Digital keypad for user interaction and configuration

Technologies Used

PIC Microcontroller
Communication Protocols:

I2C for interfacing with peripherals
UART for serial communication


Peripheral Devices:

Character LCD (CLCD) for display
Real-Time Clock (RTC) for time tracking
EEPROM for data storage
Digital keypad for user input


Hardware Features:

ADC for sensor reading
Timers for event scheduling
Interrupt handling for real-time response

Software Requirements

MPLAB X IDE
XC8 Compiler
picsimlab-simulator

Implementation Details

System operates in different modes (logging, viewing, configuration)
Events are timestamped using the RTC module
Data is written to EEPROM in a circular buffer pattern
Password protection uses a timeout mechanism after multiple failed attempts
Long press vs. short press detection for different functions
