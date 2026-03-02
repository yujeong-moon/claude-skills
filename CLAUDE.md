# Claude Skills 프로젝트 - Claude 작업 가이드

이 프로젝트는 Claude Code 커스텀 스킬을 개발하고 관리합니다.

---

## 프로젝트 목적

- Claude Code에서 사용할 수 있는 스킬 개발
- 스킬 개발 노하우 축적
- 완성된 스킬 버전 관리

---

## 다음 세션 시작 시

**필수 확인**:
- `learnings.md` 읽고 이전 교훈 파악
- `README.md`에서 완성된 스킬 목록 확인
- `drafts/` 폴더에 작업 중인 스킬이 있는지 확인

**현재 작업 중**:
- 없음 (save-progress 스킬 완료)

**다음 할 일**:
- 필요 시 새로운 스킬 개발

---

## 스킬 개발 워크플로우

### 1. 새 스킬 시작
```bash
mkdir drafts/new-skill
touch drafts/new-skill/SKILL.md
```

### 2. 개발 및 테스트
- SKILL.md 작성
- 직접 테스트 (1-2회)
- 수정 및 개선

### 3. 완성 후 이동
```bash
mv drafts/new-skill skills/
```

### 4. 문서 업데이트
- README.md에 스킬 추가
- learnings.md에 교훈 기록

### 5. Git 저장
```bash
git add .
git commit -m "Add new-skill"
git push
```

---

## 핵심 원칙

1. **간단하게 시작**: 복잡한 테스트보다 직접 써보기
2. **요구사항 명확히**: 불필요한 파일 생성 방지
3. **교훈 기록**: learnings.md에 배운 것 즉시 기록

---

## 파일 구조

```
claude-skills/
├── skills/          # 완성된 스킬 (배포 가능)
│   └── save-progress/
├── drafts/          # 작업 중인 스킬
├── tests/           # 테스트 결과
├── learnings.md     # 개발 교훈
└── README.md        # 프로젝트 소개
```

---

**마지막 업데이트**: 2026-03-02
