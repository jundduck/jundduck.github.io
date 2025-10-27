# Junseok Lee's Personal Homepage

This repository contains the source code for [my homepage](https://jundduck.github.io).

> ***Acknowledgements***  
> This homepage is built using the [al-folio](https://github.com/alshedivat/al-folio) template of [jekyil](https://jekyllrb.com/). On top of that, this repository is based on the source of [Sehyun Hwang's homepage](https://sehyun03.github.io/).


> ** Usage for Beginner"**
>🧩 1단계: 필수 프로그램 설치
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