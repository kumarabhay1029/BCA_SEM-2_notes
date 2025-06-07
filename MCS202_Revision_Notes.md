# MCS-202 Computer Organisation: Assembly Language Basics & Control Flow 🚀

---

## 📚 Learning Objectives

- Understand the basics of assembly language and its importance.
- Identify and interpret core assembly instructions.
- Explain and apply control flow instructions: `BEQ` and `J`.
- Analyze how control instructions affect program execution.

---

## 1️⃣ What is Assembly Language? 🖥️

- **Definition:**  
  Assembly language is a low-level programming language closely related to machine code. Each instruction corresponds to a direct CPU operation.
- **Why use it?**  
  - Helps understand how computers execute instructions.
  - Used in embedded systems, OS development, and performance-critical applications.
  - Foundation for learning pipelining and CPU architecture.

---

## 2️⃣ Common Assembly Instructions 📝

| Instruction    | Description                                      | Example             |
|----------------|--------------------------------------------------|---------------------|
| `LOAD`         | Load data from memory to register                 | `LOAD R1, 0(R2)`    |
| `STORE`        | Store data from register to memory                | `STORE R1, 0(R2)`   |
| `ADD`          | Add two registers, store result in a register     | `ADD R3, R1, R2`    |
| `SUB`          | Subtract one register from another                | `SUB R3, R1, R2`    |
| `BEQ`          | Branch if two registers are equal                 | `BEQ R1, R2, LABEL` |
| `J`            | Unconditional jump to label                       | `J LABEL`           |

---

## 3️⃣ Control Flow Instructions 🚦

### A. `BEQ` (Branch if Equal) 🔀

- **Syntax:** `BEQ R1, R2, LABEL`
- **Meaning:**  
  If the value in `R1` equals the value in `R2`, jump to the instruction labeled `LABEL`. Otherwise, continue to the next instruction.
- **Purpose:**  
  Enables decisions (like `if` statements) and loops.

#### Example:
```assembly
BEQ R1, R2, LOOP   # If R1 == R2, jump to LOOP
```

---

### B. `J` (Jump) 🏃

- **Syntax:** `J LABEL`
- **Meaning:**  
  Unconditionally transfers execution to the instruction labeled `LABEL`.
- **Purpose:**  
  Used to repeat actions (loops), skip code, or end programs.

#### Example:
```assembly
J END   # Jump to END label, no matter what
```

---

## 4️⃣ Example: Combining BEQ and J

```assembly
BEQ R1, R2, EQUAL      # If R1 == R2, jump to EQUAL
J   NOTEQUAL           # Otherwise, jump to NOTEQUAL

EQUAL:
    # (Code to handle equal case)
    J END

NOTEQUAL:
    # (Code to handle not equal case)

END:
    # End of program
```

---

## 5️⃣ How to Trace Control Flow? 🧭

- **If R1 == R2:**  
  - Jump directly to `EQUAL` section.
- **If R1 ≠ R2:**  
  - Skip `EQUAL` and jump to `NOTEQUAL`.
- **After handling either case:**  
  - Use `J END` to finish or continue elsewhere.

---

## 6️⃣ Visual Analogy 🎨

- **BEQ:**  
  Like a fork in a road: "If the two values are the same, take the shortcut."
- **J:**  
  Like a teleport: "Jump instantly to the finish line."

---

## 7️⃣ Quick Tips & Reminders 📝

- Branching is key for decision-making and repeating instructions.
- Always check register values before branching or jumping.
- Branches may introduce **control hazards** in pipelined CPUs (covered in detail in future lessons).

---

## 8️⃣ Practice Exercise 💡

```assembly
BEQ R3, R4, SKIP
ADD R5, R3, R4
SKIP:
SUB R6, R3, R4
```
- **Q:** What is the value of R5 and R6 if R3 = 10, R4 = 10?

---

## ⭐ Summary

- Assembly language is the closest programming language to hardware.
- `BEQ` and `J` are essential for controlling program flow.
- Understanding these basics makes advanced topics (like pipelining and hazards) much easier!

---

**Good luck with your revision! Keep practicing—you're doing great!** 🌟