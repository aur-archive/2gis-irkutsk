pkgname=2gis-irkutsk
pkgver=85
pkgrel=2
pkgdesc="Map of Irkutsk for 2GIS, May 2013"
arch=('i686' 'x86_64')
url="http://irkutsk.2gis.ru/how-get/linux/"
license=('custom')
depends=('2gis>=3.13.5.1')
source=("http://download.2gis.ru/arhives/2GISData_Irkutsk-85.orig.zip")
md5sums=('98c591556de7568a7966f6e3ff5da4d2')

package() {
  install -D -m 644 "${srcdir}/2gis/3.0/Data_Irkutsk.dgdat" "${pkgdir}/opt/2gis/irkutsk.dgdat" || return 1
  install -D -m 644 "${srcdir}/2gis/3.0/Plugins/DGisLan/Irkutsk.dglf" "${pkgdir}/opt/2gis/Plugins/DGisLan/irkutsk.dglf" || return 1
}
