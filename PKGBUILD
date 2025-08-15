# Maintainer: @zstg <zestig@duck.com>
pkgname=stratos-waybar-config
pkgver=1.0
pkgrel=1
pkgdesc="Waybar configuration for StratOS"
arch=('any')
license=('GPL3')
depends=(
    'waybar'
    'ttf-jetbrains-mono-nerd'
)
source=('.config')
optdepends=('ttf-jetbrains-mono-nerd: Default nerd font')
install=stratos-waybar-config.install
md5sums=('SKIP')
prepare() {
    cp -r "$startdir/.config/" "$srcdir/"
}
package() {
    install -d "$pkgdir/etc/skel/.config"
    cp -r "$srcdir/waybar/" "$pkgdir/etc/skel/.config/"
}