# SSSIHL-VSDSquadron-Mini-Research-Internship-Program
## Task 1
**The compiled c code of sum of numbers from 1 to n**
![es  Running  - Oracle VirtualBox 23-12-2024 1 26 36 PM](https://github.com/user-attachments/assets/de80e2af-1786-43c6-be34-79d280125fe1)
**Objdump**
![eee  Running  - Oracle VirtualBox 24-12-2024 6 31 59 AM](https://github.com/user-attachments/assets/78efaa37-336c-46be-9ab2-82e941eebf29)
##Task 2
**we saw the register values and debbuged them ** 
The commands were 
'riscv64-unknown-elf-gcc -Ofast -g -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c'
'riscv64-unknown-elf-objdump -d sum1ton.o | less'
'spike -d pk sum1ton.o'
'until pc <address_of_main>'

![b  Running  - Oracle VirtualBox 29-12-2024 2 58 05 AM](https://github.com/user-attachments/assets/bc1d5d5f-ac39-4b43-bb02-36b9a5e4a834)

![b 2 Running  - Oracle VirtualBox 29-12-2024 3 11 55 AM](https://github.com/user-attachments/assets/91f594c1-e627-4489-8cde-9855efd4e763)

![b  Running  3- Oracle VirtualBox 29-12-2024 3 00 39 AM](https://github.com/user-attachments/assets/14d55b40-1cb6-47f5-8d6f-6718f9b5e0e1)
