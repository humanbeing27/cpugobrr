It's basically a systemd service to set Intel Perf Bias to Highest Performant Possible, Set Highest Possible Frequency from /sys directory and switch to schedutil CPU frequency governor during boot.

NOTE: It's only meant for Intel CPUs using **intel_cpufreq** driver
# Installation
## Get PKGBUILD
$ ``` curl -L https://raw.githubusercontent.com/humanbeing27/cpugobrr/main/PKGBUILD -o ./PKGBUILD ```
## Build and Install
$ ``` makepkg -sircC ```
# Enabling the Service
#``` systemctl enable cpugobrr ```

Then Reboot after that.
