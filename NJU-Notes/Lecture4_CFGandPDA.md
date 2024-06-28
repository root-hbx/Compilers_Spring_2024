# Chapter 4 CFG and PDA

## CFG && CSG

Definition (Context-Free Grammar (CFG); 上下文无关文法)

上下文无关文法 G 是一个四元组 G = (T,N,S,P):

- T 是终结符号 (Terminal) 集合, 对应于词法分析器产生的词法单元 ▶ N 是非终结符号 (Non-terminal) 集合
- S 是开始 (Start) 符号 (S ∈ N 且唯一)
- P 是产生式 (Production) 集合

```bash
A ∈ N −→ α ∈ ( T ∪ N ) ∗
```

- 头部/左部 (Head) A: 单个非终结符
- 体部/右部 (Body) α: 终结符与非终结符构成的串, 也可以是空串 ε


PS: Context-Sensitive Grammar (CSG) 上下文敏感语法

```bash
aB → ab 
bB → bb

举例解释：很简单，比如这里B在前缀元素为a时，转换成ab；在前缀元素为b时，转换成bb
```

## PDA 

More info in [笔者的编译原理仓库](https://github.com/root-hbx/Compilers_Spring_2024)


## Basic Info

__Definition (推导 (Derivation))__

推导即是将某个产生式的左边替换成它的右边；每一步推导需要选择替换哪个非终结符号, 以及使用哪个产生式

- Leftmost (最左) Derivation 
- Rightmost (最右) Derivation


__Definition (Sentential Form; 句型)__

如果S⇒\*α,且α∈(T∪N) ,则称α是文法G的一个句型


__Definition (Sentence; 句子)__

如果S=\*⇒w,且w∈T ,则称w是文法G的一个句子


__Definition (文法 G 生成的语言 L(G))__

文法 G 的语言 L(G) 是它能推导出的所有句子构成的集合。

L ( G ) = { w | S ⇒\* w }

1. 语法分析器的任务: 为输入的词法单元流寻找推导、构建语法分析树, 或者报错

2. 正则表达式的表达能力严格弱于上下文无关文法

3. Theorem
>L = {anbn | n ≥ 0} 无法使用正则表达式描述

__Pumping Lemma for Regular Languages__

If L is a regular language, then there exists a number p ≥ 1 (pumping length) such that any string s in L of length ≥ p can be divided into three pieces, s = xyz, satisfying the following conditions:

(i) |y| ≥ 1 (ii) |xy| ≤ p (iii) ∀i≥0: $xy^iz$ ∈ L

