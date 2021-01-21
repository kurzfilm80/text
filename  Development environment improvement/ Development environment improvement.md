### 들어가는 말

제가 개발에 사용하고 있는 툴이 있다면, vim, ctags 정도인 것 같습니다. 두 가지만으로도 훌륭한 개발 도구가 될 수 있습니다. 하지만 언제 부족함을 느끼죠. 그리고 아주 익숙해져 버린 습관에서 벗어나는 것은 쉬운 일이 아닙니다. 호기심에 IDE를 다운 받아서 깔아보고 나서, 너무 많은 메뉴와 알 수 없는 기능들이 너무 많아서 다시 vim으로 돌아오곤 했습니다.

코딩에 있어서는 vim만으로 충분할 수 있습니다. 그러나 vim은 백업 그리고 버전/소스 관리에 있어서는 전혀 상관없는 툴이지요. 그 동안 버전/소스 관리는 완벽히 수동으로, 제 손가락으로 수행을 했습니다.

이제 그만 다른 개발자들이 사용하는 개발환경에 관심을 가져도 되지 않을까 생각을 합니다. 세상에 많은 개발자들이 1991년 만들어진 vim에만 머물러 있지 않으니까요.

참고로 이 문서도 Github, vscode를 이용해서 markdown 파일로 만들어 보았습니다.

# Trend

단연 Git이 가장 대표적인 버전 관리 시스템입니다. 구글에서 'version Control system'을 검색하면 상위에 Git이 랭크되어 있습니다. Git에 대한 그 명성은 대부분이 어렴풋이라도 알고 계실 겁니다. 많은 오픈 소스 프로젝트가 Github에서 개발되고 있습니다.

![VCS 랭킹](./pictures/clip_image001.png)

IDE 랭킹은 다음과 같습니다. Vim를 랭킹에서 찾아볼 수는 있습니다. 단 점유율 0.95%로 아주 초라한 share입니다.

![IDE 랭킹](./pictures/clip_image002.png)

특징으로는 2014년부터 vscode가 급성장하고 있습니다.

![vscode 급성장](./pictures/clip_image003.png)

아무래도 개발환경을 보완하고자 해서 IDE, 버전 관리 툴을 선택해야 한다면 이 중에서 하나씩을 골라서 구성하는 편이 trend에 맞는 선택이겠지요. 그래서 저는 Git, Vs code를 선택하였습니다.

# Git

우선 Git에 대한 간략한 소개를 하자면, Git은 리눅스를 만든 토발즈가 …어쩌구 저쩌구… 사용하는데 역사는 필요 없으니 생략하구요. Git의 가장 큰 키워드는 세 가지입니다. **버전 관리, 백업, 협업**이죠.

현재 우리가 하는 방식은 이렇습니다. 버전 관리를 위해서 패치를 개발할 때, 이전 폴더를 통째로 *.r101 등으로 복사하는 작업들이겠지요. 백업은 주기적으로 다른 서버에 소스를 통째로 압축을 해서 옮겨놓는 일입니다. 협업은 '누가 include를 고쳤는가? 누가 libsrc를 고쳤는가?' 이렇게 같이 일하는 사람들에게 묻는 것이죠.

이런 작업들을 체계적이고 편리하게 할 수 있다면, 코드를 한번 더 검증할 수 있는 시간이 마련되고, 고객사 니즈를 한번 더 생각할 수 있는 시간이 생기고, 퇴근 시간이 더 빨라지지 않을까요? 백업이라도, 버전 관리만이라도 크게 신경 쓰지 않아도 된다면, 큰 도움이 될 겁니다. Git이라는 도구가 버전 관리, 백업, 협업을 검증된 방식으로 도와주는 겁니다.

Git에 대한 개념과 사용방법은 인터넷에서 잘 정리된 곳들이 많으니, 이를 참고하시기 바랍니다. 저는 생활코딩의 "지옥에서 온 Git"으로 대략적인 개념을 잡았습니다. 일반인 대상 강의이기 때문에 쉽고 부담 없이 시청할 수 있습니다. 2배속으로 돌려봐도 될 정도입니다.

