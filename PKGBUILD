# Maintainer: Nicolas Quiénot <niQo @ aur>

pkgname=ginn
pkgver=0.2.6
pkgrel=2
pkgdesc="A deamon with jinn-like wish-granting capabilities"
url="http://launchpad.net/ginn"
arch=('i686' 'x86_64')
license=('GPL')
depends=('geis' 'bamf2' 'libxtst')
source=(http://launchpad.net/ginn/0.x/${pkgver}/+download/ginn-${pkgver}.tar.gz)

build() {
  cd ${srcdir}/${pkgname}-${pkgver}

  ./configure --prefix=/usr
  make || return 1
  make DESTDIR=${pkgdir} install || return 1
}

md5sums=('008854147f0809877b3e7ccf5af5337f')
