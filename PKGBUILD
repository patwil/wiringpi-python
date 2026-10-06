pkgname=python-wiringpi-wrapper-local
pkgver=1.0
pkgrel=1
pkgdesc="Local Python WiringPi wrapper module"
arch=('any')
license=('custom')
depends=('python')

source=('WiringPi.py')
sha256sums=('SKIP')

package() {
    local site_packages
    site_packages=$(python -c 'import site; print(site.getsitepackages()[0])')

    install -Dm644 \
        "$srcdir/WiringPi.py" \
        "$pkgdir$site_packages/WiringPi.py"
}

