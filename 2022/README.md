# summer2022

- 邮件格式

    请使用 `summer2022_项目名_姓名` 作为邮件主题

- 邮件列表

    simple-xx@googlegroups.com

- slack

    https://join.slack.com/t/simple-xx/shared_invite/zt-p9li9hrb-Ag1oZuywMljCBSSeRhCMtQ

- Gitter

    https://gitter.im/Simple-XX/community
    
- QQ

    ![IMG_3972](https://tva1.sinaimg.cn/large/008i3skNly1gqr4152kr6j30ku112tdb.jpg)

NOTE: 请优先使用 issue，以便其他同学参考


## SimpleCompiler

### 为 SimpleCompiler 支持自动化程序验证

- 项目描述

  自动化程序验证（auto-active verification）是一种有前景的形式化验证手段，是构建正确、可靠的系统的基础设施（更多具体概念可以参考学习 Dafny 项目文档）。SimpleCompiler目前支持了一个C99标准的子集的语言，本项目期望在SimpleCompiler的语言上原生支持 require, ensure，invariant等操作，并通过SMT Solver实现自动验证。

- 项目难度

    进阶

- 导师

    MisakaCenter misaka@sjtu.edu.cn

- 项目产出要求

    在SimpleCompiler的语言上原生支持 require, ensure，invariant等操作，实现以下例子的自动化程序验证
    
    ```c
    int verify(int n) {
    require(n >= 0);
    int x, y;
    x = n; y = 0;
    while (x > 0) {
    invariant(x >= 0);
    invariant(x + y == n);
    x = x - 1;
    y = y + 1;
    }
    ensure(y == n);
    return y;
    }
    ```


- 技术要求
    1. C/C++
    2. 了解霍尔逻辑（Hoare Logic）与符号执行

- 相关地址

    [SimpleCompiler](https://github.com/Simple-XX/SimpleCompiler)

    [Dafny 项目文档](https://dafny-lang.github.io/dafny/OnlineTutorial/guide)

    

## SimplePhysicsEngine

### 物理模拟之FEM模型实现与可视化整合

- 项目描述

    FEM模型实现

- 项目难度

    进阶

- 导师

    xiaoerlaigeid

    xiaoerlaigeid@qq.com

- 项目产出要求

    1. 熟悉DTK库函数，设计vtk可视化接口，代码风格统一。

    2. 实现vtk可视化接口，将现在物理仿真结果的格式进行统一设计，从而满足所有仿真结果的可视化。

    3. 基于目前只实现二维弹性形变，将它扩展到三维，扩展到塑性形变。将代码风格统一，实现通用的FEM求解器。

    4. 有限元法启发式求导很难。使用自动求导库，解决计算速度慢的问题，引入GPU或并行计算框架cuda或libtorch。

    5. 求解弹性形变问题。开发可视化demo，使用VTK库，并提供2-3个用例，撰写使用文档.。


- 技术要求
    1. C++及CMAKE工具链

    2. 阅读论文，并实现有限元求解数学模型。

    3. 自动求导库torch。

    4. 并行计算库，cuda 等。

    5. 计算机图形学，可视化。


- 相关地址

    Sifakis E, Barbic J. FEM simulation of 3D deformable solids: a practitioner's guide to theory, discretization and model reduction[M]//Acm siggraph 2012 courses. 2012: 1-50.

    https://vtk.org/Wiki/VTK/Tutorials

