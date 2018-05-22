# This is an example PKGBUILD file. Use this as a start to creating your own,
# and remove these comments. For more information, see 'man PKGBUILD'.
# NOTE: Please fill out the license field for your package! If it is unknown,
# then please put 'unknown'.

# Maintainer: Drew Noel <drewmnoel@gmail.com>

pkgname=git-find-md5
pkgver=1.0
pkgrel=1
url="https://gist.github.com/mloberg/3750653"
arch=("any")
license=('GPL')
depends=("git")
source=("https://gist.githubusercontent.com/mloberg/3750653/raw/6670f0d67bc6a4682543ab56df59e58e48f56583/gistfile1.sh"
    "0001-Suggested-Tweaks.patch")
md5sums=('b02421191c290080688736c07bbeb7fd'
         'eb5995f51c52b4bf35f2c594129eb2bf')

prepare() {
    cp gistfile1.sh git-find-md5
    patch -p0 < 0001-Suggested-Tweaks.patch
    chmod +x git-find-md5
}

package() {
    cd "$pkgdir"
    mkdir -p usr/bin/
    cp "$srcdir"/git-find-md5 usr/bin/
}
