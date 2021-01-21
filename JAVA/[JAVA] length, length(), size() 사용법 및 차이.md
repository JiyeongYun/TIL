> **1.length**
 - arrays(int[], double[], String[])
 - length는 배열의 길이를 알고자 할때 사용된다.
 
```java
int[] arr = new int[5];
System.out.println( arr.length );  // 5
```


> **2. length()**
 - String related Object(String, StringBuilder etc)
 - length()는 문자열의 길이를 알고자 할때 사용된다.

```java
String str = "Hello, World!";
System.out.println( str.length() );  // 13
 ```

> **3. size()**
 - Collection Object(ArrayList, Set etc)
 - size()는 컬렉션프레임워크 타입의 길이를 알고자 할때 사용된다.
 
```java
ArrayList<Object> arrList = new ArrayList<Object>();
System.out.println( arrList.size() );  // 0

```
