# Java程序阅读题集

## 试卷一程序阅读题（每题5分，共30分）

1. 阅读下列程序，写出输出结果：
```java
class Test {
    public static void main(String[] args) {
        int a = 21;
        int b = 5;
        System.out.print(a >= b);
    }
}
```

```answer

```

2. 阅读下列程序，写出输出结果：
```java
public class Test {
    public static void main(String[] args) {
        int[] intArray = {1,2,3,4,5,6};
        int s = 0;
        for(int i = 0; i < intArray.length; i++)
            s += intArray[i];
        System.out.println(s);
    }
}
```

```answer

```

3. 阅读下列程序，写出输出结果：
```java
public class Test {
    public static void main(String[] args) {
        String str1 = "Hello";
        String str2 = "Hel" + "lo";
        System.out.println(str1 == str2);
        System.out.println(str1.equals(str2));
    }
}
```

```answer

```

4. 阅读下列程序，如果从键盘上输入16 4，请写出程序的输出结果：
```java
import java.util.Scanner;
public class ExceptionTest {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int a = scanner.nextInt();
        int b = scanner.nextInt();
        try {
            System.out.print(a/b);
        } catch(ArithmeticException e) {
            System.out.print(5);
        } finally {
            System.out.println(0);
        }
    }
}
```

```answer

```

5. 阅读下列程序，写出输出结果：
```java
class Father {
    Father() {
        System.out.println("Father");
    }
}

class Son extends Father {
    Son() {
        System.out.println("Son");
    }
    public static void main(String[] args) {
        new Son();
    }
}
```

```answer

```

6. 阅读下列程序，写出输出结果：
```java
class Father {
    public void fun() {
        System.out.println("Father");
    }
}

class Son extends Father {
    public void fun() {
        System.out.println("Son");
    }
}

public class Test {
    public static void main(String[] args) {
        Father f = new Son();
        f.fun();
    }
}
```

```answer

```

## 试卷二程序阅读题（每题5分，共30分）

1. 阅读以下程序，写出输出结果：
```java
public class Test1 {
    public static void main(String[] args) {
        int a = 10;
        a += 5;
        System.out.println(a);
    }
}
```

```answer

```

2. 阅读以下程序，写出输出结果：
```java
public class Test2 {
    public static void main(String[] args) {
        int[] arr = {2, 4, 6, 8, 10};
        int result = 1;
        for (int num : arr) {
            result *= num;
        }
        System.out.println(result);
    }
}
```

```answer

```

3. 阅读以下程序，写出输出结果：
```java
class Test3 {
    public static void main(String[] args) {
        String str1 = "java";
        String str2 = "java";
        System.out.println(str1.equals(str2));
        System.out.println(str1.equalsIgnoreCase(str2));
    }
}
```

```answer

```

4. 阅读以下程序，如果从键盘输入字符串"abc"，则程序的输出结果是什么：
```java
import java.util.*;
public class ExceptionTest {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        try {
            int num = scanner.nextInt();
            System.out.println("输入的是:" + num);
        } catch (InputMismatchException e) {
            System.out.println("输入的不是整数!");
        }
    }
}
```

```answer

```

5. 阅读以下程序，写出输出结果：
```java
class A {
    A() {
        System.out.print("A");
    }
}
class B extends A {
    B() {
        System.out.print("B");
    }
    public static void main(String[] args) {
        new B();
    }
}
```

```answer

```

6. 阅读以下程序，写出输出结果：
```java
class Parent {
    public void show() {
        System.out.println("Parent");
    }
}
class Child extends Parent {
    @Override
    public void show() {
        System.out.println("Child");
    }
}
public class Test {
    public static void main(String[] args) {
        Parent p = new Child();
        p.show();
    }
}
```

```answer

```

## 试卷三程序阅读题（每题5分，共30分）

1. 阅读以下程序，写出输出结果：
```java
import java.util.Arrays;
import java.util.List;
import java.util.stream.Collectors;

public class StreamTest {
    public static void main(String[] args) {
        List<Integer> numbers = Arrays.asList(1, 2, 3, 4, 5);
        List<Integer> doubled = numbers.stream()
                                     .map(n -> n * 2)
                                     .collect(Collectors.toList());
        System.out.println(doubled);
    }
}
```

```answer

```

2. 阅读以下程序，写出输出结果：
```java
import java.util.Optional;

public class OptionalTest {
    public static void main(String[] args) {
        String str = null;
        String result = Optional.ofNullable(str)
                              .orElse("Default");
        System.out.println(result);

        str = "Hello";
        result = Optional.ofNullable(str)
                        .orElse("Default");
        System.out.println(result);
    }
}
```

```answer

```

3. 阅读以下程序，写出输出结果：
```java
import java.util.concurrent.CompletableFuture;

public class AsyncTest {
    public static void main(String[] args) {
        CompletableFuture<String> future = CompletableFuture
            .supplyAsync(() -> "Hello")
            .thenApply(s -> s + " World");

        System.out.println(future.join());
    }
}
```

```answer

```

4. 阅读以下程序，写出输出结果：
```java
import java.util.HashMap;
import java.util.Map;

public class MapTest {
    public static void main(String[] args) {
        Map<String, Integer> map = new HashMap<>();
        map.put("A", 1);
        map.put("B", 2);

        map.compute("A", (k, v) -> v == null ? 1 : v + 1);
        map.computeIfAbsent("C", k -> 3);

        System.out.println(map);
    }
}
```

```answer

```

5. 阅读以下程序，写出输出结果：
```java
interface Greeting {
    String greet(String name);
}

public class LambdaTest {
    public static void main(String[] args) {
        Greeting greeting = (name) -> "Hello, " + name;
        System.out.println(greeting.greet("Java"));

        Greeting formal = (String name) -> {
            return "Good morning, " + name;
        };
        System.out.println(formal.greet("World"));
    }
}
```

```answer

```

6. 阅读以下程序，写出输出结果：
```java
import java.time.LocalDateTime;
import java.time.format.DateTimeFormatter;

public class DateTimeTest {
    public static void main(String[] args) {
        LocalDateTime now = LocalDateTime.of(2025, 2, 16, 17, 9);
        DateTimeFormatter formatter = DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm");
        System.out.println(now.format(formatter));

        LocalDateTime later = now.plusHours(2);
        System.out.println(later.format(formatter));
    }
}
```

```answer
