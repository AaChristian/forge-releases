# Forge

Forge is a map editor for GoldSrc games such as Half-Life and Counter-Strike. This repository holds its installers and release notes.

**Forge is in beta.** Keep backups of your maps.

## Download

Get the latest installer from [Releases](https://github.com/AaChristian/forge-releases/releases).

Forge runs on 64-bit Windows 10 and 11. There are no Linux or macOS builds yet.

## Install

1. Download `Forge-<version>-windows-x64-setup.exe` from the newest release.
2. Run it. The installer is not code-signed, so Windows SmartScreen warns first. Choose **More info**, then **Run anyway**.
3. If your PC doesn't have Microsoft's WebView2 runtime, the installer downloads it. This needs an internet connection.

To check your download, compare its SHA-256 hash with the `.sha256` file from the same release. In PowerShell:

```powershell
Get-FileHash .\Forge-<version>-windows-x64-setup.exe -Algorithm SHA256
```

## Update

Forge checks this repository for a newer version when it starts. When there is one, an **Update** marker appears next to `FORGE BETA` in the menu bar. Click it, or choose **Help › Update to <version>…**, to read the release notes and install the update. Forge asks about unsaved changes first, then downloads the update, installs it and starts again. Your settings, game profiles, languages and prefabs are kept.

The check contacts GitHub and sends nothing about you or your maps. To turn it off, clear **Settings › General › Check for updates at startup**. **Help › Check for Updates…** still checks when you ask.

You can also update by hand: install the newer version over the old one.

## Report a problem

Open an [issue](https://github.com/AaChristian/forge-releases/issues) and include:

- the Forge version, from **Help › About Forge**
- what you did, what you expected and what happened

## License

Forge is free to use, including for maps you sell, and your maps are yours. It is provided as is, without warranty of any kind. Read the full terms in [LICENSE.md](LICENSE.md).
