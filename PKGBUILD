# Maintainer: juergen <juergen@archlinux.org>

pkgname=xemacs-sumo
pkgver=20100727
pkgrel=1
pkgdesc="XEmacs Packages"
arch=(i686 x86_64)
url="http://www.xemacs.org"
license=('GPL')
depends=('xemacs')
source=(http://ftp.xemacs.org/pub/xemacs/packages/$pkgname-${pkgver:0:4}-${pkgver:4:2}-${pkgver:6:2}.tar.bz2)
md5sums=('951ff1fb348e17bda74844788068e792')
        
build() {
  install -d $pkgdir/usr/share/xemacs
  cp -r xemacs-packages $pkgdir/usr/share/xemacs/ || return 1
  chown -R root:root $pkgdir || return 1
}
