pkgname=luajit
pkgver=2.0.4
pkgrel=2
pkgdesc='Just-in-time compiler and drop-in replacement for Lua 5.1'
arch=('x86_64')
url='http://luajit.org/'
license=('MIT')
depends=('gcc-libs')
source=("http://luajit.org/download/LuaJIT-$pkgver.tar.gz")
md5sums=('dd9c38307f2223a504cbfb96e477eca0')

build() {
  cd "LuaJIT-$pkgver"
  make amalg PREFIX=/usr
}

package() {
  cd "LuaJIT-$pkgver"

  make install DESTDIR="$pkgdir" PREFIX=/usr
  
}
