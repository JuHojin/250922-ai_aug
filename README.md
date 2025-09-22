# ✨ 김개발 포트폴리오 (AI_Aug)

정적 웹 포트폴리오 사이트입니다. 반응형 레이아웃, 부드러운 스크롤, 타이핑 애니메이션, 스크롤 트리거, 스킬 바 애니메이션을 순수 HTML/CSS/JavaScript로 구현했습니다.

<p align="left">
  <a href="https://shields.io" target="_blank"><img alt="made-with" src="https://img.shields.io/badge/Build-Vanilla%20JS-10b981?style=for-the-badge"></a>
  <img alt="license" src="https://img.shields.io/badge/License-MIT-64748b?style=for-the-badge">
  <img alt="responsive" src="https://img.shields.io/badge/Responsive-Yes-3b82f6?style=for-the-badge">
</p>

---

## 📚 목차
- [미리보기](#-미리보기)
- [실행 방법](#-실행-방법)
- [프로젝트 구조](#-프로젝트-구조)
- [주요 기능](#-주요-기능)
- [페이지 섹션](#-페이지-섹션)
- [커스터마이징](#-커스터마이징)
- [배포](#-배포)
- [브라우저 지원](#-브라우저-지원)
- [라이선스](#-라이선스)
- [작성자](#-작성자)

---

## 👀 미리보기
스크린샷 또는 GIF를 여기에 추가하세요.

```
(예시)
- hero.png
- skills.gif
```

---

## 🚀 실행 방법
- 방법 1: `index.html`을 더블클릭하여 브라우저에서 열기
- 방법 2: VS Code Live Server (권장)
  1) VS Code에서 폴더 열기
  2) Live Server 확장 설치
  3) `index.html` → "Open with Live Server"

Tip: 정적 사이트이므로 별도 빌드/의존성 설치가 필요 없습니다.

---

## 🗂️ 프로젝트 구조
```
AI_Aug/
├─ index.html   # 페이지 구조(섹션, 내비게이션, 콘텐츠)
├─ style.css    # 전체 스타일, 반응형, 애니메이션, 레이아웃
└─ script.js    # 상호작용 로직, 스크롤/타이핑/폼 검증
```

---

## 🧩 주요 기능
- 🧭 내비게이션: 햄버거 메뉴(모바일), 현재 섹션 하이라이트, 부드러운 스크롤 오프셋
- 🦄 히어로: 다국어 타이핑 애니메이션(순환), 커서 블링크, 페이드 인
- 📊 스킬: `IntersectionObserver` 기반 진행바 애니메이션(`data-width` 사용)
- 🗓️ 타임라인/프로젝트: 스크롤 진입 시 페이드/슬라이드 인 애니메이션
- 🧱 헤더: 스크롤 위치에 따른 배경/그림자 동적 변화
- ✉️ 폼: 필수값/이메일 형식 검증, 제출 알림 후 리셋
- ♿ 접근성/편의: ESC·바깥 클릭·리사이즈 시 모바일 메뉴 닫기
- ⚙️ 성능: `debounce`/`throttle` 유틸 및 스크롤 핸들러 최적화

---

## 🧭 페이지 섹션
- `#home` Hero: 인사말, 이름, 다국어 타이핑, CTA 버튼, 프로필 플레이스홀더
- `#about` About: 요약 소개, 핵심 수치(경력/프로젝트/만족도)
- `#skills` Skills: Frontend/Backend/Database/DevOps 카테고리 + 진행바
- `#experience` Experience: 타임라인 형식 경력 사항
- `#projects` Projects: 카드형 프로젝트(아이콘, 설명, 기술 태그, 링크)
- `#contact` Contact: 연락처/소셜 링크/폼
- Footer: 저작권 문구

---

## 🎨 커스터마이징
- 타이핑 문구: `index.html`의 `.typing-text` `data-texts` 배열 수정
- 스킬 수치: 각 `.skill-progress`의 `data-width` 값(예: `90%`) 변경
- 콘텐츠: 프로젝트/경력/소개 텍스트는 `index.html`에서 직접 편집
- 색상·테마: `style.css`의 버튼/그라디언트/태그 색상 값 수정
- 폼 전송: 현재 데모 알림. 실제 전송은 API 연동 필요(Fetch/Webhook 등)

---

## 🌐 배포
정적 호스팅 플랫폼에 적합합니다.
- GitHub Pages / Netlify / Vercel
- GitHub Pages 예시
  1) 리포지토리 푸시
  2) Settings → Pages → Deploy from a branch → `main`/`master`
  3) 제공된 URL 사용

---

## 🖥️ 브라우저 지원
- 최신 브라우저 기준 동작
- `IntersectionObserver` 미지원 환경에서는 스킬 애니메이션이 동작하지 않을 수 있음

---

## 📄 라이선스
MIT License (필요 시 변경 가능)

---

## ✍️ 작성자
- 김개발 (소프트웨어 엔지니어)
- 소셜 링크는 `index.html` Contact 섹션 참조
