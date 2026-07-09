# yearimkim.github.io 배포 가이드

## 1. GitHub 저장소 만들기
1. https://github.com/new 접속
2. Repository name을 정확히 `yearimkim.github.io` 로 입력 (GitHub 아이디가 `yearimkim`이어야 이 주소가 됩니다. 아이디가 다르면 `<아이디>.github.io`)
3. Public으로 생성

## 2. 파일 업로드
방법 A — 웹에서: 저장소 페이지 → "uploading an existing file" → 이 폴더의 `index.html`, `cv_yearim.pdf`, `images/` 를 드래그해서 업로드 → Commit

방법 B — 터미널:
```bash
cd yearimkim.github.io
git init && git add . && git commit -m "Initial homepage"
git remote add origin https://github.com/yearimkim/yearimkim.github.io.git
git push -u origin main
```

## 3. 확인
1–2분 후 https://yearimkim.github.io 접속. (Settings → Pages에서 Source가 main 브랜치인지 확인)

## 이후 수정할 것
- **프로필 사진**: `images/profile.jpg` 로 사진 추가 (정사각형 권장). 없으면 "YK" 원형 placeholder가 표시됨
- **Google Scholar / GitHub 링크**: `index.html`에서 `https://scholar.google.com/`, `https://github.com/` 을 본인 프로필 주소로 교체
- **arXiv 링크**: GIG 논문의 `https://arxiv.org/` 를 실제 논문 주소로 교체
- **CV 갱신**: 새 `cv_yearim.pdf` 로 파일만 교체
