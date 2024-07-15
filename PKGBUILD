# Maintainer: Alejandro Osornio <aoxo.contact@gmail.com>
pkgname=tinymist-bin
_pkgname=tinymist
pkgver=0.11.15
pkgrel=1
pkgdesc="An integrated language service for Typst"
arch=('x86_64')
url="https://github.com/Myriad-Dreamin/tinymist"
license=('Apache-2.0')
options=('strip')
provides=('tinymist')
conflicts=('tinymist-git')
depends=(gcc-libs glibc)
source=("https://github.com/Myriad-Dreamin/tinymist/releases/download/v$pkgver/$_pkgname-linux-x64?v=$pkgver")
sha256sums=('9c012cb30ce3d48dba9253eaf0bdebb6d7e9d0894b375aed3f41a59f87530df5')

package() {
	cd "$srcdir/"
	mv "$_pkgname-linux-x64?v=$pkgver" "$_pkgname"
	install -Dm0755 -t "$pkgdir/usr/bin/" "$_pkgname"
}
