# Maintainer: DrAbdulmalek <DrAbdulmalek@users.noreply.github.com>
# LocalSend on Manjaro — auto-installing launcher for the open-source file transfer app
# Build: cd localsend-manjaro && makepkg -si

pkgname=localsend-manjaro
pkgver=1.0.0
pkgrel=1
pkgdesc="LocalSend on Manjaro — auto-installing launcher for open-source wireless file transfer"
arch=('x86_64')
url="https://github.com/DrAbdulmalek/localsend-manjaro"
license=('MIT')
depends=()
optdepends=('flatpak: preferred installation method'
            'pamac: AUR helper for auto-install'
            'yay: AUR helper for auto-install')
install=
changelog=
source=("bin/localsend"
        "desktop/localsend.desktop")
sha256sums=('SKIP'
            'SKIP')

package() {
  # Launcher
  install -Dm755 "${srcdir}/bin/localsend" "${pkgdir}/usr/bin/localsend"

  # Desktop entry
  install -d "${pkgdir}/usr/share/applications"
  sed "s|@ICON@|/usr/share/icons/hicolor/256x256/apps/localsend.png|; s|@EXEC@|/usr/bin/localsend|" \
      "${srcdir}/desktop/localsend.desktop" > "${pkgdir}/usr/share/applications/localsend.desktop"

  # Icon directory
  install -d "${pkgdir}/usr/share/icons/hicolor/256x256/apps"
}