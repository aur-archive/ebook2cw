# Maintainer: kfgz <kfgz at interia pl>
# Contributor: WB2FKO <mph at sportscliche dot com>

pkgname=ebook2cw
pkgver=0.8.2
pkgrel=3
pkgdesc="Converts plain text files to Morse Code formatted as MP3 or OGG"
arch=('i686' 'x86_64')
url="http://fkurz.net/ham/ebook2cw.html"
depends=('lame' 'libvorbis')
license=('GPL')
source=(http://fkurz.net/ham/ebook2cw/${pkgname}-${pkgver}.tar.gz)
md5sums=('2069b3a4a2b21810bbf32532e2287f7d')

build() {
  cd "${srcdir}"/${pkgname}-${pkgver}
  #unset LDFLAGS
  #unset CFLAGS
  make
}

package() {
  cd "${srcdir}"/${pkgname}-${pkgver}
  make DESTDIR="${pkgdir}"/usr install
}
