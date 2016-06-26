# Maintainer: Brenton Horne <brentonhorne77 at gmail dot com>

pkgname='cinnamon-applet-weather'
_pkgname=cinnamon-weather
pkgver=1.13.2
pkgrel=1
pkgdesc='Cinnamon desktop applet for displaying local weather conditions'
arch=('any')
url='https://github.com/mockturtl/cinnamon-weather'
license=('unknown')
depends=('cinnamon')
makedepends=('git')

# Use ccprog's fix for the yahoo api format
source=("${url}/archive/v${pkgver}.tar.gz")

sha256sums=('SKIP')
_appletname='weather@mockturtl'
_appletdir="usr/share/cinnamon/applets/$_appletname"

package() {
  cd "${_pkgname}-${pkgver}"
  install -dm755 "$pkgdir/$_appletdir"
  find * -type f -exec install -Dm644 {} $pkgdir/$_appletdir/ \;
}
