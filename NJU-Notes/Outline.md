# Outline

> - this note is made by BoxuanHu in Spring 2024
> - the main topic is "Compilers"

事实上这门课的深入学习需要三个方面齐同协进

1. 知识提纲梳理
2. 知识的“书面推导与运用”
3. 代码设计与构造逻辑

这篇笔记聚焦于 __知识提纲梳理__，书面推导与运用见[笔者仓库对应部分](https://github.com/root-hbx/Compilers_Spring_2024)，代码设计见[NJU课程官网实验解析](http://docs.compilers.cpl.icu/#/2024/hw)


## Compilers

This course is taught by Prof. [Hengfeng Wei @NJU](https://github.com/hengxin)

课程设计

- 教材：[Compilers: Principles, Techniques, and Tools](https://zh.wikipedia.org/wiki/%E7%BC%96%E8%AF%91%E5%8E%9F%E7%90%86_(%E6%95%99%E6%9D%90)) （大名鼎鼎的“龙书”）
- 内容：理论部分基本按照龙书节奏叙述。包括词法分析、语法分析、语义分析、运行时环境、寄存器分配、代码优化与生成等内容
- 特点：选用了当下热门的 ANTLR （ANother Tool for Language Recognition） v4 编程语言解析生成工具辅助教学，能让使用者专心词法或者语法分析的设计

课程配套

- Course Homepage: [NJU-Compilers-Spring-2024](http://docs.compilers.cpl.icu/#/)
- Piazza: [NJU-Compilers-Chatting](https://2024-compilers-at-software-nju.zulipchat.com/#narrow/stream/419310-general)
- Course Online: [Bilibili-NJU-Compilers-Spring-2024](https://space.bilibili.com/479141149/channel/collectiondetail?sid=2312309)

## Appendix

由于时间原因，本教程Online版没有图片，仅仅是个人笔记缩略版，如需PDF教程，请移步至[Compilers @bxhu](https://github.com/root-hbx/Compilers_Spring_2024)

Reference:

- [Berkeley](http://www-inst.eecs.berkeley.edu/): [CS164 - Programming Languages and Compilers](http://www-inst.eecs.berkeley.edu/~cs164),
- [CMU](http://www.cs.cmu.edu/): 15411 - Compiler Design ( [F09](http://www.cs.cmu.edu/~fp/courses/15411-f09/), [F11](http://symbolaris.com/course/compiler11.html), [F15](https://www.cs.cmu.edu/~rjsimmon/15411-f15/))
- [MIT](http://staff.ustc.edu.cn/~yuzhang/compiler/www.eecs.mit.edu): [6.036 - Computer Language Engineering](http://6.035.scripts.mit.edu/sp16/)
- [Stanford](http://cs.stanford.edu/): [CS143 - Compilers](http://www.stanford.edu/class/cs143/)

### Compiler Generator

- **Generating Lexer**: [Flex](http://flex.sourceforge.net/) ([for windows](http://gnuwin32.sourceforge.net/packages/flex.htm)), JFlex([_link1_](http://jflex.de/), [_link2_](http://sourceforge.net/projects/jflex/))  
    **Grammar-Lex Spec.**:[ANSI-C](http://www.quut.com/c/ANSI-C-grammar-l.html)
- **Generating Parser**: [Bison](http://www.gnu.org/software/bison/) ([for windows](http://gnuwin32.sourceforge.net/packages/bison.htm)), [Java CUP](http://www2.cs.tum.edu/projects/cup/), [JavaCC](https://javacc.dev.java.net/), [ANTLR](http://www.antlr.org/) ([Why use ANTLR](http://www.bearcave.com/software/antlr/antlr_expr.html))  
    **Grammar**: [ANSI-C](http://www.quut.com/c/ANSI-C-grammar-y.html)

### Compilers

- [Compiler Explorer](https://godbolt.org/)
- **[LCC](ftp://ftp.cs.princeton.edu/pub/packages/lcc/)**: [lcc-win](http://www.cs.virginia.edu/~lcc-win32/), [paper](http://research.microsoft.com/apps/pubs/default.aspx?id=68413), [book](http://product.china-pub.com/22711)
- **GCC**: [GNU GCC](http://gcc.gnu.org/), [MinGW](http://www.mingw.org/)
- **LLVM**: [llvm.org](https://llvm.org/), [clang](https://clang.llvm.org/), [MLIR](https://mlir.llvm.org/), [CIRCT](https://circt.llvm.org/),  
    [Getting Started with LLVM Core Libraries](https://getting-started-with-llvm-core-libraries-zh-cn.readthedocs.io/zh_CN/latest/)

### ASM

- [The Art of Assembly Language](http://www.plantation-productions.com/Webster/www.artofasm.com/index.html), [LinuxASM](http://www.plantation-productions.com/Webster/LinuxAsm/index.html)
- [HLA](http://www.plantation-productions.com/Webster/HighLevelAsm/index.html)
- **Assemblers**: [The GNU Assembler](http://sourceware.org/binutils/docs/as/index.html), [NASM](http://www.nasm.us/)


### XML

- [W3C XML](http://www.w3.org/XML/), [W3C XML Schema](http://www.w3.org/XML/Schema)
- [XML.ORG.CN](http://www.xml.org.cn/), [W3School](http://www.w3school.com.cn/), [IBM DeveloperWorks - XML](http://www.ibm.com/developerworks/cn/xml/)

### Architectures

- [ACPI](http://www.acpi.info/)( [spec50](http://www.acpi.info/spec50.htm))
- **IA32**: [IA-32 Intel Architecture Software Developer’s Manual](ftp://CSArch:USTC@202.38.79.74/7-ISAs/1.80x86(IA-32)/)
- **AMD64**: [AMD Developer Guides and Manuals](http://developer.amd.com/documentation/guides/pages/default.aspx): [V1: Application Programming](http://support.amd.com/us/Processor_TechDocs/24592.pdf), [V2: System Programming](http://support.amd.com/us/Processor_TechDocs/24592.pdf), [V3: General Purpose and System Instructions](http://support.amd.com/us/Processor_TechDocs/24594.pdf), [V4: 128-bit and 256 bit media instructions](http://support.amd.com/us/Processor_TechDocs/26568.pdf), [V5: 64-Bit Media and x87 Floating-Point Instructions](http://support.amd.com/us/Processor_TechDocs/26569.pdf).
- **MIPS**: [SPIM](http://pages.cs.wisc.edu/~larus/spim.html), [See MIPS Run](ftp://CSArch:USTC@202.38.79.74/1-books/Arch/), [MIPS32/64 Archtecture for Programmers](ftp://CSArch:USTC@202.38.79.74/7-ISAs/2.MIPS/)

### Others

- [BBS](http://fbbs.ustc.edu.cn/main.html): [Compiler](http://fbbs.ustc.edu.cn/cgi/bbsdoc?board=CompilerTech), [CSArch](http://fbbs.ustc.edu.cn/cgi/bbsdoc?board=CSArch)([ftp](ftp://CSArch:USTC@202.38.79.74/1-books)), [ASM](http://fbbs.ustc.edu.cn/cgi/bbsdoc?board=ASM), [Java](http://fbbs.ustc.edu.cn/cgi/bbsdoc?board=Java)
- The [Programming Language and Compiler Research](http://www.cs.cmu.edu/~mleone/language-research.html) Home Page.
- Browse [comp.compilers](news:comp.compilers) or [comp.lang.ml](news:comp.lang.ml) newsgroups.

