# homebrew-tap

Homebrew formulae for [conduit](https://github.com/Icehunter/conduit) and other Icehunter tools.

## Usage

```bash
brew tap icehunter/tap
brew install icehunter/tap/conduit
```

Or as a one-liner:

```bash
brew install icehunter/tap/conduit
```

To upgrade:

```bash
brew upgrade icehunter/tap/conduit
```

## Updating

The `Formula/` directory is updated automatically by GoReleaser whenever a new
`v*` tag is pushed to `Icehunter/conduit`. Do not edit formulae by hand —
changes will be overwritten on the next release.

## Manual bootstrap (one-time)

If `Formula/conduit.rb` is missing because no release has run since the tap
was created, you can either:

1. Cut a new conduit release (`git tag v1.4.1 && git push --tags`), or
2. Render the formula from an existing release using GoReleaser's
   `--snapshot` mode and copy the result.

## License

Each formula is governed by its upstream project's license. The tap itself
is MIT.
