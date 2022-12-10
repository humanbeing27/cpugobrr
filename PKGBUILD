pkgname=cpugobrr
pkgver=1.1
pkgrel=1
pkgdesc="A systemd service to switch to schedutil CPU frequency governor during boot." 
url="https://github.com/humanbeing27/cpugobrr"
arch=(x86_64)
license=("GPLv3")
depends=(
        "systemd"
        "awk"
         "cpupower")
source=("https://raw.githubusercontent.com/humanbeing27/$pkgname/main/cpugobrr"
"https://raw.githubusercontent.com/humanbeing27/$pkgname/main/cpugobrr.service"
)
b2sums=("SKIP"
        "SKIP")
package() {
       mkdir -p $pkgdir/usr/bin
       install -g root -o root cpugobrr $pkgdir/usr/bin/
       chmod +x $pkgdir/usr/bin/cpugobrr
       mkdir -p $pkgdir/etc/systemd/system
       install -g root -o root cpugobrr.service $pkgdir/etc/systemd/system
}
