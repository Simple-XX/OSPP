# summer2021

- 邮件格式

    请统一使用 `summer2021_项目名_姓名` 作为邮件主题

- 邮件列表

    simple-xx@googlegroups.com

- slack

    https://join.slack.com/t/simple-xx/shared_invite/zt-p9li9hrb-Ag1oZuywMljCBSSeRhCMtQ

- Gitter

    https://gitter.im/Simple-XX/community
    
- QQ

    ![IMG_3972](https://tva1.sinaimg.cn/large/008i3skNly1gqr4152kr6j30ku112tdb.jpg)

NOTE: 请优先使用 issue，以便其他同学参考

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

- 中选学生

    陈泓佚 [laiyiwanrexiang](https://github.com/laiyiwanrexiang)

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

- 中选学生

    王浩宇 [WangNorthSea](https://github.com/WangNorthSea)

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

- 中选学生

    孙启楚 [...](...)

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
    
- 中选学生

    杨安杰 [digmouse233](https://github.com/digmouse233)

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
    
- 中选学生

    葛岩 [KehRoche](https://github.com/KehRoche)

### 为 SimpleKernel 实现测试用例和自动化测试流水线

- 项目描述

    SimpleKernel 是一个用 C++ 实现的简单内核，目前支持 x86，arm，riscv。

    需要提供目前simplekernel的测试用例以及CICD流水线。

    项目标签：kernel 文档

- 项目难度

    中

- 导师

    xiaoerlaigeid

    xiaoerlaigeid@qq.com

- 项目产出要求

    实现目前功能测试用例，并实现自动化流水线测试

- 技术要求

    内核相关知识

    C++

    x86，arm，riscv 相关知识

- 相关地址

    [SimpleKernel](https://github.com/Simple-XX/SimpleKernel)
- 中选学生

    关皓然  [...](...)
## SimpleRenderer

### 基于原生系统API的光栅化渲染器实现

- 项目描述

    使用C++和原生系统API实现一个光栅化渲染器

    项目标签：图形学 渲染器

- 项目难度

    高

- 导师

    xiaoerlaigeid

    xiaoerlaigeid@qq.com

- 项目产出要求

    1. 优化/补充已有代码
    2. 填充算法
    3. 贴图支持
    4. 背面消隐
    5. 摄像机的实现
    6. 渲染结果输出

- 技术要求

    1. 熟悉C++
    2. 熟悉图形学
    3. 了解填充算法
    4. 了解背面消隐算法
    5. 其它相关图形算法

- 相关地址

    [SimpleRenderer](https://github.com/Simple-XX/SimpleRenderer)
- 中选学生

    戴雨欣  [...](...)
## SimplePhysicsEngine

### 实现 SimplePhysicsEngine 接口以及初步基本功能

- 项目描述

    重新使用C++实现物理仿真算法。需要借助 基于CGAL和 Eigen 的 API 进行图形学中物理模拟算法的实现。实现包括 弹簧质点模型、有限元模型、碰撞检测等算法。

    项目标签：图形学 物理引擎

- 项目难度

    高

- 导师

    xiaoerlaigeid

    xiaoerlaigeid@qq.com

- 项目产出要求

    1. 重新编译 dtk 对 deformable toolkit 库当前已有内容的总结

    2. 参考dtk API进行移植 重新定义API接口

    3. 将之前未实现的FEM 算法实现 

    4. 使用当前API 编写1-2个简单demo 并可视化。（内容可以后续进行探讨）

    5. 实现文档进行简单描述。

- 技术要求

    参与者应熟悉cpp，熟悉图形学

- 相关地址

    [SimplePhysicsEngine](https://github.com/Simple-XX/SimplePhysicsEngine)

    参考代码 

    https://github.com/Deformable-Toolkit/dtk

    https://github.com/FantasyVR/LearnFEMSimpleCompiler
- 中选学生

    陈伟 [TOMsworkspace](https://github.com/TOMsworkspace)
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

- 中选学生

    刘涵之 [MisakaCenter](https://github.com/MisakaCenter)

    
