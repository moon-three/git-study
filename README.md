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

- `git branch [브랜치명]` : 브랜치 생성
- `git branch` : 브랜치 확인 (브랜치 목록, 활성 브랜치 확인)
- `git checkout [브랜치명]` : 브랜치 전환
- `git checkout -b [브랜치명]` : 브랜치 생성 및 전환
- `git merge [브랜치명]` : 브랜치 병합
