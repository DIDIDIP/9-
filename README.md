# teamP 취미 아카이브

팀원 다섯 명이 각자 좋아하는 취미를 한 페이지씩 소개하는 정적 웹사이트입니다.
HTML·CSS만 써서 빌드 과정이 없고, `index.html`을 브라우저로 열면 바로 보입니다.

## 폴더 구조

```
teamP/
├── index.html              홈 (팀원 카드 5개)
├── assets/base.css         공용 스타일 (수정 전 팀에 공유)
└── members/
    ├── lee-heeyong/        이희용
    ├── lee-yongseok/       이용석
    ├── jang-woojin/        장우진
    ├── oh-sujin/           오수진
    └── hwang-inju/         황인주
        ├── index.html      내 페이지 내용
        ├── style.css       내 페이지 꾸미기 (마음대로 수정 가능)
        └── images/         내 사진 넣는 곳
```

## 내 페이지 꾸미는 법

1. **자기 폴더만** 수정합니다. 그래야 서로 충돌이 나지 않습니다.
2. `index.html`에서 `여기에 적기`, `설명` 같은 자리 표시 문구를 바꿉니다.
3. 사진은 `images/`에 넣고 `<div class="placeholder">사진 1</div>`를
   `<img src="images/파일이름.jpg" alt="사진 설명">`으로 바꿉니다.
4. `style.css`에서 `--accent` 색을 바꾸면 페이지 강조색이 한 번에 바뀝니다.
5. 홈(`index.html`)의 내 카드에 있는 `취미: 준비 중`도 고쳐 주세요.

## 올리는 법 (Git)

```bash
git clone https://github.com/DIDIDIP/9-.git
cd 9-
git checkout -b 내이름        # 예: git checkout -b oh-sujin
# ...자기 폴더 수정...
git add members/내폴더 index.html
git commit -m "오수진 페이지 꾸미기"
git push -u origin 내이름
```

GitHub에서 **Pull request**를 만들면 팀장이 확인하고 합칩니다.
팀원은 팀장이 저장소 **Settings → Collaborators**에서 초대해야 push할 수 있습니다.

## 사이트 공개하기 (GitHub Pages)

저장소 **Settings → Pages → Branch: `main` / `(root)` → Save**를 누르면
몇 분 뒤 `https://dididip.github.io/9-/`에서 볼 수 있습니다.
무료 계정은 저장소가 **Public**이어야 Pages를 켤 수 있습니다.
