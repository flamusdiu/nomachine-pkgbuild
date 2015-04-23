# Maintainer: olav-st <olav.s.th@gmail.com>

pkgname=nomachine
pkgver=4.5.0
pkgrel=1
pkgdesc="Remote desktop application"
url="http://www.nomachine.com"
license=('custom:"Copyright 2002-2015 NoMachine S.à r.l."')
arch=('x86_64' 'i686')
options=('!strip')
conflicts=('nxmanager nxwebplayer nxserver nxnode nxclient')
install=nomachine.install

if [ "${CARCH}" = "x86_64" ]; then
  md5sums=('63226d45bdaa725eff24a46fb79e3d20')
  _carch=_x86_64
elif [ "${CARCH}" = "i686" ]; then
  md5sums=('043ef999dc3bb49b95e664d1a7faba7b')
  _carch=_i686
fi
source=("http://download.nomachine.com/download/4.5/Linux/${pkgname}_${pkgver}_${pkgrel}${_carch}.tar.gz")

package()
{
  cd "${srcdir}"

  install -d "${pkgdir}/usr/"
  cp -a NX "${pkgdir}/usr/NX"
}
