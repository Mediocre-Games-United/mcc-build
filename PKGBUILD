pkgname=mcc
pkgver=0.2.1
pkgrel=3
pkgdesc="mcc compiler collection build systems"
arch=("x86_64")
depends=("glibc" "gcc" "mingw-w64-gcc" "zip" "tar" "gzip" "curl")
options=('!debug')
makedepends=("gcc" "make" "git" "mesa" "glew")

source=('git+https://github.com/Mediocre-Games-United/mcc.git' 'git+https://github.com/Mediocre-Games-United/mcc-build.git')
sha256sums=('SKIP' 'SKIP')

package() {
    cd "$srcdir/mcc-build"
    install -Dm755 "bin/x86_64/mcc" "$pkgdir/usr/bin/mcc"

    cd "$srcdir/mcc"
    install -Dm644 "mcc.desktop" "$pkgdir/usr/share/applications/mcc.desktop"
    install -Dm644 "application-x-mcc.xml" "$pkgdir/usr/share/mime/packages/x-mcc.xml"
}
