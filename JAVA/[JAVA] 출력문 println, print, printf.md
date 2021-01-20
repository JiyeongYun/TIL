

> **println**
- ln은 line을 의미
- 괄호안 내용을 출력한 후 마지막에 개행문자가 포함되어 있어 출력후 한 줄 띄워짐.

```java
System.out.println(a + "," + b);
```


> **print**
- 괄호안 내용을 단순히 출력. 개행문자(=줄바꿈문자=\n) 포함안됨.
- 여러 번 실행시키면 한 줄에 모두 출력된다.

```java
System.out.print(a);
System.out.print(b);
```

> **printf**
- 포맷에 맞춰 출력
- C에서의 printf와 동일. %d, %s 등을 쓰기위해 사용. 개행문자 포함X

```java
System.out.printf("a의 값: %d, b의 값: %d", a, b);
System.out.printf("[%d]\n", 123);    //10진수 출력
System.out.printf("[%4d]\n", 123);   //10진수 출력, 우측정렬, 빈칸
System.out.printf("[%04d]\n", 123);  //10진수 출력, 우측정렬, 0으로 채움
System.out.printf("[%-4d]\n", 123);  //10진수 출력, 좌측정렬, 빈칸
 //System.out.printf("[%-04d]\n", 123); => 0으로 채워져서 1230으로 되면 전혀 다른 숫자가 되기 때문에 -04d는 불가능하다.

System.out.printf("[%f]\n", 12.3456);    //실수 출력
System.out.printf("[%.3f]\n", 12.3456);  //실수 출력, 반올림해서 소수점 이하 3자리
System.out.printf("[%7.3f]\n", 12.3456); //실수 출력, 반올림해서 소수점 이하 3자리, 전체자리, 우측정렬, 빈칸
System.out.printf("[%07.3f]\n", 12.3456); //실수 출력, 반올림해서 소수점 이하 3자리, 전체자리, 우측정렬, 0으로 채움
System.out.printf("[%-7.3f]\n", 12.3456); //실수 출력, 반올림해서 소수점 이하 3자리, 전체자리, 좌측정렬, 빈칸

System.out.printf("[%s]\n", "hi");   //문자열(정수, 실수) 출력
System.out.printf("[%3s]\n", "hi");  //문자열 출력, 우측정렬, 빈칸
System.out.printf("[%-3s]\n", "hi"); //문자열 출력, 좌측정렬, 빈칸

//char는 보통 string으로 취급하여 사용하기 때문에 생략
System.out.printf("[%c]\n", "c");   //문자열(정수, 실수) 출력
```
