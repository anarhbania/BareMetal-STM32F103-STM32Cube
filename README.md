# How to install BareMetal for STM32F103 in STM32CubeIDE?

## Download [STM32CubeIDE](https://www.st.com/en/development-tools/stm32cubeide.html)
## Run STM32CubeIDE
- File -> New -> STM32 Project
- Select MCU STM32F103, click Next
- Project Name: (file name), click Finish
- File -> New -> STM32 Project
- Select MCU STM32F103, click Next
- Project Name: (file name)
- Targeted Project Type: Empty, click Finish
- Copy folder "Drivers" (from first Project) to this Project
- Project -> Properties -> C/C++ General -> Paths and Symbols -> Source Location -> Add Folder "Drivers"
- Project -> Properties -> C/C++ Build -> Settings -> MCU GCC Compiler -> Include paths -> Add "../Drivers/CMSIS/Include" and "../Drivers/CMSIS/Device/ST/STM32F1xx/Include"
- Project -> Properties -> C/C++ Build -> Settings -> MCU GCC Compiler -> Preprocessor -> Add "STM32F103xx" (find in "Drivers/CMSIS/Device/ST/STM32F1xx/Include/stm32f1xx.h")
- In main.c add #include "stm32f1xx.h"
