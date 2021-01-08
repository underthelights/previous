---
layout: article
title: cheatingSHIT
key: 0
tags: alg
category: alg
date: 2021-01-08 23:38:00 +08:00
picture_frame: shadow
---
alg cheastsheet
**BE HUMBLE.**
<!--more-->

c문자, 문자열 input %[^\n]%*c

scanf warning #pragma warning(disable : 4996) 



자료형의 범위

int : –2,147,483,648 ~ 2,147,483,647 20억 / 10개

unsigned int = long :  0 ~ 4,294,967,295 40억 / 10개

long long :	–9,223,372,036,854,775,808 ~ 9,223,372,036,854,775,807 92억 / 10개

unsigned long long : 0 ~ 18,446,744,073,709,551,615



입출력

C++을 사용하고 있고 cin/cout을 사용하고자 한다면, cin.tie(NULL)과 sync_with_stdio(false)를 둘 다 적용해 주고, endl 대신 개행문자(\n)를 쓰자. 단, 이렇게 하면 더 이상 scanf/printf/puts/getchar/putchar 등 C의 입출력 방식을 사용하면 안 된다.

Java를 사용하고 있다면, Scanner와 System.out.println 대신 BufferedReader와 BufferedWriter를 사용할 수 있다. BufferedWriter.flush는 맨 마지막에 한 번만 하면 된다.



자바 2차원 배열 초기화예약

1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
19
import java.util.Arrays
 
int[][] cache = new int[11][11];
 
int cases = scn.nextInt();
 
while(cases-- > 0) {
  for (int[] row : cache) 
    Arrays.fill(row, -1);         
}
 
//한줄로 출력
System.out.println(Arrays.deepToString(cache));
            
//2줄로 출력
for (int[] arr : cache) {
  System.out.println(Arrays.toString(arr));
}
            




int형 데이터를 담으면서, 길이 n인 vector를 선언하면서

vector<int> v([벡터 길이], [초기화 값])



typedef는 #쓰지않는다.

typedef unsigned long long uint64



2차원 데이터를 써야할 땐 배열로 강제로 초기화



표준 입출력함수들과의 동기화를 끄기

cin.sync_with_stdio(false);



시스템에 저장되어있는 최대/최소값

numeric_limits(int)::max();     //  int 형 변수이 최대 표현가능 숫자를 리턴

numeric_limits(int)::min();      //  int 형 변수이 최소 표현가능 숫자를 리턴

//레퍼런스

#include <iostream>

using std::cin;

using std::cout;

using std::endl;

#include <limits>

using std::numeric_limits;





순열 구해주는 함수

stl의 next_permutation();을 사용할것



STL 메모리 비우기

vector<int>().swap(vtr);


