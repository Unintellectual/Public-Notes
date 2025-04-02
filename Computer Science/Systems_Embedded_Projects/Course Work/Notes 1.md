# Date: 04-02-2025
## Reference
- Gene Schrodoer Tech course on Bare Metal Embedded Programming: https://www.youtube.com/watch?v=rOaY1oiM1Dc&list=PL4cGeWgaBTe155QQSQ72DksLIjBn5Jn2Z
- Class 1 external docs repo: https://github.com/g-schro/mcu-class-1-external-docs
- Class 1 code: https://github.com/g-schro/mcu-class-1-code

- Prerequisites:
    - Basic knowledge of C language
    - Basic knowledge of computer concepts - CPU, instructions, memory, memory addresses, and hexadecimal numbers.
- Tools and hardware used:
    - STM32 "NUCLEO" board. NUCLEO-F410RE(I can't buy one so I'll be substituting it with NUCLEO-F411RE)
    - GSM module (GT07). (I also don't have that so I'll be substituting with the SIM800L)
    - Power supply. 3v - 24v 2a adjustable power supply

To start learning the value of the components I need are around 1733php not accounting for the delivery cost. This is the cheapest I can get this supplies especially when I added the soldering iron. I did plan on using a STM32H750VBT6 board because it is cheaper but as I've learned the NUCLEO boards have built-in components that are good for learning and prototyping and other boards are bare bones in which I have no knowledge of replicating for now. 

There are not much difference between the two NUCLEO boards but the GSM module does in terms of voltage and it does not have GPS functionality built in:
- **SIM800L:** Operates between **3.4V to 4.4V**, with a preference for **3.7V to 4.2V** and draws significant current (up to 2A during transmission).
- **GT07:** Typically operates at **3.7V to 4.2V** (like SIM800L) and also draws significant current. You would need a separate **4V power supply** or a **DC-DC boost converter** to power the GT07 module properly.



