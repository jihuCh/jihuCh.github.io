---
title: 자리수 구하기(자바 문제풀이)
author: Jihu Choi
layout: post
---
1. x = 원래 수  
2. 추출한 값을 sum에 더한다  
3. x/10으로 자리수를 줄인다  

```
import java.util.Scanner; //자바 스캐너를 불러온다
public class exam1 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt(); //유저가 입력한 값을 n에 저장한다.

        System.out.println(f(n));
    }
    private static int f(int n){
        int sum =0;
        while(n!=0){
            sum +=(n%10);//sum에 나머지(n%10)를 더한다.
            n = n/10;//10으로 나눠서 또 자리수를 줄인다.
        }

        return sum; //최종값 알려주기

        }
    }
```