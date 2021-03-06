# Other-开放题目

# 1. 温度转换

时间限制: 1000 ms 内存限制: 65536 kb

总通过人数: 394 总提交人数: 417

## 题目描述

输入一个以华氏度为单位的温度f，试输出摄氏度c，并保留两位小数。转换公式为：c = (f-32) * (5/9)

## 输入

一个正数f，代表华氏度

## 输出

对应的摄氏度，要求保留两位小数

## 输入样例

```
104
```

## 输出样例

```
40.00
```

## Tips

1.如果题目没有明确说数据为正整数时，表示数据不保证为正整数，尽量不要使用int(input())来接收数据。

2.使用input()函数时，不要加提示信息，使用print()函数输出结果时，请不要输出多余信息，否则会wa。

祝大家coding愉快！

# 2. 大数求余

时间限制: 1000 ms 内存限制: 65536 kb

总通过人数: 380 总提交人数: 384

## 题目描述

在Python出现之前，总有人问小明，一个大数除以 1000000007 的余数是多少，我也不知道为什么会有这么奇怪的要求。但是Python对于大数的运算支持得非常好，这对于初学Python的你也不是问题。

现在给出正整数a、b，试求𝑎𝑏𝑚𝑜𝑑1000000007abmod1000000007的值。

## 输入

两行，分别是正整数a、b。

## 输出

𝑎𝑏𝑚𝑜𝑑1000000007abmod1000000007 的值。

## 输入样例

```
3
228
```

## 输出样例

```
472239553
```

## 思路

如果你是士谔书院，致力于6系或者21系的同学，恕我直言，**自带高精的java和python是毫无灵魂的！！！（此乃一家之言）**。然而本题即使是用C来做，**依旧不需要写高精模板，即可通过。这需要结合一定的数论知识。建议好好思考一下**

# 3. 利息

时间限制: 1000 ms 内存限制: 65536 kb

总通过人数: 366 总提交人数: 372

## 题目描述

请你帮小明计算存款的利息。

已知本金m，年利率（人民币）r，存款年数n，你应该可以算出来复利（每年的利息也作为下一年的本金计算）吧。

但是现在小明要求今天把美元换成人民币再存，取出之日再换回美元（两日汇率不同）。

## 输入

一共5行，每行一个正数，从上到下依次为：

本金m（美元）

年利率r

存款年数n（正整数）

存款日美元兑人民币汇率a

取款日美元兑人民币汇率b

## 输出

取款日换得的美元，向下取整。

## 输入样例

```
1000
0.02
10
6.5
6.9
```

## 输出样例

```
1148
```

# 4. Hello World

时间限制: 1000 ms 内存限制: 65536 kb

总通过人数: 345 总提交人数: 353

## 题目描述

小明今天学习了Python语言，大家都知道，学一门语言一般要做的第一件事就是打印Hello World。

现在小明想要打印n次Hello World，但是小明还没有学循环，所以只能用复制粘贴的方法，粘贴打印语句。假设刚开始只有一行，问小明最少需要粘贴几次才能获得n行Hello World？

## 输入

行数n，一个正整数。

## 输出

复制粘贴的次数。

## 输入样例1

```
5
```

## 输出样例1

```
3
```

## 输入样例2

```
9
```

## 输出样例2

```
4
```

# 6. 网购打折

时间限制: 1000 ms 内存限制: 65536 kb

总通过人数: 328 总提交人数: 336

## 题目描述

网购商家的打折策略现在十分复杂，需要你设计程序计算在各个商家的打折策略下，哪家的钱数最少。

假设有两家电商的打折策略如下：

电商A：满300减50，满500减100，满1000减300（三者只能选一个）；

电商B：超过300（不含300）的部分打8折。

要求根据输入的购物金额，计算打折后的最小金额。

## 输入

购物金额n，一个正数

## 输出

打折后的最小金额，保留两位小数。

## 样例输入1：

```
1370
```

## 样例输出1：

```
1070.00
```

## 样例输入2：

```
2000
```

## 样例输出2：

```
1660.00
```

## 样例输入3：

```
400
```

## 样例输出3：

```
350.00
```

# 7.计算𝜋

时间限制: 1000 ms 内存限制: 65536 kb

总通过人数: 232 总提交人数: 245

## 题目描述

