Git Bash
시작하기
기본 리눅스 명령어
pwd 		: 현재경로
ls -la 		: 디렉토리 상세
cd ~		: 홈 디렉토리 이동
cd .. 		: 상위 디렉토리 이동
cd /c/workspace
mkdir 파일명	: 디렉토리 생성
rm -r 파일명	: 하위파일/디렉토리포함 삭제



사용자 정보 입력
git config --global user.name "dx83"
git config --global user.email "dxorder@gmail.com"

현재 디렉토리 깃 저장소로 초기화
git init
git init 디렉토리명 : 디렉토리 만들면서 깃 저장소 생성


git status		: 깃 상태 확인
git add 파일명	: 스테이징
git commit -m "메시지입력" 	: 메시지남기며 커밋
git log 		: 지금까지 커밋정보 출력
git log --stat	: 수정 사항 상세
git commit -am "메시지입력"	: 한번 커밋한 파일은 스테이징과커밋 동시 가능
git diff		: 수정 사항 출력

커밋 수정은 p65~ 참고

======================================================================
원격 저장소
https://github.com/아이디/저장소명

지역 저장소와 원격 저장소 연결
git remote add 원격저장소엘리아스 원격저장소주소
git remote add origin https://github.com/아이디/저장소명

git remote -v	: 연결 상태 확인

git push -u origin master	: 지역 저장소 모든 파일 원격 저장소에 복사
git push		: 한번이라도 연결되었다면 커밋한 파일 원격 저장소에 반영
git pull origin master		: 원격 저장소 모든 파일 지역 저장소에 복사

