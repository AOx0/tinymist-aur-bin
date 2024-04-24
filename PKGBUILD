# Maintainer: Alejandro Osornio <aoxo.contact@gmail.com>
pkgname=tinymist-bin
_pkgname=tinymist
pkgver=0.11.5
pkgrel=1
pkgdesc="An integrated language service for Typst"
arch=('x86_64')
url="https://github.com/Myriad-Dreamin/tinymist"
license=('Apache-2.0')
options=('strip')
provides=('tinymist')
conflicts=('tinymist-git')
depends=(gcc-libs glibc)
source=("https://github.com/Myriad-Dreamin/tinymist/releases/download/v$pkgver/$_pkgname-linux-x64")
sha256sums=('3a6dde916018c97f65898b96b926b4e98abdc9f6e10e5841d18d924f10f09e90')

package() {
	cd "$srcdir/"
	mv "$_pkgname-linux-x64" "$_pkgname"
	install -Dm0755 -t "$pkgdir/usr/bin/" "$_pkgname"
}
