# $Id: PKGBUILD 78820 2012-10-25 06:47:28Z foutrelis $
# Maintainer: Sergej Pupykin <pupykin.s+arch@gmail.com>
# Contributor: William Rea <sillywilly@gmail.com>

pkgname=python-galago-gtk
pkgver=0.5.0
pkgrel=6
pkgdesc="A library of simple functions that are optimized for various CPUs"
arch=('i686' 'x86_64')
url="http://galago-project.org"
options=('!libtool')
license=('LGPL')
depends=('libgalago-gtk' 'pygtk' 'python2-galago')
source=(http://galago-project.org/files/releases/source/galago-gtk-python/galago-gtk-python-$pkgver.tar.bz2)
md5sums=('3eb752eaa87d986bf272cf1266528c43')

build() {
  cd $srcdir/galago-gtk-python-$pkgver
  ./configure --prefix=/usr
  make
  make DESTDIR=$pkgdir install
}
