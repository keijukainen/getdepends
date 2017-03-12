pkgname=getdepends
pkgver=0.1
pkgrel=1
pkgdesc="Get a list of package dependencies from compiled binaries or source files"
url="https://github.com/keijukainen/${pkgname}"
license=('GPL')
arch=('x86_64')
depends=('file' 'grep' 'sed' 'coreutils' 'glibc' 'findutils' 'pacman' 'pkgfile')
source=("${pkgname}.zip::https://github.com/keijukainen/${pkgname}/archive/master.zip")
md5sums=('SKIP')

package() {
    install -Dm755 "${srcdir}/${pkgname}-master/${pkgname}" "${pkgdir}/usr/bin/${pkgname}"
    install -Dm644 "${srcdir}/${pkgname}-master/LICENSE" "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}
