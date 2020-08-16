---
title: 자바 메소드(Method) 정리
author: Jihu Choi
layout: post
---
Method를 쓰는 이유: 재사용성  
  
Method 선언: public static void  
  
public: 공동  
static: method 만들기  
void: 비어있는/return type  
  
Method 선언2: public static int  
- return을 할때 쓰는 리턴타입이다.  
  



Lecture1: 안녕하세요 method 만들기  
```java    
public class Lecture1 {  
    public static void printHello() {//printHello라는 method를 만든다.  
        System.out.println("안녕하세요.");  
        System.out.println("안녕하세요.");  
        System.out.println("안녕하세요.");  
    }  
    public static void main(String[] args) {  
  
        for (int i = 0; i < 3; i++) {  
            System.out.println("안녕하세요.");  
  
  
        }  
        printHello();//printHello라는 method를 실행한다.  
    }  
}  
```java  
  
Lecture2: 넘버 2개의 합 구하는 method   
```java  
public class Lecture2 {
    public static int sum(int a, int b) {
        return a+b;
    }
    public static void main(String[] args) {
        int number1, number2;
        number1 = 10;
        number2 = 5;

        int result = number1 + number2;

        System.out.println("합: " + result);

        int result2 = sum(3,4);
        System.out.println("합2 : "+ result2);
    }
}
```java  
    
  
Exam01: 4측연산자 method로 만들기  
```java  
public class Exam01 {  
    public static int sum(int a, int b) {  
        return a + b;  
    }  
  
    public static int sub(int a, int b) {  
        return a - b;  
    }  
  
    public static int mult(int a, int b) {  
        return a * b;  
    }  
  
    public static int div(int a, int b) {  
        return a / b;  
    }  
  
    public static void main(String[] args) {  
        int result2 = sum(5,3);  
        System.out.println("Addition: " + result2);  
  
        int result3 = sub(5,3);  
        System.out.println("Subtraction: " + result3);  
  
        int result4 = mult(5,3);  
        System.out.println("Multiplication: " + result4);  
  
        int result5 = div(5,3);  
        System.out.println("Division: " + result5);  
    }  
}  
```java  
  

Exam02: 다른방법#2  
```java  
public class Exam02 {  
    public static int sum(int a, int b) {  
        return a + b;  
    }  
  
    public static int sub(int a, int b) {  
        return a - b;  
    }  
  
    public static int mult(int a, int b) {  
        return a * b;  
    }  
  
    public static int div(int a, int b) {  
        return a / b;  
    }  
  
    public static void main(String[] args) {  
        System.out.println("Addition: "+ sum(5,3));  
  
        System.out.println("Subtraction: "+ sub(5,3));  
  
        System.out.println("Multiplication: "+ mult(5,3));  
  
        System.out.println("Division: "+ div(5,3));  
    }  
}  
```java  


Exam03: 다른방법#3  
```java  
public class Exam03 {  
    public static void sum(int a, int b) {  
        System.out.println("Addition: " + (a + b));  
    }  
  
    public static void sub(int a, int b) {  
        System.out.println("Subtraction: " + (a - b));  
    }  
  
    public static void mult(int a, int b) {  
        System.out.println("Multiplication: " + (a * b));  
    }  
  
    public static void div(int a, int b) {  
        System.out.println("Division: " + (a / b));  
    }  
  
    public static void main(String[] args) {  
        sum(3,2);  
        sub(3,2);  
        mult(3,2);  
        div(3,2);  
    }  
}  
```java  
  

Exam05: 월화수목금토일 method를 통해 print  
```java  
public class Exam05 {  
    public static void returnWeeks() {  
        String[] weeks = {"월","화", "수", "목", "금", "토", "일"};  
  
        for(int i = 0; i < weeks.length; i++){  
            System.out.println(weeks[i]);  
        }  
    }  
    public static void main(String[] args){  
        returnWeeks();  
    }  
}  
```java  
  
  
Exam06: Line 출력  
```java  
  public class Exam06 {  
    public static void main(String[] arguments){  
        System.out.println("Line 1");  
        threeLines();  
        System.out.println("Line 2");  
    }  
  
    public static void threeLines(){  
        oneLine();  
        oneLine();  
        oneLine();  
    }  
    public static void oneLine(){  
        System.out.println(">");  
    }  
}  
```java  
  

Exam07: 칼로리소모  
```java  
import java.util.Scanner;  
public class Exam07 {  
    public static void cal(double A,int B) {  
        System.out.println(A*B);  
    }  
    public static void main(String[] args) {  
        Scanner input = new Scanner(System.in);  
  
        System.out.println("소모하는 칼로리를 입력하시오. ");  
        double A = input.nextDouble();  
  
        System.out.println("하루동안 걸음을 입력하시오. ");  
        int B = input.nextInt();  
  
        System.out.println(A*B);  
  
    }  
}  
```java  
  

Exam08: 자동차 연비 구하기  
```java  
public class Exam08 {  
    public static void gasoline(double A,double B) {  
        System.out.println(Math.round(B/A) + "km/L");  
    }  
    public static void main(String[] args) {  
        gasoline(8.86,182.736);  
    }  
}  
```java  
  
  
Exam09: 시험성적 확인  
```java  
import java.util.Scanner;  
public class Exam09 {   
    public static void grade(int A) {  
        if(A>95){  
            System.out.println("A+");  
        }  
        if(A>90){  
            System.out.println("A0");  
        }  
        if(A>80){  
            System.out.println("B+");  
        }  
        if(A>70){  
            System.out.println("B0");  
        }  
        else{  
            System.out.println("C+");  
        }  
    }  
    public static void main(String[] args) {  
        Scanner input = new Scanner(System.in);  
  
        System.out.println("성적: ");  
        int A = input.nextInt();  
  
        grade(A);  
    }  
}  
```java  