利用下面的公式计算𝜋π。
$$
\frac{2}{\pi}=\frac{\sqrt2}{2}\frac{\sqrt{2+\sqrt2}}{2}\frac{\sqrt{2+\sqrt{2+\sqrt2}}}{2}\cdots
$$
当前后两次的计算误差不超过一个很小的正数𝛿δ时，停止迭代。



## 输入

一个正整数n，表示精确度𝛿=10−𝑛δ=10−n。

## 输出

迭代的次数和计算的𝜋π值，各一行，𝜋π值保留小数点后n位。

## 输入样例

```
9
```

## 输出样例

```
16
3.141592653
```

# 8. 最大公约数

时间限制: 1000 ms 内存限制: 65536 kb

总通过人数: 277 总提交人数: 278

## 题目描述

设计一个程序来求两个正整数的最大公约数gcd。提示：使用辗转相除法。

## 输入

两行，分别为正整数a、b。

## 输出

a和b的最大公约数。

## 输入样例

```
24
32
```

## 输出样例

```
8
```

# 9. 寻找新水仙花数

时间限制: 1000 ms 内存限制: 65536 kb

总通过人数: 239 总提交人数: 243

## 题目描述

水仙花数是各位的数字的三次方加起来等于自身的数。但是我们现在定义新水仙花数：三位数𝑖𝑗𝑘ijk满足𝑖𝑎+𝑗𝑏+𝑘𝑐=𝑖𝑗𝑘ia+jb+kc=ijk，其中，a、b、c是分别小于x、y、z的正整数。

**在计数时，我们规定，排列(i,j,k,a,b,c)不同，即使三位数𝑖𝑗𝑘ijk相同，也算作不同的水仙花数。**

## 输入

三行，分别是正整数x、y、z

## 输出

新水仙花数的数量

## 输入样例

```
2
2
4
```

## 输出样例

```
2
```

解释：51+11+83=51851+11+83=518，71+31+93=73971+31+93=739，新水仙花数共2种。

# 10.定积分

时间限制: 1000 ms 内存限制: 65536 kb

总通过人数: 227 总提交人数: 233

## 题目描述

我们可以把函数图像下的面积近似成若干个小矩形的面积之和。现在请你用Python编程实现定积分的计算。给出一个区间[a,b]，计算∫𝑏𝑎𝑒−𝑥2𝑑𝑥∫abe−x2dx。

e取2.71828。

为方便计算，取每个小区间左端点计算每个小矩形的面积。

## 输入

两个正整数，表示区间端点a、b。小矩形的宽度k(a<b,k<b-a)，为浮点数。a、b、k各一行，保证k*n=b-a，其中n为正整数。

## 输出

定积分计算结果，保留5位小数。

## 输入样例1

```
0
1
0.1
```

## 输出样例1

```
0.77782
```

## 样例输入2：

```
0
5
0.01
```

## 样例输出2：

```
0.89123
```

# 11. 吃鱼

时间限制: 1000 ms 内存限制: 65536 kb

总通过人数: 202 总提交人数: 206

## 题目描述

有一条鱼F，它顺着河流往下游，不能回头。一路上它会遇见很多其他的鱼，F只能吃比自己体型小的鱼。当F吃下一条鱼时，F的体型也会长大。如果这条鱼比F的一半还小，那么F可以获得该鱼全部体重；否则，F可以获得该鱼体重的一半。

给出河道里若干条鱼的体重，求F游到下游时的体重。

## 输入

共两行。

第一行，为河里从上游到下游的若干条鱼的体重，每个值之间用一个空格分隔。

第二行，为F的体重。

所有的体重值都是正整数。

## 输出

F最终的体重，保留一位小数。

## 输入样例

```
5 4 1 5 9 1 2 4
3
```

## 输出样例

```
9.0
```

解释：F吃1变4，再吃1变5，再吃2变7，再吃4变9。

## 思路

注意python的input是个字符串，python是自带split的

# 13. 代码对齐

时间限制: 1000 ms 内存限制: 65536 kb

总通过人数: 73 总提交人数: 102

## 题目描述

Python代码要求严格对齐才能执行。但是对齐问题往往很难发现，有时候只是某一行少了或者多了一个空格，就会报错。现在请你编写一个Python程序来帮你整理一下代码，解决少空格或多空格的问题。

