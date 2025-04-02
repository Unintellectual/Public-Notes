# Module 6: Real-Time Operating Systems (RTOS) and Multithreading

---

### **Overview**

This module introduces the concept of Real-Time Operating Systems (RTOS), task scheduling, inter-task communication, and multithreading. You will explore FreeRTOS, a popular open-source RTOS, and implement real-time applications using an embedded microcontroller.

---

## **Part 1: Introduction to RTOS**

### **6.1 Understanding Real-Time Systems**

#### **Objective:** Learn the fundamentals of real-time systems and their classifications.

**Topics Covered:**

- Hard vs. Soft Real-Time Systems
    
- Deterministic Execution
    
- Scheduling Algorithms: Rate Monotonic, Earliest Deadline First (EDF)
    

#### **Assignment:**

- Research real-world applications of RTOS in aerospace, automotive, and industrial control systems.
    
- Write a short essay on the differences between a general-purpose OS and an RTOS.
    

---

### **6.2 Introduction to FreeRTOS**

#### **Objective:** Learn how FreeRTOS works and its core components.

**Topics Covered:**

- Tasks and Task Scheduling
    
- Preemptive vs. Cooperative Multitasking
    
- Time Slicing and Task Priorities
    

#### **Assignment:**

- Install FreeRTOS on your STM32 microcontroller.
    
- Write a program that creates two tasks with different priorities and observes their execution.
    

---

## **Part 2: Task Management and Synchronization**

### **6.3 Creating and Managing Tasks**

#### **Objective:** Learn how to create and manage tasks in FreeRTOS.

**Topics Covered:**

- Task Creation (`xTaskCreate`)
    
- Task Deletion (`vTaskDelete`)
    
- Task States (Running, Ready, Blocked, Suspended)
    

#### **Example Code:**

```c
void Task1(void *pvParameters) {
    while (1) {
        printf("Task 1 Running\n");
        vTaskDelay(pdMS_TO_TICKS(1000));
    }
}

void Task2(void *pvParameters) {
    while (1) {
        printf("Task 2 Running\n");
        vTaskDelay(pdMS_TO_TICKS(500));
    }
}

int main() {
    xTaskCreate(Task1, "Task1", 1000, NULL, 1, NULL);
    xTaskCreate(Task2, "Task2", 1000, NULL, 2, NULL);
    vTaskStartScheduler();
}
```

#### **Assignment:**

- Modify the example to create a third task that has the lowest priority.
    
- Experiment with different priorities and observe how task execution changes.
    

---

### **6.4 Inter-task Communication**

#### **Objective:** Learn message passing and synchronization techniques in RTOS.

**Topics Covered:**

- Queues (`xQueueCreate`, `xQueueSend`, `xQueueReceive`)
    
- Semaphores (`xSemaphoreCreateBinary`, `xSemaphoreTake`, `xSemaphoreGive`)
    
- Mutexes and Priority Inversion
    

#### **Example Code:**

```c
QueueHandle_t xQueue;

void SenderTask(void *pvParameters) {
    int data = 100;
    while (1) {
        xQueueSend(xQueue, &data, portMAX_DELAY);
        vTaskDelay(pdMS_TO_TICKS(500));
    }
}

void ReceiverTask(void *pvParameters) {
    int receivedData;
    while (1) {
        xQueueReceive(xQueue, &receivedData, portMAX_DELAY);
        printf("Received: %d\n", receivedData);
    }
}

int main() {
    xQueue = xQueueCreate(10, sizeof(int));
    xTaskCreate(SenderTask, "Sender", 1000, NULL, 2, NULL);
    xTaskCreate(ReceiverTask, "Receiver", 1000, NULL, 1, NULL);
    vTaskStartScheduler();
}
```

#### **Assignment:**

- Implement a producer-consumer model using FreeRTOS queues.
    
- Modify the code to add a second producer task and observe changes in execution.
    

---

## **Part 3: Timers, Interrupts, and Resource Management**

### **6.5 Using Timers and Interrupts in RTOS**

#### **Objective:** Learn how to use software timers and integrate hardware interrupts with RTOS.

**Topics Covered:**

- Software Timers (`xTimerCreate`, `xTimerStart`)
    
- Hardware Interrupt Service Routines (ISRs)
    
- Synchronizing ISRs with Tasks
    

#### **Assignment:**

- Implement a periodic timer that toggles an LED every second.
    
- Modify the program to use an external interrupt (e.g., button press) to reset the timer.
    

---

### **6.6 Memory Management in RTOS**

#### **Objective:** Learn about dynamic memory allocation and fragmentation.

**Topics Covered:**

- Static vs. Dynamic Memory Allocation
    
- Heap Management in FreeRTOS
    
- Avoiding Memory Leaks
    

#### **Assignment:**

- Implement a program that dynamically allocates memory for an array and frees it after use.
    
- Observe how FreeRTOS handles memory allocation using `heap_4.c`.
    

---

## **Sit-in Project: Real-Time Data Logger**

### **Objective:** Create a real-time data logging system using FreeRTOS.

#### **Project Description:**

- Read sensor data (e.g., temperature) periodically using FreeRTOS tasks.
    
- Store the data in an SD card or transmit it via UART.
    
- Implement a queue to manage data transfer between tasks.
    

#### **Expected Outcome:**

- A working data logger that stores sensor readings efficiently in real time.
    

---

## **Resources for Further Learning**

### **Books:**

- "Real-Time Concepts for Embedded Systems" by Qing Li
    
- "Mastering FreeRTOS" by Richard Barry
    

### **YouTube Playlists:**

- [Embedded Systems with FreeRTOS](https://www.youtube.com/playlist?list=PLn8PRpmsu08pQBgjxYFXSsODEF3JQmm-y)
    
- [Understanding RTOS Basics](https://www.youtube.com/playlist?list=PLtRtbw8Pm63phP3Lfzz_DF_xTyzUjEUx9)
    

---

### **Module 6 Summary**

- Learned the fundamentals of RTOS and task scheduling.
    
- Implemented FreeRTOS tasks, queues, and semaphores.
    
- Explored timers, interrupts, and memory management in RTOS.
    
- Built a real-time data logger as a sit-in project.
    

**Next Module: Embedded Communication Protocols**