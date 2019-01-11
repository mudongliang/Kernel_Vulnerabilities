We did statistics based on NVD Json Vulnerability Feed,
specifically, its json files contianing CVE information.
### Our Results
Compared to [CVE_Details](https://www.cvedetails.com/vendor/33/Linux.html)'s 
CVE Statistics on Linux from 2010-2018,
we found two more CVEs(CVE-2013-7445,CVE-2010-2946),
which are categorized by the website to be only related to Canonical's Ubuntu Linux but are still CVEs about Linux Kernel.
### One False Positive
We had one false positive due to NVD's mistake that CVE-2014-4611's product should be "lib/lz4" instead of Linux Kernel, which was corrected in the latest NVD database.
### Appendix
In our statistics, CVE_Details was set to filter all Linux-related CVEs, which introduced some cases not related to Linux Kernel.Specifically,their pruduct name can be "linux_kernel_ixgbe","linux_kernel-rt","kernel","systemd","util-linux"...