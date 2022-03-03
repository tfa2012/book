# Introduction - 介绍

Welcome to The Embedded Rust Book: An introductory book about using the Rust
Programming Language on "Bare Metal" embedded systems, such as Microcontrollers.

欢迎阅读嵌入式Rust之书—一本介绍如何使用Rust编程语言编写嵌入式裸机系统的书，如微控制器。

## Who Embedded Rust is For - 嵌入式Rust为谁而准备
Embedded Rust is for everyone who wants to do embedded programming while taking advantage of the higher-level concepts and safety guarantees the Rust language provides.
(See also [Who Rust Is For](https://doc.rust-lang.org/book/ch00-00-introduction.html))

嵌入式Rust之书适用于所有想用它进行嵌入式编程的人，Rust语言为嵌入式提供了更高级概念和安全保障。

（也可以看[Rust可用于什么地方](https://doc.rust-lang.org/book/ch00-00-introduction.html)）

## Scope - 范围

The goals of this book are:

* Get developers up to speed with embedded Rust development. i.e. How to set
  up a development environment.

* Share *current* best practices about using Rust for embedded development. i.e.
  How to best use Rust language features to write more correct embedded
  software.

* Serve as a cookbook in some cases. e.g. How do I do mix C and Rust in a single
  project?

This book tries to be as general as possible but to make things easier for both
the readers and the writers it uses the ARM Cortex-M architecture in all its
examples. However, the book doesn't assume that the reader is familiar with this
particular architecture and explains details particular to this architecture
where required.

本书的目标：

- 加速开发者搭建开发环境。
- 分享Rust当前在嵌入式开发中的最佳实践，即如何正确使用Rust语言的特性编写出嵌入式软件。
- 在某些情况下它也可用作Cookbook，比如如何在一个项目中混合使用C和Rust语言。

这本书试图尽可能的一般化，让读者和开发人员更容易在ARM Cortex-M架构的例子中用起来。然而，本书并不假设读者熟悉ARM Cortex-M的体系架构，并会详细解释该体系中需要的特定内容。

## Who This Book is For - 这本书为谁而准备
This book caters towards people with either some embedded background or some Rust background, however we believe
everybody curious about embedded Rust programming can get something out of this book. For those without any prior knowledge
we suggest you read the "Assumptions and Prerequisites" section and catch up on missing knowledge to get more out of the book
and improve your reading experience. You can check out the "Other Resources" section to find resources on topics
you might want to catch up on.

这本书是为了迎合那些有一些嵌入式或一些Rust背景的人，但我们相信每个对嵌入式Rust编程感兴趣的人都可以从这本书中得到一些有用的东西。对于那些没有任何先验知识的人我们建议您阅读“假设和前提条件”部分，并补充缺失的知识，以从书中获得更多的知识并提高您的阅读体验。您可以查看“其他资料”一节，以找到有关的主题的资料阅读。

### Assumptions and Prerequisites - 假设和前提条件

* You are comfortable using the Rust Programming Language, and have written,
  run, and debugged Rust applications on a desktop environment. You should also
  be familiar with the idioms of the [2018edition] as this book targets
  Rust 2018.

[2018edition]: https://doc.rust-lang.org/edition-guide/

* You are comfortable developing and debugging embedded systems in another
  language such as C, C++, or Ada, and are familiar with concepts such as:
    * Cross Compilation
    * Memory Mapped Peripherals
    * Interrupts
    * Common interfaces such as I2C, SPI, Serial, etc.

首先需要您熟练使用Rust编程语言，有写过、运行和在桌面环境测试过Rust应用程序。本书中用到Rust语言属于[2018版次]，所以您应该要熟悉其中的习语。

### Other Resources - 其他资料
If you are unfamiliar with anything mentioned above or if you want more information about a specific topic mentioned in this book you might find some of these resources helpful.

| Topic        | Resource | Description |
|--------------|----------|-------------|
| Rust         | [Rust Book](https://doc.rust-lang.org/book/) | If you are not yet comfortable with Rust, we highly suggest reading this book. |
| Rust, Embedded | [Discovery Book](https://docs.rust-embedded.org/discovery/) | If you have never done any embedded programming, this book might be a better start |
| Rust, Embedded | [Embedded Rust Bookshelf](https://docs.rust-embedded.org) | Here you can find several other resources provided by Rust's Embedded Working Group. |
| Rust, Embedded | [Embedonomicon](https://docs.rust-embedded.org/embedonomicon/) | The nitty gritty details when doing embedded programming in Rust. |
| Rust, Embedded | [embedded FAQ](https://docs.rust-embedded.org/faq.html) | Frequently asked questions about Rust in an embedded context. |
| Interrupts | [Interrupt](https://en.wikipedia.org/wiki/Interrupt) | - |
| Memory-mapped IO/Peripherals | [Memory-mapped I/O](https://en.wikipedia.org/wiki/Memory-mapped_I/O) | - |
| SPI, UART, RS232, USB, I2C, TTL | [Stack Exchange about SPI, UART, and other interfaces](https://electronics.stackexchange.com/questions/37814/usart-uart-rs232-usb-spi-i2c-ttl-etc-what-are-all-of-these-and-how-do-th) | - |

如果您对上面提到的任何事情都不熟悉，或者你想了解更多，您可以查看下面的标题找到一些详细的资源。

| 标题                            | 资源                                                         | 描述                                                         |
| ------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Rust                            | [Rust Book](https://doc.rust-lang.org/book/)                 | 如果您还不熟悉Rust，我们强烈建议您阅读这本书                 |
| 嵌入式Rust                      | [Discovery Book](https://docs.rust-embedded.org/discovery/)  | 如果你您从来没有做过嵌入式编程，这本书或许是一个好的开始     |
| 嵌入式Rust                      | [Embedded Rust Bookshelf](https://docs.rust-embedded.org)    | 这儿您可以找到Rust嵌入式工作组的一些资源                     |
| 嵌入式Rust                      | [Embedonomicon](https://docs.rust-embedded.org/embedonomicon/) | The nitty gritty details when doing embedded programming in Rust. |
| 嵌入式Rust                      | [embedded FAQ](https://docs.rust-embedded.org/faq.html)      | Frequently asked questions about Rust in an embedded context. |
| 中断                            | [Interrupt](https://en.wikipedia.org/wiki/Interrupt)         | -                                                            |
| Memory-mapped IO/Peripherals    | [Memory-mapped I/O](https://en.wikipedia.org/wiki/Memory-mapped_I/O) | -                                                            |
| SPI, UART, RS232, USB, I2C, TTL | [Stack Exchange about SPI, UART, and other interfaces](https://electronics.stackexchange.com/questions/37814/usart-uart-rs232-usb-spi-i2c-ttl-etc-what-are-all-of-these-and-how-do-th) | -                                                            |



### Translations - 翻译

This book has been translated by generous volunteers. If you would like your
translation listed here, please open a PR to add it.

* [Japanese](https://tomoyuki-nakabayashi.github.io/book/)
  ([repository](https://github.com/tomoyuki-nakabayashi/book))

本书已有一些志愿者翻译成其它文字，如果您想让您的翻译罗列在下面，请推送PR给我们。

- [日文](https://tomoyuki-nakabayashi.github.io/book/)
  ([仓库](https://github.com/tomoyuki-nakabayashi/book))

## How to Use This Book - 如何使用这本书

This book generally assumes that you’re reading it front-to-back. Later
chapters build on concepts in earlier chapters, and earlier chapters may
not dig into details on a topic, revisiting the topic in a later chapter.

This book will be using the [STM32F3DISCOVERY] development board from
STMicroelectronics for the majority of the examples contained within. This board
is based on the ARM Cortex-M architecture, and while basic functionality is
the same across most CPUs based on this architecture, peripherals and other
implementation details of Microcontrollers are different between different
vendors, and often even different between Microcontroller families from the same
vendor.

For this reason, we suggest purchasing the [STM32F3DISCOVERY] development board
for the purpose of following the examples in this book.

[STM32F3DISCOVERY]: http://www.st.com/en/evaluation-tools/stm32f3discovery.html

## Contributing to This Book

The work on this book is coordinated in [this repository] and is mainly
developed by the [resources team].

[this repository]: https://github.com/rust-embedded/book
[resources team]: https://github.com/rust-embedded/wg#the-resources-team

If you have trouble following the instructions in this book or find that some
section of the book is not clear enough or hard to follow then that's a bug and
it should be reported in [the issue tracker] of this book.

[the issue tracker]: https://github.com/rust-embedded/book/issues/

Pull requests fixing typos and adding new content are very welcome!

## Re-using this material

This book is distributed under the following licenses:

* The code samples and free-standing Cargo projects contained within this book are licensed under the terms of both the [MIT License] and the [Apache License v2.0].
* The written prose, pictures and diagrams contained within this book are licensed under the terms of the Creative Commons [CC-BY-SA v4.0] license.

[MIT License]: https://opensource.org/licenses/MIT
[Apache License v2.0]: http://www.apache.org/licenses/LICENSE-2.0
[CC-BY-SA v4.0]: https://creativecommons.org/licenses/by-sa/4.0/legalcode

TL;DR: If you want to use our text or images in your work, you need to:

* Give the appropriate credit (i.e. mention this book on your slide, and provide a link to the relevant page)
* Provide a link to the [CC-BY-SA v4.0] licence
* Indicate if you have changed the material in any way, and make any changes to our material available under the same licence

Also, please do let us know if you find this book useful!
