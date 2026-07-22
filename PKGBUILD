pkgname=catos-kde-settings
pkgver=2.0
pkgrel=1
pkgdesc="CatOS KDE Settings"
arch=("any")
url="https://www.catos.info/"
license=("GPL")
source=("$pkgname::git+file://$PWD")
sha256sums=("SKIP")

package() {
    cd "$srcdir/$pkgname"

    if [ -d "etc" ]; then
        install -d "$pkgdir/etc"
        cp -a etc/. "$pkgdir/etc/"
    fi

    if [ -d "usr" ]; then
        install -d "$pkgdir/usr"
        cp -a usr/. "$pkgdir/usr/"
    fi
}
