# Edward Jusuk Kim — Personal Website

GitHub Pages에 바로 올릴 수 있는 정적 개인 연구자 홈페이지입니다. Jekyll이나 별도 서버 없이 `HTML + CSS`만 사용합니다.

## 파일 구성

```text
jusuk-kim.github.io/
├── index.html
├── README.md
├── .nojekyll
└── assets/
    └── css/
        └── style.css
```

- `index.html`: 홈페이지 내용과 섹션 구조
- `assets/css/style.css`: 색상, 글꼴, 배치, 모바일 디자인
- `.nojekyll`: GitHub Pages가 Jekyll 처리 없이 정적 파일을 그대로 배포하게 함
- `README.md`: 관리 및 업로드 안내

## GitHub 웹에서 업로드하기

1. 이 압축 파일을 컴퓨터에서 풉니다.
2. GitHub에서 `Jusuk-Kim/jusuk-kim.github.io` 저장소로 이동합니다.
3. **Add file → Upload files**를 선택합니다.
4. 압축을 푼 폴더 **안쪽의 모든 파일과 `assets` 폴더**를 업로드합니다. 저장소 첫 화면에 `index.html`이 직접 보여야 합니다.
5. 기존 `index.html`이 있다면 새 파일로 교체하고 **Commit changes**를 누릅니다.
6. **Settings → Pages → Build and deployment**에서 다음과 같이 설정합니다.

   ```text
   Source: Deploy from a branch
   Branch: main
   Folder: /(root)
   ```

7. 저장 후 몇 분 뒤 `https://jusuk-kim.github.io`에 접속합니다.

> `.nojekyll` 파일이 업로드 화면에서 보이지 않아도 이 사이트는 동작합니다. 해당 파일은 Jekyll 처리를 명시적으로 끄기 위한 보조 파일입니다.

## Git 명령으로 업로드하기

이미 Git을 사용하고 있다면 저장소를 복제한 뒤 이 파일들을 복사하고 다음 명령을 실행합니다.

```bash
git add .
git commit -m "Add personal academic website"
git push origin main
```

## 내용을 수정하는 위치

`index.html`에서 다음 문구를 검색해 수정하면 됩니다.

- 이름: `Edward Jusuk Kim`
- 자기소개: `My research interests lie...`
- 연구 분야: `Volumetric Streaming`, `Real-Time Networked Systems`, `3D Reconstruction & Rendering`
- 학력: `Seoul National University`
- GitHub 주소: `https://github.com/Jusuk-Kim`

디자인은 `assets/css/style.css`의 맨 위 `:root`에 있는 색상 값을 바꾸면 됩니다.

```css
:root {
  --paper: #f5f7fb;
  --ink: #111827;
  --accent: #2d5bff;
}
```

## 나중에 추가하면 좋은 항목

- 이메일
- 프로필 사진
- 연구실 및 지도교수
- 논문과 프로젝트
- CV PDF

이 정보가 준비되면 `index.html`에 새 섹션이나 링크를 추가할 수 있습니다.
