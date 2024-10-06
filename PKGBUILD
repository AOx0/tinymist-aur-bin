# Maintainer: Alejandro Osornio <aoxo.contact@gmail.com>
pkgname=tinymist-bin
_pkgname=tinymist
pkgver=0.11.28
pkgrel=2
pkgdesc="An integrated language service for Typst"
arch=('x86_64')
url="https://github.com/Myriad-Dreamin/tinymist"
license=('Apache-2.0')
options=('strip')
provides=('tinymist')
conflicts=('tinymist-git' 'tinymist-nightly-bin')
depends=(gcc-libs glibc)
source=("https://github.com/Myriad-Dreamin/tinymist/releases/download/v$pkgver/$_pkgname-linux-x64?v=$pkgver")
sha256sums=('dc5c6af9f464479aead39dfa8017faac71313f021d3f06dc39408b9edd9c4d67')

package() {
	cd "$srcdir/"
	mv "$_pkgname-linux-x64?v=$pkgver" "$_pkgname"
	install -Dm0755 -t "$pkgdir/usr/bin/" "$_pkgname"
}
