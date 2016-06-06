# Maintainer: olav-st <olav.s.th@gmail.com>

pkgname=nomachine
pkgver=5.1.26
pkgrel=1
pkgdesc="Remote desktop application"
url="http://www.nomachine.com"
license=('custom:"Copyright 2002-2015 NoMachine S.à r.l."')
arch=('x86_64' 'i686')
options=('!strip')
conflicts=('nxmanager nxwebplayer nxserver nxnode nxclient')
install=nomachine.install

source_x86_64=("http://download.nomachine.com/download/${pkgver%.*}/Linux/${pkgname}_${pkgver}_1_x86_64.tar.gz")
source_i686=("http://download.nomachine.com/download/${pkgver%.*}/Linux/${pkgname}_${pkgver}_1_i686.tar.gz")

package()
{
  cd "${srcdir}"

  install -d "${pkgdir}/usr/"
  cp -a NX "${pkgdir}/usr/NX"
}
