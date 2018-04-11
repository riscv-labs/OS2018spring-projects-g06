# sv6 for RV64 SMP - 课程设计中期报告

## 题目选择

近年来，人工智能及大数据的众多应用为计算能力提出了新的需求，而处理器核心频率的提高已经遇到困难，现如今，多核心处理器、并行化已成为提高计算系统性能的主要手段。事实上，在2013年，Austin T. Clements等人[1, 2]就提出过一种新的手段，用于优化并行系统软件的性能。此项工作提出了一个名为commuter的工具，借助符号化执行技术[10, 11]以及SMT求解器[12]，用于挖掘系统规范中潜在的并行化优化点；同时，他们用此工具辅助设计实现了一个并行度很好的精简的操作系统，名为sv6。sv6在x86-64指令集架构上实现，考虑到目前新兴的RISC-V指令集[3, 4]更开放、灵活性更好、硬件设计更简洁，为此，本课程设计计划基于上述工作，将上述工作提出的sv6移植到RISC-V 64位多核平台，以期能够推动RISC-V并行架构的发展。最后，本课程设计还计划利用commuter工具进一步优化sv6的并行性。

简言之，本课程设计的主体工作计划分成两个部分：

1. 将sv6操作系统从x86-64移植到RISC-V 64位（以下简称RV64）对称多处理器（以下简称SMP）环境。
2. 利用commuter工具优化sv6操作系统的一部分，例如网络子模块。

## 相关工作综述

### RISC-V

### sv6

### 符号化执行

### z3

### commuter

## 设计方案

本课程设计计划分为以下9个步骤进行：

1. 把RV64（SMP）的工具链，包括编译器、模拟器准备好。
2. 学习RV64指令集和特权指令集。
3. 写几个RV64的小例子。
4. 将sv6移植到RV64单核。
5. 进一步将sv6移植到RV64多核。
6. 可能需要糊一些驱动。
7. 使用sv6、Linux进行性能测试对比（可能需要使用硬件RV64）。
8. 学习符号化执行以及z3的使用。
9. 利用commuter的工作优化sv6操作系统的网络子模块。

## 小组分工

## 已完成工作

## 参考文献

1. sv6
  https://github.com/aclements/sv6

2. Commuter
  https://pdos.csail.mit.edu/archive/commuter/
  https://github.com/aclements/commuter

3. The RISC-V Instruction Set Manual Volume I: User-Level ISA

  https://riscv.org/specifications/

4. The RISC-V Instruction Set Manual Volume II: Privileged Architecture

  https://riscv.org/specifications/privileged-isa/

5. bbl-ucore
  https://ring00.github.io/bbl-ucore/

6. ucore labs RISC-V 64移植
  https://gitee.com/shzhxh/ucore_os_lab/tree/riscv64-priv-1.10

7. Booting a RISC-V Linux Kernel
  https://www.sifive.com/blog/2017/10/09/all-aboard-part-6-booting-a-risc-v-linux-kernel/

8. Entering and Exiting the Linux Kernel on RISC-V
  https://www.sifive.com/blog/2017/10/23/all-aboard-part-7-entering-and-exiting-the-linux-kernel-on-risc-v/

9. Paging and the MMU in the RISC-V Linux Kernel
  https://www.sifive.com/blog/2017/12/11/all-aboard-part-9-paging-and-mmu-in-risc-v-linux-kernel/

10. 符号执行入门
  https://zhuanlan.zhihu.com/p/26927127

11. mini-mc
    https://github.com/xiw/mini-mc

12. Z3
    https://github.com/Z3Prover/z3

