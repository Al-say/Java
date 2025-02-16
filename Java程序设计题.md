# Java程序设计题集

## 试卷一程序设计题（每题6分，共30分）

1. 定义一个接口Readable，包含方法getTitle()用于获取阅读材料标题。（6分）

```java
// 在此处编写代码

```

2. 封装一个图书类Book，实现Readable接口，包含成员变量title和author，并实现接口中的方法，重写toString方法。（6分）

```java
// 在此处编写代码

```

3. 封装一个杂志类Magazine，实现Readable接口，包含成员变量title和issueNumber，并实现接口中的方法，重写toString方法。（6分）

```java
// 在此处编写代码

```

4. 封装图书馆类Library，包含方法addReadable(Readable readable)用于添加阅读材料到图书馆，和displayReadables()用于展示图书馆中所有阅读材料信息。（6分）

```java
// 在此处编写代码

```

5. 创建测试类LibraryTest，在图书馆中添加两本图书，例如"红楼梦"（作者：曹雪芹）和"平凡的世界"（作者：路遥），然后再添加两本杂志，例如"读者"（刊号：62-1190/Z）和"软件"（刊号：12-1151/TP）。最后，展示图书馆中所有图书和杂志的信息。（6分）

```java
// 在此处编写代码

```

## 试卷二程序设计题（每题6分，共30分）

1. 定义一个Shape抽象类，包含抽象方法calculateArea()和calculatePerimeter()，分别用于计算面积和周长。（6分）

```java
// 在此处编写代码

```

2. 定义Rectangle类继承Shape类，包含width和height属性，实现父类的抽象方法。（6分）

```java
// 在此处编写代码

```

3. 定义Circle类继承Shape类，包含radius属性，实现父类的抽象方法。（6分）

```java
// 在此处编写代码

```

4. 创建一个ShapeCalculator类，包含静态方法printShapeInfo(Shape shape)，用于打印图形的面积和周长信息。（6分）

```java
// 在此处编写代码

```

5. 编写测试类ShapeTest，创建一个长为5、宽为3的矩形对象和一个半径为4的圆形对象，并使用ShapeCalculator类的printShapeInfo方法输出它们的面积和周长。（6分）

```java
// 在此处编写代码

```

## 试卷三程序设计题（每题6分，共30分）

1. 定义一个泛型接口DataProcessor<T>，包含方法process(T data)用于处理数据。（6分）

```java
// 在此处编写代码

```

2. 创建StringProcessor类实现DataProcessor<String>接口，在process方法中实现字符串转大写的功能。（6分）

```java
// 在此处编写代码

```

3. 创建NumberProcessor类实现DataProcessor<Integer>接口，在process方法中实现计算数字平方的功能。（6分）

```java
// 在此处编写代码

```

4. 创建一个ProcessorExecutor类，使用CompletableFuture实现异步处理数据的功能，包含方法executeAsync接收DataProcessor和数据，异步处理并返回结果。（6分）

```java
// 在此处编写代码

```

5. 编写测试类ProcessorTest，创建字符串处理器和数字处理器的实例，使用ProcessorExecutor异步处理"hello"和数字5，并通过Stream API将结果收集到List中展示。（6分）

```java
// 在此处编写代码

```

## 运行结果示例

试卷一运行结果示例：
```
图书馆藏书：
1. 书名：红楼梦，作者：曹雪芹
2. 书名：平凡的世界，作者：路遥
3. 杂志：读者，刊号：62-1190/Z
4. 杂志：软件，刊号：12-1151/TP
```

试卷二运行结果示例：
```
矩形信息：
- 面积：15.0
- 周长：16.0

圆形信息：
- 面积：50.27
- 周长：25.13
```

试卷三运行结果示例：
```
处理结果：
字符串处理结果：HELLO
数字处理结果：25
异步处理完成时间：2025-02-16 17:13
收集到的结果列表：[HELLO, 25]
