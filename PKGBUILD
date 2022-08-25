#!/usr/bin/env bash
# Maintainer: Gino Gravanis

pkgname=pacman-contrib-gino
pkgver=1
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
