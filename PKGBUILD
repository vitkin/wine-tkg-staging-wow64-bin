pkgname="wine-tkg-staging-wow64-bin"
pkgver=9.19
pkgrel=1
pkgdesc="A compatibility layer for running Windows programs (WOW64 with TkG-Staging patches)"
url="https://github.com/Kron4ek/Wine-Builds"
license=('LGPL-2.1-or-later')
arch=('x86_64')
depends=(alsa-lib fontconfig freetype2 gettext gnutls gst-plugins-base-libs libpcap libpulse libxcomposite libxcursor libxi libxinerama libxkbcommon libxrandr opencl-icd-loader pcsclite sdl2 unixodbc v4l-utils wayland desktop-file-utils libgphoto2)
provides=(
  "wine=$pkgver"
  "wine-staging=$pkgver"
  "wine-wow64=$pkgver"
)
conflicts=("wine")
source=("https://github.com/Kron4ek/Wine-Builds/releases/download/${pkgver}/wine-${pkgver}-staging-tkg-amd64-wow64.tar.xz")
sha256sums=('8ae9462e760aa235e4453d8e092df5e137a5eefe4c60b372258d507df7651d1b')

package() {

  ## Create usr binary directory
  mkdir -p ${pkgdir}/usr

  ## Install wine package
  cp -rf ${srcdir}/wine-${pkgver}-staging-tkg-amd64-wow64/{bin,lib,share} ${pkgdir}/usr

}
