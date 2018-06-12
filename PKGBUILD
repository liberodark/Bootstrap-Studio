# Maintainer: liberodark

pkgname=bootstrap-studio
pkgver=4.0.0
pkgrel=1
pkgdesc="Google Drive GUI"
arch=('x86_64')
url="https://bootstrapstudio.io/"
license=('Custom')
depends=('xdg-utils')
source_x86_64=("https://bootstrapstudio.io/releases/desktop/4/Bootstrap%20Studio%204%20(64bit).deb")
source=($pkgname.desktop
        $pkgname.png)
sha512sums=('ed90f9399e90e848401adf65c77aac5b976787a81717103890d4af2e0afc8661d4a9d51e0b2a419f503879297f72e37e1a440063a6e6923bb20452064718822c'
         '83d3181496fb6c2d7e4f55f0a8eb195e2575def18d63851b1f8dbd3b9d84391f65bbac04cf2d226f9891c7a269f9367d859149780bf51927f54d45701d977cc9')
sha512sums_x86_64=('ddcfcf6e19de5e1a02931829f6f25982c9cabc6e3995cf133f2fbceaef9736b8ce88af234029ea46a59fa46e886887f2489347778ae71d475edee3c1704a475d')
        
package() {
  cd $srcdir
  tar xvf data.tar.xz
  cp -r opt $pkgdir
  install -vDm644 $srcdir/$pkgname.desktop $pkgdir/usr/share/applications/$pkgname.desktop
  install -vDm644 $srcdir/$pkgname.png $pkgdir/usr/share/pixmaps/$pkgname.png
}

