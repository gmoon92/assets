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

마크다운으로 삽입할 경우:

```markdown
![설명](https://cdn.jsdelivr.net/gh/gmoon92/assets@main/images/파일명.png)
```

예시:

```text
https://cdn.jsdelivr.net/gh/gmoon92/assets@main/images/architecture-v1.png
```

```markdown
![architecture](https://cdn.jsdelivr.net/gh/gmoon92/assets@main/images/architecture-v1.png)
```

### 브랜치 버전 고정

`@main` 대신 태그를 사용하면 특정 시점의 파일을 고정할 수 있습니다.

```text
https://cdn.jsdelivr.net/gh/gmoon92/assets@v1.0/images/파일명.png
```

### 파일명 주의사항

- 파일명에 **공백이나 한글**이 포함된 경우 URL 인코딩이 필요합니다.
  - 공백 → `%20`
  - 한글 → 각 문자에 해당하는 인코딩 값

## 주의사항

- 저장소는 **Public**이어야 jsDelivr 캐싱이 동작합니다.
- 파일 덮어쓰기 시 CDN 캐시로 인해 이전 이미지가 남아 보일 수 있습니다.
- 버전 관리가 필요한 경우 파일명에 버전 접미사를 붙여 업로드하세요.
  - 예: `architecture-v1.png`, `architecture-v2.png`
