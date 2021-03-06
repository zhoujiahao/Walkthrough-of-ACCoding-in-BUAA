# C1-2014级算法第一次上机

# `A` 零崎的人间冒险Ⅰ

时间限制：1000ms  内存限制：65536kb

通过率：2/3 `(66.67%) `  正确率：2/3 `(66.67%)`

## 题目描述

零崎最近一段时间非常无聊，于是他决定进行一场冒险，然而无聊的人遇到的冒险也非常的无聊，他的冒险刚刚开始就要结束了。 理由也非常的无聊，因为一个无聊的大魔王决定用一个非常有魔(wu)力(liao)的方式毁灭世界。 魔王有三个具有魔(wu)力(liao)的杆，暂时称为ABC，还有n个具有魔(wu)力(liao)的大小全都不同的盘子，这些盘子按照大小顺序放在A杆上，现在魔王要用具有魔(wu)力(liao)的方式移动到C杆，移动的过程中，小的盘子仍然只能摆在大的盘子上面而不能发生错乱，否侧魔王的魔法就会失灵。 然而魔王似乎想找一个无聊的人来替他完成这个魔法，而无聊的零崎也觉得这个事情非常的无聊，干脆就决定还是让你们去做。 零崎也不知道这个无聊的魔王到底有多少个有魔(wu)力(liao)的盘子，所以他说多少个你们就当是多少个吧。

## 输入

多组数据，每组一个数字n表示魔王的盘子数。

## 输出

对于每组数据，输出为魔王魔法发动后盘子移动的过程，两组输出之间用空行隔开。

## 输入样例

```
1
2
```

## 输出样例

```
A to C

A to B
A to C
B to C
```

## Hint

这个无聊的魔法还有个名字叫做传说中可以毁灭世界的汉诺塔之术。

## 思路

汉诺塔大水题

# `B` 零崎的人间冒险Ⅱ

时间限制：1000ms  内存限制：65536kb

通过率：1/1 `(100.00%) `  正确率：1/1 `(100.00%)`

## 题目描述

零崎本以为他的无聊冒险马上就要结束了，然而实际上距离魔王的魔法成功发动还有很久很久，于是他的无聊冒险还可以继续…… 无聊的零崎需要给自己的冒险找点事做，然而实际上他的日常非常平和，如果说有什么意外的话，那就是他去打麻将了。零崎在玩一种叫做日式麻将的竞技游戏，然而无聊的零崎总是遭遇别人立直需要防守的场面。 零崎在防守时，会跟打现物和搏筋兜牌两种技能，然而为了不被婊得太惨，零崎不会连续搏筋兜牌。也就是说，零崎任意两次选择中不会都是搏筋兜牌。 那么对于n次舍牌，无聊的零崎会有多少种选择？ 因为无聊的零崎可以打很久的麻将，所以n可能很大，无聊的零崎决定只要结果对100007求模后的选择数。

## 输入

多组输入数据，每组一个数字n，1<=n<=Int_MAX

## 输出

每组一行，只需要选择种数对100007求模后的结果。

## 输入样例

```
1
2
```

## 输出样例

```
2
3
```

## Hint

```
听说这个也是很简单的，不然你们推推递推公式看？
ps：
n=1:刚，怂
n=2 刚怂，怂怂，怂刚
n=3 刚怂怂，刚怂刚，怂怂怂，怂怂刚，怂刚怂
```

## 思路

仔细分析你就会发现，这道题就是一个斐波那契数列...

但是数据范围是INT_MAX 所以打表的时候必须考虑对100007取模之后的值的循环

# `C` Let's play a game

时间限制：1000ms  内存限制：65536kb

通过率：2/2 `(100.00%) `  正确率：2/2 `(100.00%)`

## 题目描述

```
这是一个古老而无聊的游戏，这是一个欧几里得躺枪的游戏。
```

Nova君和LaoWang决定一分胜负。给定两个正整数a,b。Nova君和LaoWang轮流从中将较大的数字减去较小数字的整数倍（1倍，2倍等等）。并且保证每次减完不会出现负数的情况。由Nova君先手。最终在自己回合将其中一个数变为0的一放获胜。两个人智商都还行，都会采取最优策略，谁会赢呢？

## 输入

