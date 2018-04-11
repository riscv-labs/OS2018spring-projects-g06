# sv6 for RV64 SMP - 课程设计中期报告

## 题目选择

我们的主体工作将分成两部分：

1.  将sv6操作系统从x86-64位移植到RISC-V 64位（简称RV64）对称多核（简称SMP）。
2.  利用commuter的工作优化sv6操作系统的网络子模块。

## 相关工作综述

## 设计方案

对于课程设计，我们分为以下9个步骤进行：

1. 把RV64（SMP）的工具链，包括编译器、模拟器准备好。
2. 学习RV64指令集和特权指令集。
3. 写几个RV64的小例子。
4. 将sv6移植到RV64单核。
5. 进一步将sv6移植到RV64多核。
6. 可能需要糊一些驱动。
7. 使用sv6、Linux进行性能测试对比（可能需要使用硬件RV64）。
8. 学习符号化执行、z3。
9. 利用commuter的工作优化sv6操作系统的网络子模块。

## 小组分工

## 已完成工作

## 参考文献

1. sv6
  GitHub: https://github.com/aclements/sv6
2. Commuter
  https://pdos.csail.mit.edu/archive/commuter/
  GitHub: https://github.com/aclements/commuter
3. RISC-V Spec
  https://riscv.org/specifications/
  https://riscv.org/specifications/privileged-isa/
4. bbl-ucore
  https://ring00.github.io/bbl-ucore/
5. ucore labs RISC-V 64移植
  https://gitee.com/shzhxh/ucore_os_lab/tree/riscv64-priv-1.10
6. Booting a RISC-V Linux Kernel
  https://www.sifive.com/blog/2017/10/09/all-aboard-part-6-booting-a-risc-v-linux-kernel/
7. Entering and Exiting the Linux Kernel on RISC-V
  https://www.sifive.com/blog/2017/10/23/all-aboard-part-7-entering-and-exiting-the-linux-kernel-on-risc-v/
8. Paging and the MMU in the RISC-V Linux Kernel
  https://www.sifive.com/blog/2017/12/11/all-aboard-part-9-paging-and-mmu-in-risc-v-linux-kernel/
9. 符号执行入门
  https://zhuanlan.zhihu.com/p/26927127

