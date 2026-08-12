# homebrew-jot

Homebrew tap for [Jot](https://jot-transcribe.com/) — free, on-device dictation for macOS.

## Install

```
brew install --cask vineetu/jot/mac
```

Requires Apple Silicon and macOS Sequoia 15.0+. The app auto-updates via Sparkle
after install.

## Command line

The cask also puts Jot's transcriber on your PATH as `jot-cli` — it ships inside
the app bundle, so there is nothing extra to install.

```
jot-cli doctor                  # what's installed, as JSON
jot-cli setup                   # download whatever is missing
jot-cli setup --wizard          # the interactive version

jot-cli transcribe talk.mp4 --diarize -o talk.vtt
```

It is `jot-cli` rather than `jot` because macOS already ships `/usr/bin/jot`.

Source: https://github.com/vineetu/JOT-Transcribe
