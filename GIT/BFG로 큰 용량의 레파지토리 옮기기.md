## BFG Repo-Cleaner 사용하기

1. A를 clone을 bare로 받는다.<br/>

    ```$ git clone --mirror [A.git]```


2. A.git 폴더와 **같은 경로**에 [BFG RepoCleaner](https://rtyley.github.io/bfg-repo-cleaner/) 을 다운받는다.


3. A.git폴더에서 100mb넘는 것을 제거(저장소 정리)<br/>

    ```$ java -jar bfg-1.14.0.jar --strip-blobs-bigger-than 100M [A.git]```

    - 버전이 다를 수도 있으니 유의하기
    - 그런데 위의 방법은 커밋, 브랜지, 태그를 업데이트하지만 물리적으로 삭제되지 않음.

4. 해당 폴더로 들어가기<br/>

    ```$ cd A.git```

5. github에 올릴 레파지토리 만들기

6. github에 올리기<br/>

    ```$ git push --mirror [B.git]```
