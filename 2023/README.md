# OSPP2023

- 活动主页

    https://summer-ospp.ac.cn/

- 邮件格式

    请使用 `OSPP2023_项目名_姓名` 作为邮件主题

- 邮件列表

    simple-xx@googlegroups.com

- slack

    https://join.slack.com/t/simple-xx/shared_invite/zt-p9li9hrb-Ag1oZuywMljCBSSeRhCMtQ

- Gitter

    https://gitter.im/Simple-XX/community
    
- QQ

    ![Simple-XX群聊二维码](./.README.assets/Simple-XX群聊二维码.png)

NOTE: 请优先使用 issue，以便其他同学参考


## SimpleKernel

### 为 SimpleKernel 添加 UEFI 启动支持

- 项目描述
  UEFI，全称 Unified Extensible Firmware Interface，即 “统一可扩展固件接口”，是一种详细描述全新类型接口的标准，是适用于电脑的标准固件接口，旨在代替BIOS（基本输入/输出系统）。此标准由 UEFI 联盟中的 140 多个技术公司共同创建，其中包括微软公司。UEFI 旨在提高软件互操作性和解决 BIOS 的局限性。[^1]
  
  本项目期望将目前的 grub+multiboot 引导方案替换为 UEFI 方式。

- 项目难度

    进阶

- 导师

    zone zone.niuzh@hotmail.com

- 项目产出要求

    1. 为 SimpleKernel 的 x86，x86_64，aarch64 架构，添加 uefi+qemu 的启动支持
    2. 可以在 qemu 上正常启动
    3. 如果需要编译第三方工具，应当有自动化脚本
    4. 应当在启动时传递内核需要的相关信息
    5. x86 应当进入 32 位模式；x86_64，aarch64 应当进入 64 位模式
    6. TUI 或图形界面的初始化


- 技术要求
    1. linux 基础
    2. c/c++ 基础
    3. x86、arm 汇编基础
    4. 能使用 Git 进行协作开发
    5. UEFI 相关知识
    6. 体系结构基础（x86+arm）
    
- 相关地址

    [SimpleKernel](https://github.com/Simple-XX/SimpleKernel)
    
    https://wiki.osdev.org/

[^1]: https://blog.51cto.com/liuqun/1982475



## SimpleO3Sim

### 为SimpleO3Sim 完善功能支持

- 项目描述

    SimpleO3Sim 是一个简单的乱序 risc-v 处理器模拟器，当前已实现基本的乱序执行框架与 RV32I 部分指令。本项目希望对其进行进一步完善，实现完整的 RV32IZicsr 指令集，并运行起risc-v 标准测试用例。

    为便于实现这一目标并确认正确性，强烈推荐实现该模拟器与现有其他行为级模拟器的行为对齐机制。

- 项目难度

    进阶

- 导师

    chenguokai chenguokai17@mails.ucas.ac.cn

- 项目产出要求

    1. 为该模拟器实现完整的RV32IZicsr指令集支持，最终可运行对应的risc-v标准测试用例
    2. （强烈推荐）实现该模拟器与其他行为级模拟器的行为对齐机制
    3. 整理测试用例形成单元测试
    4. 其他必要的bug修复


- 技术要求

    1. Linux 基础
    2. c/c++ 基础
    3. risc-v 汇编基础
    4. git 使用基础
    5. 计算机体系结构基础
    
- 相关地址

    [SimpleO3Sim](https://github.com/Simple-XX/SimpleO3Sim/)


​    





