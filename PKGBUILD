pkgname=Similar
pkgver=2.4.2
pkgrel=1
pkgdesc="Similar logic simulator used on FH Hagenberg"
arch=(x86_64)

source=(https://www.similar.at/download/${pkgname}-${pkgver}.tar.gz Similar.desktop)
md5sums=(ed25a65b9dbeeb019774e591c7a5e809 4a4d6704249b5ac3d135e15c3a766dc7)

package() {
    mkdir ${pkgdir}/opt
    cp -r ${srcdir}/${pkgname}-${pkgver}/ ${pkgdir}/opt/Similar
    mkdir -p ${pkgdir}/usr/share/applications
    cp ${srcdir}/Similar.desktop ${pkgdir}/usr/share/applications
}