要求：

（1）把所有的tab(`'\t'`)换成4个空格。

（2）使每一行前的空格数必须是4的倍数。把空格补充成不小于自身的最小的4的倍数。如，3个空格补成4个，5个空格补成8个。

**注意：这样的要求并不能保证输出代码一定是语法正确的。**

（3）确保“#”与注释文字间至少有一个空格。只需要处理每行的第一个“#”即可，将后面的“#”看做注释中的文字。

## 输入

第一行是一个正整数n，代表代码的行数。

接下来n行，是需要整理的代码。

## 输出

整理后的代码。

## 输入样例

```
8
#terrible code
for i in range(100):
   if i % 2 == 0:
       print('%d is an even number\n'%i)
  if i % 3 == 0:
     print('%d can be divided by 3\n'%i)
#tell people it's over
print('It\'s over')
```

## 输出样例

```
# terrible code 
for i in range(100):
    if i % 2 == 0:
        print('%d is an even number\n'%i)
    if i % 3 == 0:
        print('%d can be divided by 3\n'%i)
# tell people it's over
print('It\'s over')
```

## 思路

小型字符串处理问题，可以使用正则也可以不用

# 14. 超市收银系统

时间限制: 1000 ms 内存限制: 65536 kb

总通过人数: 73 总提交人数: 116

## 题目描述

**本题描述有更改，清注意**

一般超市或商店的收银台在对商品扫码之后会得到一串数字，这串数字代表一种商品。假设已知所有商品的名称、代码和单价，现在需要你写一个程序，输入扫码得到的商品代码（假设固定为6位数字），计算所购买的每种商品的数量（件数）、总价，并按照字典序打印商品的小票（如果某种商品购买了多件，应在同一行内输出该商品的**名称**、**数量**、**单价**和**总价**）。计算所购买所有商品的总金额，并打印。 给出商品目录如下：

```
格式：名称 代码 单价
chips 932071 3.50
chocolate 114049 8.00
soap 304985 2.90
cupcake 955962 4.90
cookie 313903 6.50
milk 243813 3.20
toothbrush 961995 4.80
toothpaste 933328 9.30
teapot 914500 29.80
```

## 输入

每行为一个6位数字，代表所购买的商品代码。当所有购买商品输入完毕时，以输入0为结束输入标志。（毕竟你不可能跟收银员说我买了n件商品嘛）。

## 输出

一张小票，要求： 第一行包含“NAME”、“QUANTITY”、“PRICE”、“SUM”（代表商品的名称、数量、单价和总价），各单词之间用若干空格分隔。

接下来若干行，每行对应所购买的某种商品的明细。要求每列按照该项目内容字符数量最多的那一项填充空格补齐(第一行也要补齐)，要求每列左对齐，对齐之后项目之间还要空一格。

**总价输出保留两位小数，其余数字按照Python默认输出。**

**按照商品名称的字典序输出。提示：可使用list.sort()**

最后一行是所购买所有商品的总金额，格式为：total:xxx.xx（注意：这里是西文的冒号，保留小数点后2位）

## 输入样例

```
932071
114049
932071
932071
114049
114049
932071
0
```

## 输出样例

```
NAME      QUANTITY PRICE SUM
chips     4        3.5   14.00
chocolate 3        8.0   24.00
total:38.00
```

## 思路

注意输出的格式枚举讨论即可。存储各类商品建议采用字典结构

# 转圈圈

时间限制: 1000 ms 内存限制: 65536 kb

总通过人数: 71 总提交人数: 76

## 题目描述

情人节到了（其实是过去了），偷偷送大家一道题。

本题要求你输出一个尺寸为𝑑×𝑑d×d的数阵，数字的排列方式是从1到n循环且顺时针转圈，看样例输出。

## 输入

两行，第一行是正整数n(n<10)，第二行是正整数d(d<20)

## 输出

转圈圈的数阵

## 输入样例1

```
6
4
```

## 输出样例1

```
1 2 3 4
6 1 2 5
5 4 3 6
4 3 2 1
```

## 输入样例2

```
5
5
```

## 输出样例2

```
1 2 3 4 5
1 2 3 4 1
5 4 5 5 2
4 3 2 1 3
3 2 1 5 4
```

