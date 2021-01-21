### Scanner 클래스의 next(), nextLine() 차이

> **nextLine()**
- Enter를 치기 전까지 쓴 문자열을 모!두! 리턴
- 공백이 존재하는 한 문장을 리턴받고 싶은 경우

> **next()**
- 공백 전까지 입력받은 문자열 리턴
- 한 줄에 입력받되 단어별로 리턴받고 싶은 경우


> **예제**
```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        System.out.println("문자열입력: ");
        String str1 = scanner.nextLine();
        System.out.println(str1);
        
        System.out.println("문자열입력: ");
        String str2 = scanner.next();
        System.out.println(str2);
    }
}
```
- "안녕하세요, 반갑습니다." 라고 입력했을 때 str1(nextLine()사용)은 "안녕하세요, 반갑습니다." 라고 출력한다.
- "안녕하세요, 반갑습니다." 라고 입력했을 때 str2(next()사용)은 "안녕하세요," 라고 출력한다.


> **(*중요) 주의할 점**
```java
import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        System.out.println("첫번째 정수입력: ");
        int num = scanner.nextInt();
        System.out.println(num);
        
        System.out.println("첫번째 문자열입력: ");
        String str1 = scanner.nextLine();
        System.out.println(str1);

```
- "10" > Enter > "안녕하세요" > Enter 를 입력하면 출력은 "10"만 된다.
그 이유는 nextInt()에서는 10만 리턴하고 이후 사용자가 입력한 Enter는 그 다음으로 넘어가 nextLine()이 인식하게 된다.
따라서, nextLine()을 제대로 작동하게 하기 위해서는 2가지 방법이 있다.
  1. nextLine()을 2번 작성하여 Enter 값을 소멸시키기
  2. next() 사용하기
