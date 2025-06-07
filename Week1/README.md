# Week 1: Install & Sanity-Check the RISC-V Toolchain

This document outlines the tasks completed in **Week 1** of the RISC-V SoC Lab, focusing on installing the RISC-V bare-metal toolchain and verifying the functionality of key tools (`gcc`, `objdump`, `gdb`).

---

## 🔧 Task

Install the RISC-V toolchain and verify that it is working properly.

---

## ✅ Steps Followed

### 1. Download the Toolchain

Downloaded from the official VSD-Labs link:  
https://vsd-labs.sgp1.cdn.digitaloceanspaces.com/vsd-labs/riscv-toolchain-rv32imac-x86_64-ubuntu.tar.gz

### 2. Extract the Toolchain

Extracted the tarball using:

sudo tar -xvzf riscv-toolchain-rv32imac-x86_64-ubuntu.tar.gz -C /opt/

This created a folder named:

riscv-toolchain-rv32imac

### 3. Add to PATH (Temporarily)

Added the toolchain’s bin folder to the system PATH for the current session:

echo 'export PATH=$PATH:/opt/riscv-toolchain/bin' >> ~/.bashrc

### 4. Verify the Installation

Checked the installed tools by verifying their versions:

riscv32-unknown-elf-gcc --version
riscv32-unknown-elf-objdump --version
riscv32-unknown-elf-gdb --version

## OUTPUT:


