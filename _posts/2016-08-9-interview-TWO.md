---
layout: post
category: interview-TWO
title: interview-TWO 面试学习 
tags: interview-TWO,2017
keywords: interview-TWO,2017
---

<h2>集合二</h2>

<ul>
<li><p>
面向对象的特征有哪些方面？<br/>
抽象，继承，封装，多态
</p></li>

<li><p>
String 是最基本的数据类型吗？<br/>
答：不是。Java中的基本数据类型只有8个：byte、short、int、long、float、double、char、boolean；
</p></li>

<li><p>
float f=3.4;是否正确？<br/>
答:不正确。3.4是双精度数，需要强制类型转换float f =(float)3.4; 或者写成float f =3.4F;。
</p></li>

<li><p>
short s1 = 1; s1 = s1 + 1;有错吗?short s1 = 1; s1 += 1;有错吗？ <br/>
答：对于short s1 = 1; s1 = s1 + 1;由于1是int类型，因此s1+1运算结果也是int 型，需要强制转换类型才能赋值给short型。
而short s1 = 1; s1 += 1;可以正确编译，因为s1+= 1;相当于s1 = (short)(s1 + 1);其中有隐含的强制类型转换。
</p></li>

<li><p>
Java有没有goto？<br/>
答：goto 是Java中的保留字，在目前版本的Java中没有使用。
</p></li>

<li><p>
int和Integer有什么区别？ <br/>
答：int的包装类就是integer
</p></li>

<li><p>
解释内存中的栈(stack)、堆(heap)和静态区(static area)的用法。 <br/>
答：函数调用的现场保存都使用内存中的栈空间；<br/>
栈空间操作起来最快但是栈很小，<br/>
通常大量的对象都是放在堆空间，
</p></li>

<li><p>
解释内存中的栈(stack)、堆(heap)和静态区(static area)的用法。<br/>
答：通常我们定义一个基本数据类型的变量，一个对象的引用，还有就是函数调用的现场保存都使用内存中的栈空间；而通过new关键字和构造器创建的对象放在堆空间；程序中的字面量（literal）如直接书写的100、'hello'和常量都是放在静态区中。栈空间操作起来最快但是栈很小，通常大量的对象都是放在堆空间，理论上整个内存没有被其他进程使用的空间甚至硬盘上的虚拟内存都可以被当成堆空间来使用。
</p></li>

<li><p>
swtich 是否能作用在byte 上，是否能作用在long 上，是否能作用在String上？<br/>
答：在Java 5以前，switch(expr)中，expr只能是byte、short、char、int。从Java 5开始，Java中引入了枚举类型，expr也可以是enum类型，从Java 7开始，expr还可以是字符串（String），
但是长整型（long）在目前所有的版本中都是不可以的。
</p></li>

<li><p>
用最有效率的方法计算2乘以8？<br/>
答： 2 << 3（左移3位相当于乘以2的3次方，右移3位相当于除以2的3次方）。
</p></li>

<li><p>
数组有没有length()方法？String有没有length()方法？<br/>
答：数组没有length()方法，有length 的属性。String 有length()方法。
</p></li>

<li><p>
在Java中，如何跳出当前的多重嵌套循环？<br/>
答：在最外层循环前加一个标记如A，然后用break A;可以跳出多重循环
</p></li>

<li><p>
构造器（constructor）是否可被重写（override）？ v
答：构造器不能被继承，因此不能被重写，但可以被重载。
</p></li>

<li><p>
两个对象值相同(x.equals(y) == true)，但却可有不同的hash code，这句话对不对？<br/>
答：不对，如果两个对象x和y满足x.equals(y) == true，它们的哈希码（hash code）应当相同。
</p></li>

<li><p>
是否可以继承String类？ <br/>
答：String 类是final类，不可以被继承。
</p></li>

<li><p>
当一个对象被当作参数传递到一个方法后，此方法可改变这个对象的属性，并可返回变化后的结果，那么这里到底是值传递还是引用传递？<br/>
答：是值传递。Java语言的方法调用只支持参数的值传递。
</p></li>

<li><p>
String和StringBuilder、StringBuffer的区别？ <br/>
答：Java平台提供了两种类型的字符串：String和StringBuffer/StringBuilder，它们可以储存和操作字符串。其中String是只读字符串，而StringBuffer/StringBuilder类表示的字符串对象可以直接进行修改。
</p></li>

<li><p>
重载（Overload）和重写（Override）的区别。<br/>
答：方法的重载和重写都是实现多态的方式，<br/>
区别在于前者实现的是编译时的多态性，
而后者实现的是运行时的多态性
</p></li>

<li><p>
描述一下JVM加载class文件的原理机制？<br/>
答：JVM中类的装载是由类加载器（ClassLoader）和它的子类来实现的，Java中的类加载器是一个重要的Java运行时系统组件，它负责在运行时查找和装入类文件中的类。
</p></li>

<li><p>
char 型变量中能不能存贮一个中文汉字，为什么？ <br/>
答：char类型可以存储一个中文汉字，因为Java中使用的编码是Unicode，一个char类型占2个字节，所以放一个中文是没问题的。
</p></li>

<li><p>
抽象类（abstract class）和接口（interface）有什么异同？ <br/>
答：抽象类和接口都不能够实例化，但可以定义抽象类和接口类型的引用。
</p></li>

<li><p>
静态嵌套类(Static Nested Class)和内部类（Inner Class）的不同？<br/>
答：Static Nested Class是被声明为静态（static）的内部类，它可以不依赖于外部类实例被实例化。
</p></li>

<li><p>
Java 中会存在内存泄漏吗，请简单描述。<br/>
答：理论上Java因为有垃圾回收机制（GC）不会存在内存泄露问题（；然而在实际开发中，可能会存在无用但可达的对象，一级缓存中的对象属于持久态，垃圾回收器是不会回收这些对象的，然而这些对象中可能存在无用的垃圾对象，如果不及时关闭（close）或清空（flush）一级缓存就可能导致内存泄露。
</p></li>

<li><p>
抽象的（abstract）方法是否可同时是静态的（static）,是否可同时是本地方法（native），是否可同时被synchronized修饰？ <br/>
答：都不能。抽象方法需要子类重写，而静态的方法是无法被重写的，因此二者是矛盾的。
</p></li>

<li><p>
阐述静态变量和实例变量的区别。 <br/>
答：静态变量是被static修饰符修饰的变量，它属于类，不属于类的任何一个对象；
实例变量必须依存于某一实例，需要先创建对象然后通过对象才能访问到它；
</p></li>

<li><p>
是否可以从一个静态（static）方法内部发出对非静态（non-static）方法的调用？ <br/>
答：不可以，静态方法只能访问静态成员，因为非静态方法的调用要先创建对象，在调用静态方法时可能对象并没有被初始化。
</p></li>

<li><p>
如何实现对象克隆？ <br/>
答：有两种方式： <br/>
??1). 实现Cloneable接口并重写Object类中的clone()方法； <br/>
??2). 实现Serializable接口，通过对象的序列化和反序列化实现克隆
</p></li>

<li><p>
GC是什么？ <br/>
答：GC是垃圾收集的意思
</p></li>

<li><p>
String s = new String('xyz');创建了几个字符串对象？ <br/>
答：两个对象，一个是静态区的'xyz'，一个是用new创建在堆上的对象。
</p></li>

<li><p>
接口是否可继承（extends）接口？抽象类是否可实现（implements）接口？抽象类是否可继承具体类（concrete class）？<br/>
答：接口可以继承接口，而且支持多重继承。抽象类可以实现(implements)接口，抽象类可继承具体类也可以继承抽象类。
</p></li>

<li><p>
一个'.java'源文件中是否可以包含多个类（不是内部类）？有什么限制？ <br/>
答：可以，但一个源文件中最多只能有一个公开类（public class）而且文件名必须和公开类的类名完全保持一致。
</p></li>

<li><p>
Anonymous Inner Class(匿名内部类)是否可以继承其它类？是否可以实现接口？ <br/>
答：可以继承其他类或实现其他接口，在Swing编程和Android开发中常用此方式来实现事件监听和回调。
</p></li>

<li><p>
内部类可以引用它的包含类（外部类）的成员吗？有没有什么限制？<br/>
答：一个内部类对象可以访问创建它的外部类对象的成员，包括私有成员
</p></li>

<li><p>
Java 中的final关键字有哪些用法？<br/>
答：(1)修饰类：表示该类不能被继承；(2)修饰方法：表示方法不能被重写；(3)修饰变量：表示变量只能一次赋值以后值不能被修改（常量）。
</p></li>

