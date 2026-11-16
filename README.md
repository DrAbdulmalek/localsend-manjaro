# LocalSend on Manjaro

Native Manjaro wrapper for [LocalSend](https://github.com/localsend/localsend) — open-source, wireless file transfer between phone and computer.

## Why LocalSend instead of SHAREit?
- **Open source** (MIT license) — no reverse engineering needed
- **No accounts, no ads, no trackers**
- **Works on local network** — phone connects to computer directly
- **Native Manjaro package** — install via PKGBUILD or Flatpak

## Quick Install
```bash
# Option 1: Flatpak (easiest)
flatpak install flathub app.localsend.LocalSend

# Option 2: AUR
pamac install localsend

# Option 3: This project (Waydroid wrapper for Android LocalSend)
cd localsend-manjaro
./scripts/install.sh
```

## Features
- Share files between Manjaro and Android/iOS devices
- Encrypted P2P transfer over local network
- No internet required
- Clean, minimal UI
