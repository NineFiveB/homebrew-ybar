# homebrew-ybar

Homebrew tap for [YBar](https://github.com/NineFiveB/YBar) — a Metal-rendered,
sketchybar-compatible macOS status bar.

```sh
brew tap NineFiveB/ybar
brew install NineFiveB/ybar/ybar          # builds the latest tagged release from source
brew install --HEAD NineFiveB/ybar/ybar   # builds current main
```

Homebrew refuses a third-party tap until it is trusted. The full name trusts
this one formula; `brew trust NineFiveB/ybar` trusts the whole tap, after
which the short `brew install ybar` works too.

YBar builds from source on your machine (Command Line Tools are enough) and
is signed locally, so there is no Gatekeeper quarantine to bypass. See the
formula caveats and [docs/INSTALL.md](https://github.com/NineFiveB/YBar/blob/main/docs/INSTALL.md)
for the first-run privacy-permission walkthrough and login autostart.

## Maintenance

`Formula/ybar.rb` is mirrored from
[`packaging/homebrew/ybar.rb`](https://github.com/NineFiveB/YBar/blob/main/packaging/homebrew/ybar.rb)
in the main repository — that copy is the source of truth. On every release:
update the `url` tag and `sha256` there, then copy the file here verbatim.
