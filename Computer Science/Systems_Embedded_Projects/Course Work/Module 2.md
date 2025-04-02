# Introduction to Embedded Systems

---

### **Overview**

This module introduces the fundamentals of embedded systems, covering microcontroller architecture, real-time constraints, and the basics of firmware development. You will gain hands-on experience with basic microcontroller operations and apply your knowledge to a small project.

---

## **Part 1: Understanding Embedded Systems**

### **2.1 What is an Embedded System?**

#### **Objective:** Understand what defines an embedded system and its applications.

**Key Concepts:**

- Definition and characteristics of embedded systems
    
- Comparison with general-purpose computers
    
- Applications in consumer electronics, automotive, healthcare, and industrial automation
    

#### **Assignment:**

- Research five different embedded systems used in everyday life and describe their purpose and components.
    
- Compare an embedded system with a general-purpose computer.
    

---

### **2.2 Microcontroller vs Microprocessor**

#### **Objective:** Understand the difference between microcontrollers and microprocessors.

**Key Concepts:**

- Definitions and comparisons
    
- Architectural differences (Harvard vs. Von Neumann)
    
- Examples of popular microcontrollers and microprocessors (STM32, AVR, ESP32, ARM Cortex-M)
    

#### **Assignment:**

- List and compare three different microcontrollers, detailing their specifications and applications.
    
- Identify a real-world product that uses a microcontroller and explain its function.
    

---

### **2.3 Introduction to Microcontroller Architecture**

#### **Objective:** Learn the basic architecture of a microcontroller.

**Key Concepts:**

- CPU, RAM, ROM, Flash Memory
    
- GPIO (General Purpose Input/Output)
    
- Peripherals (Timers, ADC, PWM, UART, SPI, I2C)
    
- Power management
    

#### **Assignment:**

- Draw a block diagram of a microcontroller and label its main components.
    
- Explain the function of each component in one paragraph.
    

---

## **Part 2: Getting Started with a Microcontroller**

### **2.4 Setting Up the Development Environment for Microcontrollers**

#### **Objective:** Set up a basic development environment for embedded programming.

**Steps:**

1. Install a toolchain for embedded development (GCC ARM, STM32CubeIDE, PlatformIO, etc.).
    
2. Install a serial monitor tool (minicom, picocom, PuTTY).
    
3. Connect a microcontroller to your Linux machine and verify detection.
    
4. Write a basic firmware program in C that turns an LED on and off.
    

#### **Assignment:**

- Install the necessary software for microcontroller development.
    
- Write a C program to blink an LED on an STM32 or Arduino.
    
- Upload and test the program.
    

---

## **Hands-on Project: LED Blinker with Button Input**

#### **Objective:** Expand on the LED blinking project by adding button input functionality.

**Project Requirements:**

- An LED controlled by a button.
    
- When the button is pressed, the LED should toggle on or off.
    
- Debounce the button input using software.
    

#### **Expected Outcome:**

- A working LED-button circuit where pressing the button toggles the LED state.
    

---

## **Resources for Further Learning**

### **Books:**

- "Embedded Systems: Introduction to ARM Cortex-M Microcontrollers" by Jonathan Valvano
    
- "Exploring the STM32" by Geoffrey Brown
    

### **YouTube Playlists:**

- [Embedded Systems with STM32](https://www.youtube.com/playlist?list=PLnMKNibPkDnFThkIf9pSABzunEbzP9m2z)
    
- [Introduction to Microcontrollers](https://www.youtube.com/playlist?list=PLNBEWBj3q_cBf3m8ly1WOnRjBaMxOiK9V)
    

---

### **Module 2 Summary**

- Introduced embedded systems and their applications.
    
- Explored microcontroller vs. microprocessor differences.
    
- Learned about microcontroller architecture and peripherals.
    
- Set up a development environment for microcontrollers.
    
- Completed a hands-on LED blinking project with button input.
    

**Next Module: Interfacing with Peripherals & Communication Protocols**