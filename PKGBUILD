# Maintainer: xsigil <xsigil@users.noreply.github.com>

pkgname=ssh-to
pkgver=0.1.0
pkgrel=1
pkgdesc="Symlink-driven, transparent SSH shortcut manager"
arch=('any')
url="https://github.com/xsigil/ssh-to"
license=('MIT')
depends=('bash' 'openssh')
source=("$pkgname-$pkgver.tar.gz::$url/archive/refs/tags/v$pkgver.tar.gz")
sha256sums=('SKIP')

package() {
    cd "$pkgname-$pkgver"

    install -Dm755 bin/ssh-to "$pkgdir/usr/bin/ssh-to"
    install -Dm644 LICENSE "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
    install -Dm644 README.md "$pkgdir/usr/share/doc/$pkgname/README.md"
}
