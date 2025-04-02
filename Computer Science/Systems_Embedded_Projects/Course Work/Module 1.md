# Module 1: Foundations of Programming and Electronics

---

### **Overview**

This module introduces the fundamentals of C programming and basic electronics concepts necessary for embedded systems. You will learn the core principles of programming, circuit components, and how to apply them in simple embedded projects. Additionally, you will complete assignments, hands-on exercises, and a final project to evaluate your understanding.

---

## **Part 1: C Programming for Embedded Systems**

### **1.1 Setting Up the Development Environment**

#### **Objective:** Install essential tools and write your first C program.

**Step 0: Install Your Development Environment**

1. Install a text editor (VS Code, Sublime Text, or Vim).
    
2. Install the GCC compiler:
    
    ```sh
    sudo apt install gcc
    ```
    
3. Compile and run a simple C program:
    
    ```c
    #include <stdio.h>
    
    int main() {
        printf("Hello, Embedded World!\n");
        return 0;
    }
    ```
    
    Compile and run:
    
    ```sh
    gcc program.c -o program
    ./program
    ```
    

#### **Assignment:**

- Install a C compiler and write a "Hello World" program.
    
- Modify the program to take user input and print a response.
    

---

### **1.2 Basic Syntax and Data Types**

#### **Objective:** Understand variables, operators, and input/output functions.

**Step 1: Learning Variables and Operators**

- Variables and Data Types (`int`, `float`, `char`)
    
- Operators (`+`, `-`, `*`, `/`, `%`)
    
- Input and Output (`scanf`, `printf`)
    

#### **Example:**

```c
#include <stdio.h>
int main() {
    int a, b, sum;
    printf("Enter two numbers: ");
    scanf("%d %d", &a, &b);
    sum = a + b;
    printf("Sum: %d\n", sum);
    return 0;
}
```

#### **Assignment:**

- Create a calculator program that performs basic arithmetic operations.
    
- Experiment with different data types.
    

---

### **1.3 Control Structures**

#### **Objective:** Learn decision-making and loops in C.

**Step 2: Implementing Control Structures**

- If-else statements
    
- Loops (`for`, `while`, `do-while`)
    

#### **Example:**

```c
int i;
for(i = 0; i < 5; i++) {
    printf("Iteration %d\n", i);
}
```

#### **Assignment:**

- Write a program to find the largest of three numbers.
    
- Implement a loop that prints numbers from 1 to 100.
    

---

### **1.4 Functions and Pointers**

#### **Objective:** Learn modular programming and memory handling.

**Step 3: Understanding Functions and Pointers**

- Function syntax and usage
    
- Passing parameters and returning values
    
- Introduction to pointers and memory management
    

#### **Example:**

```c
void greet() {
    printf("Hello from a function!\n");
}
int main() {
    greet();
    return 0;
}
```

#### **Assignment:**

- Create a function to calculate the factorial of a number.
    
- Use pointers to manipulate an array.
    

---

## **Part 2: Basic Electronics for Embedded Systems**

### **2.1 Electrical Basics**

#### **Objective:** Understand voltage, current, and resistance.

**Step 4: Understanding Basic Circuit Components**

- Ohm’s Law: V = IR
    
- Breadboarding basics and circuit simulation tools (Falstad, TinkerCAD)
    

#### **Assignment:**

- Use a circuit simulator to build a simple circuit with a resistor and LED.
    

---

### **2.2 Resistors, Capacitors, and Diodes**

#### **Objective:** Learn about key electronic components.

**Step 5: Learning About Key Components**

- Resistors and their color coding
    
- Capacitor types and functions
    
- Diode polarity and LED working principle
    

#### **Assignment:**

- Calculate resistance values using color codes.
    
- Simulate capacitor charging in a simple RC circuit.
    

---

### **2.3 Using a Multimeter**

#### **Objective:** Learn how to measure voltage, resistance, and continuity.

**Step 6: Using Measurement Tools**

- Measuring voltage across components
    
- Checking resistor values and LED polarity
    

#### **Assignment:**

- Use a real multimeter to measure resistance and voltage in a test circuit.
    

---

## **Hands-on Project: LED Blinking Circuit**

### **Objective:** Write an embedded program to control an LED.

#### **Hardware Requirements:**

- 1x LED
    
- 1x 220Ω Resistor
    
- 1x Breadboard
    
- 1x Arduino (or any microcontroller)
    
- Jumper wires
    

#### **Circuit Setup:**

1. Connect the LED’s longer leg (anode) to a digital output pin on the microcontroller.
    
2. Connect the shorter leg (cathode) to ground (GND) via a 220Ω resistor.
    
3. Upload the following C code (for Arduino):
    
    ```c
    void setup() {
        pinMode(13, OUTPUT);
    }
    void loop() {
        digitalWrite(13, HIGH);
        delay(1000);
        digitalWrite(13, LOW);
        delay(1000);
    }
    ```
    

---

## **Sit-in Project: Traffic Light System**

#### **Objective:** Implement a traffic light system using LEDs.

**Step 7: Traffic Light Implementation**

- Use three LEDs (red, yellow, and green).
    
- Implement timing delays to control the switching of the lights.
    
- Use a button to act as a pedestrian crossing request.
    

#### **Expected Outcome:**

- A working traffic light simulation with timing and pedestrian control.
    

---

## **Resources for Further Learning**

### **Books:**

- "The C Programming Language" by Brian Kernighan and Dennis Ritchie
    
- "Make: Electronics" by Charles Platt
    

### **YouTube Playlists:**

- [Harvard’s CS50: Intro to Programming](https://www.youtube.com/playlist?list=PLhQjrBD2T382gdfveyad09Ierl_3Jh_wR)
    
- [CrashCourse Electronics](https://www.youtube.com/playlist?list=PLFaaszHqAZB1I9U6AdCqBXK82cBZ6lV5E)
    

---

### **Module 1 Summary**

- Learned basic C programming syntax and structure.
    
- Explored basic electronics principles.
    
- Built and tested a simple LED blinking circuit.
    
- Completed a sit-in traffic light project.
    
- Reviewed recommended books and videos.
    

**Next Module: Introduction to Embedded Systems**