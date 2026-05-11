# wishfoldat 프로젝트

## 개요
wishfoldat.org — 정보 접근성 연구 랩 퍼스널 사이트  
단일 HTML 파일 (`index.html`), Netlify 배포 예정

## 디자인 시스템

### 팔레트
| 변수 | 값 | 대비율 | 용도 |
|------|-----|--------|------|
| `--ivory` | `#F5F1E8` | — | 배경 |
| `--warm-white` | `#FEFDFB` | — | 카드 배경 |
| `--deep-blue` | `#1E3A5F` | 10.4:1 on ivory | 주요 텍스트 |
| `--soft-blue` | `#2C4A85` | 7.7:1 on ivory | AAA 링크/포인트 |
| `--warm-brown` | `#6B4423` | 7.3:1 on white | Coming Soon 배지 배경 |
| `--gold` | `#C9A961` | 장식 전용 | 구분선, 장식 |

### 폰트
- Serif: `Crimson Pro` (Google Fonts)
- Sans: `Inter` (Google Fonts)

### 접근성 기준: WCAG AAA
- 모든 본문 텍스트: 7:1 이상
- 색상 장식 요소는 `aria-hidden="true"`

## 이중언어 구조 (핵심)
- `data-lang="ko"` / `data-lang="en"` 속성으로 콘텐츠 분리
- `hidden` 속성으로 토글 (`display:none` 사용 금지 — 접근성 트리 문제)
- `<html lang="">` 동적 변경으로 WCAG 3.1.2 준수
- **절대 `[lang]` CSS 선택자 사용 금지** — `<html lang>` 매칭되어 전체 블라인드 발생

## 철학 (사이트 정체성)
- **Unfold**: 정보는 접혀 있다. 시각적 이미지, 소리, 공간 배치 안에 의미가 접혀 있고, 이를 펼치는 것이 접근성
- **Norman UX**: 어포던스, 피드백, 상태 가시성 — ATM 버튼 비유 (시각+점자+키보드 동시 지원)
- **Ted Nelson 하이퍼텍스트**: 비선형 지식, 링크는 맥락을 운반함

## Projects 섹션
- **iRead**: 시각장애인용 인터랙티브 그림책 (Coming Soon)
- **unfoldat**: PDF → 접근성 HTML 변환 도구 → unfoldat.com 링크

## 관련 프로젝트
- unfoldat.com: `C:\Users\e\Desktop\만드는중\unfoldat\`
