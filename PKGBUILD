# Maintainer: Jonathan Ryan <jryan@curious-computing.com>
# Contributor: Jakub Schmidtke <sjakub@gmail.com>

pkgname=ttf-source-sans-pro
pkgver=1.050
pkgrel=6
pkgdesc="Adobe's fonts designed for user interfaces"
arch=('any')
license=('custom:OFL')
url='http://sourceforge.net/projects/sourcesans.adobe/'
depends=('fontconfig' 'xorg-fonts-encodings' 'xorg-font-utils' 'xorg-mkfontdir' 'xorg-mkfontscale')
install=ttf-source-sans-pro.install
source=("http://downloads.sourceforge.net/project/sourcesans.adobe/SourceSansPro_FontsOnly-${pkgver}.zip")
md5sums=('fb09802ab1ce200da18dc6f7ed5671b0')

package() {
  cd "${srcdir}/SourceSansPro_FontsOnly-${pkgver}/TTF"
  install -d "${pkgdir}/usr/share/fonts/TTF"
  install -m644 *.ttf "${pkgdir}/usr/share/fonts/TTF/"
  cd "${srcdir}/SourceSansPro_FontsOnly-${pkgver}"
  install -D -m644 LICENSE.txt "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}
