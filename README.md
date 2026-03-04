# Junseok Lee's Personal Homepage

This repository contains the source code for **[Junseok Lee's homepage](https://jundduck.github.io)**.

> **Acknowledgements**  
> This homepage is built on the [al-folio](https://github.com/alshedivat/al-folio) Jekyll theme and further customized based on the structure of [Sehyun Hwang's homepage](https://sehyun03.github.io/).

## Usage Guide for Beginners

### Adding a New Section

To add a completely new content section:

1. Create a new folder such as `_newsection/`.
2. Add one or more `.md` files inside that folder, for example `item-1.md`.
3. Update `about.html` so the new section is rendered on the page.
4. Set the corresponding section flag to `true` in `about.md`.
5. Register the new collection under `collections:` in `_config.yml`.

### Editing Existing Sections

Most homepage content is managed through markdown files inside collection folders.

| Section | File |
| --- | --- |
| Education | `_education/education-1.md` |
| Experience | `_experience/experience_1.md`, `_experience/experience_2.md`, `_experience/experience_3.md` |
| Honors | `_honors/honors_1.md` |
| News | `_news/ann_1.md` |
| Email / GitHub / LinkedIn / Google Scholar | `_config.yml` |
| CV link in navigation bar | `_includes/header.html` |

## Local Development

### 1. Install Required Programs

For Windows (PowerShell):

1. Install **Ruby + Devkit** from [rubyinstaller.org](https://rubyinstaller.org/).
2. During installation, choose `Y` when prompted to install **MSYS2**.
3. Open a new PowerShell window and verify:

```bash
ruby -v
gem -v
```

### 2. Install Jekyll and Bundler

Run this once:

```bash
gem install jekyll bundler
```

### 3. Clone the Repository

If you do not already have the project locally:

```bash
git clone https://github.com/jundduck/jundduck.github.io.git
cd jundduck.github.io
```

### 4. Install Dependencies

```bash
bundle install
```

If `bundle install` fails and `_config.yml` uses `theme: jekyll-theme-primer`, try:

```bash
bundle add github-pages
```

### 5. Run the Site Locally

```bash
bundle exec jekyll serve
```

If port `4000` is already in use:

```bash
bundle exec jekyll serve --port 4001
```

When the server starts successfully, you should see output similar to:

```text
Server address: http://127.0.0.1:4000/
```

Then open `http://localhost:4000` in your browser.

## Updating and Deploying to GitHub

### 0. Configure Git Identity

```bash
git config --global user.name "Junseok Lee"
git config --global user.email "ryan082688@gmail.com"
```

### 1. Check Changed Files

```bash
git status
```

### 2. Stage Changes

```bash
git add .
```

### 3. Commit

```bash
git commit -m "Update site contents"
```

### 4. Push to GitHub

```bash
git push origin main
```
