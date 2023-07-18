# STM32F103-LCD1602_With_ADC
This C code is a main program file targeting a microcontroller, likely an STM32 microcontroller. The main purpose of this code is to read an analog voltage from an ADC channel, convert it to a digital value, and then display the voltage on an LCD using the HD44780 LCD driver library.

Let's go through the key components of the code:
![download (1)](https://github.com/ivias2000/STM32F103-LCD1602_With_ADC/assets/125237611/7adf27da-77d3-495d-a916-da93393eebce)

Includes:
The code includes various header files representing different libraries used in the project, including "main.h," "adc.h," "gpio.h," "HD44780LIB.h," and "stdio.h." These headers provide access to functions and constants required for the peripherals and libraries used in the application.

Global Variables:

ADC_Value: An unsigned 16-bit integer variable to store the ADC conversion result.
ACC_Value: An integer variable whose purpose is not clear from the code.
voltage: A floating-point variable to store the calculated voltage value.
a: A floating-point variable used in the voltage calculation.
i: An integer variable to store the whole part of the voltage value.
j: An integer variable to store the fractional part of the voltage value.
x and y: Integer variables whose purpose is not clear from the code.
arr and aar: Arrays of 16-bit unsigned integers whose purpose is not clear from the code.
Main Function:
The main function is the entry point of the program. It initializes the microcontroller's peripherals, including the ADC and LCD, and then enters an infinite loop.
![Interfacing-16X2-LCD-with-STM32-Blue-Pill](https://github.com/ivias2000/STM32F103-LCD1602_With_ADC/assets/125237611/ce2f33b3-2fd1-429a-9c77-376dbe75aa59)

ADC Reading and Voltage Calculation:
Within the infinite loop, the code continuously reads the ADC value from ADC1. It then calculates the corresponding voltage based on the ADC reading and stores the whole and fractional parts of the voltage in i and j, respectively.

LCD Display:
The calculated voltage is displayed on the LCD using the HD44780 LCD driver library. The PStr function seems to be used to display text on the LCD. However, the displayed text seems to be a long string of characters that may not fit on the LCD screen as it spans multiple lines.

System Clock Configuration:
The SystemClock_Config function configures the system clock for the microcontroller.

To use this code on GitHub, follow the steps mentioned earlier to create a new repository and upload this C code as the main program file. Additionally, you can include a README.md file in your repository to provide more information about the project and how to use the code.
![Screenshot 2023-07-18 115728](https://github.com/ivias2000/STM32F103-LCD1602_With_ADC/assets/125237611/74d4307c-3690-4267-91c8-75f6595d8052)