<li><p>
数据类型之间的转换：<br/>
- 如何将字符串转换为基本数据类型？ <br/>
- 如何将基本数据类型转换为字符串？ 
答： 
- 调用基本数据类型对应的包装类中的方法parseXXX(String)或valueOf(String)即可返回相应基本类型； <br/>
- 一种方法是将基本数据类型与空字符串（''）连接（+）即可获得其所对应的字符串；另一种方法是调用String 类中的valueOf()方法返回相应字符串
</p></li>

<li><p>
如何实现字符串的反转及替换？<br/>
答：方法很多，可以自己写实现也可以使用String或StringBuffer/StringBuilder中的方法。
</p></li>

<li><p>
比较一下Java和JavaSciprt。 <br/>
答：JavaScript 与Java是两个公司开发的不同的两个产品。Java 是原Sun公司推出的面向对象的程序设计语言；<br/>
而JavaScript是Netscape公司的产品，为了扩展Netscape浏览器的功能而开发的一种可以嵌入Web页面中运行的基于对象和事件驱动的解释性语言。
</p></li>

<li><p>
Error和Exception有什么区别？ <br/>
答：Error表示系统级的错误和程序不必处理的异常，是恢复不是不可能但很困难的情况下的一种严重问题；比如内存溢出，不可能指望程序能处理这样的情况；<br/>
Exception表示需要捕捉或者需要程序进行处理的异常，是一种设计或实现问题；也就是说，它表示如果程序运行正常，从不会发生的情况。
</p></li>

<li><p>
try{}里有一个return语句，那么紧跟在这个try后的finally{}里的代码会不会被执行，什么时候被执行，在return前还是后?<br/>
答：会执行，在方法返回调用者前执行。
</p></li>

<li><p>
Java语言如何进行异常处理，关键字：throws、throw、try、catch、finally分别如何使用？ <br/>
答：Java通过面向对象的方法进行异常处理，Java的异常处理是通过5个关键词来实现的：try、catch、throw、throws和finally。<br/>
一般情况下是用try来执行一段程序，如果系统会抛出（throw）一个异常对象，可以通过它的类型来捕获（catch）它，或通过总是执行代码块（finally）来处理；<br/>
try用来指定一块预防所有异常的程序；catch子句紧跟在try块后面，用来指定你想要捕获的异常的类型；throw语句用来明确地抛出一个异常；<br/>
throws用来声明一个方法可能抛出的各种异常（当然声明异常时允许无病呻吟）；<br/>
finally为确保一段代码不管发生什么异常状况都要被执行；<br/>
try语句可以嵌套，每当遇到一个try语句，异常的结构就会被放入异常栈中，直到所有的try语句都完成。如果下一级的try语句没有对某种异常进行处理，异常栈就会执行出栈操作，直到遇到有处理这种异常的try语句或者最终将异常抛给JVM。
</p></li>

<li><p>
列出一些你常见的运行时异常？<br/>
答： <br/>
- ArithmeticException（算术异常） <br/>
- ClassCastException （类转换异常） <br/>
- IllegalArgumentException （非法参数异常） <br/>
- IndexOutOfBoundsException （下标越界异常） <br/>
- NullPointerException （空指针异常） <br/>
- SecurityException （安全异常）
</p></li>

<li><p>
阐述final、finally、finalize的区别。 <br/>
答： <br/>
- final：修饰符（关键字）有三种用法：<br/>
如果一个类被声明为final，意味着它不能再派生出新的子类，即不能被继承<br/>
将变量声明为final，可以保证它们在使用中不被改变。<br/>
被声明为final的方法也同样只能使用，不能在子类中被重写。<br/>
 
- finally：通常放在try…catch…的后面构造总是执行代码块，这里的代码只要JVM不关闭都能执行，可以将释放外部资源的代码写在finally块中。<br/>
 
- finalize：Object类中定义的方法，Java中允许使用finalize()<br/>方法在垃圾收集器将对象从内存中清除出去之前做必要的清理工作。这个方法是由垃圾收集器在销毁对象时调用的，通过重写finalize()<br/>方法可以整理系统资源或者执行其他清理工作。

</p></li>

<li><p>
List、Set、Map是否继承自Collection接口？ <br/>
答：List、Set 是，Map 不是。<br/>
Map是键值对映射容器，
而Set存储的零散的元素且不允许有重复元素<br/>
List是线性结构的容器
</p></li>

