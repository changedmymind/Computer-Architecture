A register is a memory block that exists inside a CPU. They store data temporarily so its volatile (it gets re-written almost every clock cycle depending on how the controls are set), generally used for computation (cache stores frequently used data, even instructions). It is directly integrated into specific sections of the CPU, like for example the ALU to store operands, and it runs at the same speed as the CPU which makes it extremely fast. They usually store from 8 to 64 bits.

The main differences between a register and cache are the following:

![image](https://github.com/user-attachments/assets/2efdc717-56dd-41a3-b534-676acb00ab77)


At a hardware level registers are no other than combination of flip flops. Since 1 flip-flop stores 1 bit of data, to make an 8 bit register and arrange of 8 flip-flop in parallel is made.
So, every register is composed of multiple flip-flops in parallel. As such, the register is activated by a shared clock signal that synchronices them. Also it has control circuitry that determines when the registers: load data, holds data and outputs data. So data can be written, read and stored (temporarily).

Because registers are built using flip-flops that means that they run at the same speed than the CPU, but at the same time, this makes them less dense in terms of data because flip-flops occupy much more space than SRAM (like cache) or DRAM (RAM)

There are many types of registers like: general purpose, special purpose, floating point, control, memory address, accumulator, etc.
A modern CPU would have approximately 500 registers.

The way they work is:
- the CPU fetches data from memory a writes it in the registers
- the data get processed
- the processed data gets written onto memory

For example: the CPU loads two numbers R1 and R2. Then the ALU would perfom an operation with this two numbers and would write the result in another register R3. If needed R3 would get written in memory.

They are mainly used because they are much faster than cache and RAM.

All levels of memory in cache (L1, L2, and L3) communicate with each other, and data can jump between them.

Registers are usually made from a faster SRAM type than cache.

![image](https://github.com/user-attachments/assets/2b74bfd6-884b-4235-9880-f41e8e735af6)


