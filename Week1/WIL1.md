##배운 내용 복습

Git은 버전 관리 및 협업을 위해 사용하는 오픈소스 소프트웨어이다
-어떤 파일이 수정됐는지
-누가 수정했는지
-언제 수정됐는지
-어떻게 수정됐는지
이 모든 걸 추적하고 원하는 상태의 코드를 사용하기 위해 git이 중요하다

#git으로 파일 관리하기
1. 디렉토리에 git 저장소를 만들기
- git init
2. git으로 관리할 대상 등록하기
- git add
3.파일 수정 후 로컬 저장소로 옮기기
- git commit


#직접 사용해보기

Git 최초 설정
- git config ---global user.name "prettybat"
- git config --global user.email "gracehong3014@gmail.com

디렉토리 만들기

git으로 파일 관리하기
- git init

관리를 그만둘때
- rm -r .git

git으로 관리할 대상 등록하기
- git add

모든 파일 한 번에 등록
- git add .
하나씩 등록
- git add 파일명
unstage로 되돌리기
- git rm --cached 파일

파일 수정 후 로컬 저장소로 옮기기
- git commit

commit message는 타입으로 구분하면 보기 편하다
feat: 새로운 기능 추가
refactor : 기존 코드 개선
fix : 버그 수정
chore :  코듸 이외의 설정 변경
docs : 문서화
test : 테스트 코드

git에 commit하기
- git commit -m "commit message"


#Github에 올리기
올리기 전
- git remote add origin 주소
- git branch -M main
- git push -u origin main

올리기
- git add 파일명
- git commit -m "commit message"
- git push origin main
