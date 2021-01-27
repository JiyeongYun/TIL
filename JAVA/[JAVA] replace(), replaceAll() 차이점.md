


1. replace()
    - 바꾸고자 하는 문자열과 완전히 일치하는 곳을 '**모두**' 변경한다.

    ```java
    String str = "aabbccabcabcdd";
    str.replace("abc", "@");

    //출력: aabbcc@@dd
    ```

2. replaceAll()
    - replaceAll()은 정규식 사용이 가능
        - 참고링크: [https://velog.io/@kimtaeeeny/정규표현식-모음](https://velog.io/@kimtaeeeny/%EC%A0%95%EA%B7%9C%ED%91%9C%ED%98%84%EC%8B%9D-%EB%AA%A8%EC%9D%8C)
    - a,b,c문구가 들어간 모든 곳을 '@'로 변경한다.

    ```java
    String str = "aabbccabcabcdd";
    str.replaceAll("[abc]", "@");

    //출력: @@@@@@@@@@@@dd
    ```
