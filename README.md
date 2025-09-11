# Git Study
This is a study for learning basic git commands

## Commands
- `git init` : 로컬에서 새 저장소 생성 (초기화)
- `git add` : 변경된 파일을 스테이징 영역에 올리기
- `git commit` : 변경 사항을 로컬 저장소에 저장 (`-m "메시지"` 옵션으로 커밋 메시지 작성)
- `git remote add origin <URL>` : 로컬 저장소를 원격 저장소와 연결
- `git clone <URL> [디렉토리명]` : 원격 저장소를 복제하여 로컬 저장소 생성 (디렉토리명 지정 가능)
- `git push` : 로컬 커밋을 원격 저장소에 업로드
- `git pull` : 원격 저장소의 변경 사항을 내려받아 병합 (fetch + merge)
- `git status` : 현재 작업 디렉토리 상태 확인 (추가/수정/삭제된 파일, 스테이징 여부)
- `git log` : 커밋 내역 확인

<br>

### 🔷 branch 생성 및 전환
- `git branch [브랜치명]` : 브랜치 생성
- `git branch` : 브랜치 확인 (브랜치 목록, 활성 브랜치 확인)
- `git checkout [브랜치명]` : 브랜치 전환
- `git checkout -b [브랜치명]` : 브랜치 생성 및 전환
- `git merge [브랜치명]` : 브랜치 병합

<br>

### 🔷 stash : 임시 저장소
- `git stash` : 변경사항 저장
- `git stash apply` : 가장 최근 stash 적용 (stash는 남아있음)
- `git stash pop` : apply + drop (stash에서 삭제까지 함)
- `git stash drop` : 가장 최근 stash 삭제
- `git stash clear` : 전체 삭제

<br>
  
### 🔷 cherry-pick - 선택적 커밋 적용 (원하는 커밋만 다른 브랜치에 적용할 때 사용)
- `git cherry-pick <commit hash>` : 특정 커밋 가져오기
- `git cherry-pick <commmit1><commit2>` : 여러 커밋 가져오기
- `git cherry-pick --continue` : 충돌 해결 후 진행
- `git cherry-pick --abort` : 충돌 발생 시 작업중단

<br>

### 🔷 rebase - 히스토리 재정렬
- `git rebase <base branch>` : base branch에 맞춰 히스토리 재정렬
- `git rebase --continue` : 충돌 해결 후 계속 진행
- `git rebase --abort` : 충돌 발생 시 rebase 중단

<br>

### 🔷 reset/revert - 히스토리 되돌리기
- `git reset <commit hash>` : 히스토리 되돌리기
  - `-soft` : commit 만 되돌림
  - `-mixed` : commit + staging area 되돌림
  - `-hard` : commit + staging area + working directory 되돌림
  
- `git revert <commit hash>` : 커밋을 되돌리는 새 커밋 생성
