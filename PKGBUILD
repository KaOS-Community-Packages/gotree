pkgname=gotree
pkgver=0.2
pkgrel=1
_commit=10a34efb0a887b8c4bef4e2bd38f5f083f422c7a
_author=bvaudour
pkgdesc="A clone of the UNIX tree command written in Go"
arch=('x86_64')
url="https://github.com/bvaudour/gotree"
license=('Public Domain')
makedepends=('go')
source=("https://github.com/${_author}/gotree/archive/${_commit}.zip")
sha256sums=('7514885c4d9f0fb65c2bd5fce9ef2d379d519d74009d6adc827465972f0063d5')

package() {
	cd ..
	export GOPATH="$(pwd)"
	mkdir -p "${pkgdir}/usr/bin"
	go build -o "${pkgdir}/usr/bin/gotree" gotree-${_commit}
}
