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


