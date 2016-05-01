pkgname=gotree
pkgver=0.2
pkgrel=1
_commit=10a34ef
_author=bvaudour
pkgdesc="A clone of the UNIX tree command written in Go"
arch=('x86_64')
url="https://github.com/bvaudour/gotree"
license=('Public Domain')
makedepends=('go')
source=("https://github.com/${_author}/gotree/tarball/${_commit}/gotree.tar.gz")
sha256sums=('f6823c642735c2256133c957e0795478930be4cf95072dbaecdc68dbe5973db2')

package() {
	cd ..
	GOPATH="$(pwd)"
	echo $GOPATH
	mkdir -p "${pkgdir}/usr/bin"
	go build -o "${pkgdir}/usr/bin/gotree" ${_author}-gotree-${_commit}
}
