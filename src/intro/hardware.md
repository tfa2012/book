# Meet Your Hardware - 看看硬件

Let's get familiar with the hardware we'll be working with.

让我们先熟悉一下我们要用得硬件。

## STM32F3DISCOVERY (the "F3")

<p align="center">
<img title="F3" src="../assets/f3.jpg">
</p>

What does this board contain?

- A [STM32F303VCT6](https://www.st.com/en/microcontrollers/stm32f303vc.html) microcontroller. This microcontroller has
  - A single-core ARM Cortex-M4F processor with hardware support for single-precision floating point
    operations and a maximum clock frequency of 72 MHz.

  - 256 KiB of "Flash" memory. (1 KiB = 10**24** bytes)

  - 48 KiB of RAM.

  - A variety of integrated peripherals such as timers, I2C, SPI and USART.

  - General purpose Input Output (GPIO) and other types of pins accessible through the two rows of headers along side the board.
  
  - A USB interface accessible through the USB port labeled "USB USER".

- An [accelerometer](https://en.wikipedia.org/wiki/Accelerometer) as part of the [LSM303DLHC](https://www.st.com/en/mems-and-sensors/lsm303dlhc.html) chip.

- A [magnetometer](https://en.wikipedia.org/wiki/Magnetometer) as part of the [LSM303DLHC](https://www.st.com/en/mems-and-sensors/lsm303dlhc.html) chip.

- A [gyroscope](https://en.wikipedia.org/wiki/Gyroscope) as part of the [L3GD20](https://www.pololu.com/file/0J563/L3GD20.pdf) chip.

- 8 user LEDs arranged in the shape of a compass.

- A second microcontroller: a [STM32F103](https://www.st.com/en/microcontrollers/stm32f103cb.html). This microcontroller is actually part of an on-board programmer / debugger and is connected to the USB port named "USB ST-LINK".

For a more detailed list of features and further specifications of the board take a look at the [STMicroelectronics](https://www.st.com/en/evaluation-tools/stm32f3discovery.html) website.

A word of caution: be careful if you want to apply external signals to the board. The microcontroller STM32F303VCT6 pins take a nominal voltage of 3.3 volts. For further information consult the [6.2 Absolute maximum ratings section in the manual](https://www.st.com/resource/en/datasheet/stm32f303vc.pdf)



这块板有什么？

- 一个[STM32F303VCT6](https://www.st.com/en/microcontrollers/stm32f303vc.html)微控制器。这个控制器有：
  - 一颗支持单精度浮点运算的ARM Cortex-M4F处理器，最大运行速度为72MHz。
  - 256KB Flash
  - 48KB RAM
  - 集成多种外设，如定时器，I2C，SPI和USART。
  - GPIO和其它类型的引脚可以通过板两边的两排端子对接。
  - 通过标记为“USB USER”的接口与微控制器的USB外设通讯。
- 芯片[LSM303DLHC](https://www.st.com/en/mems-and-sensors/lsm303dlhc.html)包含有：加速度计和磁力计
- 芯片[L3GD20](https://www.pololu.com/file/0J563/L3GD20.pdf)包含有：陀螺仪
- 8个LED等排列成一个指南针样子
- 另一个微控制器：[STM32F103](https://www.st.com/en/microcontrollers/stm32f103cb.html)。这个微控制器实际上是一个板上的编程器/调试器，使用名为“USB ST-LINK”的USB端口通讯。

可以查看[STMicroelectronics](https://www.st.com/en/evaluation-tools/stm32f3discovery.html)网页了解这块板更加详细的信息。

需要提醒一句：如果您要加载信道到开发板上，请一定要加倍小心。微控制器STM32F303VCT6引脚的典型操作电压为3.3V。欲了解更多信息，请参考[手册中6.2最大绝对额定值](https://www.st.com/resource/en/datasheet/stm32f303vc.pdf)
