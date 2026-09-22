# bonjin-app/homebrew-tap

Homebrew formulae and casks for [bonjin-app](https://github.com/bonjin-app) projects.

```bash
brew tap bonjin-app/tap
brew trust bonjin-app/tap
brew install --cask prune
```

Homebrew 7 refuses to load a cask from a tap it has not been told to trust; `brew trust` is
what tells it. On Homebrew 6 that command does not exist and the other two lines are enough.

## What is in here

| Cask    | What it installs                                                                 |
| ------- | -------------------------------------------------------------------------------- |
| `prune` | [Prune](https://github.com/bonjin-app/prune) — a local-first cleaner for caches, developer leftovers and disk space |

## The builds are not signed yet

Prune is not signed with a Developer ID, so `spctl` rejects the bundle and macOS quarantines
the download. The first launch is refused; the cask's caveats say how to get through it. This
is not a claim about what the app does — it means nobody has paid for a certificate that
vouches for it.

## Where the casks come from

`Casks/prune.rb` is generated from the Prune repository, where it lives at
`packaging/homebrew/Casks/prune.rb` and is written by `scripts/update-cask.sh --publish`
against a published release. Send changes there rather than here: a change made here is
overwritten by the next release.

## Licence

MIT, the same as the projects it packages.
