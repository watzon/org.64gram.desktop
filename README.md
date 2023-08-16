# 64Gram Flatpak

# Configuration

Building the flatpak requires setting the following github config:

```
git config --global protocol.file.allow always
```

This allows git to clone a local file containing information about a repository. May not be required for all Git versions, but it was for mine.

# Building

To build run `flatpak-builder build --force-clean org.telegram.desktop.yml`

To build and install run `flatpak-builder --user --install --force-clean build org.telegram.desktop.yml`
