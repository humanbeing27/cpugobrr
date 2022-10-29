It's basically a systemd service to set Intel Perf Bias to Highest Performant Possible, Set Highest Possible Frequency from /sys directory and switch to schedutil CPU frequency governor during boot.

NOTE: It's only meant for Intel CPUs using **intel_cpufreq** driver.
# Installation
### Via Building
$ ``` curl -L https://raw.githubusercontent.com/humanbeing27/cpugobrr/main/PKGBUILD -o ./PKGBUILD ```

$ ``` makepkg -sircC ```
### Via Prebuilt package
The package is available in Releases. Download it and run the following command in directory of download :

#```pacman -U ./cpugobrr-1-2-x86_64.pkg.tar.zst ```
# Enabling the Service
#``` systemctl enable cpugobrr ```

Then Reboot after that.
