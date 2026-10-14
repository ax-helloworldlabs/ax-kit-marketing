# AX 키트 마케팅 수강 안내 페이지

2026년 10월 19일 교육의 수강생 안내 페이지입니다. HTML, CSS, JavaScript와 PDF를 함께 제공하며 설치나 빌드 없이 GitHub Pages에서 사용할 수 있습니다.

## GitHub에 올리기

1. ZIP을 압축 해제합니다.
2. 이 폴더 안의 파일과 `assets` 폴더를 저장소 최상위에 업로드합니다. `index.html`이 저장소 최상위에 있어야 합니다. ZIP 파일 자체를 올리는 방식은 아닙니다.
3. 저장소의 **Settings → Pages → Build and deployment**에서 **Source: Deploy from a branch**를 선택합니다.
4. 파일을 올린 브랜치(예: `main`)와 **/(root)**를 선택하고 **Save**를 누릅니다.
5. 배포가 완료되면 Pages에 표시되는 주소로 확인합니다.

[GitHub 공식 Pages 설정 안내](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)

기존 관리자·팀장 과정 저장소를 유지하려면 마케팅 과정용 저장소에 업로드하세요.

## 파일 구성

```text
index.html                     페이지 전체 HTML
styles.css                     디자인 및 모바일 화면
script.js                      목차 강조, 전화번호 복사, 인쇄
ax-marketing-20261019.ics        캘린더 일정
.nojekyll                      GitHub Pages 정적 파일 설정
assets/
  course-introduction.pdf      AX키트_마케팅_과정소개.pdf 원본
  course-guide.pdf             AX키트_마케팅_사전안내.pdf 원본
  ai-marketing-hero.png         상단 AI 마케팅 일러스트
README.md                      업로드 및 수정 안내
```

두 PDF는 원본 내용 그대로 포함되어 있습니다. 모든 내부 파일 연결은 상대 경로이므로 저장소 이름에 따라 주소가 달라져도 사용할 수 있습니다.

## 내용 수정

- 날짜·시간·장소·준비물·교육 내용·자료 링크: `index.html`
- 색상과 배치: `styles.css`
- 캘린더 일정: `ax-marketing-20261019.ics` (날짜·시간·장소 변경 시 함께 수정)
- PDF 교체: `assets` 안의 같은 파일명으로 교체
- 수정 후 `index.html`의 CSS·JavaScript 링크에 있는 버전 값(`v=20261014-6`)을 변경하면 이전 파일이 브라우저에 남는 문제를 줄일 수 있습니다.

현재 장소는 서울 송파구 올림픽로35길 123, 9층(신천동, 향군타워) 소강의실입니다.


## 이미지

상단 일러스트는 기본 내장 이미지 생성 도구로 제작했습니다.

사용한 프롬프트:

> Use case: stylized-concept. Asset type: hero illustration for a Korean AI marketing education participant information webpage. Create a polished editorial 3D still life, landscape 3:2 composition, a pearl-white slim laptop with an abstract blank content canvas, floating frosted-glass marketing campaign cards, one lilac chat bubble, three small violet bar-chart blocks and a soft mint circular accent. The subject illustrates analyzing customer reactions and making marketing content with AI, no people. Premium tactile clay and translucent glass materials, warm off-white background (#f8f7f4), rich lavender/violet (#654ce6), midnight plum (#27233a), subtle lime mint accent. Gentle studio light, soft shadows, refined realism, airy asymmetric arrangement, small number of cohesive objects, subject centered with breathing room around edges. Absolutely no readable text, no letters, no numbers, no logos, no watermark, no stock photo aesthetics, no robot faces, no excessive icons. Not a screenshot of a website. Finished raster illustration.
