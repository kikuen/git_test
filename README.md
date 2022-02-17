 # test_git
 테스트 기록

 # git_bash 사용

 ### git bash 란

 * Git Bash란 컴퓨터 OS와 상관없이 리눅스 베이스 터미널용 Git을 말한다.
 
 ### Git Bash에서 사용되는 Linux-base 기본 명령어 
 
 * 파일 브라우징
	+ 파일 목록 ls(list) :  -l(자세히) -a(숨김파일까지)
	+ 디렉토리(폴더) 이동 cd :  ( change directory )
	+ 현재 작업중인 디렉토리 pwd :  ( print working directory)


 ### https://git-scm.com/downloads 에서 다운로드 및 설치
 
 ### 특정 위치에서 git terminal 호출 
 
 * 저장 할려는 위치에서 git-bash 호출 하거나 cd 명령어로 이동 또는 마우스 우클릭 Git Bash Here


 ### 명령 실행을 위한 준비
 
 * git_hub Page 에서 등록 한 repositories 이름 등록
	+ $ git config --global user.name "test_git"
	
 * git_hub Page 에서 등록 한 사용자아이디(이메일) 등록
	+ $ git config --global user.email "hap0p9y@nate.com"
	
 * git 초기화 
	+ $ git init
	
 * git_원격지 와 연결 - repository 등록 후 code 탭에서 확인 가능
	+ $ git remote add origin https://github.com/kikuen/test_git.git
	
 * 원격지 연결 후 정보 확인
	+ $ git remote -v

 ## 명령어 

 ### Add
 저장소에 파일 추가(staged:무대에 오르다) - 무대에 올리다.

 (현재 디렉토리 안에 모든 파일 추가) 
 * git add .   

 (특정 파일만 추가)
 * git add [경로/파일이름]


 ### commit
 무대에 올린(staging한) 파일 커밋
 커밋시 메세지 추가(추가된 파일에 대해 타인이 알아볼 수 있도록 전달되는 간략한 메세지)

 * git commit -m '커밋메세지'


 ### push
 원격 저장소로 push
 git push [원격저장소 이름][원격저장소 브런치 이름]
 * git push origin master


 * branch-분점 - 나뉘다
 + 로컬 저장소의 변경사항을 원격 저장소(origin)의 브런치(master)에 반영


 ## 실습

 * README.md 파일 생성
 	+ $ echo "# git test reload README.md" >> README.md

 * 상태 확인
	 + $ git status

 * 반영 할 내용을 로컬 무대에 올림
 	+ $ git add README.md

 * 적용 시킬 내용 확인
	 + $ git status

 * 로컬에 적용
 	+ $ git commit -m "first commit"

 * 원격지에 적용
 	+ $ git push -u origin master

 * github repository로 가서 상태 확인

 * 파일 정보 직접 변경 후 반복







