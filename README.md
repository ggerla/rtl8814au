# rtl8814AU
Realtek 8814AU USB WiFi driver.

Forked from [Zebulon2](https://github.com/ggerla/rtl8814au)'
repository which is based on version 4.3.21 of an Edimax driver for the
EW-7833UAC device.

Updated with support for kernels >= 4.14.
Enabled USB 3 by default
Enabled VHT functionalities

# DKMS support

From your src dir

````
sudo cp -R . /usr/src/rtl8814au-4.3.21
sudo dkms build -m rtl8814au -v 4.3.21
sudo dkms install -m rtl8814au -v 4.3.21
````

This should keep your 8814AU adapter working post kernel updates.
