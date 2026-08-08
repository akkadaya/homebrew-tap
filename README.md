# Homebrew Tap

Homebrew casks for my macOS apps.

## Dropline

[Dropline](https://github.com/chen86860/dropline) — a native macOS uploader: drag & drop,
right-click in Finder or use the menu bar to send any file to your own host, and the public
URL lands on your clipboard.

```bash
brew install --cask chen86860/tap/dropline
```

Dropline requires macOS 13 Ventura or later on Apple Silicon.

The build is ad-hoc signed rather than notarised, and Homebrew quarantines whatever it
installs, so clear the flag before the first launch:

```bash
xattr -dr com.apple.quarantine /Applications/Dropline.app
```

Dropline updates itself through Sparkle, so there is no need to `brew upgrade` it. The cask
tracks `releases/latest` and therefore carries no version number.

## Easy Complete

[Easy Complete](https://github.com/chen86860/easy-complete) — an IDE-style inline autocomplete
app for macOS terminals.

```bash
brew install --cask chen86860/tap/easy-complete
```

Easy Complete requires macOS 12 Monterey or later on Apple Silicon.
