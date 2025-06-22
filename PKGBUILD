# Maintainer: bko <aur at bil dot co dot ua>

pkgname=pgadmin4-desktop
pkgver=9.4
pkgrel=1
pkgdesc='The desktop user interface for pgAdmin. pgAdmin is the most popular and feature rich Open Source administration and development platform for PostgreSQL, the most advanced Open Source database in the world.'
arch=('x86_64')
license=('PostgreSQL')
url='https://www.pgadmin.org/'
depends=("pgadmin4-server" 'xdg-utils' 'python-dbus')
provides=('pgadmin4-desktop')
source=(${pkgname}-${pkgver}-x86_64.deb::"https://ftp.postgresql.org/pub/pgadmin/pgadmin4/apt/noble/dists/pgadmin4/main/binary-amd64/${pkgname}_${pkgver}_amd64.deb")
sha256sums=('39cad4ee3192c4d6415d2ad1dfe3c7a78d7611bd7bc2fbca225844da5a31225b')

package() {
  # Extract package data
  tar -x --zstd -f data.tar.zst -C "${pkgdir}"
}
