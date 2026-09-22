# bonjin-app/homebrew-tap

Homebrew formulae and casks for [bonjin-app](https://github.com/bonjin-app) projects.

```bash
brew tap bonjin-app/tap
brew install --cask prune
```

## What is in here

| Cask    | What it installs                                                                 |
| ------- | -------------------------------------------------------------------------------- |
| `prune` | [Prune](https://github.com/bonjin-app/prune) — a local-first cleaner for caches, developer leftovers and disk space |

## The builds are not signed yet

Prune is not signed with a Developer ID, so macOS quarantines the download and Gatekeeper
refuses the first launch. Open the app once, then allow it in System Settings → Privacy &
Security. This is not a claim about what the app does; it means nobody has paid for a
certificate that vouches for it.

## Where the casks come from

`Casks/prune.rb` is generated from the Prune repository, where it lives at
`packaging/homebrew/Casks/prune.rb` and is updated by `scripts/update-cask.sh` against a
published release. Send changes there rather than here, so the two do not drift.

## Licence

MIT, the same as the projects it packages.