<li><p>
List、Map、Set三个接口存取元素时，各有什么特点？ <br/>
答：List以特定索引来存取元素，可以有重复元素。<br/>
Set不能存放重复元素（用对象的equals()方法来区分元素是否重复）。<br/>
Map保存键值对（key-value pair）映射，映射关系可以是一对一或多对一
</p></li>

<li><p>
Collection和Collections的区别？ <br/>
答：Collection是一个接口；Collections是个一个工具类，

</p></li>

<li><p>
线程的sleep()方法和yield()方法有什么区别？ <br/>
答： <br/>
sleep()方法给其他线程运行机会时不考虑线程的优先级；<br/>
yield()方法只会给相同优先级或更高优先级的线程以运行的机会； 
</p></li>

<li><p>
当一个线程进入一个对象的synchronized方法A之后，其它线程是否可进入此对象的synchronized方法B？ <br/>
答：不能。
</p></li>

<li><p>
、请说出与线程同步以及线程调度相关的方法。 <br/>
答： <br/>
- wait()：使一个线程处于等待（阻塞）状态，并且释放所持有的对象的锁； <br/>
- sleep()：使一个正在运行的线程处于睡眠状态，是一个静态方法，调用此方法要处理InterruptedException异常； <br/>
- notify()：唤醒一个处于等待状态的线程，当然在调用此方法的时候，并不能确切的唤醒某一个等待状态的线程，而是由JVM确定唤醒哪个线程，而且与优先级无关； 
- notityAll()：唤醒所有处于等待状态的线程，该方法并不是将对象的锁给所有线程，而是让它们竞争，只有获得锁的线程才能进入就绪状态；
</p></li>

<li><p>
编写多线程程序有几种实现方式？ <br/>
答：Java 5以前实现多线程有两种实现方法：一种是继承Thread类；另一种是实现Runnable接口。
</p></li>

<li><p>
synchronized关键字的用法？<br/>
答：synchronized关键字可以将对象或者方法标记为同步，以实现对对象和方法的互斥访问，

</p></li>

<li><p>
举例说明同步和异步。 <br/>
答：所谓的同步就是指阻塞式操作，而异步就是非阻塞式操作。

</p></li>

<li><p>
启动一个线程是调用run()还是start()方法？<br/>
答：启动一个线程是调用start()方法，使线程所代表的虚拟处理机处于可运行状态，这意味着它可以由JVM 调度并执行，这并不意味着线程就会立即运行。
run()方法是线程启动后要进行回调（callback）的方法。
</p></li>

<li><p>
什么是线程池（thread pool）？ <br/>
答：线程池就是事先创建若干个可执行的线程放入一个池（容器）中，需要的时候从池中获取线程不用自行创建，使用完毕不需要销毁线程而是放回池中，从而减少创建和销毁线程对象的开销。
</p></li>

<li><p>
简述synchronized 和java.util.concurrent.locks.Lock的异同？<br/>
答：Lock 能完成synchronized所实现的所有功能；<br/>
synchronized会自动释放锁，而Lock一定要求程序员手工释放，并且最好在finally 块中释放（这是释放外部资源的最好的地方）。<br/>
主要不同点：Lock有比synchronized更精确的线程语义和更好的性能，而且不强制性的要求一定要获得锁。
</p></li>

<li><p>
Java中如何实现序列化，有什么意义？<br/>
答：序列化就是一种用来处理对象流的机制，所谓对象流也就是将对象的内容进行流化。可以对流化后的对象进行读写操作，也可将流化后的对象传输于网络之间。
</p></li>

<li><p>
Java中有几种类型的流？ <br/>
答：字节流和字符流；

</p></li>

<li><p>
XML文档定义有几种形式？它们之间有何本质区别？解析XML文档有哪几种方式？ <br/>
答：XML文档定义分为DTD和Schema两种形式

</p></li>

<li><p>
你在项目中哪些地方用到了XML？<br/>
答：数据交换和信息配置。

</p></li>

