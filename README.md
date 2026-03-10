# Personal GitHub Pages site

This repo is a minimal **Jekyll** site (Home + Blog).

## Configure
- Edit `_config.yml` (name, email, and `baseurl` if needed).
- Add posts in `_posts/` as `YYYY-MM-DD-title.md`.
- Profile photo: save it as `assets/img/profile.jpg`.

## GitHub Pages
In your repo settings:
- **Settings → Pages**
- Source: **Deploy from a branch**
- Branch: `main` / root

Notes:
- For `username.github.io`, keep `baseurl: ""`.
- For a project site, set `baseurl: "/<repo-name>"`.

## Local preview (optional)
This repo includes a `Gemfile` for local preview.

### macOS prerequisites
Some Jekyll dependencies compile native extensions. Install Xcode Command Line Tools and accept the license:

```sh
xcode-select --install
sudo xcodebuild -license accept
```

### Install & run

```sh
cd /Users/wj2331/Desktop/PersonalProject/githubPage

gem install bundler
bundle install
bundle exec jekyll serve
```

Then open `http://127.0.0.1:4000`.
