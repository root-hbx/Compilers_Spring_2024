
>copied from [USTC-Compilers](http://staff.ustc.edu.cn/~yuzhang/compiler/2019f/)

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

### C & C++

- **Standards**：[C official home](http://www.open-std.org/jtc1/sc22/wg14/), [C++ official home](http://www.open-std.org/jtc1/sc22/wg21/) [ [P2137R0](https://www.open-std.org/jtc1/sc22/wg21/docs/papers/2020/p2137r0.html) ]
- **Materials**: [C Language Book Material](http://www.knosof.co.uk/cbook/cbook.html), [quut.com/C](http://www.quut.com/c/)

### Java

- **Specification**：[Java Language Specification](http://java.sun.com/docs/books/jls/), [Java Virtual Machine Specification](http://java.sun.com/docs/books/jvms/)
- **Tutorials**: [Java Tutorial](http://java.sun.com/docs/books/tutorial/), Thinking in Java([中文版](http://www.paper-translation.com/other/tij3.htm))
- **Software**: [Java SDK](http://www.java.com/zh_CN/download/index.jsp)( [1.5](http://java.sun.com/j2se/1.5.0/docs/index.html), [6](http://java.sun.com/javase/6/docs/) ), [Eclipse IDE](http://www.eclipse.org/downloads) ([AST](http://www.docjar.com/html/api/org/eclipse/jdt/core/dom/AST.java.html)), [Ant](http://ant.apache.org/)([User Manual](http://ant.apache.org/manual/))

### Scala: OO meets Functional

- Developed from 2001 in EPFL, v1.0 2003,
- [scala-lang.org](http://www.scala-lang.org/)

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

