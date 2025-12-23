# GitHub Pages 배포 가이드 (에이원 랜딩페이지)

GitHub Pages를 이용하면 무료로 웹사이트를 전 세계에 공개할 수 있습니다. 아래 단계를 따라 진행해 주세요.

## 1단계: GitHub 저장소(Repository) 만들기
1. [GitHub](https://github.com/new)에 접속하여 로그인합니다.
2. **Repository name**에 `Aone_landingpage` (또는 원하는 이름)을 입력합니다.
3. **Public**을 선택한 상태로 **Create repository** 버튼을 누릅니다.

## 2단계: 코드 업로드하기
터미널을 열고 프로젝트 폴더(`/Users/jingyulee/Desktop/MIGHTY COSMOS/a1/Aone_landingpage`)에서 다음 명령어를 순서대로 실행하세요:

```bash
# 1. Git 초기화
git init

# 2. 파일 추가 및 커밋
git add .
git commit -m "Initial commit: Aone landing page"

# 3. 브랜치 이름을 main으로 설정
git branch -M main

# 4. 내 GitHub 저장소와 연결 (복사한 URL을 넣으세요)
# 예: git remote add origin https://github.com/사용자이름/Aone_landingpage.git
git remote add origin [나의_저장소_URL]

# 5. GitHub에 업로드
git push -u origin main
```

## 3단계: GitHub Pages 활성화하기
1. GitHub 웹사이트의 내 저장소 페이지 상단에서 **Settings** 탭을 클릭합니다.
2. 왼쪽 메뉴에서 **Pages**를 선택합니다.
3. **Build and deployment** 섹션의 **Branch** 설정을 `main` 브랜치, `/ (root)` 폴더로 설정하고 **Save**를 누릅니다.
4. 약 1~2분 뒤 상단에 `Your site is live at...` 이라는 문구와 함께 웹사이트 주소가 나타납니다!

---

### 터미널 사용이 어렵다면? (가장 쉬운 방법)
1. GitHub 저장소를 만든 후 아래쪽에 있는 **"uploading an existing file"** 링크를 클릭합니다.
2. 프로젝트 폴더의 모든 파일(`index.html`, `index.css`, `index.js`, `assets` 폴더)을 브라우저 창으로 드래그 앤 드롭합니다.
3. **Commit changes**를 누르고 위의 **3단계**를 진행합니다.
