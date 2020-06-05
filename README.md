# summer2020

License: [MIT License](https://opensource.org/licenses/MIT)

邮件格式：请统一使用 `summer2020_项目名_姓名` 作为邮件主题

加入群组获取更多信息：[slack](https://join.slack.com/t/simple-xx/shared_invite/zt-eowe46jb-coTqSRQRSF44edYICElI3w)

## SimpleKernel

SimpleKernel 是一个参考早期 linux 实现的简单 x86 内核，现阶段的开发进行到多任务的实现，已经实现的内容包括使用 grub2 启动，进入 32 位保护模式，虚拟内存的初步管理。

### 修复存在的 bug

- 项目描述

    由于项目早期的遗留问题，有很多 bug 一直没有解决，在代码某处一定还藏有尚未发现的地雷，你的任务是找到它，解决它，并留下足够的测试代码。

- 项目难度

    中

- 导师

    MRNIU(https://github.com/MRNIU)
    
    mail: Zone.niuzh@hotmail.com

- 项目产出要求

    1. 解决现在已知的 bug
    2. 对指针操作、边界条件等敏感代码进行理论上的证明，排除可能存在的隐患
    3. 对可独立运行的代码文件进行单元测试（如手动实现的标准库，设备驱动程序，平台无关代码）

- 技术要求

    - 能使用 Git 进行协作开发
    - 熟悉 C，x86 汇编
    - 熟悉 linux 代码
    - 熟悉 make 的使用
    - 有一定的 debug 能力
    - 一定的 x86 硬件知识

- 相关地址

    [SimpleKernel](https://github.com/Simple-XX/SimpleKernel)

    [已知 bug](https://github.com/Simple-XX/SimpleKernel/issues)

### 优化现有内存管理代码的实现

- 项目描述

    现有的内存管理代码可谓千疮百孔，难以说是一个能够作为示例的代码，我们需要你在现有方案的基础上对代码进行重写，使用经典算法如 first-fit，buddy 重新实现内存管理系统。 

- 项目难度

    中

- 导师

    MRNIU(https://github.com/MRNIU)
    
    mail: Zone.niuzh@hotmail.com

- 项目产出要求

    1. 重新实现现有内存管理部分
    2. 使用经典算法进行管理
    3. 留出的接口向 POSIX 看齐
    4. 写说明文档，体现出如何实现的思考过程

- 技术要求

    - 能使用 Git 进行协作开发
    - 熟悉 C，x86 汇编
    - 熟悉 linux 代码
    - 熟悉 make 的使用
    - 有一定的 debug 能力
    - 相当的 x86 硬件知识

- 相关地址

    [SimpleKernel](https://github.com/Simple-XX/SimpleKernel)

### 完成多任务系统

- 项目描述

    多任务是内核不可或缺的部分，但现在我们的代码还很简陋。现有代码是对 linux 内核实现的魔改，还不能够正常使用。

- 项目难度

    高

- 导师

    MRNIU(https://github.com/MRNIU)
    
    mail: Zone.niuzh@hotmail.com

- 项目产出要求

    1. 实现多任务系统
    2. 明确区分平台无关/平台相关代码
    3. 留出的接口向 POSIX 看齐
    4. 写说明文档，体现出如何实现的思考过程

- 技术要求

    - 能使用 Git 进行协作开发
    - 熟悉 C，x86 汇编
    - 熟悉 linux 代码
    - 熟悉 make 的使用
    - 熟悉进程调度相关知识
    - 相当的 x86 硬件知识

- 相关地址

    [SimpleKernel](https://github.com/Simple-XX/SimpleKernel)



### 编写实现文档

- 项目描述

    目前的实现文档分布在开发日志、代码注释中，有的部分还有缺少，我们需要一份文档告诉使用者我们的代码是怎么来的，背后的原理是什么，为什么这样写。

- 项目难度

    中

- 导师

    MRNIU(https://github.com/MRNIU)

- 项目产出要求

    1. 编写从计算机启动到多任务系统为止的实现文档
    2. 从软件硬件两个角度讲

- 技术要求

    - 能使用 Git 进行协作开发
    - 一定的文字功底
    - 相当的 x86 硬件知识

- 相关地址

    [SimpleKernel](https://github.com/Simple-XX/SimpleKernel)



## SimpleCompiler

SimpleCompiler 目前还只是个雏形，仅实现了词法解析部分，如果你有兴趣在它开始的时候加入进来，很欢迎你的到来。



### 完善编译器架构

- 项目描述

    目前仅实现了基本的词法解析，但对于整个编译器的整体结构尚未有过考虑，我们需要一位对编译器熟悉的同学来把握大方向，站在初学者的角度，我们的代码怎么写能让别人容易理解，便于迁移呢？

- 项目难度

    中

- 导师

    MRNIU(https://github.com/MRNIU)
    
    mail: Zone.niuzh@hotmail.com

- 项目产出要求

    1. 一份架构设计，分析现有技术方案，明确我们的代码该怎么写
    2. 实现所描述的框架性代码

- 技术要求

    - 能使用 Git 进行协作开发
    - 熟悉 C/C++，x86 汇编
    - 熟悉 make 的使用
    - 熟悉编译器相关知识
    - 有一定教学经验

- 相关地址

    [SimpleCompiler](https://github.com/Simple-XX/SimpleCompiler)

