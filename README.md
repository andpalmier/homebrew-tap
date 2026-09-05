# homebrew-tap

Homebrew tap for [@andpalmier](https://github.com/andpalmier)'s command line tools.

## Install

```bash
brew install --cask andpalmier/tap/<tool>
```

For example:

```bash
brew install --cask andpalmier/tap/repopsy
```

| Tool | Description |
| --- | --- |
| [apkingo](https://github.com/andpalmier/apkingo) | Extract information from APK files |
| [mbzr](https://github.com/andpalmier/mbzr) | Search MalwareBazaar and submit samples |
| [repopsy](https://github.com/andpalmier/repopsy) | Forensic analysis of git repository history |
| [tfox](https://github.com/andpalmier/tfox) | Search the ThreatFox IOC database |
| [urlhs](https://github.com/andpalmier/urlhs) | Search URLhaus and submit URLs |
| [yrfy](https://github.com/andpalmier/yrfy) | Interact with the YARAify API |

## Why these are casks

Homebrew expects a formula to build from source. These tools ship as
pre-compiled binaries, which is what a cask is for, and GoReleaser has
deprecated its own formula support for the same reason.

Casks only work on macOS. On Linux, install with `go install`, or take the
binaries and container images from each tool's releases page.

## Editing a cask

GoReleaser rewrites every file under `Casks/` each time it publishes a release,
so anything you change here disappears with the next one. Edit the
`homebrew_casks` section in that tool's own `.goreleaser.yaml` instead.
