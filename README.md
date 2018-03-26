# Lecture Notes on Econometrics

by Qiang Gao (School of Finance, Capital University of Economics and Business)


# 高级计量经济学课件

作者：高强（首都经济贸易大学金融学院）

---

本课件是对日本经济学家林文夫（2000）所著《高级计量经济学》教材[^1]的补充。

国内新入学的研究生，本科阶段所接受的数学训练普遍不足。例如，微积分课程缺少对梯度、雅可比矩阵、海赛矩阵、多元泰勒展开的讲解；线性代数课程缺少对向量空间、坐标变换、特征分解、四个基本子空间、奇异值分解、二次型等重要概念的强调；概率论与数理统计两门特别重要的课程，通常被合并成一门课在一个学期讲完，造成学生普遍搞不清楚条件期望、条件方差、方差—协方差矩阵、多元正态分布、$$\chi^2$$分布、$$t$$分布、$$F$$分布、极大似然估计量、信息矩阵等基础概念；更不要说压根不安排实分析、微分方程、随机过程、动态优化等数学课了。

正是因为这一问题给面向研究生开设的《高级计量经济学》课程带来了极大的挑战，所以我尝试制作这些课件。这些课件并不能够取代本科阶段应有的数学教育，而是希望在《高级计量经济学》授课过程中，逢山开路，遇水搭桥，以“现学现用”为原则尽可能弥补课本假设学生知道所以没有讲但其实学生根本不知道的那些基础数学知识，作为一个教辅资料，帮助学生扎扎实实地学明白《高级计量经济学》教材中所有的数学推导。

练习题原本应该由学生亲自完成，这是学习取得成效的重要环节。但现实情况是，由于学生普遍基础不足，根本没有能力独立完成练习。所以本课件的另外一个组成部分是公布所有练习题的答案供学生参考。如果担心学生因此就有办法作弊，逃避亲自完成练习，那么可以采取随堂闭卷测验的方式考察学生是否确实掌握练习题的解法。希望本课件将练习题答案公布更多是帮助学生，而不是害到学生。

最后，本课件正在逐步建设中，许多内容尚处空缺，错误也在所难免，非常欢迎读者的批评指正（本书每一页边距空白处可随意点击“加号”添加评论）。

ps. 若网页中数学公式显示不正常，通常刷新一遍网页即可正常显示。这似乎是 `gitbook.com` 平台的技术性问题，或者是从国内网络访问国际网络的普遍性问题造成的，本人无法解决。

# 目录

## Chapter 1 Finite-Sample Properties of OLS

### Section 1 The Classical Linear Regression Model

* [Lecture Note 1.1](lecture-note/1.1.md)
    * [Review Question 1.1.1](question-solution/1.1.1.md)
    * [Review Question 1.1.2](question-solution/1.1.2.md)
    * [Review Question 1.1.3](question-solution/1.1.3.md)
    * [Review Question 1.1.4](question-solution/1.1.4.md)
    * [Review Question 1.1.5](question-solution/1.1.5.md)
    * [Review Question 1.1.6](question-solution/1.1.6.md)

### Section 2 The Algebra of Least Squares

* [Lecture Note 1.2](lecture-note/1.2.md)
    * [Review Question 1.2.1](question-solution/1.2.1.md)
    * [Review Question 1.2.2](question-solution/1.2.2.md)
    * [Review Question 1.2.3](question-solution/1.2.3.md)
    * [Review Question 1.2.4](question-solution/1.2.4.md)
    * [Review Question 1.2.5](question-solution/1.2.5.md)
    * [Review Question 1.2.6](question-solution/1.2.6.md)
    * [Review Question 1.2.7](question-solution/1.2.7.md)
    * [Review Question 1.2.8](question-solution/1.2.8.md)
    * [Review Question 1.2.9](question-solution/1.2.9.md)
    
### Section 3 Finite-Sample Properties of OLS

* [Review Question 1.3.1](question-solution/1.3.1.md)
* [Review Question 1.3.2](question-solution/1.3.2.md)
* [Review Question 1.3.3](question-solution/1.3.3.md)
* [Review Question 1.3.4](question-solution/1.3.4.md)
* [Review Question 1.3.5](question-solution/1.3.5.md)
* [Review Question 1.3.6](question-solution/1.3.6.md)
* [Review Question 1.3.7](question-solution/1.3.7.md)

### Section 4 Hypothesis Testing under Normality

* [Review Question 1.4.1](question-solution/1.4.1.md)
* [Review Question 1.4.2](question-solution/1.4.2.md)
* [Review Question 1.4.3](question-solution/1.4.3.md)
* [Review Question 1.4.4](question-solution/1.4.4.md)
* [Review Question 1.4.5](question-solution/1.4.5.md)
* [Review Question 1.4.6](question-solution/1.4.6.md)
* [Review Question 1.4.7](question-solution/1.4.7.md)

### Section 5 Relation to Maximum Likelihood

* [Review Question 1.5.1](question-solution/1.5.1.md)
* [Review Question 1.5.2](question-solution/1.5.2.md)
* [Review Question 1.5.3](question-solution/1.5.3.md)
* [Review Question 1.5.4](question-solution/1.5.4.md)
* [Review Question 1.5.5](question-solution/1.5.5.md)

### Section 6 Generalized Least Squares (GLS)

* [Review Question 1.6.1](question-solution/1.6.1.md)
* [Review Question 1.6.2](question-solution/1.6.2.md)
* [Review Question 1.6.3](question-solution/1.6.3.md)
* [Review Question 1.6.4](question-solution/1.6.4.md)

### Section 7 Application: Returns to Scale in Electricity Supply

* [Lecture Note](lecture-note/1.7.md)
* [Review Question 1.7.1](question-solution/1.7.1.md)
* [Review Question 1.7.2](question-solution/1.7.2.md)
* [Review Question 1.7.3](question-solution/1.7.3.md)
* [Review Question 1.7.4](question-solution/1.7.4.md)
* [Review Question 1.7.5](question-solution/1.7.5.md)
* [Review Question 1.7.6](question-solution/1.7.6.md)
* [Review Question 1.7.7](question-solution/1.7.7.md)
* [Review Question 1.7.8](question-solution/1.7.8.md)

### Analytical Exercises

* [Analytical Exercise 1.1](exercise-solution/1.1.md)
* [Analytical Exercise 1.2](exercise-solution/1.2.md)

## Chapter 2 Large-Sample Theory

### Section 1 Review of Limit Theorems for Sequences of Random Variables

* [Review Question 2.1.1](question-solution/2.1.1.md)
* [Review Question 2.1.2](question-solution/2.1.2.md)
* [Review Question 2.1.3](question-solution/2.1.3.md)
* [Review Question 2.1.4](question-solution/2.1.4.md)
* [Review Question 2.1.5](question-solution/2.1.5.md)

## Supplements

* [Taylor's linearization](supplements/taylor-linearization.md)
* [Variance-Covariance Matrix](supplements/var-cov-matrix.md)
* [Four Ways of Matrix Multiplication](supplements/matrix-multiplication.md)

#### 注

[^1]: Fumio Hayashi, _Econometrics_. Princeton University Press, 2000. (http://press.princeton.edu/titles/6946.html)

---

Copyright ©2018 by Qiang Gao