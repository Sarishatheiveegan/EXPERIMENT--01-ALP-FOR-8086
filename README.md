# EXPERIMENT--01-ALP-FOR-8086
### Name :MARINO SARISHA T
#### Roll no :22223240084
### Date of experiment :29.08.2025

## Aim: To Write and execute ALP on fundamental arithmetic and logical operations
## Components required: 8086  emulator 
## Theory 
Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.


 ## Running the Emulator :
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory
2.	  Run  emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color 
 
 
3.		write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 

4.	 Compile the program and check for the errors 
5.	Run (once there is no syntax error) 

6.	Click OK to see/view the output of your program on the Emulator screen. 


7.	After running the program, another menu screen will be displayed, where you have the option to “View” symbol table,
8.	 


![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)











9.	Click on emulate to start emulation 








![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)








10.	If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 






![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)







## Programs for arithmetic  operations

## Addition  of 8 bit ALP 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
ADD AX,BX
JNC Loop
INC CL
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT
```


## Output  
 <img width="1281" height="862" alt="Screenshot 2025-08-29 160732" src="https://github.com/user-attachments/assets/878268a5-540c-4c8a-bd2a-c6790681e883" />

## Subtraction   of 8 bit numbers  ALP 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
SUB AX,BX
JNC Loop
INC CL  
NOT AX
INC AX
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT      
```
 
## Output
<img width="1309" height="828" alt="Screenshot 2025-08-29 160748" src="https://github.com/user-attachments/assets/905276df-414b-4261-b36f-3432f5a72fe7" />

## Multiplication alp 
```
MOV AX,[3001H]
MOV BX,[3003H]
MUL BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```
 ## Output  
<img width="1351" height="819" alt="Screenshot 2025-08-29 160808" src="https://github.com/user-attachments/assets/ed6e5289-0799-4e1a-918d-eb2c30979025" />


## Division alp 
```
MOV AX,[3001H]
MOV BX,[3003H]
DIV BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```

## Output  
<img width="1618" height="862" alt="Screenshot 2025-08-29 152445" src="https://github.com/user-attachments/assets/e74dd171-fa21-48bb-ab12-958fc217db43" />

## LOGICAL OPERATIONS
<img width="1033" height="902" alt="Screenshot 2025-08-29 160651" src="https://github.com/user-attachments/assets/6cb65487-f87a-448b-aef0-e08aa8bf1914" />

## AND 
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
MOV [3005H],AX
HLT
```

## Output 
<img width="1656" height="852" alt="image" src="https://github.com/user-attachments/assets/fadb24be-a011-4c29-8c81-b75e69bc251f" />


## OR
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
MOV [3005H],AX
HLT
```

## Output
<img width="1599" height="849" alt="Screenshot 2025-08-29 153726" src="https://github.com/user-attachments/assets/fa312e83-2266-46ff-bff7-9a8e8943a015" />

## NAND
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## Output
<img width="1709" height="847" alt="image" src="https://github.com/user-attachments/assets/8be01d5d-cc47-4e95-98f3-92e8eb577981" />



## NOR
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## Output 
<img width="1604" height="877" alt="Screenshot 2025-08-29 154010" src="https://github.com/user-attachments/assets/c408a774-abd7-41aa-96eb-b93ef9e17168" />

## NOT
```
MOV AX,[3001H]
MOV BX,[3003H]
NOT AX
MOV [3005H],AX
HLT
```
## Output 
<img width="1581" height="817" alt="Screenshot 2025-08-29 154558" src="https://github.com/user-attachments/assets/f51ade76-ab18-4d42-9d69-461372dc8602" />

## XOR
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
MOV [3005H],AX
HLT
```
## Output 
<img width="1577" height="763" alt="Screenshot 2025-08-29 154911" src="https://github.com/user-attachments/assets/e15785a2-df69-4d27-9deb-1d98288a2016" />

## XNOR
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## Output 
<img width="1620" height="780" alt="Screenshot 2025-08-29 155646" src="https://github.com/user-attachments/assets/d096b7cc-3ac9-45be-a795-3c9c714a288f" />

## Result :
The Write and execute ALP on fundamental arithmetic and logical operations is executed successfully.
 








