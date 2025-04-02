# Module 3: Interfacing with Peripherals & Communication Protocols

---

### **Overview**

This module covers interfacing micro-controllers with peripherals such as sensors, displays, and communication modules. You will learn about common communication protocols used in embedded systems and apply them in hands-on projects.

---

## **Part 1: Peripheral Interfacing**

### **3.1 GPIO (General-Purpose Input/Output)**

#### **Objective:** Learn how to control input and output pins.

**Key Concepts:**

- Configuring GPIO pins as input or output
    
- Using internal pull-up and pull-down resistors
    
- Reading digital input from buttons/switches
    
- Controlling LEDs and buzzers
    

#### **Assignment:**

- Toggle an LED using a button.
    
- Read a switch input and control a buzzer.
    

---

### **3.2 Analog Inputs and ADC (Analog-to-Digital Conversion)**

#### **Objective:** Understand how to read sensor data using ADC.

**Key Concepts:**

- Introduction to ADC
    
- Sampling and resolution (8-bit, 10-bit, 12-bit)
    
- Reading data from a potentiometer or temperature sensor
    

#### **Assignment:**

- Read the value of a potentiometer and display it on a serial monitor.
    
- Interface a temperature sensor (LM35) and print readings.
    

---

## **Part 2: Communication Protocols**

### **3.3 UART (Universal Asynchronous Receiver-Transmitter)**

#### **Objective:** Learn serial communication between microcontrollers and computers.

**Key Concepts:**

- Basics of UART communication
    
- Setting baud rate and data frame format
    
- Sending and receiving data over a serial monitor
    

#### **Assignment:**

- Transmit "Hello, UART!" from a microcontroller to a PC.
    
- Implement UART-based communication between two microcontrollers.
    

---

### **3.4 SPI (Serial Peripheral Interface)**

#### **Objective:** Understand SPI communication for high-speed data transfer.

**Key Concepts:**

- Master-slave configuration
    
- MOSI, MISO, SCK, CS pin functions
    
- Communicating with an SPI-based sensor (e.g., an accelerometer)
    

#### **Assignment:**

- Read data from an SPI sensor and display it.
    
- Implement SPI communication between two microcontrollers.
    

---

### **3.5 I2C (Inter-Integrated Circuit)**

#### **Objective:** Learn about I2C communication and multi-device interfacing.

**Key Concepts:**

- I2C master-slave communication
    
- Addressing and data transmission
    
- Communicating with an I2C-based sensor (e.g., OLED display, EEPROM)
    

#### **Assignment:**

- Interface an I2C-based temperature sensor and display data.
    
- Read data from an I2C EEPROM and write new data to it.
    

---

## **Hands-on Project: Displaying Sensor Data on an OLED**

#### **Objective:** Combine ADC and I2C communication to display real-time sensor data.

**Project Requirements:**

- Read temperature sensor data.
    
- Use I2C to display values on an OLED screen.
    

#### **Expected Outcome:**

- A working system that shows live temperature readings on an OLED display.
    

---

## **Resources for Further Learning**

### **Books:**

- "Embedded Systems with ARM Cortex-M Microcontrollers" by Alexander G. Dean
    
- "Mastering the I2C Bus" by Vincent Himpe
    

### **YouTube Playlists:**

- [I2C & SPI Communication](https://www.youtube.com/playlist?list=PLmOP2B89bZc2tVE3qLPJVGKp-Fzstc02P)
    
- [UART Serial Communication](https://www.youtube.com/playlist?list=PLFaaszHqAZB0u0YZjYJHElR5KeLjxzDxr)
    

---

### **Module 3 Summary**

- Learned to configure GPIO for input and output.
    
- Explored ADC for reading analog sensor data.
    
- Understood UART, SPI, and I2C communication protocols.
    
- Completed a hands-on project displaying sensor data on an OLED.
    

**Next Module: Timers and Interrupts in Embedded Systems**