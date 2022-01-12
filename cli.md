## Why Git & Github?

#### 1. Git을 이용한 버전 관리

- 버전 : 컴퓨터 소프트웨어의 특정 상태
- 관리 : 어떤 일의 사무, 시설이나 물건의 유지,개량
- 프로그램 : 컴퓨터에서 실행될 때 특정 작업을 수행하는 일련의 명령어들의 모음

**git** : 분산 버전 관리 프로그램

-> 백업, 복구, 협업 가능

#### 2. Github를 이용한 포트폴리오



# CLI

## GUI vs CLI

1. GUI(Graphic User Interface)
   1. 그래픽을 통하여 사용자와 컴퓨터가 상호 작용하는 방식
2. CLI(Command Line Interface)
   1. 터미널을 통해 사용자와 컴퓨터가 상호작용 하는 방식



## CLI 사용 이유

new 라는 폴더를 만들고자 한다면...

1. GUI 에서는? : 우클릭 -> 새로만들기 -> 폴더 -> new

2. CLI 에서는? : mkdir (폴더이름)

   

## 작업 위치 (경로)

### 루트 디렉토리 ( / )

- windows 의 경우 일반적으로 `c드라이브` 를 의미

### 홈 디렉토리 (~)

#### 상대경로

- `./` : 현재 작업하고 있는 폴더를 의미합니다.
- `../` : 현재 작업하고 있는 폴더의 상위 폴더



TIP. `ctrl` + `l` 화면 정리



## 명령어

`cd` `폴더명`

- 현재 작업중인 디렉토리를 변경하는 명령어
- change directory

```bash
$ cd
-> 홈 디렉토리로 이동
$ cd folder # tab 으로 자동완성

$ cd ..

```



`ls`

- list segments
- 현재 작업중인 디렉토리의 폴더/파일 명을 보여주는 명령어

```bash
# 기본 사용
$ ls

# all(숨김파일 까지)
$ ls -a

# long
$ ls -l

$ ls -a -l
```



`mkdir`

- make directory
- 폴더를 생성하는 명령어
- 폴더 이름 사이에 공백을 넣고 싶다면 따옴표로 묶어서 입력한다.

```bash
# 폴더 한개
$ mkdir folder

# 폴더 여러개(공백으로 구분)
$ mkdir folder1 folder2 ...

# 폴더 이름에 공백 추가
$ mkdir "2022년 1월 12일"
```



`touch`

- 파일을 생성하는 명령어

```bash
$ touch file
```



win : `start` , mac : `open`

- 폴더/파일을 여는 명령어



`rm`

- remove
- CLI **완전삭제**

- 파일 삭제만 가능
- `-r` : recursive 옵션 -> 폴더 삭제 가능

```bash
$ rm test.txt
$ rm -r folder/
```



`mv`

- move
- 위치 이동
- 위치 이동할 폴더가 없다면 파일명 변경으로 작동

```bash
$ mv {이동시킬 파일/폴더} {이동할 폴더}
$ mv {변경시킬 파일/폴더} {변경할 이름}
```





`vi`

- vi 편집기
  - 명령 모드(command mode)
    - `dd` , `yy` : 한 줄 삭제 및 한 줄 붙여넣기
    - `x` : 글자 하나 삭제
  - 입력 모드(insert mode)
    - 명령모드에서 `i` (현재 커서 위치부터) 또는 `a` (커서 바로 다음 부분부터)
    - 명령모드로 돌아가려면 `ESC`
  - 마지막 행 모드(Last line mode)
    - 명령모드에서 `:` 입력 후 
    - `wq` (저장 후 종료), `q` (종료)