# Chapter 0 Overview

>- this is the my notes of Compilers in 2024
>- the course is taught by Prof. [Hengfeng Wei @NJU](https://github.com/hengxin)

## Credits

- Course Homepage: [NJU-Compilers-Spring-2024](http://docs.compilers.cpl.icu/#/)
- Piazza: [NJU-Compilers-Chatting](https://2024-compilers-at-software-nju.zulipchat.com/#narrow/stream/419310-general)
- Course Online: [Bilibili-NJU-Compilers-Spring-2024](https://space.bilibili.com/479141149/channel/collectiondetail?sid=2312309)

## Introduction

1. 高级” 语言 ⇒ (通常) “低级” 语言 (如, 汇编语言) 
2. 汇编语言经过汇编器生成机器语言
3. 汇编语言网站：[godblot](https://godbolt.org/)
4. 采用的指令集：[RISC-V](https://riscv.org/)
5. RISC-V references：
	- https://riscv-programming.org/book.html
	- http://www.riscvbook.com/
6. RISC-V Simulator：
	- https://github.com/TheThirdOne/rars
7. 语言类应用程序：
	- 配置文件解析 (.properties)  
	- CSV 文件 (Comma-Separated Values)  
	- JSON 文件 (JavaScript Object Notation)
	- SQL 引擎 (Structured Query Language) 
	- TLA+/TLAPS (TPaxos.tla)  
	- (Java) 字节码解释器  
	- C/C++ 语言编译器
	- 排版工具 (LATEX)
	- 绘图工具 (TikZ, Dot/Graphviz)
	- L-System (Cantor Set)
8. 语法分析器生成器 ANTLR
	- https://www.antlr.org/index.html
	- https://www.antlr.org/tools.html (IntelliJ Plugin)
	- http://lab.antlr.org/ (Online lab)
9. LLVM
	- https://llvm.org/
10. Reference Books
	- http://docs.compilers.cpl.icu/#/2024/resources

## Overview

- IR: Intermediate Representation (中间表示)
- Source Program -> _Front End_ -> IR -> _Back End_ -> Target Program
	- 前端 (分析阶段): 分析 __源语言__ 程序, 收集所有必要的信息
	- 后端 (综合阶段): 利用收集到的信息, 生成 __目标语言程序__ 
- Clang: a C language family frontend for LLVM
	 - https://clang.llvm.org/
-  _机器无关_ 的 __中间表示优化__

## Slide 

[0-overview](https://github.com/courses-at-nju-by-hfwei/compilers-lectures/blob/master/2024/0-overview/overview-handout.pdf)

## Supplementary Materials

- [LLVM](https://www.bilibili.com/video/BV1RF411K7F5/?vd_source=e3cbbf5ca80db268fa006d63626e267e)
- [Assembly Language](https://www.bilibili.com/video/BV1Y94y1D7at/?spm_id_from=333.788&vd_source=8a3dd36862125e80dc439254ef65d959)
- [Ruby](https://www.bilibili.com/video/BV1PU4y1z7Fs/?spm_id_from=333.788&vd_source=8a3dd36862125e80dc439254ef65d959)
- [Perl](https://www.bilibili.com/video/BV1qB4y1G7B3/?spm_id_from=333.788&vd_source=8a3dd36862125e80dc439254ef65d959)
- [Lua](https://www.bilibili.com/video/BV14t4y1E7Zr/?spm_id_from=333.788&vd_source=8a3dd36862125e80dc439254ef65d959)
- [Unity](https://www.bilibili.com/video/BV1ZB4y1V7KB/?spm_id_from=333.788&vd_source=8a3dd36862125e80dc439254ef65d959)
- [Temple OS](https://www.bilibili.com/video/BV13g411r7bY/?spm_id_from=333.788&vd_source=8a3dd36862125e80dc439254ef65d959)
- [Fortran](https://www.bilibili.com/video/BV1Qd4y1R7vX/?spm_id_from=333.788&vd_source=8a3dd36862125e80dc439254ef65d959)
- [WebAssembly](https://www.bilibili.com/video/BV12B4y1B7xq/?spm_id_from=333.788&vd_source=8a3dd36862125e80dc439254ef65d959)
- [Haskell](https://www.bilibili.com/video/BV1cS4y1b7kH/?spm_id_from=333.788&vd_source=8a3dd36862125e80dc439254ef65d959)
- [Swift](https://www.bilibili.com/video/BV1Ya411378N/?spm_id_from=333.788&vd_source=8a3dd36862125e80dc439254ef65d959)
- [Elixir](https://www.bilibili.com/video/BV1at4y1L7Ty/?spm_id_from=pageDriver&vd_source=8a3dd36862125e80dc439254ef65d959)
- [Kotlin](https://www.bilibili.com/video/BV1AW4y1B74G/?spm_id_from=333.788&vd_source=8a3dd36862125e80dc439254ef65d959)
- [redis](https://www.bilibili.com/video/BV1Wd4y1X7wy/?p=14&spm_id_from=pageDriver)

