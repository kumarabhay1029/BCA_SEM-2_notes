# 📚 MCS-202: Computer Organisation  
## Block 1, Unit 1: Computer System Architectures

---

## 🎯 Learning Objectives

- Understand the concept of computer architecture.
- Learn about major types of computer architectures: Von Neumann, Harvard, CISC, RISC, Multiprocessor, and Mobile.
- Distinguish the strengths and limitations of each architecture.
- Recognize real-world examples for every architecture.

---

## 🏗️ 1. What is Computer Architecture? 

Computer architecture is the conceptual design and fundamental operational structure of a computer system.  
It defines how a computer's hardware and software interact and how instructions are executed.

**Key components:**
- **CPU (Central Processing Unit):** The brain of the computer.
- **Memory:** Stores data and instructions.
- **Input/Output (I/O) Devices:** Devices that interact with the outside world.

---

## 🏛️ 2. Main Computer Architectures

### 2.1 Von Neumann Architecture

- **Single memory** for both data and instructions.
- **One bus** for transfers between memory and CPU.
- **Sequential execution**: Fetches one instruction or data at a time.
- **Von Neumann Bottleneck**: Cannot fetch data and instruction simultaneously, leading to slowdowns.

**Diagram:**
```
+---------------------+
|      Memory         |  <-- Both instructions & data
+---------------------+
         |
         v
+---------------------+
|        CPU          |
+---------------------+
         |
         v
+---------------------+
|   Input/Output      |
+---------------------+
```

**Examples:**  
- Most PCs and laptops (Intel, AMD processors)
- General-purpose computers

---

### 2.2 Harvard Architecture

- **Separate memories** for instructions and data.
- **Two buses**: Allows simultaneous fetch of instruction and data.
- **Faster execution** due to no bottleneck.

**Diagram:**
```
+-------------------+       +------------------+
| Instruction Memory| <---> |   CPU            |
+-------------------+       +------------------+
                                  ^
                                  |
+-------------------+       +------------------+
|     Data Memory   | <---> |   CPU            |
+-------------------+       +------------------+
```

**Examples:**  
- Microcontrollers (e.g., Arduino Uno, PIC, AVR)
- Digital Signal Processors (DSPs)
- Embedded systems (washing machines, microwave controllers)

---

### 2.3 CISC (Complex Instruction Set Computer)

- **Large and complex instruction set**: Each instruction can perform multiple operations.
- **Easier for programmers** as instructions are close to high-level language statements.
- **Slower decoding** due to complexity.

**Examples:**  
- Intel x86 processors (most desktop and laptop CPUs)

---

### 2.4 RISC (Reduced Instruction Set Computer)

- **Small, simple instruction set:** Each instruction does only one operation.
- **Easier to pipeline and often faster**.
- **Requires more instructions** for complex tasks, but each instruction executes quickly.

**Examples:**  
- ARM processors (used in most smartphones)
- MIPS processors

---

### 2.5 Multiprocessor & Mobile Architectures

- **Multiprocessor:** Multiple CPUs working together for higher performance (servers, supercomputers).
- **Mobile Architectures:** Optimized for power efficiency (e.g., ARM Cortex in smartphones).

---

## 🌟 3. Comparison Table

| Architecture    | Memory System      | Instruction Set | Example Use     | Strengths                  | Limitations                |
|-----------------|-------------------|-----------------|-----------------|----------------------------|----------------------------|
| Von Neumann     | Shared            | Varies          | PCs, Laptops    | Simplicity, flexibility    | Bottleneck, speed limits   |
| Harvard         | Separate          | Varies          | Microcontrollers| Speed, efficiency          | More complex, expensive    |
| CISC            | Shared (usually)  | Complex         | Intel x86       | Rich instructions, legacy  | Slower, complex decoding   |
| RISC            | Shared/Separate   | Simple          | ARM, MIPS       | Fast, simple, pipelining   | More code for tasks        |
| Multiprocessor  | Shared/Separate   | Varies          | Servers         | High performance, parallel | Complex programming        |

---

## 🖼️ 4. Real-World Examples

- **Von Neumann:** Your laptop, desktop PCs.
- **Harvard:** Arduino Uno, PIC microcontrollers, washing machine controllers.
- **CISC:** Intel/AMD CPUs in most computers.
- **RISC:** ARM processors in smartphones, tablets, Raspberry Pi.
- **Multiprocessor:** Supercomputers, high-end servers.

---

## 💡 5. Key Takeaways

- Computer architecture shapes how a computer works internally.
- Von Neumann is most common for general computers; Harvard is favored for embedded control.
- CISC and RISC describe instruction set philosophies, not just hardware layout.
- Multiprocessor and mobile architectures address performance and efficiency for specialized needs.

---

## 🏁 6. Quick Quiz (Self-Check)

1. What is the main limitation of Von Neumann architecture?
2. Name one device that uses Harvard architecture.
3. What does CISC stand for, and where is it used?
4. Why is RISC preferred in smartphones?

---

## 🎉 Well Done!

You've completed your first professional notes on computer system architectures!  
If you have any doubts, ask away! Otherwise, let’s move to the next unit when you’re ready. 🚀