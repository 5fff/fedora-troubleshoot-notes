# Fedora/Linux System Freezing issue caused by NVME Disconnected/Sleeps
## Solution: Disable Active-State Power Management by adding pcie_aspm kernel parameter
`sudo grubby --args=pcie_aspm.policy=performance --update-kernel=ALL`
### References:

https://www.crucial.com/support/articles-faq-ssd/ssd-disappears-or-crashes

https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/7/html/power_management_guide/aspm

https://docs.fedoraproject.org/en-US/Fedora/23/html/System_Administrators_Guide/sec-Configuring_GRUB_2_Using_the_grubby_Tool.html