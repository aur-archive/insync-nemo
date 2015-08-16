# Maintainer: Zhengyu Xu <xzy3186@gmail.com>

pkgname=insync-nemo
pkgver=1.2.8
pkgrel=1
pkgdesc="Nemo integration for insync"
url="https://www.insynchq.com/downloads"
license=('custom:insync')
options=(!strip)
arch=('any')

depends=("insync" "nemo" "python2-nemo")
makedepends=('gtk-doc')
source=("${pkgname}-${pkgver}.deb::http://s.insynchq.com/builds/${pkgname}_${pkgver}.35136-precise_all.deb")
sha256sums=("6d3223f6428190dfac1fe4966dbeae5af2fb7632bf0a1023d54be8d445df24d8")
noextract=("${pkgname}-${pkgver}.deb")

package() {
   cd $srcdir
   ar x ${pkgname}-${pkgver}.deb
   tar xvf data.tar.gz
   cp -rp usr $pkgdir
}
