# Supanova Design Skill

AI가 생성하는 랜딩페이지의 디자인 퀄리티를 극적으로 향상시키는 스킬 모음입니다. 제네릭한 AI 템플릿 대신 $150k 에이전시 수준의 프리미엄 랜딩페이지를 생성합니다.

> **Powered by [supanova.dev](https://supanova.dev)** — AI 랜딩페이지 빌더
>
> Based on [taste-skill](https://github.com/Leonxlnx/taste-skill) by [@lexnlin](https://x.com/lexnlin)

## Skills

4개의 스킬이 각각의 폴더에 `SKILL.md` 파일로 존재합니다.

### 1. taste-skill (Supanova Design Engine)
메인 디자인 스킬. AI가 처음부터 프리미엄 랜딩페이지를 생성하도록 가르칩니다. 레이아웃, 타이포그래피, 컬러, 모션, 한국어 콘텐츠 품질까지 포괄합니다.

### 2. redesign-skill (Supanova Redesign Engine)
기존 랜딩페이지를 업그레이드합니다. 처음부터 다시 만드는 대신, 현재 디자인을 진단하고 가장 임팩트 있는 개선을 우선 적용합니다.

### 3. soft-skill (Supanova Premium Aesthetic)
$150k 에이전시 퀄리티에 집중합니다. Double-Bezel 카드 아키텍처, 스프링 기반 애니메이션, 플로팅 글래스 네비게이션, 한국어 타이포그래피 표준을 정의합니다.

### 4. output-skill (Supanova Full-Output)
AI의 출력 생략을 방지합니다. 플레이스홀더, 스켈레톤, 미완성 출력을 차단하고, 모든 랜딩페이지를 완전한 HTML 파일로 출력하도록 강제합니다.

## Supanova 특화 포인트

원본 taste-skill과의 주요 차이점:

- **Standalone HTML** — React/Next.js가 아닌 단일 HTML 파일 출력 (Tailwind CDN)
- **한국어 퍼스트** — Pretendard 폰트, `word-break: keep-all`, 자연스러운 한국어 카피
- **Iconify Solar** — 일관된 아이콘 시스템
- **랜딩페이지 특화** — 일반 웹앱이 아닌 전환율 중심 랜딩페이지 패턴
- **한국 시장** — 한국 사용자 이름, 한국 기업명, 한국어 CTA 패턴

## 사용법

### Claude Code (플러그인)

플러그인으로 설치하면 4개 스킬이 자동으로 활성화됩니다. 별도의 파일 복사나 참조가 필요 없습니다.

```bash
# 프로젝트 레벨 설치
claude mcp add-plugin supanova-design-skill -- https://github.com/uxjoseph/supanova-design-skill.git

# 또는 로컬 디렉토리로 테스트
claude --plugin-dir /path/to/supanova-design-skill
```

### Cursor / Windsurf / 기타 AI 에디터

1. 필요한 스킬의 `SKILL.md` 파일을 프로젝트에 복사합니다.
2. AI 에디터에서 해당 파일을 참조하세요. (예: Cursor에서 `@SKILL.md`)

끝입니다. AI가 파일을 읽고 규칙을 따릅니다.

### 추천 조합

| 상황 | 추천 스킬 |
|------|-----------|
| 새 랜딩페이지 생성 | `taste-skill` + `output-skill` |
| 기존 페이지 업그레이드 | `redesign-skill` |
| 최고 퀄리티가 필요할 때 | `taste-skill` + `soft-skill` + `output-skill` |

## 설정 (taste-skill)

taste-skill 상단의 4개 설정값을 조정할 수 있습니다:

**DESIGN_VARIANCE** — 레이아웃의 실험성
- 1-3: 깔끔하고 정돈된 대칭 그리드
- 4-7: 오버랩, 다양한 사이즈
- 8-10: 비대칭, 넉넉한 여백, 모던

**MOTION_INTENSITY** — 애니메이션 수준
- 1-3: 거의 없음. 호버 효과 정도
- 4-7: 페이드인, 스무스 스크롤
- 8-10: 마그네틱 효과, 스프링 물리, 스크롤 트리거

**VISUAL_DENSITY** — 화면당 콘텐츠 밀도
- 1-3: 넓고 럭셔리. 한 번에 하나의 요소
- 4-7: 일반적인 앱/웹사이트 간격
- 8-10: 촘촘하고 데이터 중심

**LANDING_PURPOSE** — 페이지 목적
- conversion: 전환율 중심 (기본값)
- brand: 브랜드 이미지 중심
- portfolio: 포트폴리오/쇼케이스
- saas: SaaS 제품 소개
- ecommerce: 이커머스/제품 판매

## 기술 스택

이 스킬로 생성되는 페이지의 기본 스택:

```html
<!-- Tailwind CSS (CDN) -->
<script src="https://cdn.tailwindcss.com"></script>

<!-- Pretendard 한국어 폰트 -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/orioncactus/pretendard/dist/web/static/pretendard.min.css">

<!-- Iconify Solar 아이콘 -->
<script src="https://code.iconify.design/iconify-icon/2.3.0/iconify-icon.min.js"></script>
```

## 기여 & 피드백

- GitHub Issue 또는 Pull Request
- [supanova.dev](https://supanova.dev)

## 라이선스

원본 [taste-skill](https://github.com/Leonxlnx/taste-skill)의 라이선스를 따릅니다.
