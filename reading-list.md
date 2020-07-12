---
title: JAVA problems(문제풀이)
subtitle: Examples of JAVA basic problems and how to solve them.
layout: "page"
icon: fa-book
order: 3
---

1. How to add each digits of a number
```

import java.util.Scanner; //자바 스캐너를 불러온다

public class exam1 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt(); //유저가 입력한 값을 n에 저장한다.

        System.out.println(f(n));
    }

    private static int f(int n) {
        int sum = 0;
        while (n != 0) {
            sum += (n % 10);//sum에 나머지(n%10)를 더한다.
            n = n / 10;//10으로 나눠서 또 자리수를 줄인다.
        }

        return sum; //최종값 알려주기

    }
}
```
2. How to add all the numbers between 'a' and 'b'
```
import java.util.Scanner;
public class exam2 {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.println("A값을 입력하시오. ");
        int a = input.nextInt();
        System.out.println("B값을 입력하시오. ");
        int b = input.nextInt();


        for (int i = a; i < b; i++) {
            int add = b - 1;
            System.out.println(a + b + add);


        }
    }
}
```
3. How to write the multiplication table

```
public class exam3 {
    public static void main(String[] args) {
        for (int i = 2; i < 10; i++) {
            for (int x = 1; x < 10; x++) {
                System.out.println(i + "x" + x + "=" + i * x);
            }
        }
    }
}
```

4. How to write multiplication table #2
- Writing multiplication table in this format:
2 x 1 = 2, 2 x 2 = 4 ... 2 x 9 = 18  
3 x 1 = 3 ... 3 x 9 = 27  
...   
...  
9 x 1 = 9 ... 9 x 9 = 81  

```
public class exam4 {
    public static void main(String[] args) {

        for (int i =1; i<9;  i++) {
            for (int x = 1; x < 10; x++) {
                System.out.print(i + 1 + "x" + x + "=" + (i + 1) * x + ", ");
            }
            System.out.println("");
        }
    }
}
```

5. How to write multiplication table #3
- Writing multiplication table in this format:
2 x 1 = 2, 3 x 1 = 3, ... 9 x 1 = 9  
2 x 2 = 4, 3 x 2 = 6, ... 9 x 2 = 18  
...  
...  
2 x 9 = 18, 3 x 9 = 27, ... 9 x 9 = 81

```
public class exam5 {
    public static void main(String[] args) {
        for (int x = 1; x < 10; x++) {
            for (int i = 2; i < 10; i++) {
                System.out.print(i + "x" + x + "=" + i * x + ",\t");
            }
            System.out.println("");
        }
    }
}
```