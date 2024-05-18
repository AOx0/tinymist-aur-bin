# Maintainer: Alejandro Osornio <aoxo.contact@gmail.com>
pkgname=tinymist-bin
_pkgname=tinymist
pkgver=0.11.9
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
sha256sums=('4e8c7240309fbd489925492cb1414341d00541b8ff54698117141b93a38ce495')

package() {
	cd "$srcdir/"
	mv "$_pkgname-linux-x64" "$_pkgname"
	install -Dm0755 -t "$pkgdir/usr/bin/" "$_pkgname"
}
