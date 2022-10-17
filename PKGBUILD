pkgname=cpusdg
pkgver=1
pkgrel=2
pkgdesc="A systemd service to switch to schedutil CPU frequency governor during boot." 
url="https://github.com/humanbeing27/cpusdg"
arch=(any)
license=("GPLv3")
depends=("systemd"
         "cpupower")
provides=("cpugobrr")
conflicts=("cpugobrr")
replaces=("cpugobrr")
source=("https://raw.githubusercontent.com/humanbeing27/$pkgname/main/cpusdg",
"https://raw.githubusercontent.com/humanbeing27/$pkgname/main/cpusdg.service"
)
b2sums=("SKIP"
        "SKIP")
package() {
mkdir $pkgdir/usr
mkdir $pkgdir/usr/bin
install -g root -o root cpusdg $pkgdir/usr/bin/
chmod +x $pkgdir/usr/bin/cpusdg
mkdir $pkgdir/etc
mkdir $pkgdir/etc/systemd
mkdir $pkgdir/etc/systemd/system
install -g root -o root cpusdg.service $pkgdir/etc/systemd/system
echo "Please enable the service and restart."
}
