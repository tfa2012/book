# Summary

<!--

Definition of the organization of this book is still a work in process.

Refer to https://github.com/rust-embedded/book/issues for
more information and coordination

本书的内容和组织形式仍在开发中。

可参考https://github.com/rust-embedded/book/issues查看更多协作信息。

-->

- [Introduction](./intro/index.md)
    - [Hardware](./intro/hardware.md)
    - [`no_std`](./intro/no-std.md)
    - [Tooling](./intro/tooling.md)
    - [Installation](./intro/install.md)
        - [Linux](./intro/install/linux.md)
        - [MacOS](./intro/install/macos.md)
        - [Windows](./intro/install/windows.md)
        - [Verify Installation](./intro/install/verify.md)
- [Getting started](./start/index.md)
  - [QEMU](./start/qemu.md)
  - [Hardware](./start/hardware.md)
  - [Memory-mapped Registers](./start/registers.md)
  - [Semihosting](./start/semihosting.md)
  - [Panicking](./start/panicking.md)
  - [Exceptions](./start/exceptions.md)
  - [Interrupts](./start/interrupts.md)
  - [IO](./start/io.md)
- [Peripherals](./peripherals/index.md)
    - [A first attempt in Rust](./peripherals/a-first-attempt.md)
    - [The Borrow Checker](./peripherals/borrowck.md)
    - [Singletons](./peripherals/singletons.md)
- [Static Guarantees](./static-guarantees/index.md)
    - [Typestate Programming](./static-guarantees/typestate-programming.md)
    - [Peripherals as State Machines](./static-guarantees/state-machines.md)
    - [Design Contracts](./static-guarantees/design-contracts.md)
    - [Zero Cost Abstractions](./static-guarantees/zero-cost-abstractions.md)
- [Portability](./portability/index.md)
- [Concurrency](./concurrency/index.md)
- [Collections](./collections/index.md)
- [Design Patterns](./design-patterns/index.md)
    - [HALs](./design-patterns/hal/index.md)
        - [Checklist](./design-patterns/hal/checklist.md)
        - [Naming](./design-patterns/hal/naming.md)
        - [Interoperability](./design-patterns/hal/interoperability.md)
        - [Predictability](./design-patterns/hal/predictability.md)
        - [GPIO](./design-patterns/hal/gpio.md)
- [Tips for embedded C developers](./c-tips/index.md)
    <!-- TODO: Define Sections -->
- [Interoperability](./interoperability/index.md)
    - [A little C with your Rust](./interoperability/c-with-rust.md)
    - [A little Rust with your C](./interoperability/rust-with-c.md)
- [Unsorted topics](./unsorted/index.md)
  - [Optimizations: The speed size tradeoff](./unsorted/speed-vs-size.md)
  - [Performing Math Functionality](./unsorted/math.md)



- [介绍](./intro/index.md)
  - [硬件](./intro/hardware.md)
  - [`no_std`](./intro/no-std.md)
  - [工具](./intro/tooling.md)
  - [安装](./intro/install.md)
    - [Linux](./intro/install/linux.md)
    - [MacOS](./intro/install/macos.md)
    - [Windows](./intro/install/windows.md)
    - [安装核验](./intro/install/verify.md)
- [启动](./start/index.md)
  - [QEMU](./start/qemu.md)
  - [硬件](./start/hardware.md)
  - [内存映射寄存器](./start/registers.md)
  - [Semihosting](./start/semihosting.md)
  - [Panicking](./start/panicking.md)
  - [异常](./start/exceptions.md)
  - [中断](./start/interrupts.md)
  - [IO](./start/io.md)
- [外设](./peripherals/index.md)
  - [在Rust中的第一次尝试](./peripherals/a-first-attempt.md)
  - [借用检查](./peripherals/borrowck.md)
  - [单例](./peripherals/singletons.md)
- [静态保证](./static-guarantees/index.md)
  - [类型状态编程](./static-guarantees/typestate-programming.md)
  - [把外设当做状态机](./static-guarantees/state-machines.md)
  - [设计约定](./static-guarantees/design-contracts.md)
  - [零成本抽象](./static-guarantees/zero-cost-abstractions.md)
- [移植](./portability/index.md)
- [同步](./concurrency/index.md)
- [集合](./collections/index.md)
- [设计模式](./design-patterns/index.md)
  - [硬件抽象层](./design-patterns/hal/index.md)
    - [检查清单](./design-patterns/hal/checklist.md)
    - [命名](./design-patterns/hal/naming.md)
    - [互操作性](./design-patterns/hal/interoperability.md)
    - [可预测性](./design-patterns/hal/predictability.md)
    - [GPIO](./design-patterns/hal/gpio.md)
- [给嵌入式C开发人员的提示](./c-tips/index.md)
  <!-- TODO: Define Sections -->
- [互操作性](./interoperability/index.md)
  - [Rust中的C](./interoperability/c-with-rust.md)
  - [C中的Rust](./interoperability/rust-with-c.md)
- [未排序的话题](./unsorted/index.md)
  - [优化：速度和大小的平衡](./unsorted/speed-vs-size.md)
  - [执行数学功能](./unsorted/math.md)



---

[Appendix A: Glossary](./appendix/glossary.md)

[附录A：术语](./appendix/glossary.md)
