# EW-7833UAC (Edimax ac1750) Linux 4.10 Driver Build and Install Notes

Edimax [ac1750](http://www.edimax.com/edimax/merchandise/merchandise_detail/data/edimax/global/wireless_adapters_ac1750_dual-band/ew-7833uac/)
(also known as EW-7833UAC) is a dual-band (2.4 GHz, 5 GHz) wifi,
usb 3.0 adapter with a 180-degree adjustable antenna.
The linux kernel module (driver) is called `8814au`.
The device id numbers is 0x7392:0xa833.

The driver provided by the manufacturer
[`EW7833UAC_linux_v4.3.21_17997.20160531.zip`](http://www.edimax.us/download/drivers/Linux/EW7833UAC_linux_v4.3.21_17997.20160531.zip)
does not compile in newer Linux kernels (4.10). Admittedly, the
manufacturer states the driver works for kernels 3.16 to 4.4.

This repo contains the original code, and a patch that makes it compile
against 4.10.