多组测试数据。对于每组测试数据，给出两个数字a和b（保证Int范围内）

## 输出

对于每组数据，输出获胜者的名字。

## 输入样例

```
34 12
15 24
```

## 输出样例

```
Nova
LaoWang
```

## 思路

经典的威佐夫博弈问题

如果采取普通的博弈论搜索做法的话，需要在每一层搜索的时候先特殊判断a整除b直接结束游戏的情况

在完成了搜索的做法之后，通过观察规律你会发现这个题的结论会和黄金分割有点关系...

# `D` 零崎的人间冒险Ⅲ

时间限制：1000ms  内存限制：65536kb

通过率：0/1 `(0.00%) `  正确率：0/1 `(0.00%)`

## 题目描述

不打麻将的零崎特别的无聊，所以他又四处乱逛了。 四处乱逛的无聊零崎遇到了另一个特别无聊的人，因为这个人竟然在无聊的算各种一元n次多项式a0+a1x+a2x^2+……+anx^n！这个无聊的人算的实在太慢了令零崎忍不住想开启嘲讽模式，所以现在，快来给零崎搞一个能快速计算多项式的东西吧。（其实可能也不用特别快

## 输入

多组输入数据。 每组数据以多项式次数n开始，下一个数字为变量x，之后n+1个数字为系数a0……an。输入数据保证在int范围内

## 输出

每行一个结果，也许n特别大所以最后结果还是对1e6+7求模吧……

## 输入样例

```
1 2 1 2  
3 2 1 2 3 4
```

## 输出样例

```
5
49
```

## Hint

你听说过上古卷轴吗？你听说过彩虹小马吗？你听说过Horner Rule吗？

## 思路

霍纳法则，又称为秦九韶定理。在O(n)的时间内搞出多项式的值

# `E` Inverse number：Reborn

时间限制：1000ms  内存限制：65536kb

通过率：1/1 `(100.00%) `  正确率：1/1 `(100.00%)`

## 题目描述

输入一个正整数n，随后给出一个长度为n的整数序列a1,a2,a3...an。求给定序列的逆序数。

概念回顾：

逆序对：数列a[1],a[2],a[3]…中的任意两个数a[i],a[j]，如果a[i]>a[j],那么我们就说这两个数构成了一个逆序对。

逆序数：一个数列中逆序对的总数。

## 输入

多组测试数据。对于每组测试数据，给出序列长度n，和一个长度为n的序列a1,a2,a3...an

(0<n<=10^6，保证ai在int范围内)

## 输出

对于每组数据，输出该序列的逆序数。

## 输入样例

```
7 
3 5 4 8 2 6 9
```

## 输出样例

```
6
```

## Hint

```
1、用n^2的算法是不行不行滴╮(╯_╰)╭
2、分治法
```

## 思路

经典的归并排序求逆序对

当然了你想搞什么动态维护逆序对的权值线段树或者树状数组什么的我也不拦你...

# `F` 零崎的人间冒险Ⅳ

时间限制：1000ms  内存限制：65536kb

通过率：/ `(%) `  正确率：/ `(%)`

## 题目描述

在干掉了guangtou之后，无聊的零崎又去找事了……

说起来零崎前几周学到了一个叫做Apriori算法的东西，其第一步是挑出所有出现频率大于某个给定值的数据。然而作为一个具有一定程度的强(qiǎng )迫(pò)症的人，零崎显然希望先排个序再对其子集进行操作。

于是，现在的任务是简单的升序排列。

## 输入

多组输入数据，每组两行，第一行为一个整数n。第二行为n个整数。

## 输出

每组一行，输出n个整数的升序排列，两个整数之间用一个空格隔开。

## 输入样例

```
5
6 5 2 3 1 
```

## 输出样例

```
1 2 3 5 6
```

## 思路

这题本身sort其实可以水过...

但是作为计院/软院学生，拿sort水过就毫无意思了，你不拿这道题练一下十大排序怎么能行呢（狗头）

由于本题的数据范围限制，不适合写计数排序和桶排序，但是最差O(n^2)的冒泡插入和选择均可过

本篇包括了冒泡 插入 选择 快排的多种随机划分方式 堆排序 归并排序 基数排序 希尔排序，有需要的同学可以自行学习。

