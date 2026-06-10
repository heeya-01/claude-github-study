# Claude + GitHub 에이전트 만들기 학습 노트

> UX 디자이너가 Claude와 GitHub로 에이전트를 만들어가는 여정

---

## 학습 목표
- Claude + GitHub로 나만의 에이전트 만들기
- GitHub 기본 개념 익히기
- Claude API 이해하기

---

## 학습 로드맵
- [x] 1단계: GitHub 기본 (repo, commit, branch)
- [x] 2단계: Claude API 기초
- [ ] 3단계: 간단한 에이전트 직접 만들기
- [ ] 4단계: GitHub Actions로 자동 실행
- [ ] 5단계: 완성된 에이전트 운영

---

## 오늘 배운 것 (2026-06-10)
- Repository: 프로젝트 파일들을 저장하는 공간
- Commit: 변경사항을 저장하는 것 (저장 + 메모)
- Branch: 원본을 건드리지 않고 테스트하는 복사본
- Pull Request: 변경사항을 합쳐달라는 요청
- README.md: repo의 표지 파일

### 꼭 알아야 할 Git 명령어 5개
명령어 : 한 줄 설명 : 언제 쓰나
git clone	repo를 내 컴퓨터로 복사해오기	처음 시작할 때
git pull	GitHub의 최신 내용을 내 컴퓨터로 가져오기	다른 곳에서 수정했을 때
git add	저장할 파일 선택하기	commit 전에
git commit	변경사항 저장 + 메모 남기기	작업 완료 후
git push	내 컴퓨터 내용을 GitHub에 올리기	commit 후

### API 핵심 개념 3가지
1. API Key (열쇠)
- sk-ant-api03-xxxxxxxxxxxxx
- Claude에게 접근하는 비밀 열쇠
- 절대 공개하면 안 됨 (비용이 청구되니까!)
- GitHub에 올릴 때 특히 주의
- 
2. Request / Response (요청 / 응답)
- 내 앱 → "파리 날씨 알려줘" → Claude API
- 내 앱 ← "파리는 맑고 20도입니다" ← Claude API

3. Model (모델)
- 어떤 Claude를 쓸지 선택:
- 모델	특징
-- claude-opus-4-8 : 가장 강력, 복잡한 작업
-- claude-sonnet-4-6 : 속도+성능 균형, 일반 용도
-- claude-haiku-4-5 : 빠르고 저렴, 간단한 작업
