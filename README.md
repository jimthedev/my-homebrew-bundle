## My Homebrew Bundle

This repo contains my [Homebrew Bundle](https://github.com/Homebrew/homebrew-bundle) file.

By downloading this file and running the bundle command, this will install all of my brew formulae, brew cask apps, and mac store apps.

## Usage

### Prereqs

Ensure you have XCode / Command Line Utils installed and the license accepted.
Ensure you have [Homebrew](http://brew.sh/) installed.
Ensure you have [Homebrew Bundle](https://github.com/Homebrew/homebrew-bundle) tapped, if not run: `brew tap Homebrew/bundle`
Ensure you have [mas-cli](https://github.com/mas-cli/mas) installed, if not run `brew install mas`

### Use it

Clone this repo

Get and install my bundle
```
cd my-homebrew-bundle
brew bundle
```

All of my brew formulae, brew cask apps, and mac store apps will be installed.

## Other

### Dump

You can create a `Brewfile` from all the existing Homebrew packages you have installed with:

    $ brew bundle dump

The `--force` option will allow an existing `Brewfile` to be overwritten as well.

### Cleanup

You can also use `Brewfile` as a whitelist. It's useful for maintainers/testers who regularly install lots of formulae. To uninstall all Homebrew formulae not listed in `Brewfile`:

    $ brew bundle cleanup

Unless the `--force` option is passed, formulae will be listed rather than actually uninstalled.

### Check

You can check there's anything to install/upgrade in the `Brewfile` by running:

    $ brew bundle check

This provides a successful exit code if everything is up-to-date so is useful for scripting.
