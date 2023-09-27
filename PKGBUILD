# Maintainer: Eshan Aryan <developer at PayraOS>
# Contributor: Eshan Aryan <m.eshan@outlook.in>

pkgname=payraos-browser-config
pkgver=1.0.0
pkgrel=1
pkgdesc="PayraOS default browser settings"
arch=('any')
url="https://github.com/PayraOSDev/payraos-browser-config/$pkgname"
license=('GPL')
makedepends=('coreutils')
source=("$pkgname-$pkgver.tar.gz::$url/-/archive/$pkgver/$pkgname-$pkgver.tar.gz")
md5sums=('SKIP')

package() {
  cd $srcdir/$pkgname-$pkgver
  mkdir -p $pkgdir/usr/lib/{chrome,chromium,brave/distribution}

  for i in chrome chromium brave; do
  	cp chrome/* $pkgdir/usr/lib/$i
  done
}
