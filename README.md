It's basically a systemd service to set Intel Perf Bias to Highest Performant Possible, Set Highest Possible Frequency from /sys directory and switch to Schedutil CPU frequency governor during boot.

NOTE: It's only meant for Intel CPUs using **intel_cpufreq** and **intel_pstate** driver.
# Installation
### Via Building
```sh 
git clone https://github.com/humanbeing27/cpugobrr.git
cd cpugobrr
makepkg -sircCf
 ```
 ### Via Prebuilt package
The package is available in Releases. Download it and run the following command in directory of download :
```sh
sudo pacman -U ./cpugobrr-1-2-x86_64.pkg.tar.zst 
```
# Enabling the Service
```sh 
sudo systemctl enable cpugobrr 
```
Then Reboot after that.
