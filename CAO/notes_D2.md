# Basic Computer Structure
### This section introduces the fundamentals of computer organisation and architecture, explaining system components, design issues, and different architectural models.
- What is Computer? **DONE✅** 
- Issues in Computer Design...**NOW⭕**
- Von Neumann Architecture...**NOW⭕**
- Harvard Architecture
- Flynn's Taxonomy

---

# 1. Issues in Computer Design

A Computer involves many components that have their own speed, size and power consumption requirements. There are different operating systems that use these computers. Due to different kind of devices and software, the following issues arise in design.

## Performance
Maximising processing speed, memory speed, and I/O performance.
Designing energy-efficient systems for reducing environmental impact and improving battery life.
Processors operate much faster than memory and IO devices, creating a bottleneck that can significantly slow down the overall system.

## Security
Protecting sensitive data from unauthorized access and breaches through robust encryption and authentication.

## Compatibility and User Experience
Ensuring that systems run seamlessly across various operating systems and hardware configurations.
Designing systems that are intuitive and easy for users to operate.

## System Architecture and Infrastructure
Building fault tolerant systems that can withstand and recover from failures without significant downtime.
Modern systems are highly complex, requiring careful management of design, optimization, and integration to avoid excessive costs and development time.

## Resource and Technical Constraints
It must work within the constraints of physical limitations, acknowledging that both computer speed and memory capacity are finite.
Effective techniques are needed to manage memory usage, especially when dealing with large applications or datasets, to prevent slowdowns and crashes.

---

# 2. Von Neumann Architecture

### Von Neumann architecture is a computer design where instructions and data are stored in the same memory space. This means the CPU fetches both instructions and data from the same  memory, using the same pathways.

Historically there have been 2 types of Computers: 

- **Fixed Program Computers** - Their function is very specific, and they couldn't be reprogrammed, e.g., calculators. 
- **Stored Program Computers** - These can be programmed to carry out many different tasks; applications are stored on them, hence the name.

## Components of Von Neumann Architecture
The structure described in the figure outlines the basic components of a computer system, particularly focusing on the memory and processor. It is made up with three main components:

- CPU
- Memory
- I/O Devices

We have these 3 components lets us see more about them in detail:

## CPU (Central Processing Unit)
The central processing unit (CPU) is the main part of a computer that controls how it works. It is made up of the control unit, main memory, and the arithmetic logic unit (ALU). The CPU handles instructions from programs, processes data, stores information, and produces results. Without the CPU, a computer cannot perform tasks or run any applications.

## CU (Control Unit)
The control unit manages how the processor works by sending control signals. It decides how data should move inside the computer, controls input and output operations, and fetches the instructions from memory for execution.

## ALU (Arithmetic and Logic Unit)
The arithmetic and logic unit is the part of the CPU that handles the calculations and decision-making tasks. It performs arithmetic operations like addition and subtraction, logical operations such as comparisons, and tasks like shifting bits in data.

## Registers
Registers are the fastest type of memory located inside the CPU. They temporarily store information that the processor is currently working on, making program execution and operations faster and more efficient. Register serve as the CPU's primary working memory.

- PC (Program Counter): Keeps track of the address of the next instruction to be executed.
- IR (Instruction Register): Holds the current instruction being executed.
- MAR (Memory Address Register): Stores the address of the memory location being accessed.
- MDR (Memory Data Register): Temporarily holds data being transferred to or from memory.
- Accumulator: A register that stores intermediate results of arithmetic and logic operations.
- General Purpose Registers: Used for temporary storage of data during processing.

## Bus
The bus is a communication system that transfers data, addresses, and control signals between the CPU, memory, and I/O devices. In Von Neumann architecture, a single bus is shared for both data and instructions, which can create a bottleneck (known as the Von Neumann bottleneck).

## I/O Bus
- I/O Interface: Connects the CPU and memory to input/output devices.
- Device: Refers to external hardware like keyboards, monitors, or storage devices.

## Key Characteristics
- Single Memory for Data and Instructions: Both data and program instructions are stored in the same memory.
- Shared Bus: A single bus is used for transferring data, addresses, and control signals, which can limit performance.
- Sequential Execution: Instructions are executed one at a time in a sequential manner.

## Von Neumann bottleneck
Whatever we do to enhance performance, we cannot get away from the fact that instructions can only be done one at a time and can only be carried out sequentially. Both of these factors hold back the competence of the CPU. This is commonly referred to as the 'Von Neumann bottleneck'. We can provide a Von Neumann processor with more cache, more RAM, or faster components but if original gains are to be made in CPU performance then an influential inspection needs to take place of CPU configuration. 

## Applications
Von Neumann architecture is the foundation of most modern computing systems, where both instructions and data are stored in the same memory. Here are the some applications:

- Personal Computers and Laptops: Most PCs and laptops (Intel/AMD) use a shared memory that stores both programs and data, enabling efficient running of software like Windows and browsers. Example: Intel Core i7, AMD Ryzen processors.
- Smartphones and Tablets: ARM-based devices use the shared memory model to support multitasking and power efficiency in apps on iOS and Android. Example: Qualcomm Snapdragon, Apple A-series chips
- Embedded Systems:Microcontrollers in cars, IoT devices, and appliances use Von Neumann architecture for simple, cost-effective processing of instructions and data in the same memory. Example Arduino Uno (ATmega328), older ARM Cortex-M designs.
- Servers and Cloud Computing: Servers utilize shared memory systems to handle large-scale software and data tasks for services like AWS and Netflix.
- Gaming Consoles: Consoles like PS5 and Xbox use unified memory to run game code and manage inputs, enabling smooth gameplay.
