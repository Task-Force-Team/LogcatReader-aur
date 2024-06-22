# Maintainer: Task Force Team 

pkgname=Task-Force_LogCat-Reader
pkgver=main
pkgrel=1
pkgdesc="A GTKmm-based application to monitor and analyze log files from Android devices."
arch=('x86_64')
url="https://github.com/Task-Force-Team/LogcatReader"
license=('MIT')
depends=('gtkmm3')
makedepends=('git' 'make' 'gcc')
source=("git+https://github.com/Task-Force-Team/LogcatReader.git#tag=${pkgver}")
sha256sums=('SKIP')

build() {
  cd "${srcdir}/LogcatReader"
  make
}

package() {
  cd "${srcdir}/LogcatReader"
  make DESTDIR="${pkgdir}" install
}
