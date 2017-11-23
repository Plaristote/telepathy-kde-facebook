pkgname=telepathy-kde-facebook
_pkgdate=20171123
pkgver=1.0.0
pkgrel=1
pkgdesc='Menu entry to configure facebook IM from the telepathy KCM'
arch=('any')
depends=('purple-facebook' 'telepathy-haze' 'telepathy-kde-accounts-kcm')
source=("git+https://github.com/Plaristote/telepathy-kde-facebook.git")
md5sums=("SKIP")

package() {
  cd telepathy-kde-facebook

  services="$pkgdir/usr/share/accounts/services/kde"
  providers="$pkgdir/usr/share/accounts/providers/kde"

  mkdir -p "$services" "$providers"
  cp ktp-haze-facebook-im.service "$services"
  cp ktp-haze-facebook.provider "$providers"
}
