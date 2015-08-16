# $Id: PKGBUILD 67517 2012-03-12 22:14:18Z lcarlier $
# Contributor: Jaroslaw Swierczynski <swiergot@juvepoland.com>

pkgname=libtlen
pkgver=20041113
pkgrel=5
pkgdesc="A Tlen.pl protocol library"
arch=('i686' 'x86_64')
url="http://libtlen.sourceforge.net/"
license=("GPL")
depends=(glibc)
source=(http://downloads.sourceforge.net/sourceforge/$pkgname/$pkgname-$pkgver.tar.gz)
md5sums=('b77c0a3234a21d1b79df8a8b9a9b9534')

build() {
  cd ${srcdir}/$pkgname-$pkgver

  ./configure --prefix=/usr
  make
}

package() {
  cd ${srcdir}/$pkgname-$pkgver

  make DESTDIR=${pkgdir} install
}
