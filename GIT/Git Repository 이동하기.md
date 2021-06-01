# Move Git Repository with Commit Log



:ballot_box_with_check: 깃헙에 newRepository 미리 생성해두기 



### 1. 기존의 레파지토리 복사하기

```git clone --mirror http://github.com/JiyeongYun/oldRepository.git```



### 2. 기존의 레파지토리로 이동

```cd oldRepository.git```



### 3. 새 레파지토리 URL 설정

``` git remote set-url --push origin http://github.com/JiyeongYun/newRepository.git ```



### 4. 새 레파지토리에 push 하기

``` git push --mirror ```



### 5. 정상적으로 복사되었는지 확인하기

```git remote -v```

