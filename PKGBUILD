pkgname=archdiff
pkgver=`git log | wc -l`
pkgrel=1
pkgdesc="A tool to view a 'system' diff for Arch Linux systems."
arch=(x86_64 i686)
url="https://github.com/daaku/archdiff"
source=(archdiff.go)
license=('apache2')
md5sums=(`md5sum archdiff.go | sed -e 's/ .*//'`)

package() {
  install -d $pkgdir/usr/bin
  go build -o $pkgdir/usr/bin/archdiff
}