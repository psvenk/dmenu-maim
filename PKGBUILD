_pkgname=dmenu-maim
pkgname=$_pkgname-git
pkgver=r5.c509f75
pkgrel=1
pkgdesc='dmenu-maim'
arch=('any')
url='https://github.com/psvenk/dmenu-maim'
license=('2BSD')
depends=('dmenu' 'maim' 'xdotool' 'xclip')
makedepends=('git')
provides=($_pkgname)
conflicts=($_pkgname)
source=(git://github.com/psvenk/$_pkgname.git)
md5sums=('SKIP')

pkgver() {
	cd $srcdir/$_pkgname
	printf "r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

package() {
	cd $srcdir/$_pkgname
	install -Dm755 $_pkgname "$pkgdir/usr/bin/$_pkgname"
}
