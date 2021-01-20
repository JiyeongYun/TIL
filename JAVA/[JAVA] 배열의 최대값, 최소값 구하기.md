### 배열의 최대값, 최소값 구하기 (2가지 방법)

```java
int[] c = {3, 5, 1, 9, 2, 7, 6, 4, 8, 0};
```

> **초기화 방법 - 1**
- max, min 값을 배열의 첫 번째 값으로 초기화한다.
- max값과 현재 배열 참조 값을 비교하여 값을 구한다. 
```java
int max = c[0];
int min = c[0];
```


> **초기화 방법 - 2**
- int 가능 범위의 최소, 최대값을 활용하여 초기화한다.
- 주의: max의 초기값은 MINVALUE, min의 초기값은 MAXVALUE
```java
int max = Integer.MIN_VALUE;
int min = Integer.MAX_VALUE;
```

> **초기화 한 후 min, max를 구하는 과정 - 1**
```java
// max
for(int i = 0; i < c.length; i++){
	if(max < c[i]) max = c[i];	//max
	if(c[i] < min) min = c[i];	//min
}
```


> **초기화 한 후 min, max를 구하는 과정 - 2**
```java
for(int i = 0; i < c.length; i++){
	max = Math.max(max, array[i])	//max
	min = Math.min(min, array[i])	//min
}
```

