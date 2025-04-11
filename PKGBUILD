pkgname="wine-tkg-staging-wow64-bin"
pkgver=10.5
pkgrel=1
pkgdesc="A compatibility layer for running Windows programs (WOW64 with TkG-Staging patches)"
url="https://github.com/Kron4ek/Wine-Builds"
license=('LGPL-2.1-or-later')
arch=('x86_64')
depends=(alsa-lib fontconfig freetype2 gettext gnutls gst-plugins-base-libs libpcap libpulse libxcomposite libxcursor libxi libxinerama libxkbcommon libxrandr opencl-icd-loader pcsclite sdl2 unixodbc v4l-utils wayland desktop-file-utils libgphoto2 glibc)
provides=(
  "wine=$pkgver"
  "wine-staging=$pkgver"
  "wine-wow64=$pkgver"
)
conflicts=("wine")
source=("https://github.com/Kron4ek/Wine-Builds/releases/download/${pkgver}/wine-${pkgver}-staging-tkg-amd64-wow64.tar.xz")
sha256sums=('475be89ea7d97c06a794f095004b14a4f6e7e2bcc279ef7e65595c5c457da291')

package() {

  ## Create usr binary directory
  mkdir -p ${pkgdir}/usr

  ## Install wine package
  cp -rf ${srcdir}/wine-${pkgver}-staging-tkg-amd64-wow64/{bin,lib,share} ${pkgdir}/usr

}
