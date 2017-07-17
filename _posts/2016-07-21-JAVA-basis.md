---
layout: post
category: JAVA-basis
title: JAVA-basis 基础学习 
tags: JAVA-basis,2017
keywords: JAVA-basis,2017
---
<ul>
	
<li><p>
	boolean	不适用	false	true 或 false

</p></li>

<li><p>
	char	16 位	（无符号）	\u0000' \u0000' 到 \uffff' 或 0 到 65535
	
</p></li>

<li><p>
byte	8 位	0	-128 到 127<br/>
short	16 位	0	-32768 到 32767<br/>
int	32 位	0	-2147483648 到 2147483647<br/>
long	64 位	0	-9223372036854775808 到 9223372036854775807<br/>
float	32 位	0.0	1.17549435e-38 到 3.4028235e+38<br/>
double	64 位	0.0	4.9e-324 到 1.7976931348623157e+308
</p></li>

<li><p>
运算符	用法	返回 true 的条件……<br/>
>	&nbsp;&nbsp;&nbsp;	a > b	&nbsp;	a 大于 b<br/>
>=	&nbsp;	a >= b	&nbsp;	a 大于或等于 b<br/>
<	&nbsp;&nbsp;&nbsp;	a < b	&nbsp;	a 小于 b<br/>
<=	&nbsp;	a <= b	&nbsp;	a 小于或等于 b<br/>
==	&nbsp;	a == b	&nbsp;	a 等于 b<br/>
!=	&nbsp;	&nbsp;a != b	&nbsp;	a 不等于 b<br/>
&&	&nbsp;	a && b	&nbsp;	如果 a 和 b 均为 true，则有条件地计算 b（如果 a 为 false，则不计算 b）<br/>
||	&nbsp;	&nbsp;a || b	&nbsp;	a 或 b 为 true，则有条件地计算 b（如果 a 为 true，则不计算 b）<br/>
!	&nbsp;	&nbsp;!a	a 	&nbsp;	为 false<br/>
&	&nbsp;	a & b	&nbsp;	a 和 b 均为 true，则始终计算 b<br/>
|	&nbsp;	&nbsp;&nbsp;a | b	&nbsp;	如果 a 或 b 为 true，则始终计算 b<br/>
^	&nbsp;	&nbsp;a ^ b	&nbsp;	a 和 b 不同
</p></li>

<li><p>
	类 修饰符 <br/>
Public<br/>
可以从其他类中访问
Abstract<br/>
本类不能被实例化
Final<br/>
不能再声明子类
构造函数修饰符  
Public<br/>
可以从所有的类中访问
Protected<br/>
只能从自己的类和它的子类中访问
Private<br/>
只能在本类中访问
域/成员变量修饰符  
Public<br/>
可以从所有的类中访问
Protected<br/>
只能从本类和它的子类中访问
Private<br/>
只能从本类中访问它
Static<br/>
对该类的所有实例只能有一个域值存在
transient<br/>
不是一个对象持久状态的一部份
Volatile<br/>
可以被异步的线程所修改
final<br/>
必须对它赋予初值并且不能修改它
局部变量 修饰符 
final<br/>
必须对它赋予初值并且不能修改它
方法修饰符 
Public<br/>
可以从所有的类中访问它
Protected<br/>
只能从本类及其子类中访问它
Private<br/>
只能从本类中访问它
abstract<br/>
没有方法体，属于一个抽象类
final<br/>
子类不能覆盖它
static<br/>
被绑定于类本身而不是类的实例
native<br/>
该方法由其他编程语言实现
asnchronized<br/>
在一个线程调用它之前必须先给它加

</p></li>

</ul>
