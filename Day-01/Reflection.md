Day 01 - Reflection

What did you learn today?
Today was focused on setting up my virtual lab environment before diving into Blue Team theory. I learned that Windows 11 has strict hardware requirements even inside a virtual machine — specifically TPM 2.0 and a minimum of 4 GB RAM — and that VirtualBox needs to be configured carefully to satisfy these checks. I also learned the theoretical side: what a SOC is, how SIEM tools collect and correlate logs, how Blue Team and Red Team roles differ, and why virtual machines matter for isolation and safe testing in cybersecurity — which felt directly relevant given the VM issues I was fighting at the same time.

What challenges did you face?
The biggest challenge today was actually getting Windows 11 installed inside VirtualBox. The installation kept getting stuck — the screen would go blank right around the 50% mark, leaving me with no option but to force-shut-down the VM. This happened multiple times across multiple deployment attempts, not just once. Before reaching that point, I was also getting an unexpected boot menu screen that didn't match any of the YouTube tutorials I referenced, which made troubleshooting harder since none of the videos showed the same behavior I was seeing. I tried disabling the Hyper-V hypervisor through PowerShell (running as Administrator) since some guides suggested this fixes VirtualBox/Windows 11 conflicts, but even that didn't resolve it the way it did in the videos. I ended up trying several other combinations of settings — adjusting RAM allocation, TPM settings, and VM configuration — but was still unable to get a fully completed installation by the end of the day.

Which concepts were completely new?
The requirement for TPM 2.0 inside a virtual machine was new to me — I hadn't realized Windows 11 enforces this even in a virtualized setting, not just on physical hardware. I also hadn't previously dealt with the Hyper-V vs. VirtualBox conflict, where Windows' built-in hypervisor can interfere with third-party virtualization software at the hypervisor level, sometimes requiring it to be explicitly disabled.

How can you improve tomorrow?

