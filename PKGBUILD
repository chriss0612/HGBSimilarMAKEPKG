pkgname=similar
pkgver=2.4.2
pkgrel=1
pkgdesc="Similar logic simulator used on FH Hagenberg"
arch=(x86_64)

source=(https://www.similar.at/download/Similar-${pkgver}.tar.gz Similar.desktop https://www.similar.at/favicon.ico)
md5sums=(76a494cfaa263f5302d10038aa4fca9b cbe19fe84bb4dd3537d73cbef15b7ddf 1046da44f45c8e015a1677b13e70ef43)

makedepends=('imagemagick')

package() {
    mkdir ${pkgdir}/opt
    cp -r ${srcdir}/Similar-${pkgver}/ ${pkgdir}/opt/similar
    mkdir -p ${pkgdir}/usr/share/applications
    cp ${srcdir}/Similar.desktop ${pkgdir}/usr/share/applications
    
    mkdir -p ${pkgdir}/usr/share/pixmaps/Similar.png
    convert ${srcdir}/favicon.ico ${pkgdir}/usr/share/pixmaps/Similar.png
}
