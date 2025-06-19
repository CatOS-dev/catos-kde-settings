pkgname=catos-kde-settings
pkgver=1.0
pkgrel=2
pkgdesc="CatOS KDE Settings"
arch=("any")
url="https://www.catos.info/"
license=("GPL")
install="${pkgname}.install"
source=("$pkgname::git+file://$PWD")
sha256sums=("SKIP")

package() {
   cd "$srcdir/$pkgname"

    # 安装calamares配置文件
    install -d "$pkgdir/etc"

    # 复制配置文件（根据实际文件结构调整）
    if [ -d "etc" ]; then
        cp -r etc/* "$pkgdir/etc/"
    fi
}
