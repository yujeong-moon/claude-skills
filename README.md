# Claude Skills 개발 프로젝트

Claude Code에서 사용할 수 있는 커스텀 스킬을 개발하고 관리하는 저장소입니다.

---

## 📁 프로젝트 구조

```
claude-skills/
├── skills/          # 완성된 스킬들 (배포 준비 완료)
├── drafts/          # 작업 중인 스킬
├── tests/           # 스킬 테스트 케이스 및 결과
├── learnings.md     # 스킬 개발 시 배운 교훈
└── README.md        # 이 파일
```

---

## 🎯 완성된 스킬

### save-progress
**위치**: `skills/save-progress/`
**기능**: 작업 완료 후 Git 커밋/푸시, progress.md 업데이트, CLAUDE.md 가이드 추가, 글로벌 교훈 저장 자동화
**사용법**: "작업 완료", "저장해줘", "/save-progress"

**주요 기능**:
- Git 커밋 메시지 자동 생성 (사용자 승인)
- GitHub 푸시 (원격 저장소 없으면 생성 옵션)
- progress.md 날짜별 업데이트
- CLAUDE.md 다음 세션 가이드 추가
- 글로벌 교훈 중복 체크 및 중요도 필터링

---

## 🚀 스킬 설치 방법

### 1. Claude Code로 스킬 복사
```bash
cp -r skills/save-progress ~/.claude/skills/
```

### 2. Claude Code 재시작
스킬이 자동으로 로드됩니다.

---

## 🛠️ 스킬 개발 가이드

### 기본 원칙
1. **간단하게 시작**: 복잡한 테스트 전에 기본 동작부터
2. **요구사항 명확히**: 불필요한 파일 생성하지 않도록
3. **직접 테스트**: 서브에이전트 남발하지 말고 직접 써보기

### 개발 프로세스
1. `drafts/` 폴더에서 SKILL.md 작성
2. 직접 테스트 (1-2회)
3. 수정 및 개선
4. `skills/`로 이동
5. Git 커밋 & 푸시

### 스킬 구조
```
skill-name/
└── SKILL.md    # 스킬 정의 파일
```

**SKILL.md 기본 템플릿**:
```markdown
---
name: skill-name
description: 스킬 설명 (언제 사용하는지 포함)
---

# Skill Name

스킬 설명

## 실행 순서

1. 단계 1
2. 단계 2
...

## 주의사항
- 주의사항 1
- 주의사항 2
```

---

## 📝 개발 팁

자세한 내용은 `learnings.md` 참고

---

## 🔗 참고 링크

- [Claude Code 공식 문서](https://docs.anthropic.com/claude/docs/claude-code)
- [스킬 개발 가이드](https://docs.anthropic.com/claude/docs/skills)

---

**마지막 업데이트**: 2026-03-02
