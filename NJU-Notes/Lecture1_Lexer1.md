# Chapter 1 Lexer-1

>main topic: 词法分析器生成器 ANTLR v4

## Course Note

对于词法分析器：

- 输入: 程序文本/字符串 s (CharStream) + 词法单元 (token) 的规约
- 输出: 词法单元流 (TokenStream)

交互过程：

- 源程序 -> 词法分析器 _<-_/-> _getNextToken_/词法单元 _<-_/-> 语法分析器 -> 输出至语义分析
- 符号表分别双向链接 __词法分析器__ & __语法分析器__

词法分析器的三种设计方法

- 词法分析器生成器
- 手写词法分析器
- 自动化词法分析器

ANTLR使用方法

1. 命令行式使用 ANTLR v4： https://www.antlr.org/
2. 交互式使用 ANTLR v4： https://www.antlr.org/tools.html
3. 编程式使用 ANTLR v4： https://docs.gradle.org/current/userguide/antlr_plugin.html

[ANTLR](https://www.antlr.org/) v4 中的冲突解决规则

- 最前优先匹配: 
	- 关键字 vs. 标识符 
	- ML_COMMENT vs. DOC_COMMENT
- 最长优先匹配:
	- eg: 1.23 / >= / ifhappy
- 非贪婪匹配:
	- eg: ()??,  ()\*?,  ()+?

具体可以见video中讲解 / 下一节对于基础符号的说明

## Slide

[1-lexer-antlr](https://github.com/courses-at-nju-by-hfwei/compilers-lectures/blob/master/2024/1-lexer-antlr/1-lexer-antlr-handout.pdf)

