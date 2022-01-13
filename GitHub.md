# GitHub

## 회원가입

### 설정변경

- main 브랜치를 master 브랜치로 기본값 수정



## 원격 저장소와 로컬 저장소 연결

### Repository 생성

- git remote
- git push



## gitignore

[gitignore.io](https://gitignore.io)

- 원격 저장소에도 파일이 있고, 로컬에도 이미 있고, 이미 트래킹중인 파일을 로컬에서만 더이상 추적하지 않도록 설정 -> 잘 안씀..

```bash
$ git update-index --assume-unchanged{file name}
```

- 로컬에 있는 파일 변동 추적 멈춤
- 원격 저장소에 해당 파일이 이미 있따면 그 파일 삭제 (원격 저장소에 push 할 때 해당 파일 삭제)

```bash
$ git rm --cached {file name}
```

- 로컬, 원격 저장소 모두 파일 삭제후 추적 중지

```bash
$ git rm {file name}
```



## git clone, git pull

- git clone : 원격 저장소 repository 가져오기

```bash
$ git clone https://github.com/{userID}/{repository.git}
```

- git pull : 원격 저장소에 저장된 최신 버전을 로컬에 업데이트 하기

```bash
$ git pull
```
