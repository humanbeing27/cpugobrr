pkgname=cpugobrr
pkgver=1
pkgrel=2
pkgdesc="A systemd service to switch to schedutil CPU frequency governor during boot." 
url="https://github.com/humanbeing27/cpugobrr"
arch=(any)
license=("GPLv3")
depends=("systemd"
         "cpupower")
source=("https://raw.githubusercontent.com/humanbeing27/$pkgname/main/cpugobrr",
"https://raw.githubusercontent.com/humanbeing27/$pkgname/main/cpugobrr.service"
)
b2sums=("SKIP"
        "SKIP")
package() {
mkdir $pkgdir/usr
mkdir $pkgdir/usr/bin
install -g root -o root cpugobrr $pkgdir/usr/bin/
chmod +x $pkgdir/usr/bin/cpugobrr
mkdir $pkgdir/etc
mkdir $pkgdir/etc/systemd
mkdir $pkgdir/etc/systemd/system
install -g root -o root cpugobrr.service $pkgdir/etc/systemd/system
echo "Please enable the service(cpugobrr.sevice) and restart."
}
