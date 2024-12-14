This repository contains examples of two common errors in assembly language programming: buffer overflows and writes beyond allocated memory. The `bug.asm` file demonstrates these issues, while `bugSolution.asm` provides corrected code with added safeguards.

**Key Concepts:**

* **Buffer Overflow:** Occurs when a program attempts to write data beyond the allocated buffer size. This can overwrite adjacent memory regions, leading to unpredictable behavior or crashes.
* **Write Beyond Allocation:** Writing to memory addresses that have not been allocated or are outside of the program's address space. This usually results in a segmentation fault.

**Mitigation Strategies:**

* **Bounds Checking:** Before any memory access, verify that the index or offset is within the valid range of the buffer.
* **Memory Allocation:** Use appropriate functions to allocate sufficient memory and avoid accessing unallocated memory regions.
* **Input Validation:** Always validate user inputs to prevent attackers from deliberately overflowing buffers.

This repository serves as an educational resource for understanding and preventing these common vulnerabilities in assembly programming.