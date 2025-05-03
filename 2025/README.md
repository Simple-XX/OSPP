
# OSPP2025

- 活动主页

    https://summer-ospp.ac.cn/

- 邮件格式

    请使用 `OSPP2025_项目名_姓名` 作为邮件主题

- 邮件列表

    simple-xx@googlegroups.com

NOTE: 请优先使用 issue，以便其他同学参考

## SimpleRenderer

### SimpleRenderer 添加⾼性能渲染优化

- 项⽬描述

    SimpleRenderer 是⼀个⽤ C/C++ 编写的软件渲染器，⽬前已实现基本的渲染管线，但在处理复杂场景时存在性能瓶颈。本项⽬旨在不改变渲染器的基本架构的前提下，通过优化光栅化算法、改进内存访问模式、减少线程同步开销等⽅式，显著提升渲染性能。

    项⽬将保持软件渲染器的教育价值，同时提供更加流畅的⽤户体验，使学⽣能够学习实⽤的图形学性能优化技术。


- 项⽬难度

    进阶

- 导师

    何卓昊 zhhe2000@gmail.com

- 技术领域

    计算机图形学、性能优化

- 编程语⾔

    C/C++

- 项⽬产出要求

  1. 光栅化算法优化

        实现基于块/图块的光栅化算法（Tile-based Rasterization），代替现有的像素级处理⽅式
        
        增加视锥体裁剪和背⾯剔除测试，提前过滤不可⻅三⻆形

  2. 内存管理优化

        预分配⽚段缓冲区，避免渲染过程中的动态内存分配

        改进数据布局，提⾼缓存利⽤率
        
        实现共享内存机制，减少线程间的重复内存访问

  3. 深度测试优化

        实现早期深度测试，在光栅化阶段直接剔除被遮挡的⽚段

        减少⽚段⽣成和着⾊器调⽤次数

        优化深度缓冲区访问模式

  4. 多线程架构改进

        减少线程间的数据合并次数和同步开销

- 项⽬技术要求
    
    图形学基础，理解渲染管线流程

    C/C++ 编程能⼒，了解现代 C++ 特性

    性能优化经验，能够分析和识别性能瓶颈

    多线程编程基础，了解 OpenMP

    能使⽤ Git 进⾏协作开发

- 项⽬成果仓库
  
    https://github.com/Simple-XX/SimpleRenderer


## SimpleKernel

### 为 SimpleKernel C++ 运行时支持

- 项目描述

    TODO
  
- 项目难度

    进阶

- 导师

    牛志宏 zone.niuzh@hotmail.com

- 项目产出要求

    TODO

- 技术要求

    1. 能使用 Git 进行协作开发
    2. C/C++ 基础
    3. 熟悉 AARCH64, RISCV64, AMD64 体系结构
    4. 
    
- 相关链接

    [SimpleKernel](https://github.com/Simple-XX/SimpleKernel)
