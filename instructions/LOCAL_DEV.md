# Local Development

This repo is set up to be “clone → run” without global Ruby installs or sudo.

## Prerequisites

- macOS or Linux
- (Optional, recommended) **rbenv** for a reproducible Ruby: https://github.com/rbenv/rbenv
  - macOS: `brew install rbenv ruby-build`

> If you skip rbenv, the scripts will try to use whatever `ruby` is on your PATH.

## Clone the repo

```bash
git clone <YOUR-REPO-URL> echoia-hub
cd echoia-hub
```

## One-time setup

Installs Bundler and all gems **into `vendor/bundle` inside the repo** (no sudo/global gems):

```bash
./bin/setup
```

Behind the scenes, this will:
- (If rbenv is available) select Ruby **3.2.4** (`.ruby-version` is pinned)
- install **Bundler 2.7.2** for that Ruby
- `bundle install` into `vendor/bundle/`
- generate binstubs (`./bin/jekyll`, `./bin/bundle`) so PATH issues don’t matter

## Run the site locally

### Option A – from the repo directory
```bash
./launch
```

### Option B – global command (run from anywhere)
One-time install:
```bash
./scripts/install-launch
source ~/.zshrc   # or restart your shell
```
Then start the site from anywhere:
```bash
launch-echoia
```

The site will be at **http://localhost:4000** with livereload.

## Typical workflow

1. Create or edit content/layouts/assets
2. Run `./launch` (or `launch-echoia`) to preview
3. When it looks good, commit + push

## Useful commands

- Clean build output: `rm -rf _site .jekyll-cache`
- Reinstall gems fresh: `rm -rf vendor/bundle Gemfile.lock && ./bin/setup`
- Update gems (minor): `bundle update`

> Tip: If you change Ruby versions, run `./bin/setup` again to regenerate binstubs.

---

### What’s installed automatically?

- Ruby gems only (into `vendor/bundle`) — never touches your system Ruby
- Jekyll **3.10**, kramdown + GFM parser, webrick, and GitHub metadata plugin
- `./bin/jekyll` and `./bin/bundle` shims so you can run without PATH tweaks
