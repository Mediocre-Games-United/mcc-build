pkgname=mcc
pkgver=0.1.0
pkgrel=1
pkgdesc="mcc compiler collection build systems"
arch=("x86_64")
depends=("glibc" "gcc")
options=('!debug')
makedepends=("gcc" "make" "git")

source=("git+https://github.com/Mediocre-Games-United/mcc.git")
sha256sums=('SKIP')

build() {
    cd "$srcdir/mcc"
    git submodule update --init --recursive
    make package RELEASE=1
}
package() {
    cd "$srcdir/mcc"
    ls
    install -Dm755 "export/LINUXRELEASE/mcc" "$pkgdir/usr/bin/mcc"
}
