# Mitosyn 시작 가이드 (고객 온보딩 사이트)

정적 HTML/CSS 사이트입니다. 빌드 단계가 없으며 저장소 루트의 `index.html`이 첫 페이지입니다.

## 구성

```
index.html            # 전체 가이드(앵커 섹션 9개)
assets/css/style.css  # 라이트/다크(prefers-color-scheme) 스타일
assets/img/*.png      # 화면 예시(로컬 테스트 주소가 보이지 않도록 일부 잘라냄)
.nojekyll             # GitHub Pages의 Jekyll 처리 끄기
```

## 로컬 미리보기

`index.html`을 브라우저로 열거나, 폴더에서 `python -m http.server 8000` 실행 후 http://localhost:8000 접속.

## GitHub Pages로 게시

1. GitHub에 새 저장소를 만들고 이 폴더를 `main` 브랜치로 push 합니다.
2. 저장소 **Settings → Pages**로 이동합니다.
3. **Build and deployment → Source: Deploy from a branch**, Branch: **main**, 폴더: **/ (root)** 를 고르고 Save.
4. 몇 분 뒤 표시되는 주소(`https://<계정>.github.io/<저장소>/`)에서 확인합니다.

사용자 지정 도메인을 쓰려면 Settings → Pages → Custom domain에 입력하고 DNS를 설정하세요.

## 참고

- `og:image`는 상대 경로입니다. 일부 SNS 미리보기는 절대 URL이 필요하므로 게시 주소가 정해지면 `https://.../assets/img/webapp-analysis-top.png` 형태로 바꾸세요.
- 서비스 상태는 "출시 준비 중 (베타)"로 표기되어 있습니다. 정식 출시 시 배지와 FAQ 문구를 갱신하세요.
