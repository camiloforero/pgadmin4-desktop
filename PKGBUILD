# Maintainer: bko <aur at bil dot co dot ua>

pkgname=pgadmin4-desktop
pkgver=9.11
pkgrel=1
pkgdesc='The desktop user interface for pgAdmin. pgAdmin is the most popular and feature rich Open Source administration and development platform for PostgreSQL, the most advanced Open Source database in the world.'
arch=('x86_64')
license=('PostgreSQL')
url='https://www.pgadmin.org/'
depends=("pgadmin4-server" 'xdg-utils' 'python-dbus')
provides=('pgadmin4-desktop')
source=(${pkgname}-${pkgver}-x86_64.deb::"https://ftp.postgresql.org/pub/pgadmin/pgadmin4/apt/questing/dists/pgadmin4/main/binary-amd64/${pkgname}_${pkgver}-1.questing_amd64.deb")
sha256sums=('4d2a17ebd2a9d33cc18ad3000349da19cfbe8e1711663a7207a5b660bb9bccbc')

package() {
  # Extract package data
  tar -x --zstd -f data.tar.zst -C "${pkgdir}"
}
