pkgname=triggerlinux-archiso
_pkgname=TriggerLinux
pkgver=$(date +%Y.%m.%d.$(git ls-remote https://github.com/realKennyStrawn93/TriggerLinux HEAD | grep -Eo '^[0-9a-f]{1,}'))
pkgrel=1
pkgdesc="TriggerLinux-specific archiso fork"
arch=('x86_64')
url="https://github.com/realKennyStrawn93/TriggerLinux"
license=('GPL')
depends=('qtcreator')
source=("git+https://github.com/realKennyStrawn93/TriggerLinux#branch=master")
md5sums=('SKIP')

package() {
  mkdir -p $pkgdir/opt
  cp -r $srcdir/$_pkgname $pkgdir/opt/TriggerLinux
}
