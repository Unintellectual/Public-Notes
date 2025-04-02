# Coursework: Embedded Systems and Software Engineering

---
### **Course Overview**

This course provides a structured pathway to learning embedded systems and software engineering, covering a variety of micro-controllers, architectures, and embedded platforms. It follows a progressive approach, from fundamental concepts to practical applications, based on the YouTube playlist.

---

### **Prerequisites**

- Familiarity with Linux command line
    
- No prior knowledge of C programming or electronics required
    

---

### **Course Structure**

This course is divided into three stages:

1. **Fundamentals & Simple Projects** - Learning the basics of programming, electronics, and embedded systems through simple exercises and small projects.
    
2. **Intermediate Topics & Medium Projects** - Working with peripherals, communication protocols, and RTOS, leading to medium-sized projects.
    
3. **Advanced Topics & Final Project** - Exploring OS-level programming, power optimization, and embedded Linux while working on a major project.
    

---

### **Stage 1: Fundamentals & Simple Projects**

#### **[[Module 1]]: Foundations of Programming and Electronics**

- Introduction to C programming
    
    - Variables, data types, and operators
        
    - Control structures (if-else, loops)
        
    - Functions and modular programming
        
    - Pointers and memory management
        
- Basic electronics concepts
    
    - Ohm’s Law and circuit fundamentals
        
    - Resistors, capacitors, and diodes
        
    - Breadboarding and circuit simulation tools
        

**Simple Project:** LED Blinking using GPIO

#### **[[Module 2]]: Introduction to Embedded Systems**

- What are embedded systems?
    
- Real-world applications
    
- Microcontrollers vs. Microprocessors
    
- Overview of common microcontroller families (ARM Cortex, AVR, PIC, RISC-V)
    
- Setting up the development environment (Linux toolchain, GCC, OpenOCD, VS Code, PlatformIO)
    

**Simple Project:** Button-controlled LED

#### **[[Module 3]]: Micro-controller & Processor Architecture**

- Overview of different architectures (ARM, RISC-V, x86, MIPS)
    
- Memory organization (RAM, Flash, Registers, Cache)
    
- Clock and power management
    
- Peripherals and their functions
    

#### **[[Module 4]]: Development Tools & Debugging**

- Using IDEs (VS Code, STM32CubeIDE, Keil, PlatformIO)
    
- Writing and compiling code using GCC toolchain
    
- Flashing firmware using OpenOCD, ST-Link, and J-Link
    
- Debugging with GDB and printf debugging techniques
    

**Simple Project:** Using serial output for debugging

#### **[[Module 5]]: GPIO and Basic Peripherals**

- Configuring GPIO pins as input/output
    
- Interfacing with LEDs and push buttons
    
- Using internal pull-up/pull-down resistors
    
- Handling debouncing
    

**Simple Project:** Traffic light simulation with LEDs

---

### **Stage 2: Intermediate Topics & Medium Projects**

#### **[[Module 6]]: Timers & PWM**

- Introduction to timers and their types
    
- Configuring basic and advanced timers
    
- Generating PWM signals for LED dimming and motor control
    

**Medium Project:** LED brightness control with a potentiometer

#### **[[Module 7]]: Interrupts & Low-Level Programming**

- Understanding NVIC and ISR handling
    
- Writing interrupt-based applications
    
- Low-power modes and wake-up sources
    

**Medium Project:** Motion detector with interrupt-based sensor

#### **[[Module 8]]: Communication Protocols**

- UART: Serial communication with PC
    
- SPI: Communicating with sensors and displays
    
- I2C: Interfacing with external EEPROMs and sensors
    
- CAN bus basics
    
- USB communication and HID devices
    

**Medium Project:** OLED display with I2C communication

#### **[[Module 9]]: RTOS and Multi-Threading**

- Introduction to Real-Time Operating Systems (RTOS)
    
- Using FreeRTOS with various microcontrollers
    
- Creating and managing tasks, queues, and semaphores
    

**Medium Project:** Multi-tasking LED control using FreeRTOS

#### **[[Module 10]]: ADC, DAC, and Sensors**

- Introduction to ADC (Analog-to-Digital Conversion)
    
- Using the ADC to read sensor data
    
- Generating analog signals with DAC
    
- Interfacing with temperature and light sensors
    

**Medium Project:** Digital thermometer using ADC and LCD display

#### **Module 11: Storage and File Systems**

- Reading/writing to SD cards
    
- Implementing FAT file system
    
- Using EEPROM for persistent storage
    

**Medium Project:** Data logger with SD card storage

---

### **Stage 3: Advanced Topics & Final Project**

#### **Module 12: Power Management & Optimization**

- Low-power states and sleep modes
    
- Energy-efficient coding practices
    
- Measuring power consumption
    

#### **Module 13: Embedded Linux & Advanced Topics**

- Introduction to Embedded Linux
    
- Working with Yocto and Buildroot
    
- Device drivers and kernel modules
    
- Interfacing with external peripherals in Linux
    

**Advanced Project:** Embedded Linux-based data collector

#### **Module 14: Operating Systems & Systems Programming**

- How operating systems work: kernel, shell, and user space
    
- Understanding system calls and process management
    
- Memory management and virtual memory
    
- Filesystems and storage management
    
- Writing low-level systems programs in C
    
- Interfacing embedded systems with Linux-based applications
    

**Advanced Project:** Writing a simple device driver for Linux

#### **Module 15: Security in Embedded Systems**

- Secure boot and firmware updates
    
- Cryptography and secure communication
    
- Memory protection and access control
    

**Advanced Project:** Secure IoT device communication

#### **Module 16: Networking in Embedded Systems**

- TCP/IP stack in embedded devices
    
- MQTT, CoAP, and HTTP for IoT applications
    
- Configuring embedded Wi-Fi and Bluetooth
    

**Advanced Project:** IoT sensor node with cloud connectivity

#### **Module 17: FPGA and Hardware Acceleration Basics**

- Introduction to FPGAs vs. microcontrollers
    
- Using Verilog/VHDL for hardware description
    
- Combining embedded processors with FPGA logic
    

**Advanced Project:** FPGA-based signal processing module

#### **Module 18: Final Project**

- Designing and implementing a real-world embedded system
    
- Project ideas:
    
    - Data logger with sensor readings
        
    - Smart home automation system
        
    - Motor control for robotics
        
    - Custom HID device (keyboard/mouse emulator)
        
    - Embedded Linux-based IoT gateway
        
- Code review and debugging
    
- Presentation and documentation
    


---

### **Development Environment Setup (Linux)**

1. Install GCC ARM toolchain:
    
    ```sh
    sudo apt install gcc-arm-none-eabi gdb-multiarch openocd
    ```
    
2. Install PlatformIO for multi-platform development
    
3. Set up ST-Link, J-Link, or other debugging interfaces
    
4. Test setup by compiling and flashing a basic LED blink program
    

---
