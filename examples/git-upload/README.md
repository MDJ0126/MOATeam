# Git 업로드 검증

실제 VM에서 만든 결과를 팀원이 독립 검증하고 GitHub에 업로드한 최소 예제입니다.

## 결과

[`result.txt`](result.txt)에는 아래 문자열 한 줄과 마지막 줄바꿈이 들어 있습니다.

```text
MOA_GIT_UPLOAD_OK
```

## 실행 근거

| 항목 | 확인한 내용 |
| :-- | :-- |
| 실행 환경 | 공유 Linux VM · QEMU guest |
| 파일 생성 | 김하준 |
| 독립 검증 | 최서연 · REVIEW_PASS |
| 업무 소요 | 3분 48초 |
| 커밋 작성자 | 김하준 · kimhajun@moa.local |
| 원격 확인 | GitHub 브랜치를 다시 가져와 파일과 author·committer 확인 |

## 직접 확인하기

이 폴더에서 다음 명령을 실행하세요.

```sh
test "$(cat result.txt)" = MOA_GIT_UPLOAD_OK && echo REVIEW_PASS
```

[프로젝트 목록으로 돌아가기](../../README.md)
