# Maintainer: DarkXero <info@techxero.com>
pkgname=calamares-config-g
_destname1="/etc"
pkgver=22.11
pkgrel=1
pkgdesc="calamares Config for XeroLinux"
arch=('any')
url="https://github.com/XeroLinuxDev"
license=('GPL3')
makedepends=('git')
depends=()
conflicts=('calamares-config')
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${pkgname}::"git+${url}/${pkgname}")
sha256sums=('SKIP')
package() {
	install -dm755 ${pkgdir}${_destname1}
	cp -r ${srcdir}/${pkgname}${_destname1}/* ${pkgdir}${_destname1}
	rm ${srcdir}/${pkgname}/creds.sh
	rm ${srcdir}/${pkgname}/push.sh
	rm ${srcdir}/${pkgname}/README.md
	rm ${srcdir}/${pkgname}/PKGBUILD
	rm ${srcdir}/${pkgname}/LICENSE
}