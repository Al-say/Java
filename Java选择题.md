# Java选择题集

## 试卷一选择题

1. 下面4种类型的文件中（）可以在Java虚拟机中运行。
   - A. .java	是 Java 源文件，得先编译，不能直接在 JVM 运行。
   - B. .jre  是 Java 运行环境，不是文件类型。
   - C. .exe 是 Windows 可执行文件，JVM 不能运行。
   - D. .class 是编译后的字节码文件，JVM 能直接加载运行。

```answer
D
```

2. 下列选项中，不属于基本数据类型的是（）
   - A. String 是类，属于引用数据类型，不是基本数据类型。
   - B. short 是基本整数类型。
   - C. boolean 是基本逻辑类型。
   - D. char 是基本字符类型。

```answer
A
```

3. 假设int x=2，三元表达式x>0?x+1:5（）
   - A. 0
   - B. 2
   - C. 3
   - D. 5

```answer
C
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
B
```

5. 下列关于继承的描述中，错误的是（）
   - A. Java中一个类只能有一个直接父类：Java 是单继承，一个类只能有一个直接父类，描述正确。
   - B. 多个类可以继承一个父类：多个不同子类可继承同一个父类，能实现代码复用，描述正确。
   - C. 一个类可以派生出很多个类：一个父类能派生出多个子类，可构建类层次结构，描述正确。
   - D. Java是支持多继承的：Java 不支持类的多继承，只是能用接口实现类似效果，描述错误。

```answer
D
```

6. 在异常处理时，释放资源关闭文件一般在（）语句块内完成。
   - A. try：放可能出错代码，不是用来释放资源的。
   - B. catch：捕获并处理异常，主要是处理逻辑，非专门释放资源。
   - C. finally：不管有无异常都会执行，常用来释放资源、关闭文件等。
   - D. throw：主动抛出异常，和释放资源没关系。

```answer
C
```

7. 以下关于String类的常见操作中，哪个是方法会返回指定字符ch在字符串中最后一次出现位置的索引（）
   - A. `indexOf(int ch)`：返回指定字符首次出现的索引。
   - B. `lastIndexOf(int ch)`：返回指定字符最后一次出现的索引，符合题意。
   - C. `indexOf(String str)`：返回指定子串首次出现的索引。
   - D. `lastIndexOf(String str)`：返回指定子串最后一次出现的索引。

```answer
B
```

8. String s="Computer"；则s.substring(3,4)返回的字符串是（）
   - A. u
   - B. ut
   - C. p
   - D. pu

```answer
C
```

9. 使用Iterator时，判断是否存在下一个元素可以使用（）方法。
   - A. `hasNext()`：`Iterator` 接口方法，用于判断是否有下一个元素。
   - B. `hash()`：`Iterator` 无此方法，和判断无关。
   - C. `hasPrevious()`：是 `ListIterator` 方法，用于判断是否有前一个元素。
   - D. `next()`：用于获取下一个元素，不用于判断。

```answer
A
```

10. 下列选项中，FileWriter类中read()方法读取到流末尾的返回值是（）
    - A. 0
    - B. -1
    - C. 1
    - D. 无返回值

```answer
B
```

## 试卷二选择题

1. 下列哪个关键字用于表示方法不需要返回值？（）
   - A. `public` 是访问修饰符，控制访问权限，与返回值无关。
   - B. `static` 表示成员属类本身，不决定方法是否有返回值。
   - C. `void` 作方法返回类型，表明方法无需返回值。
   - D. `return` 用于返回值或提前终止方法，非表示无返回值。

```answer
C
```

2. 下列选项中，属于Java基本数据类型的是（）
   - A. Integer 是 int 的包装类，属引用类型，非基本类型。
   - B. Float 是 float 的包装类，是引用类型，不是基本类型。
   - C. String 是类，属于引用类型，并非基本类型。
   - D. byte 是有符号 8 位整数，是 Java 基本数据类型。

```answer
D
```

3. 假设int a=5，表达式++a*2的值是（）
   - A. 10
   - B. 11
   - C. 12
   - D. 14

```answer
C
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
C
```

5. 关于Java抽象类，下列描述正确的是（）
   - A. 抽象类可以被实例化 :抽象类不能实例化，因为可能含无实现的抽象方法。
   - B. 抽象类中必须包含抽象方法,抽象类不一定含抽象方法，有`abstract`修饰就行
   - C. 子类继承抽象类后必须实现抽象方法. 普通子类继承抽象类要实现抽象方法，抽象子类可不实现。
   - D. 一个类只能继承一个抽象类. Java 类是单继承，一个类只能继承一个抽象类。

```answer
D
```

6. Java中用于捕获异常的代码块是（）
   - A. `throw`：在方法内手动抛出异常对象，非捕获异常。
   - B. `throws`：在方法声明处指明可能抛的异常，不捕获。
   - C. `catch`：捕获并处理`try`块抛出的异常，用于捕获。
   - D. `finally`：无论有无异常都会执行，非用于捕获。

```answer
C
```

7. 以下哪个String类的方法用于获取字符串的长度？（）
   - A. `length()`：`String`类方法，用于获取字符串长度。
   - B. `size()`：常见于集合类，用于返回集合元素数量，`String`类无此方法。
   - C. `count()`：`String`类没有该方法，`Stream` API 用其统计元素数。
   - D. `getSize()`：`String`类不存在此方法。

```answer
A
```

8. String s="HelloWorld"; s.indexOf("World")返回的值是（）
   - A. 5
   - B. 6
   - C. 7
   - D. -1

```answer
A
```

