pkgname=cloc
pkgver=1.70
pkgrel=1
pkgdesc='Count lines of code'
arch=('x86_64')
url='https://github.com/AlDanial/cloc'
license=('GPL2')
depends=('perl>=5.006' 'perl-regex-common' 'perl-algorithm-diff')
source=("${url}/releases/download/v${pkgver}/cloc-${pkgver}.tar.gz")
md5sums=('c71182e2a705133fba2b3f402f17a353')

check() {
  cd "${srcdir}/${pkgname}-${pkgver}/Unix"
  make test
}


package() {
  cd "${srcdir}/${pkgname}-${pkgver}/Unix"
  make prefix="${pkgdir}" install
}

