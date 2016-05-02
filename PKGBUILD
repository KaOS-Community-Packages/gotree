pkgname=gotree
pkgver=0.3
pkgrel=1
_commit=dc0b1c60353d72f66d823698a815d8aa121a2f70
_author=bvaudour
pkgdesc="A clone of the UNIX tree command written in Go"
arch=('x86_64')
url="https://github.com/bvaudour/gotree"
license=('Public Domain')
makedepends=('go')
source=("https://github.com/${_author}/gotree/archive/${_commit}.zip")
sha256sums=('60f381b3c4aa86e829fe89bd8e67ad3cda9ee093920d8feaea70d2c7dc670e29')

package() {
	cd ..
	export GOPATH="$(pwd)"
	mkdir -p "${pkgdir}/usr/bin"
	go build -o "${pkgdir}/usr/bin/gotree" gotree-${_commit}
}
