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

## Tools

- [apkingo](https://github.com/andpalmier/apkingo): extract information from APK files.
- [mbzr](https://github.com/andpalmier/mbzr): search MalwareBazaar and submit samples.
- [repopsy](https://github.com/andpalmier/repopsy): forensic analysis of git repository history.
- [tfox](https://github.com/andpalmier/tfox): search the ThreatFox IOC database.
- [urlhs](https://github.com/andpalmier/urlhs): search URLhaus and submit URLs.
- [yrfy](https://github.com/andpalmier/yrfy): interact with the YARAify API.

## Notes

- Casks are macOS only. On Linux, use `go install` or a release binary.
- macOS binaries are unsigned and not notarized.
- Casks do not remove the quarantine attribute. If macOS blocks a binary, build it with `go install` or wait for signed releases.
- GoReleaser rewrites `Casks/` on every release. Edit `homebrew_casks` in each tool's GoReleaser config instead.
