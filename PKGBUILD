# Maintainer: Gino Gravanis

pkgname=pacman-contrib-gino
pkgver=1.0.0.g29e58c9
pkgrel=1
pkgdesc='Utilities for pacman'
arch=('i686' 'x86_64')
license=('MIT')
depends=(grep pacman pacman-contrib)

pkgver() {
   git -C "$BUILDDIR" describe --long --tags | sed 's/-/./g'
}

package() {
   install -D "$BUILDDIR/bindep" "$pkgdir/usr/bin/bindep"
}
