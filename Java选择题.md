# Java选择题集

## 试卷一选择题

1. 下面4种类型的文件中（）可以在Java虚拟机中运行。
   - A. .java
   - B. .jre
   - C. .exe
   - D. .class

```answer

```

2. 下列选项中，不属于基本数据类型的是（）
   - A. String
   - B. short
   - C. boolean
   - D. char

```answer

```

3. 假设int x=2，三元表达式x>0?x+1:5（）
   - A. 0
   - B. 2
   - C. 3
   - D. 5

```answer

```

4. 阅读下列程序：
```java
class Person {
    void say() {
        System.out.println("hello");
    }
}

class Example {
    public static void main(String[] args) {
        Person p2 = new Person();
        Person p1 = new Person();
        p2.say();
        p1.say();
        p2 = null;
        p2.say();
    }
}
```
下列选项中描述正确的是（）
- A. 输出1个hello
- B. 输出2个hello后会抛出异常
- C. 输出3个hello后会抛出异常
- D. 不会输出hello，直接抛出异常

```answer

```

5. 下列关于继承的描述中，错误的是（）
   - A. Java中一个类只能有一个直接父类
   - B. 多个类可以继承一个父类
   - C. 一个类可以派生出很多个类
   - D. Java是支持多继承的

```answer

```

6. 在异常处理时，释放资源关闭文件一般在（）语句块内完成。
   - A. try
   - B. catch
   - C. finally
   - D. throw

```answer

```

7. 以下关于String类的常见操作中，哪个是方法会返回指定字符ch在字符串中最后一次出现位置的索引（）
   - A. indexOf(int ch)
   - B. lastIndexOf(int ch)
   - C. indexOf(String str)
   - D. lastIndexOf(String str)

```answer

```

8. String s="Computer"；则s.substring(3,4)返回的字符串是（）
   - A. u
   - B. ut
   - C. p
   - D. pu

```answer

```

9. 使用Iterator时，判断是否存在下一个元素可以使用（）方法。
   - A. hasNext()
   - B. hash()
   - C. hasPrevious()
   - D. next()

```answer

```

10. 下列选项中，FileWriter类中read()方法读取到流末尾的返回值是（）
    - A. 0
    - B. -1
    - C. 1
    - D. 无返回值

```answer

```

## 试卷二选择题

1. 下列哪个关键字用于表示方法不需要返回值？（）
   - A. public
   - B. static
   - C. void
   - D. return

```answer

```

2. 下列选项中，属于Java基本数据类型的是（）
   - A. Integer
   - B. Float
   - C. String
   - D. byte

```answer

```

3. 假设int a=5，表达式++a*2的值是（）
   - A. 10
   - B. 11
   - C. 12
   - D. 14

```answer

```

4. 阅读下列程序，下列选项中描述正确的是（）
```java
class Vehicle {
    void run() {
        System.out.println("Vehicle is running");
    }
}
class Car extends Vehicle {
    void run() {
        System.out.println("Car is running");
    }
}
public class Main {
    public static void main(String[] args) {
        Vehicle v = new Vehicle();
        Car c = new Car();
        v.run();
        c.run();
        v = c;
        v.run();
    }
}
```
- A. 输出三次"Vehicle is running"
- B. 输出三次"Car is running"
- C. 输出"Vehicle is running"，然后输出两次"Car is running"
- D. 输出"Car is running"，然后输出两次"Vehicle is running"

```answer

```

5. 关于Java抽象类，下列描述正确的是（）
   - A. 抽象类可以被实例化
   - B. 抽象类中必须包含抽象方法
   - C. 子类继承抽象类后必须实现抽象方法
   - D. 一个类只能继承一个抽象类

```answer

```

6. Java中用于捕获异常的代码块是（）
   - A. throw
   - B. throws
   - C. catch
   - D. finally

```answer

```

7. 以下哪个String类的方法用于获取字符串的长度？（）
   - A. length()
   - B. size()
   - C. count()
   - D. getSize()

```answer

```

8. String s="HelloWorld"; s.indexOf("World")返回的值是（）
   - A. 5
   - B. 6
   - C. 7
   - D. -1

```answer

```

9. 在Java中，使用哪个接口来实现对象的排序？（）
   - A. Iterable
   - B. Comparable
   - C. Comparator
   - D. Serializable

```answer

```

10. 如果在使用BufferedReader读取文件时遇到文件末尾，其readLine()方法会返回（）
    - A. 空字符串("")
    - B. null
    - C. EOF
    - D. 0

```answer

```

## 试卷三选择题

1. 关于Java类加载器的说法，错误的是（）
   - A. Bootstrap ClassLoader是Java虚拟机的内置类加载器
   - B. Application ClassLoader负责加载应用程序的类
   - C. 类加载器采用双亲委派模型
   - D. Extension ClassLoader可以加载任意路径的类文件

```answer

```

2. 下列关于Java集合框架的说法，正确的是（）
   - A. ArrayList是线程安全的
   - B. Vector是线程安全的
   - C. LinkedList支持随机访问
   - D. HashMap允许key为null但value不能为null

```answer

```

3. 关于Java多线程，以下说法错误的是（）
   - A. 实现Runnable接口可以创建线程
   - B. 一个线程可以多次调用start()方法
   - C. synchronized关键字可以用于方法和代码块
   - D. wait()方法必须在synchronized块中使用

```answer

```

4. 阅读以下程序：
```java
public class ThreadTest {
    public static void main(String[] args) {
        Thread t = new Thread(() -> {
            System.out.println("Running");
        });
        t.start();
        t.start();
    }
}
```
运行结果是（）
- A. 打印两次"Running"
- B. 打印一次"Running"并抛出IllegalThreadStateException
- C. 打印一次"Running"
- D. 直接抛出IllegalThreadStateException

```answer

```

5. 关于Java反射，以下说法正确的是（）
   - A. 反射不能访问private成员
   - B. 反射可以在运行时获取类的所有信息
   - C. 反射只能创建有默认构造器的对象
   - D. 反射不能调用方法

```answer

```

6. 以下哪个注解不是Java内置的（）
   - A. @Override
   - B. @Deprecated
   - C. @Autowired
   - D. @SuppressWarnings

```answer

```

7. 关于Java泛型，下列说法错误的是（）
   - A. 泛型可以用在类和方法上
   - B. 基本数据类型可以直接用作泛型类型
   - C. 泛型有类型擦除机制
   - D. 可以使用通配符?定义泛型类型

```answer

```

8. 以下Lambda表达式的使用，错误的是（）
   - A. () -> System.out.println("Hello")
   - B. (int x) -> x * x
   - C. (x, y) -> return x + y
   - D. (String s) -> s.length()

```answer

```

9. 以下关于Java Stream API的说法，错误的是（）
   - A. stream()方法可以将集合转换为流
   - B. 流操作分为中间操作和终端操作
   - C. 流可以重复使用
   - D. collect()是终端操作

```answer

```

10. Optional类的正确使用方式是（）
    - A. Optional.of(null)
    - B. Optional.ofNullable(null)
    - C. Optional.get()直接获取值
    - D. Optional.ifPresent()判断是否为空

```answer
