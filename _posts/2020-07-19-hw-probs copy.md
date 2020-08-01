---
title: 자바 more 문제풀이(11부터 21)
author: Jihu Choi
layout: post
---
11.public class Prob11 {  
    public static void main(String[] args) {  
        System.out.print("1~100 3의 배수 이면서 7의배수 출력 : ");  
  
        for (int i = 1; i <= 100; i++) {  
            // 3의 배수 && 5의 배수  
            if ((i % 3 == 0) && (i % 7 == 0)) {  
                System.out.print(i + " ");  
            }  
        }  
        System.out.println("");  
    }  
}  
  

12.?
  

13.?  
  

14.public class Prob14 {  
    public static void main(String[] args) {  
        for (int x = 1; x < 10; x++) {  
            for (int i = 2; i < 10; i++) {  
                System.out.print(i + "x" + x + "=" + i * x + ",\t");  
            }  
            System.out.println("");  
        }  
    }  
}  
  
  
15.public class Prob15 {  
    public static void main(String[] args) {  
        System.out.print("1~100 3의 배수 이면서 7의배수 출력 : ");  
  
        for (int i = 1; i <= 100; i++) {  
            // 3의 배수 && 5의 배수  
            if ((i % 3 == 0) && (i % 7 == 0)) {  
                System.out.print(i + " ");  
            }  
        }  
        System.out.println("");  
    }  
}  
  
  
16.public class Prob16 {  
    public static void main(String args[]) {  
        System.out.println("The Odd Numbers are:");  
        for (int i = 1; i <= 100; i++) {  
            if (i % 2 != 0) {  
                System.out.print(i + " ");  
            }  
        }  
    }  
}  
  
  
17.public class Prob17 {  
    public static void main(String args[]) {  
        int n = 100;  
        System.out.print("Even Numbers from 1 to "+n+" are: ");  
        for (int i = 1; i <= n; i++) {  
            //if number%2 == 0 짝수 구하기  
            if (i % 2 == 0) {  
                System.out.print(i + " ");  
            }  
        }  
    }  
}  
    
  
18.public class Prob18 {  
    public static void main(String[] args){  
        int hap=0;  
        for(int i=0; i<=100; i++){  
            if(i%2==0){  
                hap += i;  
            }  
        }  
        System.out.println("1부터 100까지 짝수의 합은 :" +hap);  
    }  
}  
  

19.public class Prob19 {  
    public static void main(String[] args) {  
        int even = 0;  
        int odd = 0;  
        int i = 0;  
        int sum = 0;  
  
        while (i <= 100) {  
            if (i % 2 == 0) {  
                even = even + i;  
            } else {  
                odd = odd + i;  
            }  
            i++;  
        }  
        System.out.println("1부터 100까지의 수 중 홀수의 합: " + odd);  
  
    }  
}  
  
  
20.public class Prob20 {  
    public static void main(String[] args) {  
  
        int i = 0;  
        int even = 0;  
        int odd = 0;  
  
        while (i <= 100) {  
            if (i % 2 == 0) {  
                even = even + i;  
            } else {  
                odd = odd + i;  
            }  
            i++;  
        }  
int sum = even + odd;  
        System.out.println("1부터 100까지의 수 중 짝수의 합과 홀수의 합: " + sum);  
  
    }  
}  
   
  
21.??