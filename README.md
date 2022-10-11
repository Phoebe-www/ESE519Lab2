# ESE519Lab2
Siyun Wang
Tested on: DELL Inspiron 5505, Windows 10

## Terminal
I first downloaded the Kali Linux system. I created a new “12.txt” file on it. Using “bash”, “cd Documents”, “vi”, and “cat” commands.

![image](https://user-images.githubusercontent.com/113930091/194969108-ba7c28d8-4371-4cb9-976c-ba4986e36c51.png)

## Setup Gide for SDK on your Windows Machine for Raspberry Pi Pico.
Follow the steps below to install the C/C++ SDK, browse the pico-examples repositorys and then run the "hello_usb.c" program.

1. Arm GNU Toolchain
2. CMake
3. Build Tools for Visual Studio 2022
4. Python 3.10
5. Git

## 1. Arm GNU Toolchain
I installed Arm GNU Toolchain (https://developer.arm.com/downloads/-/arm-gnu-toolchain-downloads), and downloaded the Windows version.

![image](https://user-images.githubusercontent.com/113930091/194969871-b0663edd-a1b7-4cfe-9109-d2924d1b1b71.png)


## 2. CMake
Choose Windows x64 ZIP.(https://cmake.org/download/)

![image](https://user-images.githubusercontent.com/113930091/194970085-8986309e-7285-40b9-a8d9-d7d390ed56f2.png)

## 3. Build Tools for Visual Studio 2022
(https://visualstudio.microsoft.com/zh-hans/downloads/)
![image](https://user-images.githubusercontent.com/113930091/194970335-a58f8ea6-cb52-49e8-90d6-597064674835.png)

## 4. Python 3.10
(https://www.python.org/downloads/windows/)
![image](https://user-images.githubusercontent.com/113930091/194970578-7100e27c-819b-4fa2-a82c-e17b23e91d14.png)

## 5. Git
(https://git-scm.com/download/win)
![image](https://user-images.githubusercontent.com/113930091/194970740-5ab91d2e-aacb-4570-a4e4-9e0dea8bfdce.png)


## Getting the SDK and examples
Execute the below commands in the command line.

![image](https://user-images.githubusercontent.com/113930091/194971075-f1e47f75-1b14-4402-8e20-4f64a8d1e5ba.png)

##  Building "Hello World" from the Command Line
- From the Windows menu, select Windows > Visual Studio 2022 > Developer Command Prompt for VS 2022 to open a Developer Command Prompt window.

![image](https://user-images.githubusercontent.com/113930091/194971937-63516c17-8d44-4bc1-9444-9af56b5c50e3.png)

- Close our current Command Prompt window and open a second Developer Command Prompt window, and this environment variable will be set correctly before proceeding.

![image](https://user-images.githubusercontent.com/113930091/194972227-4c27772b-81e4-4b3f-b5c4-c6d664571209.png)


## SERIAL CONSOLE – PuTTY
- Download the latest version of PuTTY.

![image](https://user-images.githubusercontent.com/113930091/194973213-a103e311-c415-46f1-9530-b4ccb7affe04.png)

- Open Device Manager. Click on Ports (COM & LPT).

 ![image](https://user-images.githubusercontent.com/113930091/194973529-8b40bc4f-8b80-48f7-a61d-4f8d245c0e9a.png)
 
- After the board plugged in, you could find something new in the list with (COM_) where _ is a number.

 ![image](https://user-images.githubusercontent.com/113930091/194974140-9bec9b2f-9cbf-42b0-b394-939a290509c8.png)
 ![image](https://user-images.githubusercontent.com/113930091/194975418-915e11eb-2bd6-4b1e-aab7-280279866185.png)

## Flashing and Running "Hello World"
- Before plugging in, press and hold "reset" button. After plugging in, press and release the BOOTSEL button to force it into USB mass storage mode. The board should automatically display as an external drive. You can can now drag and drop U2 binaries onto the external drive.

- Now we can see "Hello world!" being printed in the serial console.

![image](https://user-images.githubusercontent.com/113930091/194976249-8778978b-d556-447c-9ea9-3e233cbec232.png)
