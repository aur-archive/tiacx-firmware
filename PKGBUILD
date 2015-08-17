# $Id: PKGBUILD 100069 2010-11-20 03:49:49Z pierre $
# Maintainer: Tobias Powalowski <tpowa@archlinux.org>
# Contributor: Giovanni Scafora <giovanni@archlinux.org>

pkgname=tiacx-firmware
pkgver=2
pkgrel=3
pkgdesc="Firmware for Texas Instruments ACX100/ACX111 wireless chips."
arch=('any')
url="http://acx100.sourceforge.net/"
license=('MPL')
install=tiacx-firmware.install
depends=('sh')
source=("http://pet.inf.ufsc.br/mirrors/archlinux/other/tiacx-firmware/acx-firmware-20060207.tar.bz2")
md5sums=('b8efea38c2c598190604dfa297cc9675')

build() {
  cd ${srcdir}
  install -d ${pkgdir}/usr/share
  cp -r fw "${pkgdir}/usr/share/tiacx"
  find ${pkgdir} -type d -exec chmod 755 {} \;
  find ${pkgdir} -type f -exec chmod 644 {} \;
}
