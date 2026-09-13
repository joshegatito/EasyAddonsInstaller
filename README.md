# Easy addons installer

Update channel for **Easy addons installer**, a mod manager for Left 4 Dead.

## What is this repository for

The application reads `version.json` on every startup to find out whether a newer
release is available. If there is one, it blocks until the user updates.

| File | Purpose |
|---|---|
| `version.json` | Manifest: latest published version, download URL and SHA-256 checksum |
| Releases | The actual `.exe` for each version |

## version.json

```json
{
    "version": "4.1.0",
    "url": "https://github.com/joshegatito/EasyAddonsInstaller/releases/download/v4.1.0/Easy.addons.installer.exe",
    "sha256": "...",
    "notas": "One line per change"
}
```

The checksum is mandatory: the application discards any download whose hash does
not match, which protects users from a corrupted or tampered file.

## Releases

Download the latest version from the [Releases](https://github.com/joshegatito/EasyAddonsInstaller/releases) page.

Requires Left 4 Dead (AppID 500). Mods for Left 4 Dead 2 are not supported.
