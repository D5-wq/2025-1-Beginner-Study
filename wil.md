[개발 입문 스터디 1주차]
*깃(git)이란?
소프트웨어 개발에서 사용되는 분산 버전 관리 시스템이다.
협업 과정에서 소스코드의 변경 내역을 추적하고 관리하여 버전을 관리할 수 있는 오픈소스 소프트웨어다. 
주요 개념
Repository: 변경 내역을 추적하고 관리하는 단위이다. 하나의 보관소.
Commit: 변경 내역을 저장소에 기록하는 작업이다.

파일의 상태는 크게 Untracked 와 Tracked로 나뉘며, Tracked에서는 다시 Unmodified, Modified, Staged로 나뉜다. 그 사이에서 Add, Edit, Stage, Remove등을 하며 상태를 변경시킬 수 있다.
실습
-git init
디렉토리에 Repository를 만들어야 한다.(파일명은 본인의 이름과 같게)
-git add
관리할 대상을 지정해야 한다.
git add <파일명>을 하면 하나의 파일을 지정할 수 있으며, git add .을 사용하면 모든 파일을 선택할 수 있다.
-git commit
파일이 수정되었다면 로컬 저장소로 옮기면 된다.

* Github
Github는 Git을 지원하는 웹호스팅 서비스이다.
버전관리와 협업을 위한 Git를 사용자 입장에서 더 편리하게 이용할 수 있도록 돕는다.
Github에서는 전체 소스코드를 업로드, 다운로드 할 수 있다.

실습
2가지 프로그램을 설치해야 한다.
Visual Studio Code와 Git을 다운로드 받는다.
Git을 설치하는 과정에서 default branch name 창이 뜨면 아래의 선택지를 고른 후 이름을 main으로 설정한다.
VS code에서는 Terminal이라는 것을 사용하는데 기본값은 powershell이다. git bash 형태의 new terminal을 만들어준다.
git을 이용하기 위해서 최초 설정이 필요하다.
github에서 회원가입을 한 후 내 깃허브 이름과 주소를 등록한다.
$ git config --global user.name "<깃허브 이름>"
$ git config --global user.name "<깃허브 이메일>"
이름과 이메일이 기억나지 않는다면 Github 내의 Settings에 들어가서 확인할 수 있다.
디렉토리를 만들기 위해서는 새폴더를 만들고 VS code에서 해당폴더를 열면 된다.
이후 과정은 다음과 같다.($생략)
git init
git add <Readme.md>
git commit -m <자기소개 글>
git remote add origin <github 주소>
git branch -M main
git push -u origin main

그리고 다음과 같은 과정을 거쳐 github에 올리면 된다.
git add <Readme.md>
git commit -m <자기소개 글>
git push origin main

처음에는 이해도 어렵고 git과 github라는 프로그램 자체가 처음이라 어렵기만 했다.
스터디 당시에도 짧은 시간으로 인해 많은 분들이 따라가기 어려워할 것 같았고 나 역시 그랬다.
이후 혼자서 강의록과 녹화 영상본을 찾아보며 추가적인 공부를 하였다.
나의 경우 내 이름으로 된 Repository가 아닌 Beginner-Study에 처음 추가를 해버려서 삭제도 못하고 당황을 했었다.
그 파일을 삭제하고 난 뒤 몇 번 더 시도를 하니 원래 내 이름 Repository에 자기소개를 추가할 수 있었다.
그런데 궁금한것은 나는 git이나 Vs code를 이용한 것이 아니라 Github 자체에서 자기소개를 작성하고 수정했다.
원래 Vs code를 작성해서 Terminal을 통해서만 접근 가능한 것이 아니었나? 싶었고
그렇다면 Vs code에서 코드를 다 작성해서 복사 붙여넣기만 하면 업로드가 되는건가 싶었다.
(물론 이전에 파일 위치나 저장 공간은 git을 통해야겠지만서도)

1주차이고 아직 작성할 스펙이 많지 않아서 자기소개는 간단하게 작성하였다.
더 많이 배워갈 수 있도록 열심히 해야겠다.