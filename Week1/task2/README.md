# Task 2: Cross-Compile "Hello, RISC-V"

Create a minimal C "Hello World" program and successfully cross-compile it for the RISC-V RV32 architecture, producing a
 valid 32-bit RISC-V ELF executable that demonstrates proper toolchain functionality


---

## ✅ Steps Followed


###1: Create the Hello World C Program:


Create a minimal C program that demonstrates basic functionality and printf usage.

nano hello.c

**C Program Code:**

#include <stdio.h>

int main() {
printf("Hello, RISC-V!\n");
return 0;
}


### 2: Cross-Compile for RISC-V Architecture

Compile the C program using the RISC-V toolchain with the default configuration that works with your specific toolchain setup.

 Cross-compile using default toolchain configuration (THIS WORKS!)

riscv32-unknown-elf-gcc -o hello.elf hello.c

###  3: Verify the Compiled ELF Binary

Check that the compiled binary is a valid 32-bit RISC-V executable.

# Check the ELF file properties and architecture

file hello.elf

Output:


hello.elf: ELF 32-bit LSB executable, UCB RISC-V, RVC, soft-float ABI, version 1 (SYSV), statically linked, not stripped

###  4: Additional Working Verification Commands

 riscv32-unknown-elf-objdump -h hello.elf


# output:

