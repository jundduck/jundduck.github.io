# Junseok Lee's Personal Homepage

This repository contains the source code for **[Junseok Lee's homepage](https://jundduck.github.io)**.

> **Acknowledgements**  
> This homepage is built on the [al-folio](https://github.com/alshedivat/al-folio) Jekyll theme and further customized based on the structure of [Sehyun Hwang's homepage](https://sehyun03.github.io/).


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## 🚀 Quick Start (Jekyll Setup)

### 1. Install Ruby
- https://rubyinstaller.org/ 에서 Ruby 설치
- 설치 중 MSYS2(Y) 선택

ruby -v
gem -v

### 2. Install Jekyll
gem install jekyll bundler

### 3. Clone Repo
git clone https://github.com/jundduck/jundduck.github.io.git
cd jundduck.github.io

### 4. Install Dependencies
bundle install

에러 발생 시:
bundle add github-pages
bundle install

### 5. Run Server
bundle exec jekyll serve

포트 충돌 시:
bundle exec jekyll serve --port 4001

👉 브라우저에서 접속: http://localhost:4000

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 🔄 Updating and Deploying to GitHub

### 0. Configure Git Identity
git config --global user.name "Junseok Lee"  
git config --global user.email "ryan082688@gmail.com"

### 1. Check Changed Files
git status

### 2. Stage Changes
git add .

### 3. Commit
git commit -m "Update site contents"

### 4. Push to GitHub
git push origin main