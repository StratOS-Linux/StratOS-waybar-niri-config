# Maintainer: @magitian <magitian@duck.com>
pkgname=stratos-waybar-niri-config
pkgver=1.0
pkgrel=1
pkgdesc="Waybar (Niri) configuration for StratOS"
arch=('any')
license=('GPL3')
depends=(
    'waybar'
    'ttf-jetbrains-mono-nerd'
)
provides=('stratos-waybar-config')
source=()
optdepends=('ttf-jetbrains-mono-nerd: Default nerd font')
install=stratos-waybar-niri-config.install
prepare() {
    cp -r "$startdir/.config/" "$srcdir/"
}
package() {
    install -d "$pkgdir/etc/skel/.config"
    cp -r "$srcdir/.config/waybar/" "$pkgdir/etc/skel/.config/"
}
