add : 커밋할 목록에 추가

commit : 커밋 (히스토리의 한단위) 만들기
        save path : local
push : 현재까지 역사 (commits) Github에 밀어넣기
        upload

GUI대신 CLI 경험하자 : GUI는 무겁다.


# git add report_card.pdf
# : Prompt
git : Git의 Sub-command 중 하나
report_card.pdf : Arguments

# git config --global user.name "Taeung Song"
-- () : Long Name option

# git commit -s
- : 로 시작하면 보통은 Short Name Option

# Git 초기화
git config --global --unset credential.helper
git config --system --unset credential.helper

# git config --global user.email "creationwork@naver.com"
# git config --global user.name "wonhyung.yang"

# pwd
    : 현재 디렉토리 정보 확인
# cd , mkdir , ls
    : linux command와 동일
# git init
    : master setting create .git file

# rm -rf report-card
    : linux command와 동일 파일 삭제

# git (상태확인 명령어)
    show, log, shortlog, diff, status

# git commit -m "report card: Print a message of introduction"
    -m : msg options

# ! warning : LF will be replaced by CRLF in report_card.c 
        The file will have its original line endings in your working directory

# https://github.com/Dodebuge/test_git.git


# git push origin master : (충돌 오류 발생)
    --> solution : --force


# git commit , add delete
    git add test; git commit -sm "test"
    git push origin master
    git reset HEAD~1
    git push origin master --force

    ! reset HEAD~N HEAD에서 N번째 RESET한다.

# git Pull-request

    // git branch -> 현재 브랜치 확인
    // git checkout (branch name)
    // git checkout -- (file name) : 복구용으로 가능
        -b (branch name)
    // branch : 백업용으로 사용
    // 