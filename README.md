
# SSSIHL-VSDSquadron-Mini-Research-Internship-Program

## Task 1
**The compiled C code of sum of numbers from 1 to n:**

![Running - Oracle VirtualBox 23-12-2024 1:26:36 PM](https://github.com/user-attachments/assets/de80e2af-1786-43c6-be34-79d280125fe1)

**Objdump Output:**

![Running - Oracle VirtualBox 24-12-2024 6:31:59 AM](https://github.com/user-attachments/assets/78efaa37-336c-46be-9ab2-82e941eebf29)

---

## Task 2
**We examined the register values and debugged the program.**  
The commands used were:

```bash
riscv64-unknown-elf-gcc -Ofast -g -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c
riscv64-unknown-elf-objdump -d sum1ton.o | less
spike -d pk sum1ton.o
until pc <address_of_main>

```
![b  Running  - Oracle VirtualBox 29-12-2024 2 58 05 AM](https://github.com/user-attachments/assets/773cbdb7-9ec3-49ad-bba9-a74aa408d5fa)
![b 2 Running  - Oracle VirtualBox 29-12-2024 3 11 55 AM](https://github.com/user-attachments/assets/4bb931fd-43f0-47a3-be23-467315e1138c)
![b  Running  3- Oracle VirtualBox 29-12-2024 3 00 39 AM](https://github.com/user-attachments/assets/2677fb1f-f721-487b-859d-64f9d12f6461)

## Task 3
# 15 Unique RISC-V Instructions with 32-bit Opcode

Here are 15 unique RISC-V instructions along with their corresponding 32-bit opcode and breakdown:

## 1. `beqz a5, 1017c`
- **Instruction Code**: `0x02078863`
- **Format**: `beqz a5, 1017c` (Branch if equal to zero)  
  **Code breakdown**:
  - `beq` (Branch if equal)  
  - `a5` (source register)  
  - `1017c` (offset).

## 2. `addi sp, sp, -16`
- **Instruction Code**: `0xff010113`
- **Format**: `addi sp, sp, -16` (Add immediate to stack pointer)  
  **Code breakdown**:
  - `addi` (Add immediate)  
  - `sp` (destination and source registers)  
  - `-16` (immediate).

## 3. `auipc a0, 0x12`
- **Instruction Code**: `0x00012517`
- **Format**: `auipc a0, 0x12` (Add upper immediate to program counter)  
  **Code breakdown**:
  - `auipc` (Add upper immediate to PC)  
  - `a0` (destination register)  
  - `0x12` (immediate value).

## 4. `addi a0, a0, -340`
- **Instruction Code**: `0xeac50513`
- **Format**: `addi a0, a0, -340` (Add immediate to `a0`)  
  **Code breakdown**:
  - `addi` (Add immediate)  
  - `a0` (destination and source registers)  
  - `-340` (immediate).

## 5. `sd ra, 8(sp)`
- **Instruction Code**: `0x00113423`
- **Format**: `sd ra, 8(sp)` (Store doubleword)  
  **Code breakdown**:
  - `sd` (Store doubleword)  
  - `ra` (source register)  
  - `8(sp)` (memory address).

## 6. `auipc ra, 0x0`
- **Instruction Code**: `0x00000097`
- **Format**: `auipc ra, 0x0` (Add upper immediate to program counter)  
  **Code breakdown**:
  - `auipc` (Add upper immediate to PC)  
  - `ra` (destination register)  
  - `0x0` (immediate value).

## 7. `jalr zero`
- **Instruction Code**: `0x000000e7`
- **Format**: `jalr zero` (Jump and link register)  
  **Code breakdown**:
  - `jalr` (Jump and link register)  
  - `zero` (register value used for jump).

## 8. `ld ra, 8(sp)`
- **Instruction Code**: `0x00813083`
- **Format**: `ld ra, 8(sp)` (Load doubleword)  
  **Code breakdown**:
  - `ld` (Load doubleword)  
  - `ra` (destination register)  
  - `8(sp)` (memory address).

## 9. `li a5, 1`
- **Instruction Code**: `0x00100793`
- **Format**: `li a5, 1` (Load immediate value into register `a5`)  
  **Code breakdown**:
  - `li` (Load immediate)  
  - `a5` (destination register)  
  - `1` (immediate value).

## 10. `sb a5, 1944(gp)`
- **Instruction Code**: `0x78f18c23`
- **Format**: `sb a5, 1944(gp)` (Store byte)  
  **Code breakdown**:
  - `sb` (Store byte)  
  - `a5` (source register)  
  - `1944(gp)` (memory address).

## 11. `addi sp, sp, 16`
- **Instruction Code**: `0x01010113`
- **Format**: `addi sp, sp, 16` (Add immediate to stack pointer)  
  **Code breakdown**:
  - `addi` (Add immediate)  
  - `sp` (destination and source registers)  
  - `16` (immediate value).

## 12. `ret`
- **Instruction Code**: `0x00008067`
- **Format**: `ret` (Return from function)  
  **Code breakdown**:
  - `ret` (Return).

## 13. `auipc a5, 0xffff0`
- **Instruction Code**: `0xffff0797`
- **Format**: `auipc a5, 0xffff0` (Add upper immediate to program counter)  
  **Code breakdown**:
  - `auipc` (Add upper immediate to PC)  
  - `a5` (destination register)  
  - `0xffff0` (immediate value).

## 14. `addi a5, a5, -396`
- **Instruction Code**: `0xe7478793`
- **Format**: `addi a5, a5, -396` (Add immediate to `a5`)  
  **Code breakdown**:
  - `addi` (Add immediate)  
  - `a5` (destination and source registers)  
  - `-396` (immediate value).

## 15. `jr zero`
- **Instruction Code**: `0x00078c63`
- **Format**: `jr zero` (Jump register)  
  **Code breakdown**:
  - `jr` (Jump register)  
  - `zero` (register value used for jump).

