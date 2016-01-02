# Maintainer: Rainux Luo <rainux@gmail.com>
# Contributor: Daniel Wallace <daniel.wallace12@gmail.com>

pkgname=awesome-gnome
pkgver=0.0.1
pkgrel=3
pkgdesc='Setup awesome as window manager of GNOME 3'
arch=('any')
url='http://awesome.naquadah.org/wiki/Quickly_Setting_up_Awesome_with_Gnome'
license=('CCPL')
depends=('awesome' 'gdm>=3.0.0')
install=awesome-gnome.install
source=($pkgname.desktop
        awesome.desktop
        awesome.session)
md5sums=('0adaf444fb792e6d918379f6989f66dd'
         '871ecdef3228176b42e9e455c63e942f'
         '72d1b2d982650851cfcd1f12bb4fbff5')

package() {
    cd $srcdir
    install -Dm644 $srcdir/${source[2]} $pkgdir/usr/share/gnome-session/sessions/${source[2]}
    install -Dm644 $srcdir/${source[1]} $pkgdir/usr/share/applications/${source[1]}
    install -Dm644 $srcdir/${source[0]} $pkgdir/usr/share/xsessions/${source[0]}
}

# vim:set sts=2 ts=2 sw=2 et:
