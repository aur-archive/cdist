pkgname=cdist
pkgver=3.1.12
pkgrel=1
pkgdesc='A Usable Configuration Management System"'
arch=('any')
url='http://www.nico.schottelius.org/software/cdist/'
license=('GPL3')
depends=('python>=3.2.0')
source=("http://pypi.python.org/packages/source/c/cdist/cdist-${pkgver}.tar.gz")

package() {
    cd cdist-${pkgver}
    python3 setup.py build install --root="${pkgdir}"
    find "$pkgdir" -type d -exec chmod 0755 {} \;
    find "$pkgdir" -type f -exec chmod a+r {} \;
}
md5sums=('669034726cce48a0fb7eb123e09d03c3')
