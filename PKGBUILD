# Maintainer: Dev Ninja ninja_os@yahoo.com

pkgname=ninjaos-keyring
pkgver=1
pkgrel=1
pkgdesc="NinjaOS Pacman GPG keyring"
url="http://www.ninjaos.org"
arch=('any')
license=('GPL')
install="${pkgname}.install"
source=("ninjaos.gpg"
        "ninjaos-trusted")
sha256sums=('9e303ac88178e0c8f3aac0e6d472ceba0287ee272cadf3d5abb91b8a2858b712'
            'd75cc03ebb4b068b2b7c58db308a5d62921551e8ab36a2e5190572f2f1171b87')

package() {
  cd "${srcdir}"
  mkdir -p "${pkgdir}/usr/share/pacman/keyrings"
  install -Dm644 ninjaos.gpg "$pkgdir/usr/share/pacman/keyrings/ninjaos.gpg"
  install -Dm644 ninjaos-trusted "$pkgdir/usr/share/pacman/keyrings/ninjaos-trusted"
}

