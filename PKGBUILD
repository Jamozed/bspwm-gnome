# Maintainer: Jake Wakeling <jake[at]omkov[dot]net>
pkgname=bspwm-gnome
pkgver=20220127
pkgrel=1
pkgdesc="bspwm with GNOME session integration"
arch=('any')
url="https://github.com/Jamozed/bspwm-gnome"
license=('unknown')
depends=(
	'bspwm'
	'gnome-session'
	'gnome-settings-daemon'
)
provides=('bspwm-gnome')
conflicts=('bspwm-gnome')

package() {
	install -m0755 -D "bspwm-gnome" "$pkgdir/usr/bin/bspwm-gnome"
	install -m0644 -D "bspwm-gnome.desktop" "$pkgdir/usr/share/applications/bspwm-gnome.deskop"
	install -m0644 -D "bspwm-gnome.session" "$pkgdir/usr/share/gnome-session/sessions/bspwm-gnome.session"
	install -m0755 -D "bspwm-gnome-session" "$pkgdir/usr/bin/bspwm-gnome-session"
	install -m0644 -D "bspwm-gnome-xsession.desktop" "$pkgdir/usr/share/xsessions/bspwm-gnome.desktop"
}
