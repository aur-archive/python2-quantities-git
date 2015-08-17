# Maintainer: Gustavo Castro <gustawho[at]gmail[dot]com>
pkgname=python2-quantities-git
pkgver=375.bc3feb4
pkgrel=3
pkgdesc="Support for physical quantities based on the popular numpy library"
url="http://packages.python.org/quantities"
arch=('any')
license=('BSD')
depends=('python2-numpy' 'python2-nose')
provides=('python2-quantities')
conflicts=('python2-quantities')
makedepends=('git')
source=('git+https://github.com/python-quantities/python-quantities.git')
md5sums=('SKIP')

pkgver() {
  cd $srcdir/python-quantities
  echo $(git rev-list --count HEAD).$(git rev-parse --short HEAD)
}

package(){
  cd $srcdir/python-quantities
  python2 setup.py install --root="$pkgdir"
} 
