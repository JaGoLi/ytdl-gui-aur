# Maintainer: Jason Goulet-Lipman <jason.gouletlipman@gmail.com>

pkgname=youtubedl-gui
pkgver=2.0
pkgrel=1
pkgdesc="Download Youtube videos to local audio or video files."
arch=('x86_64')
url="https://github.com/JaGoLi/ytdl-gui"
license=('GPL3')
depends=(youtube-dl qt5-base ffmpeg)
makedepends=(qt5-quickcontrols)
source=("$pkgname-$pkgver.tar.gz::https://github.com/JaGoLi/ytdl-gui/archive/$pkgver.tar.gz")
sha256sums=('59c60fc76344f8ef218fdda71818c6ec045e19964be507f265223db0b7f08b4e')

build() {
	cd "ytdl-gui-${pkgver}"
	make build
}

package() {
	cd "ytdl-gui-${pkgver}"
	make DESTDIR="${pkgdir}/" install
}
