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
```    
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
```  
  
Lecture2: 넘버 2개의 합 구하는 method   
```  
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
```  
    
  
Exam01: 4측연산자 method로 만들기  
```  
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
```  
  

Exam02: 다른방법#2  
```  
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
```  


Exam03: 다른방법#3  
```  
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
```  
  
  
Exam05: 월화수목금토일 method를 통해 print  
```  
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
```  



