# homebrew-ybar

Homebrew tap for [YBar](https://github.com/NineFiveB/YBar) — a Metal-rendered,
sketchybar-compatible macOS status bar.

```sh
brew tap NineFiveB/ybar
brew install ybar          # builds the latest tagged release from source
brew install --HEAD ybar   # builds current main
```

YBar builds from source on your machine (Command Line Tools are enough) and
is signed locally, so there is no Gatekeeper quarantine to bypass. See the
formula caveats and [docs/INSTALL.md](https://github.com/NineFiveB/YBar/blob/main/docs/INSTALL.md)
for the first-run privacy-permission walkthrough and login autostart.

## Maintenance

`Formula/ybar.rb` is mirrored from
[`packaging/homebrew/ybar.rb`](https://github.com/NineFiveB/YBar/blob/main/packaging/homebrew/ybar.rb)
in the main repository — that copy is the source of truth. On every release:
update the `url` tag and `sha256` there, then copy the file here verbatim.
