# Maintainer: Alejandro Osornio <aoxo.contact@gmail.com>
pkgname=tinymist-bin
_pkgname=tinymist
pkgver=0.11.28
pkgrel=3
pkgdesc="An integrated language service for Typst"
arch=('x86_64')
url="https://github.com/Myriad-Dreamin/tinymist"
license=('Apache-2.0')
options=('strip')
provides=('tinymist')
conflicts=('tinymist-git' 'tinymist-nightly-bin')
depends=(gcc-libs glibc)
source=("https://github.com/Myriad-Dreamin/tinymist/releases/download/v$pkgver-4/$_pkgname-linux-x64?v=$pkgver-4")
sha256sums=('bbe2bc153d7a6951d5f3d2e2c909107fec611f066c0d9523697fae5bd4b347f7')

package() {
	cd "$srcdir/"
	mv "$_pkgname-linux-x64?v=$pkgver-4" "$_pkgname"
	install -Dm0755 -t "$pkgdir/usr/bin/" "$_pkgname"
}
