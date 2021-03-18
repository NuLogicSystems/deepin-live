# $Id$
# Maintainer: James Kittsmiller (AJSlye) <james@nulogicsystems.com>
# Contributor: Bernhard Landauer <oberon@manjaro.org>

pkgname=deepin-live
pkgver=3.3
pkgrel=1
pkgdesc="Scripts and config for Manjaro-Deepin live session"
arch=('any')
source=('deepin-live'
    'deepin-live.desktop'
    'dde-file-manager.json')
sha256sums=('638f03133ddda5a8634361927a79d9b0d0bee19ad48269426f58c0cff309c515'
            'bd8048b5720e92d2e5c7be4f7d0c95cb058a7c35c80288aeb93436d13db0cb40'
            '9c1917bf4f62be08069262cfd0a9bc5f398bd73532f68da9be2820579c189b38')

package() {
    install -Dm755 $pkgname $pkgdir/usr/bin/$pkgname
    install -Dm644 $pkgname.desktop $pkgdir/etc/skel/.config/autostart/$pkgname.desktop
    install -Dm644 dde-file-manager.json $pkgdir/etc/skel/.config/deepin/dde-file-manager.json
}
