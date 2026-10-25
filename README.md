# 엔지니어랩 할인쿠폰 — GitHub Pages 업로드 안내

## 1. 홈페이지 정보
- 홈페이지 URL: https://engineerlab-coupon-guide.github.io/
- GitHub Organization 이름: `engineerlab-coupon-guide`
- 저장소(Repository) 이름: `engineerlab-coupon-guide.github.io`
- 저장소 공개 범위(Visibility): **Public**
- 배포 브랜치: **main**
- Pages 폴더: **/ (root)**
- 타겟 링크: https://engineerlab-guide.netlify.app/secret-code/
- 랜딩 이미지 클릭 연결: https://www.engineerlab.co.kr/ee/promotion/2025/partner/index.php?partnerID=e7288

## 2. 업로드 방법 (처음 하시는 분 기준)
1. GitHub에 로그인해 `engineerlab-coupon-guide` Organization이 있는지 확인합니다. 없다면 직접 만듭니다. GitHub에서 계정/조직 생성이나 이름 사용 가능 여부는 별도로 확인해야 합니다.
2. `engineerlab-coupon-guide.github.io`라는 이름으로 **Public** 저장소를 만듭니다. 이미 있다면 해당 저장소를 엽니다.
3. 전달받은 홈페이지 ZIP 파일의 압축을 **먼저 해제**합니다.
4. 압축 해제 폴더를 열면 `index.html`, `assets`, `favicon.png`, `robots.txt`, `sitemap.xml`, `.nojekyll`, `README.md`가 있습니다.
5. GitHub 저장소에서 **Add file → Upload files**를 눌러 압축 해제한 **파일과 폴더 전체를 저장소 최상위**에 업로드합니다. ZIP 파일 자체를 업로드하면 안 됩니다.
6. 아래쪽의 Commit changes(또는 Commit files)를 눌러 `main` 브랜치에 반영합니다.
7. 저장소 **Settings → Pages → Build and deployment**로 이동합니다.
8. Source는 **Deploy from a branch**, Branch는 **main**, Folder는 **/ (root)**로 선택하고 Save를 누릅니다.
9. GitHub Pages에서 배포 결과가 표시되면 https://engineerlab-coupon-guide.github.io/ 에 접속해 페이지를 확인합니다.

## 3. 확인해야 할 사항
- 모바일과 PC에서 페이지가 잘 보이는지 확인합니다. 스크롤 중에도 상단 헤더가 고정되어 있는지 확인합니다.
- 본문 최상단의 긴 이미지 전체를 클릭하면 **새 탭에서 엔지니어랩 e7288 프로모션 페이지**가 열려야 합니다.
- 본문의 '엔지니어랩 할인쿠폰 자세히 알아보기'는 **타겟링크**(https://engineerlab-guide.netlify.app/secret-code/)로 이동합니다.
- **고정 헤더의 `엔지니어랩 할인쿠폰` 버튼**을 클릭해도 동일한 프로모션 페이지가 열립니다.
- 썸네일은 `assets/images/thumbnail.webp`이며 `og:image`와 `twitter:image`에 사용됩니다. 랜딩 원본은 `assets/images/landing.webp`(936×8416)입니다.
- 검색 노출을 위해 원하는 검색엔진의 웹마스터 도구에서 소유 확인 및 사이트맵(https://engineerlab-coupon-guide.github.io/sitemap.xml)을 제출할 수 있습니다. 검색 노출이나 상위 순위는 보장되지 않습니다.

- 이미지에 나타나는 `4+2만원`은 4만원 쿠폰과 2만원 쿠폰을 각각 발급받는다는 뜻이 아니라, 일반 4만원 대비 시크릿코드 적용 시 총 6만원 혜택을 의미합니다.

## 4. 수정·재업로드
- 글 내용: `index.html` 편집 → 저장소에 재업로드 → 커밋
- 스타일: `assets/css/style.css` 수정 → 재업로드 → 커밋 (헤더 고정 및 반응형 스타일 포함)
- 랜딩 이미지: 같은 이름의 `assets/images/landing.webp` 파일 교체. 원본 가로세로 비율이 달라지면 `index.html`의 width/height 속성도 변경해야 합니다.
- 페이지가 갱신되지 않으면 GitHub Pages 배포 상태, 최상위의 `index.html` 존재 여부, 브라우저 캐시를 차례로 확인하세요.

## 5. 파일 구성
```text
index.html
favicon.png
robots.txt
sitemap.xml
.nojekyll
README.md
assets/
  css/
    style.css
  images/
    landing.webp     (936 × 8416)
    thumbnail.webp   (1254 × 1254)
```

본 파일은 GitHub 저장소를 만들거나 실제 배포한 결과물이 아닙니다. 배포는 저장소 소유자가 진행해야 합니다.

## 6. 네이버 사이트명·SEO·GEO 점검
- 사이트명은 **엔지니어랩 할인쿠폰**으로 통일했습니다. 헤더 `.brand-words`, 푸터, `og:site_name`, `application-name`, WebSite JSON-LD `name`이 동일합니다.
- `WebPage` 구조화 데이터는 제목·설명과 `엔지니어랩 할인` 관련 주제를 명시합니다. 실제 운영 조직과 혼동될 수 있는 Organization 마크업은 넣지 않았습니다.
- `<title>`은 `엔지니어랩 할인쿠폰 | 6만원 받는 방법과 시크릿코드 e7288`이며, 본문에는 일반 가입과 e7288의 할인 차이를 명확히 비교한 표가 있습니다.
- **네이버 사이트명 표시·검색 1위·AI 브리핑 인용은 검색엔진이 결정**합니다. 마크업으로 원하는 표시를 강제할 수 없습니다.
- 재업로드 후 네이버 서치어드바이저에서 사이트 소유확인 상태 확인 → `sitemap.xml` 제출 → 홈 URL 검사 및 웹페이지 수집 요청 → 검색 노출·클릭 리포트를 확인하세요.
- 네이버 검색 브랜드 영역에 다른 사이트명이 표시되면 먼저 검색 로봇의 재수집 상태를 확인하고, 충분히 반영되지 않을 때는 네이버 고객센터를 참고하세요.
- 검색 순위와 AI 브리핑 노출을 위해 인위적인 중복 문서나 키워드 반복을 추가하지 마세요. 실제 프로모션 조건이 바뀌면 본문도 함께 갱신하세요.