9. 在Java中，使用哪个接口来实现对象的排序？（）
   - A. `Iterable`：主要用于支持`for - each`循环遍历集合元素，和对象排序无关。
   - B. `Comparable`：类实现该接口并重写`compareTo`方法，可定义对象自然排序规则，用于对象排序。
   - C. `Comparator`：能定义定制排序规则，当类无`Comparable`或原规则不适用时使用，可实现对象排序。
   - D. `Serializable`：是标记接口，用于指示对象可序列化，与排序功能无关。

```answer
B、C
```

10. 如果在使用BufferedReader读取文件时遇到文件末尾，其readLine()方法会返回（）
    - A. 空字符串("")
    - B. null
    - C. EOF
    - D. 0

```answer
B
```

## 试卷三选择题

1. 关于Java类加载器的说法，错误的是（）
   - A. Bootstrap ClassLoader是Java虚拟机的内置类加载器-加载核心类库，说法正确。
   - B. Application ClassLoader负责加载应用程序的类-即用户类路径下的类，说法正确。
   - C. 类加载器采用双亲委派模型-保证核心类库安全和唯一，说法正确。
   - D. Extension ClassLoader可以加载任意路径的类文件-只加载 Java 扩展目录（如 jre/lib/ext）下的类，非任意路径，说法错误。

```answer
D
```

2. 下列关于Java集合框架的说法，正确的是（）
   - A. ArrayList是线程安全的-非线程安全，多线程操作可能致数据问题。
   - B. Vector是线程安全的-方法用 `synchronized` 同步，是线程安全的。
   - C. LinkedList支持随机访问- 基于链表，随机访问需遍历，不支持高效随机访问。
   - D. HashMap允许key为null但value不能为null- 允许 `key` 和 `value` 都为 `null`。

```answer
B
```

3. 关于Java多线程，以下说法错误的是（）
   - A. 实现Runnable接口可以创建线程
   - B. 一个线程可以多次调用start()方法：一个线程对象的 `start()` 方法只能调用一次。
   - C. synchronized关键字可以用于方法和代码块
   - D. wait()方法必须在synchronized块中使用

```answer
B
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
- B. 打印一次"Running"并抛出IllegalThreadStateException-`Thread` 对象的 `start()` 方法只能被调用一次。
- C. 打印一次"Running"
- D. 直接抛出IllegalThreadStateException

```answer
B
```

5. 关于Java反射，以下说法正确的是（）
   - A. 反射不能访问private成员-反射借助`setAccessible(true)`能打破权限限制，可访问和操作`private`成员，该说法错误。
   - B. 反射可以在运行时获取类的所有信息-反射在运行时能利用`Class`类的方法获取类的名称、成员、构造方法等各类信息，说法正确。
   - C. 反射只能创建有默认构造器的对象-反射通过`Constructor`类可获取指定参数的构造方法，进而创建有参构造的对象，并非只能创建有默认构造器的对象，该说法错误。
   - D. 反射不能调用方法- 反射可通过`Class`类获取`Method`对象，用`invoke()`方法调用对应方法，该说法错误。

```answer
B
```

6. 以下哪个注解不是Java内置的（）
   - A. `@Override`：Java 内置注解，标记方法重写父类方法，辅助编译器检查。
   - B. `@Deprecated`：Java 内置注解，标记类、方法等已过时，使用时编译器会警告。
   - C. `@Autowired`：由 Spring 框架提供，用于依赖注入，并非 Java 内置。
   - D. `@SuppressWarnings`：Java 内置注解，可抑制编译器发出的警告。

```answer
C
```

7. 关于Java泛型，下列说法错误的是（）
   - A. 泛型可以用在类和方法上
   - B. 基本数据类型可以直接用作泛型类型-泛型类型参数须为引用类型，基本数据类型（如`int`）不能直接用，要用包装类（如`Integer`），说法错误。
   - C. 泛型有类型擦除机制
   - D. 可以使用通配符?定义泛型类型

```answer
B
```

8. - A. `() -> System.out.println("Hello")`：无参，执行打印语句，符合 Lambda 语法，可赋值给`Runnable`等接口实例，使用正确。
   - B. `(int x) -> x * x`：接收一个`int`参数，返回其平方，语法无误，能赋值给对应函数式接口，使用正确。
   - C. `(x, y) -> return x + y`：Lambda 单行语句无需`return`，若多行需用`{}`括起并加`return`，此写法错误。
   - D. `(String s) -> s.length()`：接收`String`参数，返回其长度，符合语法，可赋值给相应函数式接口，使用正确。

```answer
C
```

9. 以下关于Java Stream API的说法，错误的是（）
   - A. 集合（如`List`）有`stream()`方法，可将集合转换为流，使用方便，说法正确。
   - B. 流操作分为中间操作（如`filter`、`map`）和终端操作（如`forEach`、`collect`），中间操作可链式调用，说法正确。
   - C. 流是一次性对象，执行终端操作后即被消费，再次使用会抛`IllegalStateException`，不能重复用，说法错误。
   - D. `collect()`是终端操作，能把流元素收集到集合等数据结构，说法正确。

```answer
C
```

10. Optional类的正确使用方式是（）
    - A. `Optional.of(null)`：`Optional.of()` 要求传入非空值，传入 `null` 会抛 `NullPointerException`，使用错误。
    - B. `Optional.ofNullable(null)`：`Optional.ofNullable()` 可处理可能为 `null` 的值，值为 `null` 创建空实例，不为 `null` 则包含该值，使用正确。
    - C. `Optional.get()` 直接获取值：`get()` 要在 `Optional` 有值时才能用，空值调用会抛 `NoSuchElementException`，不能直接用，使用错误。
    - D. `Optional.ifPresent()` 判断是否为空：`ifPresent()` 用于值存在时执行操作，判断是否为空用 `isPresent()`，使用错误。

```answer
B