- 입구 수업 : [https://opentutorials.org/module/3733](https://opentutorials.org/module/3733)
- 본격 수업 : [https://opentutorials.org/course/2708](https://opentutorials.org/course/2708)

언급하고 싶은 내용이 있다면 Github입니다. Git이 버전 관리 툴이고, Github는 Git을 바탕으로 인터넷 호스팅 서비스와 WEB 인터페이스, 편리한 추가 기능을 제공해주는 웹서비스업체입니다. 더 쉽게 설명하자면, 인터넷에 나의 소스들을 백업할 수 있는 공간이라고 해두죠.

# Visual Studio Code

Visual Studio라는 이름 때문에 부담이 될 수 있습니다. 우리는 vim을 써왔으니까요. 용량의 차이, 첫 화면을 보기까지의 시간, 차이가 아주 큽니다. 하지만 Visual Studio Code는 Visual Studio와 결이 많이 다릅니다. vscode(visual studio code)는 IDE이기
보다 text 편집기에 가깝기 때문입니다. 하지만 그렇다고 해서 IDE가 가지고 있는 편리함을 못 누리는 것이 아닙니다. 휴대폰에 앱을 깔듯이 extentions을 설치하면, 다양한 기능을 사용할 수 있습니다.

무엇보다도 vim extentions을 설치하면, 고향 같은 vim 환경을 그대로 사용할 수 있습니다. ctags를 돌리지 않아도, tags 파일 구성을 고민할 필요도 없이, ‘ctrl + ]’ 단축키로 define에 접근할 수 있습니다. 또한 remote-ssh extentions을 사용하면 내 노트북의 vscode에서 원격서버를 바로 접속해서 소스를 확인하고 수정할 수도 있습니다. (단, 제약사항으로 redhat 7 이상에서 사용가능, redhat 6라도 GLIBC 2.17이상을 수동 설치하면 사용 가능)

##### vscode 주요 장점

- vim 환경 그대로 사용 가능
- 원격서버/WSL/Docker container에 있는 소스도, 마치 로컬 PC에서 작업하는 것과 같이 사용 가능(remote-development extentions 설치)

##### 참조 링크

- [vscode 설치 방법](https://code.visualstudio.com/)
- [remote-development extentions 설치 방법](https://technote.kr/320)

# WSL2

Windows Subsystem for Linux은 윈도우 10에서 리눅스를 사용할 수 있는 도구입니다. 예전에는 Virsual Host를 윈도우에 설치하고 그 위에 다시 Linux를 설치했습니다. 리눅스를 사용하기 위해서 Virsual Host을 실행하고, 리눅스를 부팅해서 사용해야 했습니다. 이제는 WSL 덕분에 윈도우에서 언제나 터미널만 열면 리눅스에 접속해서 사용할 수 있습니다.

윈도우에서도 Git을 사용할 수는 있지만 사내 소스들이 리눅스 기반 소스이기 때문에, 내 노트북에 소스들을 저장하고 관리하기 위해서는 리눅스를 로컬에 설치해야 합니다. WSL2이 이를 편리하게 해주죠.

아래 링크를 참조하셔서 WSL2를 설치하시면 됩니다.

* [WSL2 설치 방법](https://www.44bits.io/ko/post/wsl2-install-and-basic-usage)

# (너와) 나의 개발환경

제 노트북에서 xshell을 이용해서 소스가 있는 서버에 접속하고 vim으로 소스를 편집하고 빌드를 합니다. 테스트 서버에서 바이너리를 원격으로 복사해서 실행하지요. 테스트를 하고, 결과를 확인합니다.

소스 서버가 인터넷이 연결 가능한지 가능하지 않은지에 따라 두 가지 방식이 있습니다. Gibhub로 접근할 수 있는지 여부에 따라서 구성이 달라지기 때문입니다.

* 소스 서버 인터넷 가능
* 소스 서버 인터넷 불가

# Git, vscode, WSL2 개발환경

### 소스 서버가 인터넷 불가능한 경우

대부분이 이와 유사한 방식으로 작업을 하실 겁니다. 소스&빌드 서버와 테스트 서버가 보통은 사내 서버나 고객사 테스트 베드에 있기 때문이지요.

![소스 서버 인터넷 불가능한 상황의 개발환경](./pictures/devenv.png)

우선 노트북에는 vscode와 WSL2이 설치되어 있습니다. WSL2의 리눅스에는 소스가 있고 Git으로 관리되고 있죠. 소스를 1차적으로 수정하고 열람할 때는 vscode로 하면 됩니다. vscode에는 remote-develoment라는 extentions이 WSL로 연결해서 작업할 수 있도록 지원해 주니까요. 마치 로컬에서 작업하는 것처럼 만들어 줍니다.

소스 편집이 완료되면 Git을 이용(Pull)하여 WSL2의 리눅스에서 소스&빌드 서버로 변경 내용을 동기화합니다. 그 이후에 빌드, 바이너리 릴리즈, 테스트는 전과 동일한 방식으로 작업을 합니다. 빌드를 하면서 소스&빌드 서버에서 소스를 바로 수정하고 싶은 경우도 있습니다. 그런 경우에 그냥 소스&빌드 서버에서 작업을 하고 완료를 하고 난 뒤에 다시 WSL2의 리눅스와 동기화 해주면 됩니다.

어느 정도 작업이 완료가 되고 나면, WSL2의 리눅스와 Github를 동기화하도록 합니다.

### 소스 서버가 인터넷이 가능한 경우

vscode의 remote-develoment extentions으로 소스&빌드 서버에 접속을 해서 편집 및 개발 작업을 합니다. 소스&빌드 서버와 Github는 바로 연결해서 동기화하여 사용하면 됩니다. 단, 앞서 언급한 바와 같이 소스&빌드 서버가 GLIBC 2.17 이상을 사용할 수 있어야 합니다.

![소스 서버가 인터넷이 가능한 경우](./pictures/devenv_srcserve_internet_ok.png)

### 생각해 볼 수 있는 환경

내 노트북 WSL2의 리눅스를 소스&빌드 서버로 사용하는 방법도 있습니다. 단순한 구조로 사용할 수 있어서 편리합니다. 하지만 많은 제약 조건이 있습니다. WSL2의 리눅스가 Test server와 호환이 가능해야 합니다.

![생각해 볼 수 있는 환경](./pictures/ideal_devenv.png)

현재 WSL2로 설치가 가능한 리눅스 목록은 다음과 같습니다. 호환 가능성에 대해서는 각자 판단하시기 바랍니다.

* 무료 : Alpine WSL, Ubuntu, Debian, Kali Linux, Raft WSL, SUSE Linux
* 유료 : Fedora Remix For WSL, CentOS

# 실습

### 사전작업

* github 가입
* 노트북에 wsl2 Ubuntu 설치
* vscode 설치

### 프로젝트 내용

* 이름 : hello_ariel
* 개발사항 : "hello, ariel." 출력
* 보완사항#1(wsl2 리눅스에서 편집) : "nice to you, too." 출력
* 보완사항#2(소스&빌드 서버에서 편집) : "how's it going?" 출력

### 1. Github repository 만들기

Github에서 새로운 repository를 생성합니다.. Public을 선택하면 모든 사용자에게 공개되기 때문에 Private을 선택하고, README 파일과 .gitignore 파일을 기본으로 생성하기로 합니다. .gitignore 파일은 git이 추적하지 않을 파일들에 목록을 가지고 있습니다. C의 경우 *.o 파일을 추적할 필요가 없기 때문에, 이런 파일들의 목록이 들어갑니다. Github에서는 언어를 선택하면 기본적인 .gitignore 목록을 만들어 줍니다.

![repo 만들기#1](./pictures/num2.png)

hello_ariel repository가 생성되었고, 최초로 commit을 수행합니다.

![repo 만들기#2](./pictures/num3.png)

main branch에 최초 commit이 수행되었습니다.

![repo 만들기#3](./pictures/num4.png)

### 2. 노트북 WSL2 리눅스 Clone

github에서 https 서비스 주소를 확인합니다.

![실습4](./pictures/num5.png)

wsl2 linux로 접속하여 원하는 repository를 생성할 디렉토리로 이동하여, git clone을 실행하도록 합니다. git clone을 실행하면 현재 github hello_ariel repository를 그대로 가져옵니다. github에서 만들어둔 README.md와 .gitignore 파일을 확인할 수 있습니다.

```bash
kurzfilm@DESKTOP-6LCQ1SN:~$ cd ~/git.repo/ariel
kurzfilm@DESKTOP-6LCQ1SN:~/git.repo/ariel$ git clone https://github.com/kurzfilm80/hello_ariel.git
Cloning into 'hello_ariel'...
Username for 'https://github.com': kurzfilm80
Password for 'https://kurzfilm80@github.com':
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (4/4), 910 bytes | 910.00 KiB/s, done.
kurzfilm@DESKTOP-6LCQ1SN:~/git.repo/ariel$ cd hello_ariel/
kurzfilm@DESKTOP-6LCQ1SN:~/git.repo/ariel/hello_ariel$ ls
README.md
kurzfilm@DESKTOP-6LCQ1SN:~/git.repo/ariel/hello_ariel$ ls -al
total 20
drwxr-xr-x 3 kurzfilm kurzfilm 4096 Jan 21 17:49 .
drwxr-xr-x 7 kurzfilm kurzfilm 4096 Jan 21 17:49 ..
drwxr-xr-x 8 kurzfilm kurzfilm 4096 Jan 21 17:49 .git
-rw-r--r-- 1 kurzfilm kurzfilm  430 Jan 21 17:49 .gitignore
-rw-r--r-- 1 kurzfilm kurzfilm   13 Jan 21 17:49 README.md
```


### 3. 소스&빌드 서버에서 Clone

소스&빌드 서버에 접속하여 원하는 

### 4.개발, 빌드&테스트

### 5. 보완사항#1 개발, 빌드 & 테스트

### 6. 보완사항#2 개발, 빌드 & 테스트