<li><p>
Statement和PreparedStatement有什么区别？哪个性能更好？<br/>
答：与Statement相比，①PreparedStatement接口代表预编译的语句，它主要的优势在于可以减少SQL的编译错误并增加SQL的安全性；<br/>
②PreparedStatement中的SQL语句是可以带参数的，避免了用字符串连接拼接SQL语句的麻烦和不安全；<br/>
③当批量处理SQL或频繁执行相同的查询时，PreparedStatement有明显的性能上的优势，由于数据库可以将编译优化后的SQL语句缓存起来，下次执行相同结构的语句时就会很快

</p></li>

<li><p>
使用JDBC操作数据库时，如何提升读取数据的性能？如何提升更新数据的性能？ <br/>
答：要提升读取数据的性能，可以指定通过结果集对象的setFetchSize()方法指定每次抓取的记录数；<br/>
要提升更新数据的性能可以使用PreparedStatement语句构建批处理，将若干SQL语句置于一个批处理中执行。

</p></li>

<li><p>
在进行数据库编程时，连接池有什么作用？<br/>
答：由于创建连接和释放连接都有很大的开销，为了提升系统访问数据库的性能，可以事先创建若干连接置于连接池中，需要时直接从连接池获取，使用结束时归还连接池而不必关闭连接，从而避免频繁创建和释放连接所造成的开销，这是典型的用空间换取时间的策略（浪费了空间存储连接，但节省了创建和释放连接的时间）。
</p></li>

<li><p>
什么是DAO模式？<br/>
答：DAO（Data Access Object）顾名思义是一个为数据库或其他持久化机制提供了抽象接口的对象，在不暴露底层持久化方案实现细节的前提下提供了各种数据访问操作。DAO模式实际上包含了两个模式，一是Data Accessor（数据访问器），二是Data Object（数据对象）
</p></li>

<li><p>
事务的ACID是指什么？ <br/>
答： <br/>
- 原子性(Atomic)：事务中各项操作，要么全做要么全不做，任何一项操作的失败都会导致整个事务的失败； <br/>
- 一致性(Consistent)：事务结束后系统状态是一致的； <br/>
- 隔离性(Isolated)：并发执行的事务彼此无法看到对方的中间状态； <br/>
- 持久性(Durable)：事务完成后所做的改动都会被持久化，即使发生灾难性的失败。通过日志和同步备份可以在故障发生后重建数据。
</p></li>

<li><p>
JDBC能否处理Blob和Clob？<br/>
答： 可以<br/>
Blob是指二进制大对象（Binary Large Object），<br/>
而Clob是指大字符对象（Character Large Objec），
</p></li>

<li><p>
简述正则表达式及其用途。 <br/>
答：在编写处理字符串的程序时，经常会有查找符合某些复杂规则的字符串的需要。正则表达式就是用于描述这些规则的工具。换句话说，正则表达式就是记录文本规则的代码。
</p></li>

<li><p>
Java中是如何支持正则表达式操作的？ <br/>
答：Java中的String类提供了支持正则表达式操作的方法，包括：matches()、replaceAll()、replaceFirst()、split()。

</p></li>

<li><p>
获得一个类的类对象有哪些方式？ <br/>
答： <br/>
- 方法1：类型.class，例如：String.class 
- 方法2：对象.getClass()，例如：'hello'.getClass() 
- 方法3：Class.forName()，例如：Class.forName('java.lang.String')

</p></li>

<li><p>
如何通过反射创建对象？ <br/>
答： <br/>
- 方法1：通过类对象调用newInstance()方法，例如：String.class.newInstance() <br/>
- 方法2：通过类对象的getConstructor()或getDeclaredConstructor()方法获得构造器（Constructor）对象并调用其newInstance()<br/>方法创建对象，例如：String.class.getConstructor(String.class).newInstance('Hello');

</p></li>

<li><p>
简述一下你了解的设计模式。 <br/>
答：所谓设计模式，是为了可重用代码、让代码更容易被他人理解、保证代码可靠性。设计模式使人们可以更加简单方便的复用成功的设计和体系结构。将已证实的技术表述成设计模式也会使新系统开发者更加容易理解其设计思路。

</p></li>

<li><p>
什么是UML？ <br/>
答：UML是统一建模语言（Unified Modeling Language）的缩写，它发表于1997年，综合了当时已经存在的面向对象的建模语言、方法和过程，是一个支持模型化和软件系统开发的图形化语言，为软件开发的所有阶段提供模型化和可视化支持。使用UML可以帮助沟通与交流，辅助应用设计和文档的生成，还能够阐释系统的结构和行为。
</p></li>

</ul>