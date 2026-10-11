# comsil_5_github

C++ 연결 리스트·스택 실습과 GitHub 브랜치·PR 연습이 함께 들어 있는 저장소다. 2024년 4월 10일과 13일에 커밋했다.

## C++ 실습 (`실습 1` 커밋)

`LinkedList<T>` 템플릿을 만들고, 이를 상속한 `Stack<T>`을 만든다. 메뉴로 값을 넣고 빼고 출력한다.

- `LinkedList.h`: 노드(`Node<T>`)와 `LinkedList<T>`. `Insert`는 맨 앞에 넣고 `Delete`는 맨 뒤 노드를 지우므로 먼저 넣은 값이 먼저 나온다. `Print`는 `[번호|값]->[번호|값]` 꼴로 출력한다
- `Stack.h`: `LinkedList<T>`를 상속하고 `Delete`를 다시 정의해 맨 앞 노드를 지운다. 나중에 넣은 값이 먼저 나온다
- `main.cpp`: 처음에 자료구조를 고른다(1은 Stack, 그 밖은 Linked List). 메뉴는 삽입, 삭제, 출력, 종료다. 값은 정수(`int`)로 받는다
- `Makefile`: `g++`로 `main.cpp`를 빌드해 `a.out`을 만든다

```bash
make
./a.out
make clean
```

## Git 연습

`branch1.txt`, `branch1_1.txt`, `branch2.txt`는 브랜치마다 한 줄씩 적은 파일이다. 2024-04-13에 `branch1`, `branch1_2`, `branch1_1`, `branch2` 브랜치를 만들어 PR 4건(#1, #2, #3, #5)을 `main`에 병합했다. `eemieueFile.txt`는 `실습 2` 커밋에서 추가한 한 줄짜리 파일이다.
