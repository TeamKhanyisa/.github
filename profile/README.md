## Hi there 👋 We Are TeamKhanyisa!

# TeamKhanyisa

🔐 얼굴인식 + 블록체인 기반 스마트 도어락 프로젝트

## Repository
- [Frontend](https://github.com/TeamKhanyisa/frontend)
- [Backend](https://github.com/TeamKhanyisa/backend)
- [Device](https://github.com/TeamKhanyisa/device)
- [Blockchain](https://github.com/TeamKhanyisa/blockchain)

## Branch Strategy

| 브랜치 | 용도 | 네이밍 예시 |
|--------|------|------------|
| `main` | 운영/배포용. 항상 안정적 | main |
| `dev` | 통합 개발용. 모든 feature 브랜치 병합 | dev |
| `feature/*` | 새로운 기능 개발 | feature/login-ui<br>feature/doorlock-motor-control |
| `release/*` | 배포 전 안정화 브랜치 | release/v1.0 |
| `hotfix/*` | 운영 중 긴급 버그 수정 | hotfix/security-bug |

### Branch Workflow
1. 새 기능 개발
   - `dev`에서 `feature/기능명` 브랜치 생성
   - 작업 후 커밋 → Push → PR → `dev`에 Merge
2. 릴리스 준비
   - `dev` → `release/vX.X` 생성
   - QA/테스트 후 `main`에 Merge
   - 태그(Tag) 기록
3. 운영 중 버그 수정
   - `main`에서 `hotfix/문제명` 브랜치 생성
   - 수정 후 테스트 → `main`과 `dev` 모두 Merge

## Commit & PR Convention

| 타입 | 용도 | 예시 |
|------|------|------|
| `feat` | 새로운 기능 추가 | feat: 로그인 기능 추가 |
| `fix` | 버그 수정 | fix: 도어락 모터 오류 수정 |
| `docs` | 문서 수정 | docs: README 업데이트 |
| `chore` | 잡일, 설정 변경 | chore: 패키지 버전 업데이트 |
| `refactor` | 코드 리팩토링 | refactor: 모터 제어 함수 개선 |
| `test` | 테스트 관련 | test: 도어락 단위 테스트 추가 |

**Pull Request 규칙**
- 최소 1명 이상 코드 리뷰 후 Merge
- 제목도 커밋 컨벤션과 동일하게 작성
- 내용에 변경 사항 간단 요약 필수
