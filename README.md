It's basically a systemd service to set Intel Perf Bias to Highest Performant Possible, Set Highest Possible Frequency from /sys directory and switch to schedutil CPU frequency governor during boot.

NOTE: It's only meant for Intel CPUs using **intel_cpufreq** driver.
# Installation
### Via Building
```sh 
git clone https://github.com/humanbeing27/cpugobrr.git
cd cpugobrr
makepkg -sircCf
 ```
# Enabling the Service
```sh 
sudo systemctl enable cpugobrr 
```
Then Reboot after that.
