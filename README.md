# MLB 26FW 사내PR 대시보드

GitHub Pages 업로드용 정리본입니다.

## 구조
- `index.html`
- `assets/` : 경량화된 이미지/영상 (34개)

## 업로드 방법
저장소 루트에 `index.html`과 `assets` 폴더를 그대로 올리면 됩니다.
모든 경로가 상대경로(`assets/...`)라 별도 수정은 필요 없습니다.
이후 Settings > Pages 에서 브랜치를 지정하면 배포됩니다.

## 변경 이력 (v10)
- ITEM 01 · CURVE PADDING 카피 수정
  - 제목: "야구공의 곡선을 입은 경량패딩" → "가볍지만 실루엣은 새롭게, THE NEW CURVE 경량패딩"
  - 핑크 강조 문구: "초경량 소재와 4LAYERS 특수 공정으로 가벼운 착용감은 물론, 유니크한 곡선으로 완성하는 커브패딩만의 실루엣"
- ITEM 02 · SLEEK 카피 수정
  - 제목: "야구화에서 온 로우 프로파일 스니커즈" → "MLB 헤리티지를 담은 로우 프로파일 슈즈, THE NEW SLEEK"
  - 핑크 강조 문구: "슬림한 로우 프로파일 쉐입과 가벼운 중량, 유연한 아웃솔로 편안함과 힙한 무드를 동시에 완성하는 스포티브 스니커즈"

## 변경 이력 (v9)
- AMBASSADOR 02 · RESCENE 최상단: 메인 영상(`rescene-main-film.mp4`) → 가로형 단체 화보 이미지(`rescene-main-visual.webp`, 1920×1280)로 교체
- ITEM 02 · SLEEK 첫 번째 이미지: `sleek-look.webp` 신규 세로 착용컷(900×1350)으로 교체
- 사용하지 않게 된 `rescene-main-film.mp4`(3.5MB)·`rescene-film-poster.webp` 제거
- 인플루언서 컷 8종: 한글+공백 파일명(`인플컷 (1).JPEG` 등) → ASCII 파일명(`influencer-01~08.webp`)으로 정리하고 WebP로 변환
  - GitHub Pages에서 비ASCII·공백 파일명은 인코딩 이슈로 404가 날 수 있어 전면 교체
- `.filmbox img` 스타일 추가 (영상 자리에 들어간 이미지의 폭·테두리 일치)

## 변경 이력 (v8)
- 히어로 이미지: CMYK 원본(20MB) -> sRGB 변환본으로 교체, 로컬 절대경로를 상대경로로 수정
- 히어로 이미지에 width/height 지정 (로딩 중 레이아웃 시프트 방지)
- `.nb{white-space:nowrap}` 유틸 추가 — 지정 구간 줄바꿈 방지
- 폰트 폴백에 Noto Sans KR 추가 (CDN 차단 환경 대응)
- 미사용 에셋 `명동PSD T18_하단.jpg`(20MB) 제외

## 용량
- 전체 약 6.8 MB (v8 9.3MB 대비 약 2.5 MB 감소)
- 최대 단일 파일: `karina-fall-film.mp4` 3.4 MB
- GitHub 단일 파일 권장 한도(50MB)·저장소 권장 한도(1GB) 대비 여유 있음
- 미사용 예비 에셋 `lifestyle-*.webp` 8종(약 0.8MB)은 교체용으로 남겨둠 — 필요 없으면 삭제 가능
