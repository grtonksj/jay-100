# 🎀 백일잔치 초대장

모바일 최적화 정적 초대장입니다. GitHub Pages로 자동 배포됩니다.

## 📁 파일 구조

```
.
├── index.html              # 메인 초대장
├── assets/                 # 사진 저장 폴더
│   ├── photo1.jpg
│   └── ...
└── .github/
    └── workflows/
        └── deploy.yml      # GitHub Pages 자동 배포
```

## ✏️ 수정 체크리스트

`index.html` 안에서 `✏️` 주석을 검색해 아래 항목을 수정하세요.

| 항목 | 위치 |
|------|------|
| 아이 이름 | `<title>`, `hero-title`, `hero-name` |
| 날짜/시간 | `hero-date`, `info-card`, `EVENT` 변수 |
| 장소 | `info-card location` |
| 주차 안내 | `info-card parking` |
| 부모 이름 | `parent-names`, `footer` |
| 연락처 | `footer` |
| RSVP 폼 링크 | `rsvp-btn` href |
| 카카오맵 링크 | `map-btn.kakao` href |
| 네이버지도 링크 | `map-btn.naver` href |
| OG 이미지 | `<head>` 내 og:image |

## 📸 사진 추가

`assets/` 폴더에 사진을 넣고 슬라이드 부분을 수정하세요:

```html
<!-- 현재 이모지 → 실제 사진으로 교체 -->
<div class="slide" style="background-image:url('./assets/photo1.jpg'); background-size:cover; background-position:center;"></div>
```

## 🚀 GitHub Pages 배포

1. **저장소 설정**: Settings → Pages
2. **Source 변경**: `GitHub Actions` 선택
3. `main` 브랜치에 push → 자동 배포!
4. 배포 URL: `https://{username}.github.io/{repo-name}/`

> 처음 배포 후 2~3분 소요됩니다.
