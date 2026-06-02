# assets

jsDelivr CDN 이미지 호스팅 저장소입니다.

## 폴터 구조

```text
assets
└── images/
    └── *.png, *.jpg, *.gif, *.svg ...
```

## CDN URL

GitHub 파일 경로를 다음 형식으로 변환하여 사용합니다.

```text
https://cdn.jsdelivr.net/gh/gmoon92/assets@main/images/{파일명}
```

예시:

```text
https://cdn.jsdelivr.net/gh/gmoon92/assets@main/images/architecture-v1.png
```

## 주의사항

- 저장소는 **Public**이어야 jsDelivr 캐싱이 동작합니다.
- 파일 덮어쓰기 시 CDN 캐시로 인해 이전 이미지가 남아 보일 수 있습니다.
- 버전 관리가 필요한 경우 파일명에 버전 접미사를 붙여 업로드하세요.
  - 예: `architecture-v1.png`, `architecture-v2.png`
