# Maintainer: YeonGyu Jeong <81887821@hanmail.net>
pkgname=xfce4-systemd
pkgver=1.0
pkgrel=1
pkgdesc="systemd integration for xfce4"
arch=('any')
url="https://github.com/81887821/xfce4-systemd"
license=('MIT')
depends=('xfce4-session')
source=('xfce4-session.service' 'xfce4-systemd.desktop')
sha256sums=('1a20af18287a921f745abe385ab1ab653404b8c807ffccd3e5ee5a48bc77f9e7'
            '384e95b29210963141d8c426f002652f5aeca8838b62c49897064c2ff51975f2')

package() {
    install -m 644 -D "${srcdir}/xfce4-session.service" "${pkgdir}/usr/lib/systemd/user/xfce4-session.service"
    install -m 644 -D "${srcdir}/xfce4-systemd.desktop" "${pkgdir}/usr/share/xsessions/xfce4-systemd.desktop"
}
