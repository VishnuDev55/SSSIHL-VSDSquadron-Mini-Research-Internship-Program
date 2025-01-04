
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



