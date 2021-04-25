# summer2021

- 邮件格式

    请统一使用 `summer2021_项目名_姓名` 作为邮件主题

- 邮件列表

    simple-xx@googlegroups.com

- slack

    https://join.slack.com/t/simple-xx/shared_invite/zt-p9li9hrb-Ag1oZuywMljCBSSeRhCMtQ

    (30 days from 4.23)

- Gitter

    https://gitter.im/Simple-XX/community

## SimpleCPU

### 为SimpleCPU实现可背靠背执行Cache

- 项目描述

    作为现代处理器的关键组件之一，Cache能够充分发掘软件执行中存在的局部性，有效克服冯诺伊曼体系结构下存储墙问题。一个正确且高效的Cache能够有效提升SimpleCPU的执行效率。

    项目标签：risc-v CPU Cache

- 项目难度

    高

- 导师

    陈国凯

    chenguokai17@mails.ucas.ac.cn

- 项目产出要求

    一个使用Chisel 3语言实现并在verilator仿真环境下正常工作的组相连Cache，在连续访存情形下可连续命中。

    Cache可位于AXI接口或SRAM接口处，容量不小于2KB，至少为2路组相连，支持使用risc-v fence系列指令控制。应有机制确保Cache的存在不干扰外设正常工作。

- 技术要求

    参与者应熟悉Chisel或/及verilog语言，熟悉AXI协议

    最好熟悉RISC-V指令集

- 相关地址

    [SimpleCPU](https://github.com/Simple-XX/SimpleCPU)

### 为SimpleCPU增加Sv39模式TLB支持

- 项目描述

    TLB是现代处理器安全运行的重要保障，也是现代操作系统运行所必需的组件，RISC-V作为新一代开源指令集，其TLB设计规范汲取众家之长，为软件提供了简洁直观的接口。而这也对其硬件实现提出了较高要求。

    项目标签：RISC-V CPU TLB

- 项目难度

    高

- 导师

    陈国凯 

    chenguokai17@mails.ucas.ac.cn

- 项目产出要求

    一个使用Chisel语言实现的符合RISC-V sv39标准的TLB。

    TLB实现后，处理器应当能够运行risc-v官方测试集中开启TLB的测试点。

- 技术要求

    参与者应熟悉Chisel或/及verilog语言，对操作系统和TLB有一定了解

    最好熟悉RISC-V指令集

- 相关地址

    [SimpleCPU](https://github.com/Simple-XX/SimpleCPU)

### 为SimpleCPU增加Supervisor和User态支持

- 项目描述

    RISC-V当前已定义Machine、Supervisor、User三种特权态，在不同的特权态下软件允许执行的指令、允许操纵的CSR不同，软件也可以借此实现一些安全特性。特别地，配合前述TLB功能即可实现完善的内核/用户程序隔离保护。

    项目标签：RISC-V CPU

- 项目难度

    高

- 导师

    陈国凯

    chenguokai17@mails.ucas.ac.cn

- 项目产出要求

    一个支持M/S/U特权态规范中全部CSR、全部所需功能的特权态实现，实现相关访问限制与异常触发。

- 技术要求

    参与者应熟悉Chisel或/及verilog语言

    最好熟悉RISC-V指令集

- 相关地址

    [SimpleCPU](https://github.com/Simple-XX/SimpleCPU)

### 为SimpleCPU拆分流水线优化时序

- 项目描述

    当前SimpleCPU采用二级流水线结构，时序有较大不足，需要将其流水线进行拆分。

    项目标签：RISC-V CPU

- 项目难度

    高

- 导师

    陈国凯

    chenguokai17@mails.ucas.ac.cn

- 项目产出要求

    将现有流水线拆分为至少3级，并尽可能保证时序划分合理。

- 技术要求

    参与者应熟悉Chisel或/及verilog语言。

    最好熟悉RISC-V指令集，有时序优化经验

- 相关地址

    [SimpleCPU](https://github.com/Simple-XX/SimpleCPU)



## SimpleKernel

### 编写项目文档

- 项目描述

    SimpleKernel 是一个用 C++ 实现的简单内核，目前支持 x86，arm，riscv。

    需要一份文档帮助使用者熟悉代码。

    项目标签：kernel 文档

- 项目难度

    中

- 导师

    牛志宏

    a6813140@hotmail.com

- 项目产出要求

    为每个 branch 编写 README，介绍原理与代码实现

    说明每个代码目录下的文件用途，有需要注意的地方要单独说明

    整理相关资料，存放在相应的目录下

- 技术要求

    内核相关知识

    C++

    x86，arm，riscv 相关知识

- 相关地址

    [SimpleKernel](https://github.com/Simple-XX/SimpleKernel)

### 多平台内存管理优化

- 项目描述

    对多平台的内存管理进行改进。

    Simple Kernel 已经完成了 x86 平台下的物理内存探测以及二级分页下的虚拟内存，现在需要进行拓展。

    项目标签：kernel 内存管理

- 项目难度

    高

- 导师

    牛志宏

    a6813140@hotmail.com

- 项目产出要求

    1. arm，riscv64 下的物理内存探测与管理
    2. 重新设计虚拟内存部分，支持最多 4 级页表
    3. malloc，free 的实现
    4. new，delete 的实现(C++17)

- 技术要求

    内核相关知识

    内存管理相关知识

    C++

    x86，arm，riscv 相关知识

- 相关地址

    [SimpleKernel](https://github.com/Simple-XX/SimpleKernel)

### 多平台多核与任务管理

- 项目描述

    抽象出多核、任务管理相关数据与操作，并实现 x86，arm，riscv 下的任务管理

    项目标签：kernel 任务管理

- 项目难度

    高

- 导师

    牛志宏

    a6813140@hotmail.com

- 项目产出要求

    1. 平台无关的多核抽象
    2. 平台无关的任务抽象
    3. x86/arm/riscv 下任务管理的实现

- 技术要求

    内核相关知识

    C++

    任务管理相关知识

    x86，arm，riscv 相关知识

- 相关地址

    [SimpleKernel](https://github.com/Simple-XX/SimpleKernel)

## SimpleRenderer

## SimpleCompiler

### 完善编译器架构

- 项目描述

    SimpleCompiler 目前仅完成了部分前端处理，需要进行完善

    项目标签：Compiler x86

- 项目难度

    高

- 导师

    牛志宏

    a6813140@hotmail.com

- 项目产出要求

    支持部分 C99 标准的前端

    x86 平台下的后端

    简单的优化

    设计师需要考虑跨平台问题

- 技术要求

    C++

    编译原理

    x86 指令集

- 相关地址

    [SimpleCompiler](https://github.com/Simple-XX/SimpleCompiler)

    