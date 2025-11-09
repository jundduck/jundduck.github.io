# Junseok Lee's Personal Homepage

This repository contains the source code for [my homepage](https://jundduck.github.io).

> ***Acknowledgements***  
> This homepage is built using the [al-folio](https://github.com/alshedivat/al-folio) template of [jekyil](https://jekyllrb.com/). On top of that, this repository is based on the source of [Sehyun Hwang's homepage](https://sehyun03.github.io/).


> ** Usage for Beginner"**
새로운 거 추가
1. _(새로운거) 폴더 만들기

2. 그 안에 .md파일 만들기

3. about.html에 새로운 거 쓰기

4. about.md에 true 쓰기

5. config.yaml에 collections에 추가







수정
> education -> _education/education-1.md에서 내용 수정

> experience -> _experience/experience_1,2,3.md 내용 수정

> honors -> _honors/honors_1.md 내용 수정

> news -> _news/ann_1.md 내용 수정

> 메일, 깃허브, 링크드인, 구글 스칼라 주소 수정 -> _config.yaml 수정

CV -> header.html에 네비바에서 CV 수정



로컬에서 작업 -> 깃허브에 푸시
# 0. 계정
git config --global user.name "Junseok Lee"
git config --global user.email "ryan082688@gmail.com"

# 1. 변경된 파일 확인
git status

# 2. 모든 변경 파일 스테이징
git add .

# 3. 커밋 메시지 작성
git commit -m "Update site contents"

# 4. 원격 저장소로 푸시
git push origin main










🧩 1단계: 필수 프로그램 설치
🖥️ Windows일 경우

(아래는 PowerShell 기준입니다)

Ruby + Devkit 설치

https://rubyinstaller.org/
 에서
최신 버전 Ruby+Devkit (3.x) 다운로드 후 설치

설치 중 “MSYS2 설치 실행(Y/N)” → Y 눌러야 합니다.

설치 완료 후 새 PowerShell 열고 확인:

ruby -v
gem -v

🧰 2단계: Jekyll & Bundler 설치

(한 번만 하면 됩니다)

gem install jekyll bundler

📦 3단계: 레포지토리 복제 (GitHub에서 내 사이트 내려받기)
git clone https://github.com/jundduck/jundduck.github.io.git
cd jundduck.github.io

⚙️ 4단계: 의존성(Gem) 설치
bundle install


⚠️ 만약 여기서 에러나면
_config.yml에 theme: jekyll-theme-primer 라면,
그냥 bundle add github-pages 명령으로 GitHub Pages 버전 맞춰줍니다.

🧪 5단계: 로컬에서 사이트 실행하기
bundle exec jekyll serve
안되면 토글 bundle exec jekyll serve --port 4001

실행 후 이런 메시지가 뜨면 성공 👇

Server address: http://127.0.0.1:4000/


👉 브라우저에서 http://localhost:4000 열면 실제 사이트가 로컬에서 그대로 보입니다.