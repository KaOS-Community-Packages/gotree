pkgname=gotree
pkgver=0.0.1
pkgrel=1
_commit=5af89d2
_author=boynton
pkgdesc="A simple tree command clone written in Go"
arch=('x86_64')
url="https://github.com/boynton/tree"
license=('Custom')
makedepends=('go')
source=("https://github.com/${_author}/tree/tarball/${_commit}/tree.tar.gz")
sha256sums=('6580ec4766d6d63e885d8bdb79ecdc6832dd7aa1c9fb2d9d1107f5ca5ddbe37a')

package() {
	mkdir -p "${pkgdir}/usr/bin"
	go build -o "${pkgdir}/usr/bin/${pkgname}" "${srcdir}/${_author}-tree-${_commit}/tree.go"
}
