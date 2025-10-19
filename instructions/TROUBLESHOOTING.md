# Troubleshooting

### “You must use Bundler 2 or greater with this lockfile.”
- You are using system `/usr/bin/bundle`. Always run the repo’s binstub:
  ```bash
  ./bin/jekyll serve --livereload
  ```
- Or reselect rbenv Ruby and try again:
  ```bash
  export PATH="$HOME/.rbenv/bin:$HOME/.rbenv/shims:$PATH"
  eval "$(rbenv init - zsh 2>/dev/null || rbenv init - bash)"
  rbenv shell 3.2.4
  ./launch
  ```

### “Could not find gem …” or native build errors
- Clean and reinstall:
  ```bash
  rm -rf vendor/bundle Gemfile.lock .bundle
  ./bin/setup
  ```

### Clicking “Tell me more” jumps to About page
- On each page, set an **in-page** anchor target in front matter:
  ```yaml
  banner_cta_url: "#about"
  ```
- Make sure the page has an element with `id="about"`.

### How do I preview math (MathJax)?
- Add `mathjax: true` to page front matter if your layout checks it, or ensure the MathJax include is present in the layout.

### I changed Ruby; things are weird
- Re-run the bootstrap: `./bin/setup`
