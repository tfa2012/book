# Appendix A: Glossary - 附录A：词汇表

The embedded ecosystem is full of different protocols, hardware components and
vendor-specific things that use their own terms and abbreviations. This Glossary
attempts to list them with pointers for understanding them better.

嵌入式生态系统中充满着不同的协议、硬件组件和各供应商自定义的things。本词汇表尝试列举出一些重点出来，以便更好地理解它们。

### BSP

A Board Support Crate provides a high level interface configured for a specific
board. It usually depends on a [HAL](#hal) crate.
There is a more detailed description on the [memory-mapped registers page](../start/registers.md)
or for a broader overview see [this video](https://youtu.be/vLYit_HHPaY).

电路板支持库crate（Board Support Crate）是某个特定电路板的高层接口库。通常它依赖于HAL crate。[memory-mapped registers page](../start/registers.md)这篇文章有更加详细的描述，或者看这个[视频](https://youtu.be/vLYit_HHPaY)。

### FPU

Floating-point Unit. A 'math processor' running only operations on floating-point numbers.

浮点运算单元。仅用于计算浮点数操作的“数学处理器”。

### HAL

A Hardware Abstraction Layer crate provides a developer friendly interface to a microcontroller's
features and peripherals. It is usually implemented on top of a [Peripheral Access Crate (PAC)](#pac).
It may also implement traits from the [`embedded-hal`](https://crates.io/crates/embedded-hal) crate.
There is a more detailed description on the [memory-mapped registers page](../start/registers.md)
or for a broader overview see [this video](https://youtu.be/vLYit_HHPaY).

硬件抽象层crate给开发人员提供了访问微控制器的功能和外设的友好接口。这层通常在[Peripheral Access Crate (PAC)](#pac)上实现，也可能在[`embedded-hal`](https://crates.io/crates/embedded-hal)crate的基础上实现。

[memory-mapped registers page](../start/registers.md)这篇文章有更加详细的描述，或者看这个[视频](https://youtu.be/vLYit_HHPaY)。

### I2C

Sometimes referred to as `I²C` or Inter-IC. It is a protocol meant for hardware communication
within a single integrated circuit. See [here][i2c] for more details

I2C又叫做`I²C`或者Inter-IC。它是一种在单一集成电路内用于硬件通信的协议。这篇[文章][i2c]有更详细的说明。

[i2c]: https://en.wikipedia.org/wiki/I2c

### PAC

A Peripheral Access Crate provides access to a microcontroller's peripherals. It is one of
the lower level crates and is usually generated directly from the provided [SVD](#svd), often
using [svd2rust](https://github.com/rust-embedded/svd2rust/). The [Hardware Abstraction Layer](#hal)
would usually depend on this crate.
There is a more detailed description on the [memory-mapped registers page](../start/registers.md)
or for a broader overview see [this video](https://youtu.be/vLYit_HHPaY).

外设访问Crate（Peripheral Access Crate）提供对微控制器的外设访问接口。这是底层crate之一，通常直接由SVD生成，比如svd2rust工具。HAL依赖于PAC。[memory-mapped registers page](../start/registers.md)这篇文章有更加详细的描述，或者看这个[视频](https://youtu.be/vLYit_HHPaY)。

### SPI

Serial Peripheral Interface. See [here][spi] for more information.

[spi]: https://en.wikipedia.org/wiki/Serial_peripheral_interface

### SVD

System View Description is an XML file format used to describe the programmers view of a
microcontroller device. You can read more about it on
[the ARM CMSIS documentation site](https://www.keil.com/pack/doc/CMSIS/SVD/html/index.html).

系统视图描述（System View Description）是一个XML文件格式，是站在编译工具的角度上描述微控制器的组成。可以看[the ARM CMSIS documentation site](https://www.keil.com/pack/doc/CMSIS/SVD/html/index.html)了解更详细的信息。

### UART

Universal asynchronous receiver-transmitter. See [here][uart] for more information.

[uart]: https://en.wikipedia.org/wiki/Universal_asynchronous_receiver-transmitter

### USART

Universal synchronous and asynchronous receiver-transmitter. See [here][usart] for more information.

[usart]: https://en.wikipedia.org/wiki/Universal_synchronous_and_asynchronous_receiver-transmitter
