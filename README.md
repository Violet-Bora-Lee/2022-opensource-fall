# 2022-opensource-fall
서강대학교 게임&amp;평생 교육원 오픈소스 이해, 가을학기 강의

## 리눅스 커맨드라인 기초
> 모르면 실습이 불가능한 기초 커맨드라인 3가지
1. pwd: print working directory
2. ls: list
3. cd: change directory

## vim 에디터

### 입력모드와 명령모드

```bash
vim abc.txt // abc.txt 파일을 vim 에디터로 열기
```
- 파일을 처음에 열면 명령모드로 진입한다
- 입력 하려면, 입력모드로 진입해야함
  - 키보드에서 i누르기
- 명령모드 진입은 키보드 esc키 누르기
  - 저장하기(write) --> :w
  - 나오기(quit) --> :q
  - 저장하고 나오기 --> :wq
  
### 스왑파일 생성시 해결 방법
#### 스왑파일이 생기는 경우
1. 두 응용프로그램에서 하나의 파일을 동시에 수정
2. 크래시 때문에 파일이 비 정상적으로 닫힌 경우
#### 해결방법
리커버리모드로 수정중인 파일을 복구하고, 스왑파일을 삭제한다.
```bash
vim -r abc.txt
```
  
TEMP
- HTML과 CSS 이해

## git

>  대표적으로 쓰이는 버전 관리 시스템(Version Control Sysem, VCS)

### git과 GitHub의 차이점
- git은 버전 관리 시스템이다
- GitHub는 git이라는 기술을 기반으로 만든 플랫폼
  - GitHub에서 만들었는데, GitHub를 마이크로소프트가 인수함

### 다양한 버전 관리 시스템
- 이름 변경
  - 최종.hwp, 최종1.hwp, 최종2.hwp
- 자동저장 기능
- git 이전의 버전 관리 시스템
  - SVN, CVS, Mercurial
- 요즘엔 git이 거의 표준이 됨

# 2022-09-29
## 커밋
- 커밋은 논리적 변경이 있을 때 하나만듬

# 2022-10-06

## 스테이징 영역
- 커밋에 포함시킬 변경분만 올리는 영역
  - stage의 뜻: 무대
- 스테이징 영역을 잘 활용해야 커밋을 잘 만들 수 있음

# 2022-10-13

## 중간고사 내용 정리

1. 기본적으로 알아야 할 커맨드라인 명령어
  - pwd, cd, ls: 약자
2. vim사용법
  - 명령모드와 입력모드의 차이, 어떻게 각 모드로 전환할 수 있는지
  - 명령모드에서 저장하고 빠져나오는 방법
3. 버전관리를 사용하는 이유
  - 3가지 적기
4. 깃과 깃허브의 차이
5. 저장소와 일반 디렉터리의 차이
  - 저장소 만들때 쓰는 명령어(git init)
6. 커밋 로그를 보고싶을때 치는 명령어
7. 커밋은 언제 만드는가
8. HEAD의 정의: 현재 체크아웃한 브랜치의 가장 최신 커밋을 가리키는 포인터
9. 현재 상태를 확인하는 명령어(git status)
10. 스테이징 영역이 왜 존재하는가?
11. 원하는 파일을 스테이징 영역에 올릴때 쓰는 명령어
12. 커밋 메시지가 "abc"인 커밋을 만들고 싶을 때 어떻게 하나?
  - git commit -m "abc"
  - git commit 하고 엔터친 후, abc 입력
13. .gitignore파일의 역할
14. 브랜치는 언제 만드는가?
15. 브랜치 관련 명령어
  - 현재 생성된 브랜치 목록 확인하기: git branch
  - abc라는 이름을 가진 브랜치 만들기: git branch abc
  - abc 브랜치로 이동해서 작업할 준비하기: git checkout abc / git switch abc
  - abc라는 이름을 가진 브랜치 만들고, 해당 브랜치로 이동해서 작업할 준비하기: git checkout -b abc
16. a라는 브랜치를 b라는 브랜치로 병합할 때,
  - 1. b라는 브랜치 체크아웃하기
  - 2. git merge a
