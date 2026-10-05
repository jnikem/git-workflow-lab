# 명령어 정리
- git status : 현재 상태 확인
- git add . : 변경 파일을 staging에 올림
- git commit -m "메시지" : 스냅샷 확정
- git push : 서버에 반영
- git log --oneline --graph --all : 히스토리 그래프

## 머지 3종
| 방식 | 그래프 | 남는 것 |
|---|---|---|
| Merge commit | 갈라졌다 합쳐짐 | 원래 커밋 + 머지 커밋 |
| Squash | 한 줄 | 압축 커밋 1개 |
| Rebase | 한 줄 | 복사된 새 커밋 (해시 변경) |

- 이미 push한 커밋에는 rebase 금지 (해시가 바뀌어서 남의 것과 충돌)