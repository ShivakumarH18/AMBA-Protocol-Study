# AMBA Protocol Study

## 📘 Project Overview
This repository contains a detailed theoretical study of the AMBA (Advanced Microcontroller Bus Architecture) protocol developed by ARM. The study focuses on understanding the architecture, purpose, and working principles of different AMBA bus protocols used in modern SoC design.

### 1️⃣ AMBA Architecture
- Purpose of AMBA in System-on-Chip (SoC) design
- Bus hierarchy and modular architecture
- Role of bridges between bus domains

### 2️⃣ APB (Advanced Peripheral Bus)
- Used for low-speed peripherals
- Two-phase transfer: Setup and Access
- Signals: PSEL, PENABLE, PWRITE, PREADY
- Read and Write timing behavior

### 3️⃣ AHB (Advanced High-performance Bus)
- Medium-speed bus
- Address and Data phase separation
- Pipelined architecture
- HREADY-based handshake mechanism
- Burst transfer concept

### 4️⃣ AXI (Advanced eXtensible Interface)
- High-performance bus for memory and accelerators
- Separate read and write channels
- VALID/READY handshake mechanism
- Support for burst transactions
- Parallel data flow

### 5️⃣ AXI4 vs AXI4-Lite
- AXI4 supports burst and high throughput
- AXI4-Lite supports single transfers
- AXI4-Lite used for control registers
- Design trade-offs between performance and simplicity

## 🔄 Handshake Mechanisms Studied
- APB: PSEL + PENABLE (+ PREADY)
- AHB: HREADY
- AXI: VALID and READY handshake protocol

## 🧠 Real SoC Integration Understanding
- AXI used between CPU and DDR memory
- AXI-Lite used for control registers of DMA/GPU
- APB used for UART, GPIO, I2C peripherals
- Use of AHB/APB bridges in hierarchical bus design

## 🎯 Learning Outcome
Through this study, I gained a clear understanding of:
- Why multiple bus protocols exist inside a chip
- Performance vs power trade-offs in bus design
- How handshake mechanisms ensure reliable communication
- Real-world SoC integration of AMBA protocols



## 🚀 Future Work
RTL implementation and simulation of selected AMBA protocols will be added in future updates to strengthen practical understanding.
