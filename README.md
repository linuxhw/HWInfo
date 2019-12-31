Devices with bad Linux-compatibility
====================================

This is a project to find PCI/USB devices with bad Linux-compatibility based on the [hwinfo](https://github.com/openSUSE/hwinfo)
reports collected by Linux users at https://linux-hardware.org.

In the scope of this project, the device is considered badly supported by Linux if driver
is not found for this device in at least one user probe on any Linux distribution.

You can find appropriate hwinfo report in this repository by a probe ID as follows:

    find . -name {PROBE ID}

Everyone can contribute to this repository by uploading probes of their computers
by the [hw-probe](https://github.com/linuxhw/hw-probe) tool:

    sudo hw-probe -all -upload

Total reports: 65980.

Contents
--------

1. [ About ](#about)
2. [ PCI Devices ](#pci-devices)
   * [ Bluetooth ](#bluetooth-pci)
   * [ Card reader ](#card-reader-pci)
   * [ Communication controller ](#communication-controller-pci)
   * [ Firewire controller ](#firewire-controller-pci)
   * [ Flash memory ](#flash-memory-pci)
   * [ Graphics card ](#graphics-card-pci)
   * [ Modem ](#modem-pci)
   * [ Multimedia controller ](#multimedia-controller-pci)
   * [ Net/ethernet ](#netethernet-pci)
   * [ Net/wireless ](#netwireless-pci)
   * [ Network ](#network-pci)
   * [ Sd host controller ](#sd-host-controller-pci)
   * [ Sound ](#sound-pci)
   * [ Storage ](#storage-pci)
   * [ Storage/ata ](#storageata-pci)
   * [ Storage/raid ](#storageraid-pci)
   * [ System peripheral ](#system-peripheral-pci)
   * [ Tv card ](#tv-card-pci)
   * [ Usb controller ](#usb-controller-pci)
3. [ USB Devices ](#usb-devices)
   * [ Audio ](#audio-usb)
   * [ Bluetooth ](#bluetooth-usb)
   * [ Camera ](#camera-usb)
   * [ Card reader ](#card-reader-usb)
   * [ Chipcard ](#chipcard-usb)
   * [ Converter ](#converter-usb)
   * [ Disk ](#disk-usb)
   * [ Dvb card ](#dvb-card-usb)
   * [ Fingerprint reader ](#fingerprint-reader-usb)
   * [ Hardware key ](#hardware-key-usb)
   * [ Hasp ](#hasp-usb)
   * [ Hub ](#hub-usb)
   * [ Human interface ](#human-interface-usb)
   * [ Imaging ](#imaging-usb)
   * [ Input/keyboard ](#inputkeyboard-usb)
   * [ Input/mouse ](#inputmouse-usb)
   * [ Modem ](#modem-usb)
   * [ Net/wimax ](#netwimax-usb)
   * [ Net/wireless ](#netwireless-usb)
   * [ Network ](#network-usb)
   * [ Sound ](#sound-usb)
   * [ Tv card ](#tv-card-usb)
   * [ Ups ](#ups-usb)
   * [ Video ](#video-usb)
   * [ Wireless ](#wireless-usb)

About
-----

The structure of the repository is the following:

    {COMPUTER TYPE}/{VENDOR}/{MODEL PREFIX}/{MODEL}/{HWID}/{OS}/{KERNEL}/{ARCH}/{PROBE ID}

    ( e.g. Notebook/Dell/XPS/XPS L421X/D7DA07727B83/ROSA-2014.1/3.14.22-NRJ-LAPTOP-3ROSA/X86_64/F74F6103A1 )

PCI Devices
-----------

Non-100% value in the 'Missed' column indicates that the driver for a device is available
in the latest kernel versions. You can find corresponding hwinfo reports for listed devices
by a probe ID.

Missed — percentage of probes with missed driver for the device,
Linux  — the minimum Linux kernel version in which the driver was found,
Probe  — latest probe ID with missed driver for the device.

### Bluetooth (PCI)

9 out of 9 (100%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1814:3298 | 103c:18ec | Ralink          | RT3290 Bluetooth         | 99%    | 4.18.0   | 96C288C457 |
| 1814:3298 | 103c:191c | Ralink          | RT3290 Bluetooth         | 100%   |          | B6260EAFCE |
| 1814:3298 | 105b:e056 | Ralink          | RT3290 Bluetooth         | 99.2%  | 5.3.12   | 12F5A59D53 |
| 1814:3298 | 10cf:1772 | Ralink          | RT3290 Bluetooth         | 100%   |          | 1135E21142 |
| 1814:3298 | 1814:3298 | Ralink          | RT3290 Bluetooth         | 100%   |          | EF1E6295A8 |
| 1814:3298 | 1a3b:210b | Ralink          | RT3290 Bluetooth         | 100%   |          | 2333E930AF |
| 1814:3298 | 1a3b:2787 | Ralink          | RT3290 Bluetooth         | 100%   |          | 375A7150DE |
| 1814:3298 | 1a3b:2987 | Ralink          | RT3290 Bluetooth         | 100%   |          | 1F5B5C1D86 |
| 1814:3298 | 1a3b:2f87 | Ralink          | RT3290 Bluetooth         | 100%   |          | F65DC130D7 |

### Card reader (PCI)

26 out of 800 (3.25%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 10ec:5227 | 1179:0001 | Realtek Semi... | RTS5227 PCI Express C... | 7.1%   | 4.15.0   | 550460AAAC |
| 10ec:5227 | 1462:10f4 | Realtek Semi... | RTS5227 PCI Express C... | 100%   |          | 852662BDF3 |
| 10ec:5227 | 17aa:220c | Realtek Semi... | RTS5227 PCI Express C... | 1.8%   | 4.1.15   | 54B33D56BB |
| 10ec:5229 | 10ec:5229 | Realtek Semi... | RTS5229 PCI Express C... | 1.5%   | 3.10.51  | 13AB4D878D |
| 10ec:522a | 103c:806e | Realtek Semi... | RTS522A PCI Express C... | 100%   |          | 62A9EF950E |
| 10ec:522a | 103c:8079 | Realtek Semi... | RTS522A PCI Express C... | 11.1%  | 4.4.1    | 15E62C605F |
| 10ec:522a | 103c:80a4 | Realtek Semi... | RTS522A PCI Express C... | 33.3%  | 4.9.60   | B01FB51118 |
| 10ec:522a | 103c:80ff | Realtek Semi... | RTS522A PCI Express C... | 54.5%  | 4.7.2    | B7B039F46E |
| 10ec:522a | 103c:8100 | Realtek Semi... | RTS522A PCI Express C... | 100%   |          | 2B56F34E21 |
| 10ec:522a | 103c:8101 | Realtek Semi... | RTS522A PCI Express C... | 16%    | 4.9.60   | BC496704F4 |
| 10ec:522a | 103c:820c | Realtek Semi... | RTS522A PCI Express C... | 25%    | 4.9.20   | FAE1CD27F3 |
| 10ec:522a | 103c:8392 | Realtek Semi... | RTS522A PCI Express C... | 66.7%  | 4.9.20   | 142D7492C2 |
| 10ec:522a | 103c:84db | Realtek Semi... | RTS522A PCI Express C... | 33.3%  | 4.15.0   | 06EE78EE4D |
| 10ec:522a | 17aa:5048 | Realtek Semi... | RTS522A PCI Express C... | 25%    | 4.15.0   | A549AED5B4 |
| 10ec:522a | 17aa:5113 | Realtek Semi... | RTS522A PCI Express C... | 20%    | 4.15.0   | 32F7318757 |
| 10ec:525a | 1028:079f | Realtek Semi... | RTS525A PCI Express C... | 11.8%  | 4.15.0   | F6081D54B1 |
| 10ec:525a | 1028:081b | Realtek Semi... | RTS525A PCI Express C... | 12.5%  | 3.10.0   | 05CDC89A9D |
| 10ec:525a | 103c:860f | Realtek Semi... | RTS525A PCI Express C... | 100%   |          | BDD15B19B1 |
| 10ec:5287 | 1025:0866 | Realtek Semi... | RTL8411B PCI Express ... | 4.8%   | 3.14.25  | 0583AEE10F |
| 10ec:5287 | 1558:6509 | Realtek Semi... | RTL8411B PCI Express ... | 100%   |          | 13AB4D878D |
| 10ec:5289 | 1025:0724 | Realtek Semi... | RTL8411 PCI Express C... | 3.4%   | 3.14.53  | 6A087DD575 |
| 10ec:5289 | 1043:1447 | Realtek Semi... | RTL8411 PCI Express C... | 6.2%   | 3.14.44  | F23B5BF0DA |
| 1aea:6601 | 0001:0001 | Alcor Micro     | AU6601 PCI-E Flash ca... | 60%    | 4.9.0    | 740C1D3CBF |
| 1aea:6601 | 1179:f900 | Alcor Micro     | AU6601 PCI-E Flash ca... | 50%    | 5.0.0    | 43A9D7922A |
| 1aea:6621 | 1aea:6621 | Alcor Micro     | Alcor Micro PCIe Card... | 73.3%  | 5.0.0    | 8BD52CD8F7 |
| 1aea:6625 | 103c:83a9 | Alcor Micro     | Alcor Micro PCIe Card... | 100%   |          | E44D4D3221 |

### Communication controller (PCI)

275 out of 2856 (9.63%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 04f1:2f20 | 04f1:200c |                 | Communication controller | 100%   |          | 6759172767 |
| 104c:8035 | 103c:0934 | Texas Instru... | PCIxx21/PCIxx11 Smart... | 100%   |          | 16F00AAE37 |
| 104c:8035 | 103c:0944 | Texas Instru... | PCIxx21/PCIxx11 Smart... | 100%   |          | A770CF025E |
| 104c:8035 | 103c:099c | Texas Instru... | PCIxx21/PCIxx11 Smart... | 100%   |          | AFE75774F3 |
| 104c:8038 | 1028:0182 | Texas Instru... | PCI6515 SmartCard Con... | 100%   |          | 0077E52877 |
| 104c:8038 | 1028:0186 | Texas Instru... | PCI6515 SmartCard Con... | 100%   |          | DEEA511BCD |
| 104c:8038 | 1028:0187 | Texas Instru... | PCI6515 SmartCard Con... | 100%   |          | 358447EB4E |
| 104c:803d | 103c:309f | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | 5BE41E5F47 |
| 104c:803d | 103c:30a3 | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | B38A821821 |
| 104c:803d | 103c:30aa | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | 9C1BF7D811 |
| 104c:803d | 103c:30ac | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | 3604EF7ED6 |
| 104c:803d | 103c:30ad | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | 9F51D8D813 |
| 104c:803d | 103c:30b1 | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | 25DD8AF3EE |
| 104c:803d | 1071:8212 | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | 01F778FE4E |
| 1093:c801 |           | National Ins... | PCI-GPIB                 | 100%   |          | 29A0FC6CE0 |
| 11c1:0480 | 1668:0500 | LSI             | Venus Modem (V90, 56K... | 25%    | 3.14.22  | 0A61436F40 |
| 11c1:048c | 11c1:044c | LSI             | V.92 56K WinModem        | 100%   |          | 4ED412D115 |
| 11c1:0620 | 11c1:0620 | LSI             | Lucent V.92 Data/Fax ... | 100%   |          | 56F0C1E96B |
| 11c1:0630 | 11c1:0630 | LSI             | PCI-SV92EX Soft Modem    | 100%   |          | 961F173B92 |
| 11c1:0630 | 11c1:0631 | LSI             | PCI-SV92EX Soft Modem    | 100%   |          | A496E46CB4 |
| 125d:2838 | 125d:2838 | ESS Technology  | ES2838/2839 SuperLink... | 100%   |          | 5E6A0F1B7E |
| 127a:2015 | 127a:2015 | Rockwell Int... | HSF 56k Data/Fax/Voic... | 100%   |          | 55EC1147BA |
| 13f6:0211 | 13f6:0211 | C-Media Elec... | CM8738                   | 100%   |          | 61730F8246 |
| 14f1:1033 | 13e0:020d | Conexant Sys... | HCF 56k Data/Fax Modem   | 100%   |          | 87F8B4B22A |
| 14f1:1035 | 148d:1035 | Conexant Sys... | HCF 56k Data/Fax/Voic... | 100%   |          | 36CC45E684 |
| 14f1:10b6 | 14f1:10b6 | Conexant Sys... | CX06834-11 HCF V.92 5... | 100%   |          | 151D253025 |
| 14f1:2013 | 13e0:0212 | Conexant Sys... | HSF 56k Data/Fax Modem   | 100%   |          | 3ED411EF5C |
| 14f1:2014 | 14f1:2014 | Conexant Sys... | HSF 56k Data/Fax/Voic... | 100%   |          | 445429C65F |
| 14f1:2702 | 1028:8d88 | Conexant Sys... | HSFi modem RD01-D270     | 100%   |          | F11822D259 |
| 14f1:2702 | 14f1:2007 | Conexant Sys... | HSFi modem RD01-D270     | 100%   |          | 83629CDF01 |
| 14f1:2f00 | 122d:8d88 | Conexant Sys... | HSF 56k HSFi Modem       | 100%   |          | E29EC46FD7 |
| 14f1:2f00 | 14f1:2002 | Conexant Sys... | HSF 56k HSFi Modem       | 100%   |          | 6D6FC71CEB |
| 14f1:2f00 | 14f1:2003 | Conexant Sys... | HSF 56k HSFi Modem       | 100%   |          | AF474622B9 |
| 14f1:2f00 | 14f1:2004 | Conexant Sys... | HSF 56k HSFi Modem       | 100%   |          | 1A7E23374F |
| 14f1:2f00 | 187e:3409 | Conexant Sys... | HSF 56k HSFi Modem       | 100%   |          | C1BD1568DC |
| 14f1:2f02 | 1767:000b | Conexant Sys... | HSF 56k HSFi Data/Fax    | 100%   |          | DFC83A3DB4 |
| 14f1:2f12 | 16ec:2016 | Conexant Sys... | HSF Data/Fax/Voice (USA) | 100%   |          | 3ADDAB1A1D |
| 14f1:2f20 | 14f1:200c | Conexant Sys... | HSF 56k Data/Fax Modem   | 100%   |          | 32F7F650B9 |
| 14f1:2f20 | 14f1:200f | Conexant Sys... | HSF 56k Data/Fax Modem   | 100%   |          | A309FDA4F4 |
| 14f1:2f20 | 14f1:2014 | Conexant Sys... | HSF 56k Data/Fax Modem   | 100%   |          | 585D8319DA |
| 14f1:2f30 | 14f1:200f | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | 6126EB96B3 |
| 14f1:2f30 | 14f1:2014 | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | 1930575F3E |
| 14f1:2f30 | 14f1:2051 | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | AB7A62E5F5 |
| 14f1:2f30 | 14f1:2075 | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | BBF84F3432 |
| 14f1:2f30 | 14f1:20d5 | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | 7DA787439E |
| 14f1:2f40 | 14f1:2000 | Conexant Sys... | PCI CX11261 Soft Modem   | 100%   |          | 425DC02AFD |
| 14f1:2f50 | 14f1:207c | Conexant Sys... | Conexant SoftK56 Data... | 100%   |          | DE599FD63C |
| 14f1:2f81 | 14f1:0000 | Conexant Sys... | PCIe CX95610 Soft Modem  | 100%   |          | B48AA8562A |
| 14f1:2f82 | 14f1:0000 | Conexant Sys... | PCIe CX95610 Soft Modem  | 100%   |          | 039AFB9C35 |
| 1fd4:1999 | 1fd4:0101 | SUNIX           | Multiport serial cont... | 100%   |          | 4415A64795 |
| 5372:6870 | 1000:0010 |                 | Communication controller | 100%   |          | 2C1DD09A17 |
| 8086:02e0 | 1028:0950 | Intel           | Comet Lake Management... | 100%   |          | 20ABB6DE72 |
| 8086:02e0 | 1028:0954 | Intel           | Comet Lake Management... | 100%   |          | 8740133E10 |
| 8086:02e0 | 103c:866e | Intel           | Comet Lake Management... | 100%   |          | 8FF42ABD82 |
| 8086:02e0 | 1043:1c71 | Intel           | Comet Lake Management... | 100%   |          | 4EA8D503AE |
| 8086:02e0 | 1558:1404 | Intel           | Comet Lake Management... | 100%   |          | 24222EF94C |
| 8086:02e0 | 17aa:3806 | Intel           | Comet Lake Management... | 50%    | 5.3.0    | DFE8A137BA |
| 8086:02e0 | 1d72:1901 | Intel           | Comet Lake Management... | 100%   |          | 4D4D89C508 |
| 8086:06e0 | 8086:7270 | Intel           | 400 Series Chipset Fa... | 100%   |          | 9BFAB5575C |
| 8086:0801 | 8086:0801 | Intel           | Moorestown SPI Ctrl 1    | 100%   |          | D1874B6708 |
| 8086:0802 | 8086:0802 | Intel           | Moorestown I2C 0         | 100%   |          | D1874B6708 |
| 8086:0803 | 8086:0803 | Intel           | Moorestown I2C 1         | 100%   |          | D1874B6708 |
| 8086:0804 | 8086:0804 | Intel           | Moorestown I2C 2         | 100%   |          | D1874B6708 |
| 8086:19d3 | 8086:19d3 | Intel           | Atom Processor C3000 ... | 100%   |          | 50B6A72C0C |
| 8086:1c3a | 1025:0504 | Intel           | 6 Series/C200 Series ... | 0.7%   | 3.14.25  | 8FE3AF49FB |
| 8086:1c3a | 1043:11d7 | Intel           | 6 Series/C200 Series ... | 3.8%   | 3.10.34  | A5A0DA657B |
| 8086:1c3a | 1043:844d | Intel           | 6 Series/C200 Series ... | 0.2%   | 3.0.38   | BED9B97265 |
| 8086:1c3a | 17aa:3975 | Intel           | 6 Series/C200 Series ... | 0.6%   | 3.10.34  | 2239D316E8 |
| 8086:1c3a | 8086:7270 | Intel           | 6 Series/C200 Series ... | 1.2%   | 3.14.22  | D5C9D589F2 |
| 8086:1d3a | 1028:05d2 | Intel           | C600/X79 series chips... | 6.7%   | 4.15.0   | 949DD823D7 |
| 8086:1d3a | 15d9:0628 | Intel           | C600/X79 series chips... | 50%    | 3.10.0   | 99E743CA9E |
| 8086:1d3a | 15d9:0636 | Intel           | C600/X79 series chips... | 100%   |          | 53FB02A9EF |
| 8086:1d3a | 15d9:0709 | Intel           | C600/X79 series chips... | 100%   |          | 9F3D443A21 |
| 8086:1d3b | 1028:048c | Intel           | C600/X79 series chips... | 100%   |          | 6756F6E03F |
| 8086:1d3b | 1028:04ce | Intel           | C600/X79 series chips... | 100%   |          | D1FAA99D53 |
| 8086:1d3b | 1028:04f7 | Intel           | C600/X79 series chips... | 100%   |          | 6839F6245C |
| 8086:1d3b | 1028:04f8 | Intel           | C600/X79 series chips... | 100%   |          | E8BE4F8032 |
| 8086:1d3b | 1028:0528 | Intel           | C600/X79 series chips... | 100%   |          | 5A372D2A35 |
| 8086:1d3b | 1043:84ef | Intel           | C600/X79 series chips... | 100%   |          | 996F55BB36 |
| 8086:1d3b | 15d9:0628 | Intel           | C600/X79 series chips... | 100%   |          | F7519BF7BE |
| 8086:1d3b | 15d9:062c | Intel           | C600/X79 series chips... | 100%   |          | 2B1034E588 |
| 8086:1d3b | 15d9:0636 | Intel           | C600/X79 series chips... | 100%   |          | 53FB02A9EF |
| 8086:1d3b | 15d9:0665 | Intel           | C600/X79 series chips... | 100%   |          | CEC82EF5D0 |
| 8086:1d3b | 15d9:0702 | Intel           | C600/X79 series chips... | 100%   |          | 376BED560D |
| 8086:1d3b | 15d9:0703 | Intel           | C600/X79 series chips... | 100%   |          | 8C793BB137 |
| 8086:1d3b | 15d9:0705 | Intel           | C600/X79 series chips... | 100%   |          | B3D08DD227 |
| 8086:1d3b | 15d9:0709 | Intel           | C600/X79 series chips... | 100%   |          | 9F3D443A21 |
| 8086:1d3b | 15d9:070a | Intel           | C600/X79 series chips... | 100%   |          | B4C8ABC585 |
| 8086:1d3b | 1849:1d3b | Intel           | C600/X79 series chips... | 100%   |          | 2021C0A4A3 |
| 8086:1d3b | 8086:1d3b | Intel           | C600/X79 series chips... | 100%   |          | AA487A5EDB |
| 8086:1d3b | 8086:357e | Intel           | C600/X79 series chips... | 100%   |          | F65EC09250 |
| 8086:1e3a | 1019:99f2 | Intel           | 7 Series/C216 Chipset... | 66.7%  | 5.0.0    | 45F3B356CF |
| 8086:1e3a | 1025:0647 | Intel           | 7 Series/C216 Chipset... | 0.8%   | 3.10.34  | 86D2D3B0E1 |
| 8086:1e3a | 1025:0724 | Intel           | 7 Series/C216 Chipset... | 25%    | 4.1.16   | 6A087DD575 |
| 8086:1e3a | 1025:074f | Intel           | 7 Series/C216 Chipset... | 100%   |          | 6566319F04 |
| 8086:1e3a | 1028:052c | Intel           | 7 Series/C216 Chipset... | 14.3%  | 4.15.0   | 779B6B3344 |
| 8086:1e3a | 1028:058b | Intel           | 7 Series/C216 Chipset... | 100%   |          | 42A50DEDAB |
| 8086:1e3a | 1043:1447 | Intel           | 7 Series/C216 Chipset... | 8.3%   | 3.14.44  | F23B5BF0DA |
| 8086:1e3a | 1043:1477 | Intel           | 7 Series/C216 Chipset... | 1.7%   | 3.14.15  | 731932629B |
| 8086:1e3a | 1043:84ca | Intel           | 7 Series/C216 Chipset... | 1.8%   | 3.10.34  | C7C6CD6D36 |
| 8086:1e3a | 1179:fb41 | Intel           | 7 Series/C216 Chipset... | 3.6%   | 3.10.42  | 67009EFFAA |
| 8086:1e3a | 1458:1c3a | Intel           | 7 Series/C216 Chipset... | 0.1%   | 3.10.0   | A644A3A3AD |
| 8086:1e3a | 17aa:21f9 | Intel           | 7 Series/C216 Chipset... | 12.5%  | 3.14.15  | B7014678B5 |
| 8086:1e3a | 17aa:21fa | Intel           | 7 Series/C216 Chipset... | 1%     | 3.10.42  | CEFD5E879B |
| 8086:1e3a | 17aa:3083 | Intel           | 7 Series/C216 Chipset... | 25%    | 4.9.111  | E3BF127788 |
| 8086:1e3a | 17aa:3977 | Intel           | 7 Series/C216 Chipset... | 0.3%   | 3.10.42  | 2DD89E3983 |
| 8086:1e3a | 1849:1e3a | Intel           | 7 Series/C216 Chipset... | 0.7%   | 3.10.0   | 8505F4654F |
| 8086:1e3a | 8086:1e3a | Intel           | 7 Series/C216 Chipset... | 6.2%   | 3.10.34  | CE8124E5F4 |
| 8086:29d4 | 103c:281e | Intel           | 82Q33 Express MEI Con... | 2.2%   | 3.14.44  | 13EF653132 |
| 8086:2e14 | 103c:3034 | Intel           | 4 Series Chipset HECI... | 4.8%   | 3.14.44  | A40772FC80 |
| 8086:2e14 | 103c:3048 | Intel           | 4 Series Chipset HECI... | 1.8%   | 3.10.34  | 90437162AD |
| 8086:2e14 | 8086:1003 | Intel           | 4 Series Chipset HECI... | 14.3%  | 4.4.0    | 53C6C139DA |
| 8086:2e44 | 8086:0025 | Intel           | 4 Series Chipset HECI... | 100%   |          | 8C4EFA23E2 |
| 8086:319a | 1043:1181 | Intel           | Celeron/Pentium Silve... | 17.4%  | 4.15.0   | 76D01F63C2 |
| 8086:319a | 1043:1df0 | Intel           | Celeron/Pentium Silve... | 100%   |          | 5D4E6E95F1 |
| 8086:319a | 1043:1eb0 | Intel           | Celeron/Pentium Silve... | 16.7%  | 4.15.0   | 00EECF27F3 |
| 8086:34e0 | 1028:0979 | Intel           | Management Engine Int... | 22.2%  | 5.0.0    | 7F4CE08DF9 |
| 8086:34e0 | 1028:097c | Intel           | Management Engine Int... | 20%    | 5.0.0    | 90B19AF55F |
| 8086:3b64 | 103c:3674 | Intel           | 5 Series/3400 Series ... | 16.7%  | 4.15.0   | F4DE983D96 |
| 8086:3b64 | 1043:1c77 | Intel           | 5 Series/3400 Series ... | 0.7%   | 3.14.25  | 7FDEE4E7BB |
| 8086:3b64 | 105b:0dd5 | Intel           | 5 Series/3400 Series ... | 20%    | 4.1.25   | 6B384CAEA8 |
| 8086:5a9a | 1849:5a9a | Intel           | Celeron N3350/Pentium... | 5.6%   | 4.9.14   | 633A8B8ADF |
| 8086:5a9a | 8086:7270 | Intel           | Celeron N3350/Pentium... | 0.9%   | 4.4.0    | 8ADD68C95A |
| 8086:5a9c | 1025:1084 | Intel           | Communication controller | 100%   |          | EB24B13C29 |
| 8086:5a9c | 1028:075f | Intel           | Communication controller | 100%   |          | 3D61CAE371 |
| 8086:5a9c | 1043:8738 | Intel           | Communication controller | 100%   |          | 82BDD3F39F |
| 8086:5a9c | 17aa:3802 | Intel           | Communication controller | 100%   |          | B02B76DC46 |
| 8086:5a9c | 17aa:3803 | Intel           | Communication controller | 100%   |          | F8913A087C |
| 8086:5a9c | 17aa:3809 | Intel           | Communication controller | 100%   |          | 2CE172A9F5 |
| 8086:5a9c | 8086:7270 | Intel           | Communication controller | 100%   |          | DFF4987122 |
| 8086:5a9e | 1025:1084 | Intel           | Communication controller | 100%   |          | EB24B13C29 |
| 8086:5a9e | 1028:075f | Intel           | Communication controller | 100%   |          | 3D61CAE371 |
| 8086:5a9e | 1043:8738 | Intel           | Communication controller | 100%   |          | 82BDD3F39F |
| 8086:5a9e | 17aa:3802 | Intel           | Communication controller | 100%   |          | B02B76DC46 |
| 8086:5a9e | 17aa:3803 | Intel           | Communication controller | 100%   |          | F8913A087C |
| 8086:5a9e | 17aa:380a | Intel           | Communication controller | 100%   |          | 2CE172A9F5 |
| 8086:5a9e | 8086:7270 | Intel           | Communication controller | 100%   |          | DFF4987122 |
| 8086:8c3a | 1028:0620 | Intel           | 8 Series/C220 Series ... | 33.3%  | 5.3.0    | F801FAB1AD |
| 8086:8c3a | 1028:0623 | Intel           | 8 Series/C220 Series ... | 100%   |          | 29D0AD2441 |
| 8086:8c3a | 1043:8534 | Intel           | 8 Series/C220 Series ... | 0.1%   | 3.14.25  | 4712036FF4 |
| 8086:8c3a | 1458:1c3a | Intel           | 8 Series/C220 Series ... | 0.2%   | 3.10.0   | E996F15E3E |
| 8086:8c3a | 1462:7816 | Intel           | 8 Series/C220 Series ... | 5.6%   | 3.14.33  | 093472BA51 |
| 8086:8c3a | 1462:7823 | Intel           | 8 Series/C220 Series ... | 23.1%  | 3.14.25  | 4C0C5DE2E6 |
| 8086:8c3a | 15d9:0921 | Intel           | 8 Series/C220 Series ... | 50%    | 4.15.0   | DB25C87154 |
| 8086:8c3a | 17aa:3978 | Intel           | 8 Series/C220 Series ... | 2.7%   | 3.14.44  | 825E182B0C |
| 8086:8c3a | 1849:8c3a | Intel           | 8 Series/C220 Series ... | 0.5%   | 3.10.0   | 5A36CE2620 |
| 8086:8c3a | 8086:204a | Intel           | 8 Series/C220 Series ... | 12.5%  | 4.1.25   | 8C48173C7B |
| 8086:8c3b | 1025:0790 | Intel           | 8 Series/C220 Series ... | 100%   |          | CD73F91550 |
| 8086:8c3b | 15d9:0921 | Intel           | 8 Series/C220 Series ... | 100%   |          | 5315690568 |
| 8086:8c3b | 1849:8c3b | Intel           | 8 Series/C220 Series ... | 100%   |          | 9E52EE363E |
| 8086:8c3b | 8086:7270 | Intel           | 8 Series/C220 Series ... | 100%   |          | 06197CCB84 |
| 8086:8cba | 1043:8534 | Intel           | 9 Series Chipset Fami... | 1.3%   | 3.14.25  | 68DBF33470 |
| 8086:8cba | 1458:1c3a | Intel           | 9 Series Chipset Fami... | 0.7%   | 3.14.22  | 5A77B72FE5 |
| 8086:8d3a | 1043:8600 | Intel           | C610/X99 series chips... | 4.1%   | 4.1.25   | A16A7137A3 |
| 8086:8d3a | 1458:7270 | Intel           | C610/X99 series chips... | 6.2%   | 4.1.15   | AF58D23265 |
| 8086:8d3a | 15d9:0831 | Intel           | C610/X99 series chips... | 16.7%  | 3.10.0   | 52D5275C7F |
| 8086:8d3a | 15d9:0852 | Intel           | C610/X99 series chips... | 100%   |          | 2E6D79F345 |
| 8086:8d3a | 19e5:2061 | Intel           | C610/X99 series chips... | 100%   |          | 5EB4DFC951 |
| 8086:8d3a | 8086:35c5 | Intel           | C610/X99 series chips... | 100%   |          | 08100751B7 |
| 8086:8d3a | 8086:35c9 | Intel           | C610/X99 series chips... | 100%   |          | 5F9F099F36 |
| 8086:8d3a | 8086:7270 | Intel           | C610/X99 series chips... | 33.3%  | 4.4.0    | 0F42B6C827 |
| 8086:8d3b | 1028:0601 | Intel           | C610/X99 series chips... | 100%   |          | AF9F6ACE3F |
| 8086:8d3b | 1028:0639 | Intel           | C610/X99 series chips... | 100%   |          | 3BA1B5FC84 |
| 8086:8d3b | 1028:063a | Intel           | C610/X99 series chips... | 100%   |          | FF3ACF2BDC |
| 8086:8d3b | 1043:85f6 | Intel           | C610/X99 series chips... | 100%   |          | 7436C74DCB |
| 8086:8d3b | 1458:1000 | Intel           | C610/X99 series chips... | 100%   |          | 9C8A2165C3 |
| 8086:8d3b | 15d9:0821 | Intel           | C610/X99 series chips... | 100%   |          | 17BF7A3CBC |
| 8086:8d3b | 15d9:0824 | Intel           | C610/X99 series chips... | 100%   |          | 6C96E4A591 |
| 8086:8d3b | 15d9:0831 | Intel           | C610/X99 series chips... | 100%   |          | 64918C950D |
| 8086:8d3b | 15d9:0834 | Intel           | C610/X99 series chips... | 100%   |          | EEE6327556 |
| 8086:8d3b | 15d9:0835 | Intel           | C610/X99 series chips... | 100%   |          | 7479576DA8 |
| 8086:8d3b | 15d9:0852 | Intel           | C610/X99 series chips... | 100%   |          | 2E6D79F345 |
| 8086:8d3b | 15d9:7270 | Intel           | C610/X99 series chips... | 100%   |          | 5F6D0233A8 |
| 8086:8d3b | 19e5:2061 | Intel           | C610/X99 series chips... | 100%   |          | 5EB4DFC951 |
| 8086:8d3b | 1d49:0a00 | Intel           | C610/X99 series chips... | 100%   |          | 817865DED6 |
| 8086:8d3b | 8086:35c5 | Intel           | C610/X99 series chips... | 100%   |          | 08100751B7 |
| 8086:8d3b | 8086:35c9 | Intel           | C610/X99 series chips... | 100%   |          | 5F9F099F36 |
| 8086:8d3b | 8086:7270 | Intel           | C610/X99 series chips... | 100%   |          | E5DA683598 |
| 8086:8d3b | 8086:8d3b | Intel           | C610/X99 series chips... | 100%   |          | 2903921AEB |
| 8086:9c3a | 17aa:220c | Intel           | 8 Series HECI #0         | 7.3%   | 4.1.15   | ED4BEF796D |
| 8086:9cba | 17aa:390b | Intel           | Wildcat Point-LP MEI ... | 6.9%   | 4.9.60   | AB6BD693BE |
| 8086:9d3a | 1025:1094 | Intel           | Sunrise Point-LP CSME... | 8.3%   | 4.9.9    | E7D6077756 |
| 8086:9d3a | 1028:06de | Intel           | Sunrise Point-LP CSME... | 7.1%   | 4.15.0   | AE7AD1E7D9 |
| 8086:9d3a | 1028:06fd | Intel           | Sunrise Point-LP CSME... | 40%    | 4.15.0   | 98D787F0D4 |
| 8086:9d3a | 1028:0782 | Intel           | Sunrise Point-LP CSME... | 20%    | 4.18.0   | 49389100FC |
| 8086:9d3a | 1028:079f | Intel           | Sunrise Point-LP CSME... | 23.5%  | 4.15.0   | D18E59C26A |
| 8086:9d3a | 1028:081b | Intel           | Sunrise Point-LP CSME... | 25%    | 3.10.0   | D1454B26C6 |
| 8086:9d3a | 103c:8079 | Intel           | Sunrise Point-LP CSME... | 13.5%  | 4.4.1    | F1A8589F00 |
| 8086:9d3a | 103c:80a4 | Intel           | Sunrise Point-LP CSME... | 33.3%  | 4.9.60   | B01FB51118 |
| 8086:9d3a | 103c:80ff | Intel           | Sunrise Point-LP CSME... | 54.5%  | 4.7.2    | B7B039F46E |
| 8086:9d3a | 103c:8100 | Intel           | Sunrise Point-LP CSME... | 100%   |          | 2B56F34E21 |
| 8086:9d3a | 103c:8101 | Intel           | Sunrise Point-LP CSME... | 16%    | 4.9.60   | BC496704F4 |
| 8086:9d3a | 103c:820c | Intel           | Sunrise Point-LP CSME... | 25%    | 4.9.20   | FAE1CD27F3 |
| 8086:9d3a | 1043:1ccd | Intel           | Sunrise Point-LP CSME... | 14.3%  | 4.9.20   | A4B26975E9 |
| 8086:9d3a | 1179:f820 | Intel           | Sunrise Point-LP CSME... | 25%    | 4.15.0   | B781D8419A |
| 8086:9d3a | 17aa:225c | Intel           | Sunrise Point-LP CSME... | 6.2%   | 3.10.0   | 4438A85B31 |
| 8086:9d3a | 17aa:225d | Intel           | Sunrise Point-LP CSME... | 9.1%   | 4.14.35  | 7D7E6AD5D5 |
| 8086:9d3a | 17aa:3801 | Intel           | Sunrise Point-LP CSME... | 2.6%   | 4.9.9    | 412EAC636F |
| 8086:9d3a | 17aa:3808 | Intel           | Sunrise Point-LP CSME... | 4.8%   | 4.9.20   | 9B61CC7F7F |
| 8086:9d3a | 17aa:380c | Intel           | Sunrise Point-LP CSME... | 16.7%  | 4.9.111  | C3352134E9 |
| 8086:9d3a | 17aa:3819 | Intel           | Sunrise Point-LP CSME... | 12.5%  | 4.9.0    | 18379EBD5C |
| 8086:9d3a | 17aa:382d | Intel           | Sunrise Point-LP CSME... | 3.3%   | 4.9.60   | 65FE9A36B5 |
| 8086:9d3a | 17aa:5048 | Intel           | Sunrise Point-LP CSME... | 16.7%  | 4.15.0   | 842B139FE7 |
| 8086:9d3a | 1d72:1808 | Intel           | Sunrise Point-LP CSME... | 100%   |          | 8D36FC215C |
| 8086:9d3a | 8086:1999 | Intel           | Sunrise Point-LP CSME... | 3.7%   | 4.9.155  | B1A55C7D69 |
| 8086:9d3e |           | Intel           | Skylake-U/Y CSME: HEC... | 86.1%  | 4.18.7   | 8132DC0ECA |
| 8086:9d3e | 103c:82cb | Intel           | Skylake-U/Y CSME: HEC... | 100%   |          | FDB567A59E |
| 8086:9de0 | 1028:08a8 | Intel           | Cannon Point-LP MEI C... | 14.3%  | 4.15.0   | B6DF9FEC5F |
| 8086:a13a | 1019:9bc9 | Intel           | 100 Series/C230 Serie... | 100%   |          | 744A3F2E54 |
| 8086:a13a | 1019:9c56 | Intel           | 100 Series/C230 Serie... | 50%    | 4.15.0   | 093E3BB0DE |
| 8086:a13a | 1028:06de | Intel           | 100 Series/C230 Serie... | 16.7%  | 5.0.0    | BC4C6EBBA7 |
| 8086:a13a | 1028:06f7 | Intel           | 100 Series/C230 Serie... | 66.7%  | 4.15.0   | E2D11AD2AC |
| 8086:a13a | 103c:8392 | Intel           | 100 Series/C230 Serie... | 66.7%  | 4.9.20   | 142D7492C2 |
| 8086:a13a | 1043:1080 | Intel           | 100 Series/C230 Serie... | 25%    | 5.0.0    | 5B1076EA3C |
| 8086:a13a | 1043:1d6d | Intel           | 100 Series/C230 Serie... | 100%   |          | 9D6C0DD372 |
| 8086:a13a | 1043:8694 | Intel           | 100 Series/C230 Serie... | 10.6%  | 4.4.0    | 89F4BB64D7 |
| 8086:a13a | 1458:1c3a | Intel           | 100 Series/C230 Serie... | 10.9%  | 3.10.0   | 53E6A4F263 |
| 8086:a13a | 1462:116e | Intel           | 100 Series/C230 Serie... | 100%   |          | 1C47BC90E4 |
| 8086:a13a | 1462:1190 | Intel           | 100 Series/C230 Serie... | 16.7%  | 4.9.9    | 2B70AAB06F |
| 8086:a13a | 1462:7970 | Intel           | 100 Series/C230 Serie... | 20%    | 4.9.20   | AC10EFBB42 |
| 8086:a13a | 1462:7977 | Intel           | 100 Series/C230 Serie... | 40%    | 4.9.60   | D1DED92F20 |
| 8086:a13a | 1462:7982 | Intel           | 100 Series/C230 Serie... | 20%    | 4.15.0   | AE97650E7C |
| 8086:a13a | 1462:7995 | Intel           | 100 Series/C230 Serie... | 50%    | 4.15.0   | 7D25E0B2DD |
| 8086:a13a | 1462:7996 | Intel           | 100 Series/C230 Serie... | 8.3%   | 4.4.0    | 29D13E00C3 |
| 8086:a13a | 15d9:0884 | Intel           | 100 Series/C230 Serie... | 50%    | 4.15.7   | BB8832ACBD |
| 8086:a13a | 1734:121d | Intel           | 100 Series/C230 Serie... | 12.5%  | 4.4.0    | 29C7E9E412 |
| 8086:a13a | 17aa:3802 | Intel           | 100 Series/C230 Serie... | 3%     | 4.4.16   | 25576A8571 |
| 8086:a13a | 1849:a13a | Intel           | 100 Series/C230 Serie... | 4.9%   | 4.3.3    | 9869646781 |
| 8086:a13a | 8086:1999 | Intel           | 100 Series/C230 Serie... | 12.5%  | 4.9.20   | 13B41B547A |
| 8086:a13b | 15d9:0884 | Intel           | 100 Series/C230 Serie... | 50%    | 4.15.7   | BB8832ACBD |
| 8086:a13b | 8086:1999 | Intel           | 100 Series/C230 Serie... | 33.3%  | 5.0.0    | 13B41B547A |
| 8086:a1ba | 8086:7270 | Intel           | C620 Series Chipset F... | 16.7%  | 4.9.60   | F823B40D84 |
| 8086:a1bb | 1028:0718 | Intel           | C620 Series Chipset F... | 100%   |          | 97313ACF09 |
| 8086:a1bb | 1028:07cb | Intel           | C620 Series Chipset F... | 100%   |          | 5B9EC879FC |
| 8086:a1bb | 1043:871e | Intel           | C620 Series Chipset F... | 100%   |          | A1916FC246 |
| 8086:a1bb | 15d9:095d | Intel           | C620 Series Chipset F... | 100%   |          | 0DFD787765 |
| 8086:a1bb | 15d9:096d | Intel           | C620 Series Chipset F... | 100%   |          | 8A5CFA81DD |
| 8086:a1bb | 15d9:0987 | Intel           | C620 Series Chipset F... | 100%   |          | 893E9D69F2 |
| 8086:a1bb | 8086:35ce | Intel           | C620 Series Chipset F... | 100%   |          | 9CF9DCEEE9 |
| 8086:a1bb | 8086:7270 | Intel           | C620 Series Chipset F... | 100%   |          | 8E73F804F5 |
| 8086:a1be | 1028:0718 | Intel           | C620 Series Chipset F... | 100%   |          | 97313ACF09 |
| 8086:a1be | 1028:07cb | Intel           | C620 Series Chipset F... | 100%   |          | 5B9EC879FC |
| 8086:a1be | 1043:871e | Intel           | C620 Series Chipset F... | 100%   |          | A1916FC246 |
| 8086:a1be | 1590:00eb | Intel           | C620 Series Chipset F... | 100%   |          | 9E91D0ED19 |
| 8086:a1be | 15d9:095d | Intel           | C620 Series Chipset F... | 100%   |          | 0DFD787765 |
| 8086:a1be | 15d9:096d | Intel           | C620 Series Chipset F... | 100%   |          | 8A5CFA81DD |
| 8086:a1be | 15d9:0987 | Intel           | C620 Series Chipset F... | 100%   |          | 893E9D69F2 |
| 8086:a1be | 8086:35ce | Intel           | C620 Series Chipset F... | 100%   |          | 9CF9DCEEE9 |
| 8086:a1be | 8086:7270 | Intel           | C620 Series Chipset F... | 100%   |          | 8E73F804F5 |
| 8086:a2ba | 1458:1c3a | Intel           | 200 Series PCH CSME H... | 2.3%   | 3.10.0   | 1A67024C19 |
| 8086:a2ba | 1462:7a71 | Intel           | 200 Series PCH CSME H... | 28.6%  | 4.9.9    | 309262E3D6 |
| 8086:a328 | 1025:1264 | Intel           | Cannon Lake PCH Seria... | 4.1%   | 4.15.0   | C4FA903BED |
| 8086:a328 | 1028:08a1 | Intel           | Cannon Lake PCH Seria... | 33.3%  | 4.18.0   | AACC137FAA |
| 8086:a328 | 103c:843c | Intel           | Cannon Lake PCH Seria... | 14.3%  | 5.0.0    | E5E15DF58D |
| 8086:a328 | 1849:a328 | Intel           | Cannon Lake PCH Seria... | 100%   |          | B2FAC79AFD |
| 8086:a360 | 1025:1264 | Intel           | Cannon Lake PCH HECI ... | 4.1%   | 4.15.0   | C4FA903BED |
| 8086:a360 | 1028:0851 | Intel           | Cannon Lake PCH HECI ... | 100%   |          | 05D6B79D2F |
| 8086:a360 | 1028:086f | Intel           | Cannon Lake PCH HECI ... | 5.9%   | 4.15.0   | 2261D3C647 |
| 8086:a360 | 1028:0877 | Intel           | Cannon Lake PCH HECI ... | 16.7%  | 4.15.0   | 3FBDBB7E9C |
| 8086:a360 | 103c:843c | Intel           | Cannon Lake PCH HECI ... | 14.3%  | 5.0.0    | E5E15DF58D |
| 8086:a360 | 103c:84db | Intel           | Cannon Lake PCH HECI ... | 33.3%  | 4.15.0   | 06EE78EE4D |
| 8086:a360 | 103c:860f | Intel           | Cannon Lake PCH HECI ... | 100%   |          | BDD15B19B1 |
| 8086:a360 | 1043:1041 | Intel           | Cannon Lake PCH HECI ... | 28.6%  | 4.19.1   | F38CA9409C |
| 8086:a360 | 1043:8694 | Intel           | Cannon Lake PCH HECI ... | 7.2%   | 4.12.14  | 0B771C098E |
| 8086:a360 | 1458:1c3a | Intel           | Cannon Lake PCH HECI ... | 8.2%   | 4.15.0   | 05D00CC5D7 |
| 8086:a360 | 1462:126a | Intel           | Cannon Lake PCH HECI ... | 100%   |          | 3CEF0087AA |
| 8086:a360 | 1462:7b23 | Intel           | Cannon Lake PCH HECI ... | 33.3%  | 4.18.0   | 37076CEBE8 |
| 8086:a360 | 1462:7b33 | Intel           | Cannon Lake PCH HECI ... | 16.7%  | 4.15.0   | F08CE9BD47 |
| 8086:a360 | 17aa:2267 | Intel           | Cannon Lake PCH HECI ... | 8.3%   | 4.19.11  | AAB68A3B33 |
| 8086:a360 | 17aa:3135 | Intel           | Cannon Lake PCH HECI ... | 33.3%  | 4.15.0   | AA1BE9CBEC |
| 8086:a360 | 17aa:3136 | Intel           | Cannon Lake PCH HECI ... | 50%    | 5.0.0    | 02ECA27578 |
| 8086:a360 | 17aa:36e7 | Intel           | Cannon Lake PCH HECI ... | 25%    | 4.15.0   | 1B722DF896 |
| 8086:a360 | 1849:a360 | Intel           | Cannon Lake PCH HECI ... | 15.4%  | 4.15.0   | B2FAC79AFD |
| 8086:a364 | 1849:a364 | Intel           | Cannon Lake PCH HECI ... | 100%   |          | B2FAC79AFD |
| 9710:9900 | a000:2000 | MosChip Semi... | MCS9900 Multi-I/O Con... | 100%   |          | 7D609B3954 |

### Firewire controller (PCI)

5 out of 735 (0.68%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 01c1:5811 | 0043:8294 |                 | FireWire (IEEE 1394)     | 100%   |          | 44D8BC1D36 |
| 104c:8023 | 1297:5106 | Texas Instru... | TSB43AB22A IEEE-1394a... | 28.6%  | 4.12.14  | 35D850590E |
| 1102:4001 | 1102:0010 | Creative Labs   | SB Audigy FireWire Port  | 2.2%   | 3.14.15  | 2A34C16AB3 |
| 1180:0832 | 17aa:20c7 | Ricoh           | R5C832 IEEE 1394 Cont... | 1.2%   | 3.10.19  | 28EA2CFCFB |
| 11c1:5901 | 11c1:5900 | LSI             | FW643 [TrueFire] PCIe... | 0.9%   | 3.14.44  | 1BD87674B0 |

### Flash memory (PCI)

33 out of 58 (56.90%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1524:0520 | 1025:007a | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | E4219525B9 |
| 1524:0520 | 1025:007f | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | 246BC5476B |
| 1524:0520 | 1025:0090 | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | 5979EB4500 |
| 1524:0520 | 1025:009f | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | 005CF3D43E |
| 1524:0520 | 1025:010f | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | 7D53608E50 |
| 1524:0520 | 1179:ff01 | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | C27B4CD3AF |
| 1524:0530 | 1025:007a | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | E4219525B9 |
| 1524:0530 | 1025:007f | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 246BC5476B |
| 1524:0530 | 1025:0090 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 5979EB4500 |
| 1524:0530 | 1025:009f | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 005CF3D43E |
| 1524:0530 | 1025:010f | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 7D53608E50 |
| 1524:0530 | 1179:ff01 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | C27B4CD3AF |
| 1524:0530 | 14c0:0020 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 0351248973 |
| 1524:0530 | 1558:5401 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 8CF7873695 |
| 1524:0530 | 1734:10c1 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | AAAB07D2AE |
| 1524:0530 | 1734:10d7 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | CA3AC06D30 |
| 1524:0530 | 17aa:2079 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | EDAE63A429 |
| 1524:0720 | 1025:011b | ENE Technology  | Memory Stick Card Rea... | 100%   |          | 89AEC2CFFD |
| 1524:0720 | 1025:012a | ENE Technology  | Memory Stick Card Rea... | 100%   |          | C95503E7D2 |
| 1524:0720 | 1025:012e | ENE Technology  | Memory Stick Card Rea... | 100%   |          | 48841846AC |
| 1524:0720 | 1462:2fb3 | ENE Technology  | Memory Stick Card Rea... | 100%   |          | D6A996DA64 |
| 1524:0720 | 1462:2fbd | ENE Technology  | Memory Stick Card Rea... | 100%   |          | 6502446C70 |
| 1524:0730 | 1025:011b | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 89AEC2CFFD |
| 1524:0730 | 1025:012a | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | C95503E7D2 |
| 1524:0730 | 1025:012e | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 48841846AC |
| 1524:0730 | 1462:2fb3 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | D6A996DA64 |
| 1524:0730 | 1462:2fbd | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 6502446C70 |
| 1524:0730 | 1558:0664 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 51E2E84C28 |
| 1524:0730 | 1558:0668 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 41C9811E8B |
| 1524:0730 | 1558:0669 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 647FD58075 |
| 1524:0730 | 1558:0801 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | A28F10A223 |
| 1524:0730 | 1558:5408 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | C3A0F0B364 |
| 1524:0730 | 1558:5409 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 97181C941C |

### Graphics card (PCI)

392 out of 10268 (3.82%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1002:130f | 1849:130f | AMD             | Kaveri [Radeon R7 Gra... | 7.7%   | 3.14.44  | 50841878AE |
| 1002:15d8 | 1002:15d8 | AMD             | Picasso                  | 27.8%  | 5.0.0    | B95C8FA611 |
| 1002:15d8 | 1025:134d | AMD             | Picasso                  | 11.1%  | 5.0.0    | 5537E9D247 |
| 1002:15d8 | 1025:134f | AMD             | Picasso                  | 33.3%  | 5.0.0    | 7721B3FB75 |
| 1002:15d8 | 103c:85ad | AMD             | Picasso                  | 100%   |          | 0D375562BD |
| 1002:15d8 | 103c:85ea | AMD             | Picasso                  | 9.1%   | 5.0.0    | 557904478C |
| 1002:15d8 | 103c:8615 | AMD             | Picasso                  | 50%    | 5.0.0    | 048229855F |
| 1002:15d8 | 1043:18f1 | AMD             | Picasso                  | 15.4%  | 5.0.0    | 25325D332C |
| 1002:15d8 | 1462:7b87 | AMD             | Picasso                  | 50%    | 5.3.11   | 5BCFE2F1CE |
| 1002:15d8 | 17aa:3801 | AMD             | Picasso                  | 25%    | 5.0.0    | 871E08E432 |
| 1002:15d8 | 17aa:3808 | AMD             | Picasso                  | 10%    | 5.0.0    | 74AB3EBC38 |
| 1002:15d8 | 17aa:5124 | AMD             | Picasso                  | 40%    | 5.0.0    | 7B7D62D2A5 |
| 1002:15d8 | 17aa:5126 | AMD             | Picasso                  | 11.1%  | 5.0.0    | 44939F005D |
| 1002:15dd | 1002:15dd | AMD             | Raven Ridge [Radeon V... | 3.5%   | 4.15.0   | FE440B51CA |
| 1002:15dd | 103c:8434 | AMD             | Raven Ridge [Radeon V... | 50%    | 4.18.0   | E30D68CA01 |
| 1002:15dd | 1043:876b | AMD             | Raven Ridge [Radeon V... | 9.7%   | 4.15.0   | F48E23AB6A |
| 1002:15dd | 1458:d000 | AMD             | Raven Ridge [Radeon V... | 8.7%   | 3.10.0   | 1F49F312CB |
| 1002:15dd | 1462:7a36 | AMD             | Raven Ridge [Radeon V... | 28.6%  | 4.16.18  | 41871808C5 |
| 1002:15dd | 1462:7c02 | AMD             | Raven Ridge [Radeon V... | 16.7%  | 4.15.0   | AD51164983 |
| 1002:15dd | 17aa:36f5 | AMD             | Raven Ridge [Radeon V... | 100%   |          | 7E41940C9C |
| 1002:4752 | 103c:3208 | AMD             | Rage 3 [Rage XL PCI]     | 100%   |          | 2C877CF870 |
| 1002:4752 | 8086:3439 | AMD             | Rage 3 [Rage XL PCI]     | 100%   |          | 0F21E859FA |
| 1002:4752 | 8086:345e | AMD             | Rage 3 [Rage XL PCI]     | 100%   |          | 97CC3C4274 |
| 1002:4c4d | 1002:4c4d | AMD             | Rage Mobility AGP 2x ... | 100%   |          | 5C43AB36E8 |
| 1002:4c4d | 10cf:1074 | AMD             | Rage Mobility AGP 2x ... | 100%   |          | 66D6816956 |
| 1002:4c66 | 1028:011d | AMD             | RV250/M9 GL [Mobility... | 25%    | 3.14.44  | 680157DC8E |
| 1002:6600 | 103c:194d | AMD             | Mars [Radeon HD 8670A... | 19%    | 3.14.25  | 2EDF7E28BE |
| 1002:6600 | 103c:195d | AMD             | Mars [Radeon HD 8670A... | 100%   |          | 1A786FF081 |
| 1002:6604 | 103c:8150 | AMD             | Opal XT [Radeon R7 M2... | 16.7%  | 4.15.0   | FD1C0C441E |
| 1002:6610 | 1028:2120 | AMD             | Oland XT [Radeon HD 8... | 100%   |          | F3873460A2 |
| 1002:6610 | 1787:2012 | AMD             | Oland XT [Radeon HD 8... | 100%   |          | 50841878AE |
| 1002:665c | 1043:0456 | AMD             | Bonaire XT [Radeon HD... | 40%    | 4.15.0   | 8EACB4F7F2 |
| 1002:66af | 1002:081e | AMD             | Vega 20 [Radeon VII]     | 16.7%  | 4.15.0   | 0F37A61AA0 |
| 1002:6740 | 103c:3388 | AMD             | Whistler [Radeon HD 6... | 21.4%  | 3.14.44  | 17C76F0730 |
| 1002:6741 | 17aa:21ef | AMD             | Whistler [Radeon HD 6... | 14.3%  | 4.18.0   | A8D9E5EF41 |
| 1002:6741 | 17aa:3976 | AMD             | Whistler [Radeon HD 6... | 4.8%   | 4.1.15   | 70A3F923C2 |
| 1002:6759 | 1787:2308 | AMD             | Turks PRO [Radeon HD ... | 2.5%   | 4.1.34   | 1B7D670A36 |
| 1002:675b | 1002:7600 | AMD             | Turks [Radeon HD 7600... | 50%    | 4.15.0   | B511052CC4 |
| 1002:6760 | 103c:1672 | AMD             | Seymour [Radeon HD 64... | 4.5%   | 3.14.44  | 4F9C19A9C0 |
| 1002:6760 | 106b:00e1 | AMD             | Seymour [Radeon HD 64... | 100%   |          | 772B6F3A59 |
| 1002:6761 | 1297:4012 | AMD             | Seymour LP [Radeon HD... | 100%   |          | DE0CC0AB6F |
| 1002:6770 | 17aa:3623 | AMD             | Caicos [Radeon HD 645... | 20%    | 4.1.15   | 02882EF37B |
| 1002:6778 | 1028:2120 | AMD             | Caicos XT [Radeon HD ... | 5.1%   | 3.10.0   | 469794DF63 |
| 1002:6779 | 103c:2128 | AMD             | Caicos [Radeon HD 645... | 20%    | 4.1.13   | FE2C73039A |
| 1002:6779 | 1043:03da | AMD             | Caicos [Radeon HD 645... | 0.9%   | 3.10.34  | 9734ABB0D4 |
| 1002:6779 | 1043:047b | AMD             | Caicos [Radeon HD 645... | 50%    | 4.15.0   | 423A12D8A5 |
| 1002:6779 | 174b:e164 | AMD             | Caicos [Radeon HD 645... | 1.7%   | 3.14.33  | 8A4E34A210 |
| 1002:67b1 | 1002:0b00 | AMD             | Hawaii PRO [Radeon R9... | 25%    | 4.19.66  | 2FAE8819F7 |
| 1002:67df | 1002:0b37 | AMD             | Ellesmere [Radeon RX ... | 14.3%  | 4.20.5   | 5CC9EEEBFE |
| 1002:67df | 1462:3413 | AMD             | Ellesmere [Radeon RX ... | 8%     | 4.9.87   | 3F7E1BB390 |
| 1002:67df | 1da2:e366 | AMD             | Ellesmere [Radeon RX ... | 1.7%   | 4.9.20   | A9ED28807E |
| 1002:67ef | 174b:e344 | AMD             | Baffin [Radeon RX 460... | 20%    | 4.9.124  | 98A829DCFD |
| 1002:67ef | 174b:e348 | AMD             | Baffin [Radeon RX 460... | 9.1%   | 4.9.20   | 72DD80DA38 |
| 1002:67ff | 1da2:e348 | AMD             | Baffin [Radeon RX 550... | 6.7%   | 4.9.60   | CEDA0A30C3 |
| 1002:6819 | 1043:042c | AMD             | Pitcairn PRO [Radeon ... | 8.3%   | 3.14.22  | EBBD83B0CA |
| 1002:6819 | 1043:045b | AMD             | Pitcairn PRO [Radeon ... | 11.8%  | 3.14.33  | A12C16610A |
| 1002:6819 | 174b:a001 | AMD             | Pitcairn PRO [Radeon ... | 20%    | 4.9.0    | 97B72D7509 |
| 1002:6821 | 1028:05ee | AMD             | Venus XT [Radeon HD 8... | 14.3%  | 3.14.44  | 31B0BECCAB |
| 1002:6823 | 1028:05eb | AMD             | Venus PRO [Radeon HD ... | 23.1%  | 3.14.44  | E52F291884 |
| 1002:682f | 1028:0572 | AMD             | Chelsea LP [Radeon HD... | 3.7%   | 3.14.44  | 609E372F78 |
| 1002:6840 | 1028:0598 | AMD             | Thames [Radeon HD 750... | 4.5%   | 3.14.25  | 988B8C4B4A |
| 1002:6840 | 103c:1840 | AMD             | Thames [Radeon HD 750... | 14.3%  | 3.14.44  | B0552C0AF2 |
| 1002:6840 | 103c:1842 | AMD             | Thames [Radeon HD 750... | 6.2%   | 3.14.44  | 2266C4AA6C |
| 1002:6840 | 1179:fb81 | AMD             | Thames [Radeon HD 750... | 12.5%  | 3.14.33  | 611479F524 |
| 1002:6840 | 144d:c0d8 | AMD             | Thames [Radeon HD 750... | 5.4%   | 3.14.22  | 935529F421 |
| 1002:6841 | 1028:057f | AMD             | Thames [Radeon HD 755... | 22.2%  | 4.15.0   | C38BDE084A |
| 1002:6841 | 103c:17f4 | AMD             | Thames [Radeon HD 755... | 17.4%  | 3.14.44  | C79BD3EFCD |
| 1002:6841 | 104d:90ac | AMD             | Thames [Radeon HD 755... | 1.8%   | 3.10.19  | A41A94F4F5 |
| 1002:68a1 | 1025:0475 | AMD             | Broadway PRO [Mobilit... | 100%   |          | 3B1F271BB2 |
| 1002:68d8 | 1462:2201 | AMD             | Redwood XT [Radeon HD... | 20%    | 4.15.0   | DDF9D08A22 |
| 1002:68d8 | 174b:e152 | AMD             | Redwood XT [Radeon HD... | 6.2%   | 4.1.15   | D67A015497 |
| 1002:68e0 | 103c:143a | AMD             | Park [Mobility Radeon... | 5.7%   | 3.10.51  | E4428DA94F |
| 1002:68e0 | 104d:9071 | AMD             | Park [Mobility Radeon... | 7.7%   | 4.1.34   | F28BA85F16 |
| 1002:68e4 | 1043:1c92 | AMD             | Robson CE [Radeon HD ... | 2.9%   | 3.14.44  | 7FDEE4E7BB |
| 1002:68e4 | 17aa:397a | AMD             | Robson CE [Radeon HD ... | 7%     | 3.10.34  | AF0EC73528 |
| 1002:68f9 | 1028:2126 | AMD             | Cedar [Radeon HD 5000... | 33.3%  | 4.1.34   | D5A5261203 |
| 1002:68f9 | 1462:2181 | AMD             | Cedar [Radeon HD 5000... | 20%    | 5.2.17   | DA73296417 |
| 1002:6938 | 1043:04f5 | AMD             | Tonga XT / Amethyst X... | 33.3%  | 4.5.5    | 0E1E35C6E2 |
| 1002:6939 | 1682:9380 | AMD             | Tonga PRO [Radeon R9 ... | 100%   |          | A3F6229CAA |
| 1002:6939 | 174b:e308 | AMD             | Tonga PRO [Radeon R9 ... | 8.3%   | 4.9.60   | 77EF398855 |
| 1002:699f | 1043:0511 | AMD             | Lexa PRO [Radeon 540/... | 1.8%   | 4.15.18  | A994473A14 |
| 1002:699f | 1458:22f3 | AMD             | Lexa PRO [Radeon 540/... | 50%    | 4.15.0   | 03EEED62F1 |
| 1002:699f | 1462:8a90 | AMD             | Lexa PRO [Radeon 540/... | 23.8%  | 3.10.0   | 28B8E9271B |
| 1002:699f | 148c:2380 | AMD             | Lexa PRO [Radeon 540/... | 16.7%  | 4.15.0   | F48405DCFD |
| 1002:731f | 1da2:e409 | AMD             | Navi 10 [Radeon RX 57... | 100%   |          | 40061999CC |
| 1002:791f | 1462:6b30 | AMD             | RS690M [Radeon Xpress... | 100%   |          | 4940058A56 |
| 1002:9498 | 174b:9498 | AMD             | RV730 PRO [Radeon HD ... | 25%    | 3.14.44  | 5A0B34CAC9 |
| 1002:94c3 | 1028:0402 | AMD             | RV610 [Radeon HD 2400... | 25%    | 5.0.0    | BBA0FE2672 |
| 1002:954f | 1462:1618 | AMD             | RV710 [Radeon HD 4350... | 50%    | 3.14.53  | 51837DE98F |
| 1002:9553 | 1043:1c42 | AMD             | RV710/M92 [Mobility R... | 5.3%   | 4.1.15   | 6D866DDF45 |
| 1002:9553 | 1179:ff82 | AMD             | RV710/M92 [Mobility R... | 75%    | 3.14.44  | 4B659DFE57 |
| 1002:9610 | 1458:d000 | AMD             | RS780 [Radeon HD 3200]   | 21.1%  | 4.1.38   | 059B3E7104 |
| 1002:9616 | 1043:8388 | AMD             | RS780L [Radeon 3000]     | 0.7%   | 3.10.0   | 8A29337DB7 |
| 1002:9712 | 103c:1609 | AMD             | RS880M [Mobility Rade... | 22.2%  | 3.10.0   | 1DD894B330 |
| 1002:9714 | 1849:9714 | AMD             | RS880 [Radeon HD 4290]   | 50%    | 4.1.25   | CAFF866F87 |
| 1002:9807 | 1002:9807 | AMD             | Wrestler [Radeon HD 6... | 100%   |          | 3027B15C31 |
| 1002:9830 | 1043:8623 | AMD             | Kabini [Radeon HD 840... | 1.7%   | 3.14.44  | 7A3C73F361 |
| 1002:9851 | 1025:088c | AMD             | Mullins [Radeon R4/R5... | 100%   |          | D0E8E1E8D9 |
| 1002:9851 | 103c:2269 | AMD             | Mullins [Radeon R4/R5... | 9.1%   | 4.9.20   | 912D4C6523 |
| 1002:9851 | 103c:226b | AMD             | Mullins [Radeon R4/R5... | 16.7%  | 4.1.34   | 8016AF5575 |
| 1002:9851 | 103c:22cd | AMD             | Mullins [Radeon R4/R5... | 10%    | 4.15.0   | 46004F2E8E |
| 1002:9851 | 17aa:3801 | AMD             | Mullins [Radeon R4/R5... | 8%     | 4.1.15   | A30A019453 |
| 1002:9874 | 103c:80b6 | AMD             | Wani [Radeon R5/R6/R7... | 33.3%  | 4.18.0   | C7EEDACBF5 |
| 1002:9874 | 17aa:5113 | AMD             | Wani [Radeon R5/R6/R7... | 25%    | 4.15.0   | 32F7318757 |
| 1002:98e4 | 1025:1087 | AMD             | Stoney [Radeon R2/R3/... | 20%    | 4.15.0   | AF870DDF65 |
| 1002:98e4 | 17aa:39f9 | AMD             | Stoney [Radeon R2/R3/... | 11.1%  | 4.9.60   | C23D0EF968 |
| 1002:9900 | 103c:1849 | AMD             | Trinity [Radeon HD 76... | 12.5%  | 3.14.44  | FE4579E9D1 |
| 1002:990d | 17aa:3804 | AMD             | Richland [Radeon HD 8... | 9.1%   | 3.16.0   | BCE345B263 |
| 1002:9991 | 103c:1850 | AMD             | Trinity 2 [Radeon HD ... | 50%    | 4.9.60   | 898F2B7197 |
| 1002:9996 | 1462:7721 | AMD             | Richland [Radeon HD 8... | 16.7%  | 3.14.44  | 373FA45C3B |
| 10de:0140 | 1458:3126 | Nvidia          | NV43 [GeForce 6600 GT]   | 100%   |          | 9F8066CA65 |
| 10de:0141 | 1043:81ee | Nvidia          | NV43 [GeForce 6600]      | 50%    | 4.1.38   | 71BC5B9631 |
| 10de:0141 | 1458:3126 | Nvidia          | NV43 [GeForce 6600]      | 33.3%  | 4.9.60   | 7E447609BE |
| 10de:0148 | 1179:0001 | Nvidia          | NV43M [GeForce Go 6600]  | 100%   |          | D5D7DAB02F |
| 10de:01d1 | 1028:0405 | Nvidia          | G72 [GeForce 7300 LE]    | 20%    | 3.14.13  | D866167EB1 |
| 10de:01d3 |           | Nvidia          | G72 [GeForce 7200 GS ... | 14.3%  | 4.1.25   | 17445004F4 |
| 10de:0244 | 103c:30b7 | Nvidia          | C51 [GeForce Go 6150]    | 6.2%   | 3.10.34  | 0CA0AF6291 |
| 10de:0292 | 105b:0f03 | Nvidia          | G71 [GeForce 7900 GS]    | 50%    | 4.1.15   | 7296E03F32 |
| 10de:0298 | 1028:019b | Nvidia          | G71M [GeForce Go 7900... | 40%    | 4.15.0   | 267C8D9563 |
| 10de:0298 | 1179:ff31 | Nvidia          | G71M [GeForce Go 7900... | 100%   |          | FED8975477 |
| 10de:031a | 104d:814f | Nvidia          | NV31M [GeForce FX Go5... | 100%   |          | 88ABDEBE09 |
| 10de:0326 |           | Nvidia          | NV34 [GeForce FX 5500]   | 3.7%   | 3.18.16  | 427DFF8FF9 |
| 10de:0326 | 1462:911a | Nvidia          | NV34 [GeForce FX 5500]   | 33.3%  | 4.9.41   | FFD7AFA075 |
| 10de:03d0 | 1043:8234 | Nvidia          | C61 [GeForce 6150SE n... | 15.4%  | 3.14.53  | 7A7933F5D5 |
| 10de:03d1 | 1019:2609 | Nvidia          | C61 [GeForce 6100 nFo... | 10%    | 4.15.0   | 5343BC19E6 |
| 10de:03d6 | 1043:83a4 | Nvidia          | C61 [GeForce 7025 / n... | 10.7%  | 3.14.44  | BEE3209225 |
| 10de:0402 | 1043:8258 | Nvidia          | G84 [GeForce 8600 GT]    | 33.3%  | 4.1.25   | 8CDD8FFE23 |
| 10de:0402 | 10de:050e | Nvidia          | G84 [GeForce 8600 GT]    | 83.3%  | 4.9.124  | 87142BF4F1 |
| 10de:0405 | 1043:15d2 | Nvidia          | G84M [GeForce 9500M GS]  | 11.1%  | 3.14.44  | 4137AC8F54 |
| 10de:0407 | 1028:01f2 | Nvidia          | G84M [GeForce 8600M GT]  | 22.2%  | 4.1.15   | 512FDA5C91 |
| 10de:040f | 10de:049a | Nvidia          | G84GL [Quadro FX 1700]   | 4.5%   | 4.1.25   | 092205321D |
| 10de:0421 | 1acc:0857 | Nvidia          | G86 [GeForce 8500 GT]    | 50%    | 4.18.0   | 629F7B490A |
| 10de:0426 | 104d:9005 | Nvidia          | G86M [GeForce 8400M GT]  | 100%   |          | 9B1280E7FC |
| 10de:0426 | 104d:9018 | Nvidia          | G86M [GeForce 8400M GT]  | 100%   |          | 8A814A5779 |
| 10de:0427 | 103c:30cf | Nvidia          | G86M [GeForce 8400M GS]  | 11.1%  | 3.14.53  | AB1EF36E83 |
| 10de:0428 | 1043:1513 | Nvidia          | G86M [GeForce 8400M G]   | 20%    | 4.1.15   | E0EEE8D1CC |
| 10de:042e | 1043:17c2 | Nvidia          | G86M [GeForce 9300M G]   | 6.7%   | 3.14.33  | 4E30CC5479 |
| 10de:0531 | 103c:30cf | Nvidia          | C67 [GeForce 7150M / ... | 51.7%  | 4.1.15   | 1031D661DB |
| 10de:0533 | 1025:0126 | Nvidia          | C67 [GeForce 7000M / ... | 14.3%  | 4.1.34   | 590A68AE68 |
| 10de:053b | 1565:1406 | Nvidia          | C68 [GeForce 7050 PV ... | 50%    | 4.15.0   | 0B8A392B30 |
| 10de:0602 | 10de:057c | Nvidia          | G92 [GeForce 8800 GT]    | 75%    | 4.19.20  | DA7914FBED |
| 10de:0614 | 1043:8314 | Nvidia          | G92 [GeForce 9800 GT]    | 20%    | 3.14.44  | A3AFA44F01 |
| 10de:062f | 10de:060e | Nvidia          | G94 [GeForce 9800 S]     | 100%   |          | D677F0444F |
| 10de:0640 |           | Nvidia          | G96C [GeForce 9500 GT]   | 1.2%   | 3.14.44  | 64980968F9 |
| 10de:06cd | 3842:1470 | Nvidia          | GF100 [GeForce GTX 470]  | 50%    | 4.15.0   | A0225AA660 |
| 10de:06e9 | 1043:19b2 | Nvidia          | G98M [GeForce 9300M GS]  | 2.8%   | 3.10.34  | 914F5D7BD7 |
| 10de:0848 | 1043:82e2 | Nvidia          | C77 [GeForce 8300]       | 12.5%  | 3.10.19  | E1B7D175A1 |
| 10de:0849 | 1043:82f2 | Nvidia          | C77 [GeForce 8200]       | 33.3%  | 3.14.44  | E3ADCE0E5E |
| 10de:0868 | 103c:2a83 | Nvidia          | C79 [nForce 760i SLI]    | 100%   |          | D677F0444F |
| 10de:0a28 | 103c:7001 | Nvidia          | GT216M [GeForce GT 230M] | 9.1%   | 3.10.34  | 2E7C7E635C |
| 10de:0a34 | 1642:3928 | Nvidia          | GT216M [GeForce GT 240M] | 100%   |          | 0921BB94E0 |
| 10de:0a65 |           | Nvidia          | GT218 [GeForce 210]      | 1.1%   | 3.14.25  | 3C2FD252E1 |
| 10de:0a65 | 1043:8354 | Nvidia          | GT218 [GeForce 210]      | 4.3%   | 3.14.44  | 11CCF345FC |
| 10de:0a65 | 1043:8490 | Nvidia          | GT218 [GeForce 210]      | 53.8%  | 4.9.9    | A6659EE127 |
| 10de:0a65 | 1458:3629 | Nvidia          | GT218 [GeForce 210]      | 7.7%   | 4.1.15   | 8C3172A9F3 |
| 10de:0a65 | 1462:8094 | Nvidia          | GT218 [GeForce 210]      | 3.1%   | 3.14.44  | B7812DD3C1 |
| 10de:0a65 | 3842:1310 | Nvidia          | GT218 [GeForce 210]      | 33.3%  | 4.9.124  | 9CB0AC857A |
| 10de:0a74 | 1025:0296 | Nvidia          | GT218M [GeForce G210M]   | 66.7%  | 4.18.0   | 64727A44DB |
| 10de:0dd8 | 103c:084a | Nvidia          | GF106GL [Quadro 2000]    | 25%    | 4.9.41   | CED13A5341 |
| 10de:0df8 | 10de:0835 | Nvidia          | GF108GL [Quadro 600]     | 15.4%  | 3.10.0   | AF1ECD5263 |
| 10de:0dfc | 1028:0535 | Nvidia          | GF108GLM [NVS 5200M]     | 13.3%  | 3.14.25  | 813731AB25 |
| 10de:0e22 | 3842:1370 | Nvidia          | GF104 [GeForce GTX 460]  | 100%   |          | 957AF816F5 |
| 10de:0f02 | 1043:84f6 | Nvidia          | GF108 [GeForce GT 730]   | 9.1%   | 3.14.44  | 309F371381 |
| 10de:0fc1 | 1043:83f3 | Nvidia          | GK107 [GeForce GT 640]   | 2.8%   | 3.14.44  | 9C1344C76E |
| 10de:0fc2 | 10de:093c | Nvidia          | GK107 [GeForce GT 630... | 50%    | 4.9.20   | 84224B6ADA |
| 10de:0fc6 | 1043:8427 | Nvidia          | GK107 [GeForce GTX 650]  | 11.8%  | 3.14.44  | 4E0DC79606 |
| 10de:0fc6 | 1462:2802 | Nvidia          | GK107 [GeForce GTX 650]  | 40%    | 4.18.0   | 128A90D3B7 |
| 10de:0ffa | 10de:094b | Nvidia          | GK107GL [Quadro K600]    | 23.1%  | 4.1.15   | 949DD823D7 |
| 10de:100a | 1462:2983 | Nvidia          | GK110B [GeForce GTX 7... | 100%   |          | 91D43B6213 |
| 10de:107c | 10de:102f | Nvidia          | GF119 [NVS 315]          | 33.3%  | 4.18.0   | 9E55C4BDEE |
| 10de:1086 | 1043:8387 | Nvidia          | GF110 [GeForce GTX 57... | 16.7%  | 3.14.22  | BC8749820A |
| 10de:11c6 | 1043:8446 | Nvidia          | GK106 [GeForce GTX 65... | 25%    | 3.14.44  | 3730F9BE71 |
| 10de:11c8 | 1569:11c8 | Nvidia          | GK106 [GeForce GTX 65... | 8.3%   | 4.1.15   | CE85A9AD63 |
| 10de:1200 | 1043:838b | Nvidia          | GF114 [GeForce GTX 56... | 18.2%  | 3.14.44  | 5C1D6C3562 |
| 10de:1210 | 1462:10bd | Nvidia          | GF114M [GeForce GTX 5... | 14.3%  | 4.1.15   | 7CEA76DF9B |
| 10de:1244 |           | Nvidia          | GF116 [GeForce GTX 55... | 5.6%   | 3.14.44  | 3736215480 |
| 10de:1244 | 3842:1556 | Nvidia          | GF116 [GeForce GTX 55... | 25%    | 4.15.0   | 4BE9CE0F72 |
| 10de:1287 | 1043:84f5 | Nvidia          | GK208B [GeForce GT 730]  | 36.4%  | 4.1.16   | 8AA494134E |
| 10de:1287 | 1043:8501 | Nvidia          | GK208B [GeForce GT 730]  | 11.1%  | 4.1.15   | 930D8056C3 |
| 10de:1287 | 1043:850c | Nvidia          | GK208B [GeForce GT 730]  | 50%    | 4.18.0   | 6CF789DF63 |
| 10de:1287 | 10de:1083 | Nvidia          | GK208B [GeForce GT 730]  | 100%   |          | 5E5919C697 |
| 10de:1287 | 10de:1287 | Nvidia          | GK208B [GeForce GT 730]  | 9.1%   | 4.1.25   | 8603D5BDF5 |
| 10de:1288 | 1462:8c90 | Nvidia          | GK208B [GeForce GT 720]  | 25%    | 4.1.15   | 74EDF3551E |
| 10de:1288 | 1569:1288 | Nvidia          | GK208B [GeForce GT 720]  | 50%    | 4.9.60   | 7E9CD09A5D |
| 10de:128b | 1043:8572 | Nvidia          | GK208B [GeForce GT 710]  | 6.7%   | 4.1.25   | 7902B95176 |
| 10de:128b | 1043:85f7 | Nvidia          | GK208B [GeForce GT 710]  | 25%    | 4.9.124  | 08A7929F4A |
| 10de:1380 | 1043:84bb | Nvidia          | GM107 [GeForce GTX 75... | 16.7%  | 4.4.0    | E7D55807C9 |
| 10de:1380 | 1043:84bc | Nvidia          | GM107 [GeForce GTX 75... | 16.7%  | 4.1.25   | 59CCFFE44E |
| 10de:1380 | 10de:8412 | Nvidia          | GM107 [GeForce GTX 75... | 100%   |          | 3A624021F2 |
| 10de:1380 | 1458:362d | Nvidia          | GM107 [GeForce GTX 75... | 17.6%  | 4.1.25   | C67CC4D736 |
| 10de:1380 | 1462:3102 | Nvidia          | GM107 [GeForce GTX 75... | 25%    | 4.1.15   | 6158505A7F |
| 10de:1380 | 1642:3e32 | Nvidia          | GM107 [GeForce GTX 75... | 33.3%  | 4.15.0   | E5BFC5E8A5 |
| 10de:1380 | 1acc:752e | Nvidia          | GM107 [GeForce GTX 75... | 100%   |          | 356C1804FA |
| 10de:1381 | 1043:84f0 | Nvidia          | GM107 [GeForce GTX 750]  | 14.3%  | 4.1.15   | 8E80E31C5C |
| 10de:1381 | 10de:1073 | Nvidia          | GM107 [GeForce GTX 750]  | 16.7%  | 4.9.20   | 02666C5333 |
| 10de:1381 | 1458:362e | Nvidia          | GM107 [GeForce GTX 750]  | 50%    | 4.1.16   | FED7D6BB61 |
| 10de:1381 | 1458:3642 | Nvidia          | GM107 [GeForce GTX 750]  | 25%    | 4.1.15   | 8276D533D6 |
| 10de:1381 | 1462:8a9c | Nvidia          | GM107 [GeForce GTX 750]  | 29.4%  | 4.1.25   | DF2090C762 |
| 10de:13c2 | 1019:1029 | Nvidia          | GM204 [GeForce GTX 970]  | 100%   |          | F39DBBFB9A |
| 10de:13c2 | 1043:8508 | Nvidia          | GM204 [GeForce GTX 970]  | 12.5%  | 4.15.0   | 3DD9F6A674 |
| 10de:13c2 | 10de:1131 | Nvidia          | GM204 [GeForce GTX 970]  | 75%    | 4.1.15   | 675FB21B01 |
| 10de:13c2 | 1458:367a | Nvidia          | GM204 [GeForce GTX 970]  | 16.7%  | 4.1.15   | 3E15147646 |
| 10de:13c2 | 1458:367b | Nvidia          | GM204 [GeForce GTX 970]  | 100%   |          | 37FD9139AF |
| 10de:13c2 | 1462:3160 | Nvidia          | GM204 [GeForce GTX 970]  | 25%    | 4.15.0   | 7980C33879 |
| 10de:13c2 | 19da:1366 | Nvidia          | GM204 [GeForce GTX 970]  | 20%    | 4.15.0   | BBB6E540DE |
| 10de:13c2 | 3842:2974 | Nvidia          | GM204 [GeForce GTX 970]  | 33.3%  | 4.15.0   | 3251848CE3 |
| 10de:13c2 | 3842:2978 | Nvidia          | GM204 [GeForce GTX 970]  | 20%    | 4.1.15   | 3251848CE3 |
| 10de:13f1 | 10de:1153 | Nvidia          | GM204GL [Quadro M4000]   | 100%   |          | B8D85B966B |
| 10de:1401 | 1458:36aa | Nvidia          | GM206 [GeForce GTX 960]  | 100%   |          | 1CFE050B29 |
| 10de:1401 | 1458:36ad | Nvidia          | GM206 [GeForce GTX 960]  | 50%    | 5.0.0    | A8A89AC09A |
| 10de:1401 | 1458:36b0 | Nvidia          | GM206 [GeForce GTX 960]  | 100%   |          | B99D4A956B |
| 10de:1401 | 1462:3205 | Nvidia          | GM206 [GeForce GTX 960]  | 100%   |          | 7D2485C593 |
| 10de:1401 | 3842:2966 | Nvidia          | GM206 [GeForce GTX 960]  | 100%   |          | 33DA9C195D |
| 10de:1406 | 1028:072b | Nvidia          | GM206 [GeForce GTX 96... | 100%   |          | 4B9D75483A |
| 10de:17c2 | 10de:1132 | Nvidia          | GM200 [GeForce GTX TI... | 100%   |          | 2369E0376D |
| 10de:1b06 | 1043:85e2 | Nvidia          | GP102 [GeForce GTX 10... | 100%   |          | 5D1A48EE4E |
| 10de:1b06 | 3842:6696 | Nvidia          | GP102 [GeForce GTX 10... | 20%    | 4.18.0   | 35DAE7072E |
| 10de:1b80 | 1043:8592 | Nvidia          | GP104 [GeForce GTX 1080] | 100%   |          | 974C88BAC1 |
| 10de:1b80 | 1458:3717 | Nvidia          | GP104 [GeForce GTX 1080] | 50%    | 5.0.0    | 3F1B997D89 |
| 10de:1b80 | 1462:3367 | Nvidia          | GP104 [GeForce GTX 1080] | 50%    | 5.0.0    | A6B7FD949D |
| 10de:1b81 |           | Nvidia          | GP104 [GeForce GTX 1070] | 50%    | 4.9.20   | D326BF619F |
| 10de:1b81 | 1043:8597 | Nvidia          | GP104 [GeForce GTX 1070] | 100%   |          | 90D8E62525 |
| 10de:1b81 | 1043:859f | Nvidia          | GP104 [GeForce GTX 1070] | 100%   |          | D68BCE418A |
| 10de:1b81 | 1043:85a0 | Nvidia          | GP104 [GeForce GTX 1070] | 25%    | 4.19.28  | 691E406FAF |
| 10de:1b81 | 10b0:1b81 | Nvidia          | GP104 [GeForce GTX 1070] | 100%   |          | 8FB6824328 |
| 10de:1b81 | 1458:36fc | Nvidia          | GP104 [GeForce GTX 1070] | 33.3%  | 4.9.20   | CD8505D488 |
| 10de:1b82 | 1043:8623 | Nvidia          | GP104 [GeForce GTX 10... | 33.3%  | 5.0.0    | 510B031CE9 |
| 10de:1be1 | 103c:846a | Nvidia          | GP104BM [GeForce GTX ... | 100%   |          | 28EE5CFE8C |
| 10de:1be1 | 1462:11ff | Nvidia          | GP104BM [GeForce GTX ... | 50%    | 5.3.0    | C2E855B5BC |
| 10de:1c02 |           | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | A248371C4D |
| 10de:1c02 | 103c:82fc | Nvidia          | GP106 [GeForce GTX 10... | 50%    | 4.15.0   | 75C701DDBD |
| 10de:1c02 | 1043:85b1 | Nvidia          | GP106 [GeForce GTX 10... | 33.3%  | 4.15.0   | 39F3C43A6B |
| 10de:1c02 | 10de:11c2 | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | CAE0B302DB |
| 10de:1c02 | 10de:1c02 | Nvidia          | GP106 [GeForce GTX 10... | 40%    | 4.18.0   | AC3662FF5F |
| 10de:1c02 | 1458:3722 | Nvidia          | GP106 [GeForce GTX 10... | 4.5%   | 4.15.0   | CC9A8D1703 |
| 10de:1c02 | 1458:3724 | Nvidia          | GP106 [GeForce GTX 10... | 33.3%  | 4.15.0   | 4736EC35EF |
| 10de:1c02 | 1462:3287 | Nvidia          | GP106 [GeForce GTX 10... | 10%    | 4.13.0   | CCB4D48D08 |
| 10de:1c02 | 1462:8c95 | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | EB775E1534 |
| 10de:1c02 | 3842:6162 | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | FCC69B7D1E |
| 10de:1c03 |           | Nvidia          | GP106 [GeForce GTX 10... | 50%    | 4.15.0   | 74B6562CCD |
| 10de:1c03 | 1043:85a4 | Nvidia          | GP106 [GeForce GTX 10... | 50%    | 4.15.0   | 725B24FE69 |
| 10de:1c03 | 1043:85a6 | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | EB6CD37E93 |
| 10de:1c03 | 1043:85ae | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | 7DC13C6D0D |
| 10de:1c03 | 1043:85e0 | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | 2C9527A545 |
| 10de:1c03 | 10de:1c03 | Nvidia          | GP106 [GeForce GTX 10... | 60%    | 4.15.0   | 186DBB4515 |
| 10de:1c03 | 1458:3716 | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | 8E3EE6F0BA |
| 10de:1c03 | 1458:3739 | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | 1DDF0EC6EC |
| 10de:1c03 | 1458:3776 | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | 28D68A2C46 |
| 10de:1c03 | 1462:3281 | Nvidia          | GP106 [GeForce GTX 10... | 50%    | 4.15.0   | E044F153CE |
| 10de:1c03 | 1462:3283 | Nvidia          | GP106 [GeForce GTX 10... | 14.3%  | 4.13.0   | 9043D81B30 |
| 10de:1c03 | 196e:119f | Nvidia          | GP106 [GeForce GTX 10... | 50%    | 5.0.0    | B7F1DC4760 |
| 10de:1c03 | 19da:1438 | Nvidia          | GP106 [GeForce GTX 10... | 25%    | 4.18.0   | EF4553CD64 |
| 10de:1c03 | 3842:6163 | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | D94180D023 |
| 10de:1c81 | 10de:11c0 | Nvidia          | GP107 [GeForce GTX 1050] | 66.7%  | 4.15.0   | 1276D33239 |
| 10de:1c81 | 10de:1c81 | Nvidia          | GP107 [GeForce GTX 1050] | 66.7%  | 4.18.0   | 6E08766029 |
| 10de:1c81 | 1458:372c | Nvidia          | GP107 [GeForce GTX 1050] | 50%    | 4.15.0   | 1A7DB52C9A |
| 10de:1c81 | 1458:372d | Nvidia          | GP107 [GeForce GTX 1050] | 50%    | 4.15.0   | CAFF866F87 |
| 10de:1c81 | 1458:3765 | Nvidia          | GP107 [GeForce GTX 1050] | 50%    | 4.15.0   | 2FEBF6828E |
| 10de:1c81 | 1458:3766 | Nvidia          | GP107 [GeForce GTX 1050] | 66.7%  | 5.3.5    | BE505B8545 |
| 10de:1c81 | 1462:3354 | Nvidia          | GP107 [GeForce GTX 1050] | 100%   |          | 844A6EF03C |
| 10de:1c81 | 1462:8c97 | Nvidia          | GP107 [GeForce GTX 1050] | 44.4%  | 4.15.0   | 9784B3BFB0 |
| 10de:1c81 | 174b:5454 | Nvidia          | GP107 [GeForce GTX 1050] | 50%    | 4.15.0   | 42EF2AA13B |
| 10de:1c81 | 19da:2454 | Nvidia          | GP107 [GeForce GTX 1050] | 50%    | 4.15.0   | F67985779A |
| 10de:1c81 | 3842:6150 | Nvidia          | GP107 [GeForce GTX 1050] | 100%   |          | F2560038AF |
| 10de:1c82 | 1043:85d3 | Nvidia          | GP107 [GeForce GTX 10... | 85.7%  | 4.15.0   | 79B1E21D1A |
| 10de:1c82 | 1043:85d6 | Nvidia          | GP107 [GeForce GTX 10... | 33.3%  | 4.15.0   | E48D3747A9 |
| 10de:1c82 | 1043:85fb | Nvidia          | GP107 [GeForce GTX 10... | 100%   |          | 16C69C53FF |
| 10de:1c82 | 1043:85ff | Nvidia          | GP107 [GeForce GTX 10... | 14.3%  | 4.15.0   | 4FF6F8B306 |
| 10de:1c82 | 1043:8613 | Nvidia          | GP107 [GeForce GTX 10... | 21.4%  | 4.15.0   | 4F0A8E2C5B |
| 10de:1c82 | 1043:8627 | Nvidia          | GP107 [GeForce GTX 10... | 100%   |          | 70C1FC426A |
| 10de:1c82 | 1043:862a | Nvidia          | GP107 [GeForce GTX 10... | 50%    | 4.15.0   | F08CE9BD47 |
| 10de:1c82 | 10b0:1c82 | Nvidia          | GP107 [GeForce GTX 10... | 100%   |          | 85FF8C6337 |
| 10de:1c82 | 10de:11bf | Nvidia          | GP107 [GeForce GTX 10... | 6.7%   | 4.15.0   | 0E4E505931 |
| 10de:1c82 | 10de:1c82 | Nvidia          | GP107 [GeForce GTX 10... | 36.8%  | 4.15.0   | F2CA33243F |
| 10de:1c82 | 1458:3729 | Nvidia          | GP107 [GeForce GTX 10... | 100%   |          | D18B737840 |
| 10de:1c82 | 1458:3733 | Nvidia          | GP107 [GeForce GTX 10... | 33.3%  | 4.15.0   | E510EC2AB5 |
| 10de:1c82 | 1462:3351 | Nvidia          | GP107 [GeForce GTX 10... | 35.7%  | 4.15.0   | B2CD0963B2 |
| 10de:1c82 | 1462:8c96 | Nvidia          | GP107 [GeForce GTX 10... | 15.8%  | 4.15.0   | DF0EE54A66 |
| 10de:1c82 | 19da:2454 | Nvidia          | GP107 [GeForce GTX 10... | 33.3%  | 4.15.0   | 1FE17AADBB |
| 10de:1c8d | 1043:11d1 | Nvidia          | GP107M [GeForce GTX 1... | 25%    | 4.19.80  | C2FD6ACB71 |
| 10de:1cb1 | 10de:11bc | Nvidia          | GP107GL [Quadro P1000]   | 100%   |          | 555F102847 |
| 10de:1cb6 | 1028:1264 | Nvidia          | GP107GL [Quadro P620]    | 100%   |          | AD29AF92C2 |
| 10de:1d01 | 1043:85f4 | Nvidia          | GP108 [GeForce GT 1030]  | 50%    | 4.15.0   | 04C0BFBF31 |
| 10de:1d01 | 1043:85f5 | Nvidia          | GP108 [GeForce GT 1030]  | 50%    | 4.15.0   | C9B3B14E25 |
| 10de:1d01 | 1043:8642 | Nvidia          | GP108 [GeForce GT 1030]  | 100%   |          | 1AD00E6974 |
| 10de:1d01 | 10de:1d01 | Nvidia          | GP108 [GeForce GT 1030]  | 66.7%  | 5.0.0    | 61F5096F4A |
| 10de:1d01 | 1458:375c | Nvidia          | GP108 [GeForce GT 1030]  | 16.7%  | 4.15.0   | 5E946FBF6A |
| 10de:1d01 | 1462:8c98 | Nvidia          | GP108 [GeForce GT 1030]  | 26.1%  | 4.15.0   | E244A01D83 |
| 10de:1d01 | 19da:1476 | Nvidia          | GP108 [GeForce GT 1030]  | 50%    | 4.18.0   | 2B0D032DAD |
| 10de:1e02 | 10de:12a3 | Nvidia          | TU102 [TITAN RTX]        | 100%   |          | 30502C41DE |
| 10de:1e04 | 1458:37c4 | Nvidia          | TU102 [GeForce RTX 20... | 100%   |          | 931EA9A398 |
| 10de:1e07 | 1462:3711 | Nvidia          | TU102 [GeForce RTX 20... | 100%   |          | 62128222FA |
| 10de:1e07 | 1462:3715 | Nvidia          | TU102 [GeForce RTX 20... | 100%   |          | CE19512CBB |
| 10de:1e07 | 19da:1503 | Nvidia          | TU102 [GeForce RTX 20... | 100%   |          | C8FDC5E958 |
| 10de:1e07 | 3842:2487 | Nvidia          | TU102 [GeForce RTX 20... | 100%   |          | C3DCC51002 |
| 10de:1e81 | 3842:3287 | Nvidia          | TU104 [GeForce RTX 20... | 100%   |          | 3DA3A9D9AD |
| 10de:1e82 | 1043:8676 | Nvidia          | TU104 [GeForce RTX 2080] | 100%   |          | 48041296CA |
| 10de:1e82 | 10b0:1e87 | Nvidia          | TU104 [GeForce RTX 2080] | 100%   |          | 73CF7CEE79 |
| 10de:1e82 | 1462:3722 | Nvidia          | TU104 [GeForce RTX 2080] | 100%   |          | ACBAD1E6CE |
| 10de:1e87 | 1458:37a8 | Nvidia          | TU104 [GeForce RTX 20... | 100%   |          | AAD0551E27 |
| 10de:1eb1 | 10de:12a0 | Nvidia          | TU104GL [Quadro RTX 4... | 100%   |          | B95F8101E5 |
| 10de:1f02 | 10de:1f02 | Nvidia          | TU106 [GeForce RTX 2070] | 100%   |          | C8C1A01026 |
| 10de:1f02 | 1458:37c8 | Nvidia          | TU106 [GeForce RTX 2070] | 100%   |          | 69F2264D39 |
| 10de:1f07 | 1043:8670 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | AF6DA5211E |
| 10de:1f07 | 1043:8671 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | AC29A018F8 |
| 10de:1f07 | 10de:12ad | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | 55119E58D9 |
| 10de:1f07 | 1462:3732 | Nvidia          | TU106 [GeForce RTX 20... | 50%    | 5.0.0    | F1B7697C91 |
| 10de:1f08 | 10de:1f08 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | 3CF95EC244 |
| 10de:1f08 | 1458:3fc2 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | 8DF2C93C38 |
| 10de:1f08 | 196e:130f | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | 328F236B37 |
| 10de:1f08 | 3842:2167 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | 32073E3911 |
| 10de:1f11 | 103c:8574 | Nvidia          | TU106M [GeForce RTX 2... | 100%   |          | 29CB9464AE |
| 10de:1f11 | 1043:140f | Nvidia          | TU106M [GeForce RTX 2... | 50%    | 5.3.0    | EFC1AC12C7 |
| 10de:1f47 | 10de:13ad | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | E0192EBFC1 |
| 10de:1f50 | 103c:8603 | Nvidia          | TU106BM [GeForce RTX ... | 100%   |          | 8295B3DB5F |
| 10de:1f82 | 1462:3800 | Nvidia          | TU117 [GeForce GTX 1650] | 100%   |          | D5F4BDB1B5 |
| 10de:1f91 | 1043:109f | Nvidia          | TU117M [GeForce GTX 1... | 100%   |          | 25325D332C |
| 10de:2182 | 1043:86a3 | Nvidia          | TU116 [GeForce GTX 16... | 100%   |          | E891AAE560 |
| 10de:2182 | 10de:2182 | Nvidia          | TU116 [GeForce GTX 16... | 100%   |          | C4788779C1 |
| 10de:2182 | 1458:3fbe | Nvidia          | TU116 [GeForce GTX 16... | 100%   |          | CECF83927E |
| 10de:2182 | 1462:3750 | Nvidia          | TU116 [GeForce GTX 16... | 100%   |          | FB532E634D |
| 10de:2182 | 1462:375a | Nvidia          | TU116 [GeForce GTX 16... | 100%   |          | CA561AA481 |
| 10de:2184 | 1458:3fc7 | Nvidia          | TU116 [GeForce GTX 1660] | 100%   |          | C4C123186E |
| 10de:2184 | 1462:8d91 | Nvidia          | TU116 [GeForce GTX 1660] | 50%    | 5.3.11   | C38867C0EF |
| 10de:2184 | 7377:150a | Nvidia          | TU116 [GeForce GTX 1660] | 100%   |          | 30939907C1 |
| 8086:0042 | 1849:0042 | Intel           | Core Processor Integr... | 8.3%   | 3.14.33  | 1D9934126C |
| 8086:0106 | 1025:0504 | Intel           | 2nd Generation Core P... | 4.3%   | 4.1.38   | 8FE3AF49FB |
| 8086:0162 | 1028:052c | Intel           | Xeon E3-1200 v2/3rd G... | 14.3%  | 4.15.0   | 29A0FC6CE0 |
| 8086:0162 | 1043:84ca | Intel           | Xeon E3-1200 v2/3rd G... | 20.8%  | 3.14.44  | C7C6CD6D36 |
| 8086:0162 | 1849:0162 | Intel           | Xeon E3-1200 v2/3rd G... | 2.4%   | 3.10.0   | 8505F4654F |
| 8086:0166 | 1025:0647 | Intel           | 3rd Gen Core processo... | 0.7%   | 3.10.34  | 86D2D3B0E1 |
| 8086:0412 | 1462:7816 | Intel           | Xeon E3-1200 v3/4th G... | 20%    | 4.9.20   | 093472BA51 |
| 8086:041a | 1462:7823 | Intel           | Xeon E3-1200 v3 Proce... | 100%   |          | 7755195EF6 |
| 8086:0f31 | 1025:0936 | Intel           | Atom Processor Z36xxx... | 5.6%   | 4.12.14  | 1718CF1D36 |
| 8086:0f31 | 17aa:3695 | Intel           | Atom Processor Z36xxx... | 50%    | 4.15.0   | 08BB09B100 |
| 8086:1902 | 1043:8694 | Intel           | HD Graphics 510          | 10.7%  | 4.8.14   | A91734714E |
| 8086:1902 | 1462:7996 | Intel           | HD Graphics 510          | 20%    | 4.9.20   | BFAA613B9E |
| 8086:1902 | 8086:2212 | Intel           | HD Graphics 510          | 100%   |          | FF56929B10 |
| 8086:1912 | 1043:8694 | Intel           | HD Graphics 530          | 8.3%   | 4.4.0    | 575CE93124 |
| 8086:1912 | 1458:d000 | Intel           | HD Graphics 530          | 25%    | 4.9.41   | 53E6A4F263 |
| 8086:1916 | 1025:1094 | Intel           | Skylake GT2 [HD Graph... | 8.3%   | 4.9.9    | E7D6077756 |
| 8086:1916 | 1028:06de | Intel           | Skylake GT2 [HD Graph... | 7.1%   | 4.15.0   | AE7AD1E7D9 |
| 8086:1916 | 1028:06fd | Intel           | Skylake GT2 [HD Graph... | 25%    | 4.15.0   | 569785286A |
| 8086:1916 | 103c:8079 | Intel           | Skylake GT2 [HD Graph... | 5.4%   | 4.1.15   | 82F5250E0D |
| 8086:1916 | 103c:80a4 | Intel           | Skylake GT2 [HD Graph... | 33.3%  | 4.9.60   | B01FB51118 |
| 8086:1916 | 103c:80ff | Intel           | Skylake GT2 [HD Graph... | 50%    | 4.7.2    | B7B039F46E |
| 8086:1916 | 103c:8100 | Intel           | Skylake GT2 [HD Graph... | 100%   |          | 2B56F34E21 |
| 8086:1916 | 103c:8101 | Intel           | Skylake GT2 [HD Graph... | 5%     | 4.9.60   | BC496704F4 |
| 8086:1916 | 103c:820c | Intel           | Skylake GT2 [HD Graph... | 25%    | 4.9.20   | FAE1CD27F3 |
| 8086:1916 | 1043:1ccd | Intel           | Skylake GT2 [HD Graph... | 14.3%  | 4.9.20   | A4B26975E9 |
| 8086:1916 | 1179:f822 | Intel           | Skylake GT2 [HD Graph... | 25%    | 4.15.0   | B781D8419A |
| 8086:1916 | 17aa:3824 | Intel           | Skylake GT2 [HD Graph... | 6.2%   | 4.9.9    | 412EAC636F |
| 8086:1916 | 17aa:382c | Intel           | Skylake GT2 [HD Graph... | 16.7%  | 4.9.0    | 18379EBD5C |
| 8086:1916 | 17aa:5048 | Intel           | Skylake GT2 [HD Graph... | 20%    | 4.15.0   | 842B139FE7 |
| 8086:191b | 1028:06de | Intel           | HD Graphics 530          | 16.7%  | 5.0.0    | BC4C6EBBA7 |
| 8086:191b | 1043:1080 | Intel           | HD Graphics 530          | 25%    | 5.0.0    | 5B1076EA3C |
| 8086:191b | 1043:1d6d | Intel           | HD Graphics 530          | 100%   |          | 9D6C0DD372 |
| 8086:191b | 1462:1190 | Intel           | HD Graphics 530          | 16.7%  | 4.9.9    | 2B70AAB06F |
| 8086:1921 | 17aa:39e8 | Intel           | HD Graphics 520          | 20%    | 4.9.111  | C3352134E9 |
| 8086:22b1 | 1025:1012 | Intel           | Atom/Celeron/Pentium ... | 4.3%   | 4.9.20   | 16D1C62342 |
| 8086:22b1 | 1028:0725 | Intel           | Atom/Celeron/Pentium ... | 25%    | 4.9.20   | 92DCC778AC |
| 8086:22b1 | 1043:10c0 | Intel           | Atom/Celeron/Pentium ... | 3%     | 4.9.9    | E6AFAB9B56 |
| 8086:22b1 | 1558:0945 | Intel           | Atom/Celeron/Pentium ... | 5.9%   | 4.1.15   | BDAF59B6EB |
| 8086:2572 | 103c:12bc | Intel           | 82865G Integrated Gra... | 20%    | 4.1.34   | DD4DD47556 |
| 8086:2772 | 8086:464c | Intel           | 82945G/GZ Integrated ... | 34.6%  | 3.10.0   | 70309E8B8E |
| 8086:27a2 | 1025:0107 | Intel           | Mobile 945GM/GMS, 943... | 50%    | 4.1.34   | 290DB67DA7 |
| 8086:27a2 | 104d:820f | Intel           | Mobile 945GM/GMS, 943... | 33.3%  | 3.14.44  | 811EFEE1FC |
| 8086:27a2 | 1462:0341 | Intel           | Mobile 945GM/GMS, 943... | 25%    | 4.1.15   | C71F72F074 |
| 8086:2992 | 1734:10b5 | Intel           | 82Q963/Q965 Integrate... | 25%    | 4.1.15   | BF1BADE95D |
| 8086:2e12 | 1028:027f | Intel           | 4 Series Chipset Inte... | 1.8%   | 3.14.44  | BDF53B02DC |
| 8086:2e12 | 17aa:3048 | Intel           | 4 Series Chipset Inte... | 16.7%  | 4.1.15   | 128FC416E3 |
| 8086:3e90 | 1458:d000 | Intel           | Coffee Lake UHD Graph... | 33.3%  | 4.15.0   | 5C08307156 |
| 8086:3e91 | 1043:8694 | Intel           | 8th Gen Core Processo... | 22.2%  | 4.15.0   | DA54361164 |
| 8086:3e91 | 1849:3e91 | Intel           | 8th Gen Core Processo... | 9.1%   | 4.15.0   | 59151791CF |
| 8086:3e92 | 1028:0851 | Intel           | UHD Graphics 630 (Des... | 100%   |          | 05D6B79D2F |
| 8086:3e92 | 103c:843c | Intel           | UHD Graphics 630 (Des... | 50%    | 5.1.3    | E5E15DF58D |
| 8086:3e92 | 1043:8694 | Intel           | UHD Graphics 630 (Des... | 3.4%   | 4.15.0   | 0B771C098E |
| 8086:3e98 | 1462:7b98 | Intel           | UHD Graphics 630 (Des... | 100%   |          | 297E534CF0 |
| 8086:3e9b | 1025:1264 | Intel           | UHD Graphics 630 (Mob... | 4.3%   | 4.15.0   | C4FA903BED |
| 8086:3e9b | 1462:126a | Intel           | UHD Graphics 630 (Mob... | 50%    | 3.10.0   | 039A05F3EB |
| 8086:3ea0 | 1028:08a8 | Intel           | UHD Graphics 620 (Whi... | 14.3%  | 4.15.0   | B6DF9FEC5F |
| 8086:5912 | 1043:8694 | Intel           | HD Graphics 630          | 1.3%   | 4.4.49   | B0DE2CBA6A |
| 8086:5916 | 1028:0768 | Intel           | HD Graphics 620          | 7.7%   | 4.9.9    | 2BB9B79D2E |
| 8086:5916 | 1028:0782 | Intel           | HD Graphics 620          | 20%    | 4.18.0   | 49389100FC |
| 8086:5916 | 17aa:39f1 | Intel           | HD Graphics 620          | 4%     | 4.9.60   | 65FE9A36B5 |
| 8086:5916 | 8086:2212 | Intel           | HD Graphics 620          | 4.5%   | 4.9.41   | B1A55C7D69 |
| 8086:5917 | 17aa:225e | Intel           | UHD Graphics 620         | 12.5%  | 4.15.0   | 7D7E6AD5D5 |
| 8086:8108 | 1028:02b1 | Intel           | US15W/US15X SCH [Poul... | 100%   |          | 7D4473A4A5 |
| 8086:8a52 | 1028:097c | Intel           | Iris Plus Graphics G7    | 60%    | 5.4.2    | 66554C2B07 |
| 8086:8a56 | 1028:0979 | Intel           | UHD Graphics 920         | 22.2%  | 5.0.0    | 7F4CE08DF9 |
| 8086:9b41 | 1028:0954 | Intel           | UHD Graphics             | 100%   |          | 8740133E10 |
| 8086:a011 | 1462:104e | Intel           | Atom Processor D4xx/D... | 20%    | 4.1.15   | 5F15F028A8 |

### Modem (PCI)

50 out of 103 (48.54%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1002:4378 | 103c:3085 | AMD             | IXP SB400 AC'97 Modem... | 66.7%  | 5.0.0    | 215D2A28A4 |
| 1039:7013 | 1025:0083 | Silicon Inte... | AC'97 Modem Controller   | 100%   |          | 94017E086A |
| 1057:3052 | 1057:3020 | Motorola        | SM56 Data Fax Modem      | 100%   |          | F60B0BE33D |
| 1057:3052 | 1631:3034 | Motorola        | SM56 Data Fax Modem      | 100%   |          | B7CEC1644D |
| 10b9:5457 | 103c:0850 | ULi Electronics | M5457 AC'97 Modem Con... | 100%   |          | 4E9D284D9C |
| 10b9:5457 | 104d:8158 | ULi Electronics | M5457 AC'97 Modem Con... | 100%   |          | 2BA72A0486 |
| 10de:00d9 | 103c:006d | Nvidia          | nForce3 Audio            | 100%   |          | E1BAA5BDE6 |
| 11c1:0440 | 11c1:0440 | LSI             | 56k WinModem             | 100%   |          | 6B2E5020C2 |
| 11c1:0449 | 1468:0410 | LSI             | L56xM+S [Mars-2] WinM... | 100%   |          | A8A13EFBA0 |
| 11c1:044c | 11c1:044c | LSI             | LT WinModem              | 100%   |          | 461D79E9EB |
| 11c1:044e | 11c1:044e | LSI             | LT WinModem              | 100%   |          | 6203763CC5 |
| 11c1:044e | 1235:044e | LSI             | LT WinModem              | 100%   |          | 3D74179CB7 |
| 11c1:044e | 13e0:0401 | LSI             | LT WinModem              | 100%   |          | E9ACA9663F |
| 11c1:0450 | 144f:1515 | LSI             | LT WinModem              | 100%   |          | 32D5B1A614 |
| 1543:3052 | 1543:3000 | SILICON Labo... | Intel 537 [Winmodem]     | 100%   |          | 75C969D54B |
| 2000:2800 | 163c:2800 | Smart Link      | SmartPCI2800 V.92 PCI... | 100%   |          | 9DEE04D2CB |
| 2003:8800 | 16ef:2800 | Smart Link      | LM-I56N                  | 100%   |          | 8B4AE6CF41 |
| 2003:8800 | 1801:2800 | Smart Link      | LM-I56N                  | 100%   |          | 413AE4FF4F |
| 8086:1040 | 8086:1000 | Intel           | 536EP Data Fax Modem     | 100%   |          | 1263C61735 |
| 8086:2446 | 1025:1027 | Intel           | 82801BA/BAM AC'97 Mod... | 100%   |          | E0A83557FF |
| 8086:2486 | 134d:4c21 | Intel           | 82801CA/CAM AC'97 Mod... | 100%   |          | 38C172234D |
| 8086:2486 | 14f1:5421 | Intel           | 82801CA/CAM AC'97 Mod... | 100%   |          | 4F9273C63C |
| 8086:24c6 | 1014:0524 | Intel           | 82801DB/DBL/DBM (ICH4... | 100%   |          | BE49E35FA4 |
| 8086:24c6 | 1014:0559 | Intel           | 82801DB/DBL/DBM (ICH4... | 83.3%  | 3.14.53  | 1811B66E00 |
| 8086:24c6 | 103c:3080 | Intel           | 82801DB/DBL/DBM (ICH4... | 100%   |          | 6802B34FDD |
| 8086:24c6 | 103c:3084 | Intel           | 82801DB/DBL/DBM (ICH4... | 100%   |          | 24A093E347 |
| 8086:24c6 | 10cf:10d1 | Intel           | 82801DB/DBL/DBM (ICH4... | 66.7%  | 3.14.25  | EA732BEA27 |
| 8086:24c6 | 1179:0001 | Intel           | 82801DB/DBL/DBM (ICH4... | 66.7%  | 4.9.0    | B36ADF3084 |
| 8086:24c6 | 1179:ff31 | Intel           | 82801DB/DBL/DBM (ICH4... | 80%    | 4.1.38   | E9BD04F647 |
| 8086:24c6 | 14f1:5422 | Intel           | 82801DB/DBL/DBM (ICH4... | 25%    | 3.14.44  | 4EBB330BF9 |
| 8086:24c6 | 1734:103c | Intel           | 82801DB/DBL/DBM (ICH4... | 100%   |          | 6F452862B4 |
| 8086:24d6 | 1025:0045 | Intel           | 82801EB/ER (ICH5/ICH5... | 100%   |          | 41CC7EB08C |
| 8086:24d6 | 1179:0001 | Intel           | 82801EB/ER (ICH5/ICH5... | 100%   |          | A7D4DEEF9E |
| 8086:266d | 1014:0574 | Intel           | 82801FB/FBM/FR/FW/FRW... | 83.3%  | 4.9.41   | BABCA7BCDE |
| 8086:266d | 1014:0576 | Intel           | 82801FB/FBM/FR/FW/FRW... | 50%    | 3.14.33  | 9809E004BA |
| 8086:266d | 1025:0066 | Intel           | 82801FB/FBM/FR/FW/FRW... | 70%    | 3.14.44  | 50122B9E8E |
| 8086:266d | 1025:006a | Intel           | 82801FB/FBM/FR/FW/FRW... | 55.6%  | 3.14.25  | 77353D6C03 |
| 8086:266d | 103c:0934 | Intel           | 82801FB/FBM/FR/FW/FRW... | 100%   |          | 16F00AAE37 |
| 8086:266d | 103c:0944 | Intel           | 82801FB/FBM/FR/FW/FRW... | 33.3%  | 3.14.44  | A770CF025E |
| 8086:266d | 103c:099c | Intel           | 82801FB/FBM/FR/FW/FRW... | 14.3%  | 3.14.44  | C60AB5C121 |
| 8086:266d | 103c:3080 | Intel           | 82801FB/FBM/FR/FW/FRW... | 50%    | 4.9.9    | 0572E8425C |
| 8086:266d | 103c:3081 | Intel           | 82801FB/FBM/FR/FW/FRW... | 100%   |          | 1481661DEB |
| 8086:266d | 103c:3082 | Intel           | 82801FB/FBM/FR/FW/FRW... | 100%   |          | 91C7AE2180 |
| 8086:266d | 103c:309d | Intel           | 82801FB/FBM/FR/FW/FRW... | 33.3%  | 4.1.16   | 837230178B |
| 8086:266d | 103c:30c4 | Intel           | 82801FB/FBM/FR/FW/FRW... | 50%    | 4.1.25   | 87F8EF65AE |
| 8086:266d | 107b:0460 | Intel           | 82801FB/FBM/FR/FW/FRW... | 100%   |          | B62ECA10E8 |
| 8086:266d | 1179:0001 | Intel           | 82801FB/FBM/FR/FW/FRW... | 75%    | 3.14.44  | 8488B3D0B9 |
| 8086:266d | 144d:2115 | Intel           | 82801FB/FBM/FR/FW/FRW... | 50%    | 4.1.22   | 88BAF3B388 |
| 8086:266d | 14f1:5423 | Intel           | 82801FB/FBM/FR/FW/FRW... | 51.5%  | 3.14.44  | 18E748759E |
| 8086:266d | 17aa:207c | Intel           | 82801FB/FBM/FR/FW/FRW... | 100%   |          | EDAE63A429 |

### Multimedia controller (PCI)

157 out of 195 (80.51%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 0002:8290 | 107d:2609 |                 | Multimedia controller    | 100%   |          | 95D420F37F |
| 1002:4d51 | 1002:b041 | AMD             | Unified AVStream Driver  | 100%   |          | 2CF316774E |
| 1002:ac12 | 1002:b539 | AMD             | Theater HD T507 (DVB-... | 100%   |          | DD5E0979B0 |
| 1002:ac12 | 12ab:0003 | AMD             | Theater HD T507 (DVB-... | 100%   |          | EA55AE13AC |
| 1002:ad18 | 1682:ad18 | AMD             | Multimedia controller    | 100%   |          | 3108FE53D3 |
| 1022:15e2 | 1022:15e2 | AMD             | Raven/Raven2/FireFlig... | 55.6%  | 4.19.8   | 9809687258 |
| 1022:15e2 | 1025:1233 | AMD             | Raven/Raven2/FireFlig... | 71.4%  | 5.0.0    | 856A212CAA |
| 1022:15e2 | 1025:134d | AMD             | Raven/Raven2/FireFlig... | 11.1%  | 5.0.0    | 5537E9D247 |
| 1022:15e2 | 1025:134f | AMD             | Raven/Raven2/FireFlig... | 33.3%  | 5.0.0    | 7721B3FB75 |
| 1022:15e2 | 103c:8433 | AMD             | Raven/Raven2/FireFlig... | 33.3%  | 5.0.0    | 2BCAD0A319 |
| 1022:15e2 | 103c:8434 | AMD             | Raven/Raven2/FireFlig... | 100%   |          | E2E650868B |
| 1022:15e2 | 103c:8496 | AMD             | Raven/Raven2/FireFlig... | 40%    | 5.0.0    | 53B6114671 |
| 1022:15e2 | 103c:84a3 | AMD             | Raven/Raven2/FireFlig... | 100%   |          | 6A706DA421 |
| 1022:15e2 | 103c:84ae | AMD             | Raven/Raven2/FireFlig... | 70.2%  | 5.0.0    | 3617ECED9F |
| 1022:15e2 | 103c:84d2 | AMD             | Raven/Raven2/FireFlig... | 85.7%  | 5.3.0    | 7D68F90A4F |
| 1022:15e2 | 103c:85dd | AMD             | Raven/Raven2/FireFlig... | 5.3%   | 5.0.0    | B1985C9EC5 |
| 1022:15e2 | 103c:85ea | AMD             | Raven/Raven2/FireFlig... | 16.7%  | 5.0.0    | 2CFA8723C1 |
| 1022:15e2 | 17aa:36f5 | AMD             | Raven/Raven2/FireFlig... | 100%   |          | 7E41940C9C |
| 1022:15e2 | 17aa:380b | AMD             | Raven/Raven2/FireFlig... | 75%    | 5.3.0    | 52036BD95B |
| 1022:15e2 | 17aa:3811 | AMD             | Raven/Raven2/FireFlig... | 66.7%  | 5.0.0    | 8CFF91E24B |
| 1022:15e2 | 17aa:3812 | AMD             | Raven/Raven2/FireFlig... | 37.5%  | 5.0.0    | B49AAC1247 |
| 1022:15e2 | 17aa:3814 | AMD             | Raven/Raven2/FireFlig... | 40%    | 5.0.0    | 45CAB02B32 |
| 1022:15e2 | 17aa:5124 | AMD             | Raven/Raven2/FireFlig... | 40%    | 5.0.0    | 7B7D62D2A5 |
| 1022:15e2 | 17aa:5126 | AMD             | Raven/Raven2/FireFlig... | 44.4%  | 5.0.0    | ADEC400398 |
| 1022:15e2 | 19e5:3e06 | AMD             | Raven/Raven2/FireFlig... | 33.3%  | 5.0.0    | 2CDCEA8607 |
| 1022:15e2 | 19e5:3e10 | AMD             | Raven/Raven2/FireFlig... | 33.3%  | 5.4.2    | 042C4B3C5A |
| 102b:8350 | 102b:9000 | Matrox Elect... | Matrox Multimedia con... | 100%   |          | B3EE98B7CC |
| 1057:3410 | 1057:ffff | Motorola        | DSP56361 Digital Sign... | 100%   |          | 16A7890585 |
| 1057:3410 | 11af:eed2 | Motorola        | DSP56361 Digital Sign... | 100%   |          | 16A7890585 |
| 1057:3410 | 11af:eee1 | Motorola        | DSP56361 Digital Sign... | 100%   |          | 16A7890585 |
| 109e:0878 |           | Brooktree       | Bt878 Audio Capture      | 100%   |          | 80274F5B0C |
| 109e:0878 | 0070:ff02 | Brooktree       | Bt878 Audio Capture      | 100%   |          | 84495E0FB8 |
| 109e:0878 | 0070:ff04 | Brooktree       | Bt878 Audio Capture      | 100%   |          | 2C877CF870 |
| 109e:0878 | 1047:f331 | Brooktree       | Bt878 Audio Capture      | 100%   |          | 444FFBC8A6 |
| 109e:0878 | 107d:6607 | Brooktree       | Bt878 Audio Capture      | 100%   |          | 6027467F3B |
| 109e:0878 | 107d:6609 | Brooktree       | Bt878 Audio Capture      | 100%   |          | 4A6B13BAEA |
| 109e:0878 | 1461:0001 | Brooktree       | Bt878 Audio Capture      | 100%   |          | E8072B6F3A |
| 109e:0878 | 1461:0002 | Brooktree       | Bt878 Audio Capture      | 100%   |          | A22609B54B |
| 109e:0878 | 1461:0003 | Brooktree       | Bt878 Audio Capture      | 6.2%   | 3.14.25  | 7A69435C43 |
| 109e:0878 | 1461:0004 | Brooktree       | Bt878 Audio Capture      | 100%   |          | F2B7867CAA |
| 109e:0878 | 800a:763d | Brooktree       | Bt878 Audio Capture      | 100%   |          | 08DCF9AA49 |
| 109e:0878 | 800b:763d | Brooktree       | Bt878 Audio Capture      | 100%   |          | 08DCF9AA49 |
| 109e:0878 | 800c:763d | Brooktree       | Bt878 Audio Capture      | 100%   |          | 08DCF9AA49 |
| 109e:0878 | 800d:763d | Brooktree       | Bt878 Audio Capture      | 100%   |          | 08DCF9AA49 |
| 109e:0878 | bd11:4100 | Brooktree       | Bt878 Audio Capture      | 100%   |          | C20B184FC3 |
| 10b5:9056 | 1a0e:006f | PLX Technology  | PCI9056 32-bit 66MHz ... | 100%   |          | C6B09D560F |
| 10b5:9056 | 1a0e:0073 | PLX Technology  | PCI9056 32-bit 66MHz ... | 50%    | 4.15.0   | 5122F7EE54 |
| 10cf:202a | 104d:81fa | Fujitsu Limi... | Integrated MPEG Encoder  | 100%   |          | 7F0BB0CC92 |
| 10cf:2030 | 104d:9062 | Fujitsu Limi... | Fujitsu Multimedia co... | 100%   |          | 2628EBE1BB |
| 1131:7160 | 1461:0455 | Philips Semi... | SAA7160                  | 100%   |          | F85808C04C |
| 1131:7160 | 1461:0555 | Philips Semi... | SAA7160                  | 100%   |          | D400943350 |
| 1131:7160 | 1461:0655 | Philips Semi... | SAA7160                  | 100%   |          | 58A8ECB02A |
| 1131:7160 | 1461:0855 | Philips Semi... | SAA7160                  | 100%   |          | BBDA8BED86 |
| 1131:7160 | 1461:0955 | Philips Semi... | SAA7160                  | 100%   |          | D6813FBC7C |
| 1131:7160 | 1461:0a55 | Philips Semi... | SAA7160                  | 100%   |          | 99DDBBF195 |
| 1131:7160 | 1461:1055 | Philips Semi... | SAA7160                  | 100%   |          | 9E921922BA |
| 1131:7160 | 1461:1455 | Philips Semi... | SAA7160                  | 100%   |          | 8D0B9127EF |
| 1131:7160 | 1461:1855 | Philips Semi... | SAA7160                  | 100%   |          | FA070462FC |
| 1131:7160 | 1461:2355 | Philips Semi... | SAA7160                  | 100%   |          | B98B8362E0 |
| 1131:7160 | 1461:2655 | Philips Semi... | SAA7160                  | 100%   |          | A74B989748 |
| 1131:7160 | 1461:7561 | Philips Semi... | SAA7160                  | 100%   |          | A010F0A8F5 |
| 1131:7160 | 1461:7992 | Philips Semi... | SAA7160                  | 100%   |          | 3ACD33354F |
| 1131:7160 | 16be:0034 | Philips Semi... | SAA7160                  | 100%   |          | 2B8D93B7EC |
| 1131:7160 | 185b:e750 | Philips Semi... | SAA7160                  | 100%   |          | 891F7E03D0 |
| 1131:7160 | 1ae4:0700 | Philips Semi... | SAA7160                  | 100%   |          | E9FCA3B9C8 |
| 1131:7160 | 6281:0001 | Philips Semi... | SAA7160                  | 11.1%  | 4.9.76   | 30EC426B43 |
| 1131:7160 | 6928:0001 | Philips Semi... | SAA7160                  | 100%   |          | 8C8F8EFAB1 |
| 1131:7160 | 6928:0002 | Philips Semi... | SAA7160                  | 100%   |          | 016B4BAE90 |
| 1131:7160 | e517:12ab | Philips Semi... | SAA7160                  | 100%   |          | 786069DE60 |
| 1131:7160 | e519:12ab | Philips Semi... | SAA7160                  | 100%   |          | 786069DE60 |
| 1131:7162 | 11bd:0100 | Philips Semi... | SAA7162                  | 100%   |          | EF8A743A1E |
| 1131:7162 | 11bd:0101 | Philips Semi... | SAA7162                  | 100%   |          | 003EB89135 |
| 1131:7231 | 12ab:0762 | Philips Semi... | SAA7231                  | 100%   |          | 6DFEC77A25 |
| 1131:7231 | 12ab:0763 | Philips Semi... | SAA7231                  | 100%   |          | 6F6F611F59 |
| 1131:7231 | 1461:0b0f | Philips Semi... | SAA7231                  | 100%   |          | 791CA50070 |
| 1131:7231 | 1461:110f | Philips Semi... | SAA7231                  | 100%   |          | 90DFBFB6FA |
| 1131:7231 | 1461:1400 | Philips Semi... | SAA7231                  | 100%   |          | 4F99536247 |
| 1131:7231 | 1461:2a0f | Philips Semi... | SAA7231                  | 100%   |          | FF848E7FFB |
| 1131:7231 | 1461:2b07 | Philips Semi... | SAA7231                  | 100%   |          | 8672A3F85D |
| 1131:7231 | 1461:2b0f | Philips Semi... | SAA7231                  | 100%   |          | F92CB57F54 |
| 1131:7231 | 1461:3301 | Philips Semi... | SAA7231                  | 100%   |          | 7E1176A7C2 |
| 1131:7231 | 1461:7983 | Philips Semi... | SAA7231                  | 100%   |          | 6186ACA9BB |
| 1131:7231 | 16be:0008 | Philips Semi... | SAA7231                  | 100%   |          | 1BA5C50EAD |
| 1131:7231 | 5ace:8000 | Philips Semi... | SAA7231                  | 100%   |          | FA070462FC |
| 1131:7231 | 5ace:8150 | Philips Semi... | SAA7231                  | 100%   |          | 8603D5BDF5 |
| 1131:7231 | 5ace:8201 | Philips Semi... | SAA7231                  | 100%   |          | 75F255A4E2 |
| 11bd:0040 | 11bd:0045 | Pinnacle Sys... | Royal TS Function 1      | 100%   |          | FF0A7B1FC8 |
| 11bd:0041 | 11bd:0045 | Pinnacle Sys... | RoyalTS Function 2       | 100%   |          | FF0A7B1FC8 |
| 11bd:0042 | 11bd:0045 | Pinnacle Sys... | Royal TS Function 3      | 100%   |          | FF0A7B1FC8 |
| 11bd:bede | 11bd:0022 | Pinnacle Sys... | AV/DV Studio Capture ... | 100%   |          | 12C434B6C4 |
| 11bd:bede | 11bd:0023 | Pinnacle Sys... | AV/DV Studio Capture ... | 100%   |          | EBD8A5801D |
| 127e:0010 | 127e:0010 | Winnov, L.P.    | Videum 1000 Plus         | 100%   |          | 37BC71433C |
| 14b5:0200 |           | Creamware       | Scope                    | 100%   |          | 783F215994 |
| 14b5:0300 |           | Creamware       | Pulsar                   | 100%   |          | 783F215994 |
| 14b5:0600 | 14b5:0600 | Creamware       | Pulsar2                  | 100%   |          | 783F215994 |
| 14e4:1570 | 14e4:1570 | Broadcom Inc... | 720p FaceTime HD Camera  | 22.4%  | 4.15.0   | 1A26D7B485 |
| 14e4:1612 | 14e4:2612 | Broadcom        | BCM70012 Video Decode... | 100%   |          | 5495F2E86E |
| 14e4:1615 | 105b:0d77 | Broadcom        | BCM70015 Video Decode... | 100%   |          | B036D312E6 |
| 14e4:1615 | 14e4:1615 | Broadcom Inc... | BCM70015 Video Decode... | 100%   |          | 9910E4B9BB |
| 14f1:8002 | 14f1:0084 | Conexant Sys... | Conexant Multimedia c... | 100%   |          | 380140EB8D |
| 14f1:8803 | 185b:e000 | Conexant Sys... | CX2388x TV Capture Chip  | 100%   |          | 5B85C2F248 |
| 14f1:8804 | 0070:1402 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | 186479593C |
| 14f1:8804 | 0070:6902 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | B4A53FAFC1 |
| 14f1:8804 | 0070:6906 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | BCEE476272 |
| 14f1:8804 | 0070:9002 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | 9531621804 |
| 14f1:8804 | 0070:9202 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | DFF9C11E07 |
| 14f1:8804 | 1822:0023 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | AB36F565A4 |
| 1745:2100 | 1043:48b0 | ViXS Systems    | XCode 2100 Series        | 100%   |          | AD1D92439F |
| 1745:3000 | 104d:9049 | ViXS Systems    | Colossus Encoder Device  | 100%   |          | 2628EBE1BB |
| 1797:6805 |           | Intersil Tec... | HV4000 series DVR card   | 100%   |          | B2C845B843 |
| 1797:6805 | 1797:6804 | Intersil Tec... | HV4000 series DVR card   | 100%   |          | B2C845B843 |
| 1797:6814 | 000a:6814 | Intersil Tec... | TW6816 multimedia vid... | 100%   |          | 91371F93D7 |
| 1797:6815 | 000a:6815 | Intersil Tec... | TW6816 multimedia vid... | 100%   |          | 91371F93D7 |
| 1797:6816 | 000a:6816 | Intersil Tec... | TW6816 multimedia vid... | 100%   |          | 91371F93D7 |
| 1797:6817 | 000a:6817 | Intersil Tec... | TW6816 multimedia vid... | 100%   |          | 91371F93D7 |
| 1822:4e35 | 1822:0048 | Twinhan Tech... | Mantis DTV PCI Bridge... | 100%   |          | CB1A0D9CDD |
| 1a00:0001 | 1a00:0001 |                 | Multimedia controller    | 100%   |          | 16A7890585 |
| 544d:6178 | 6209:0001 | TBS Technolo... | DVB Tuner PCIe Card      | 100%   |          | C7E1E32971 |
| 544d:6178 | 6902:0002 | TBS Technolo... | DVB Tuner PCIe Card      | 100%   |          | B58CD9FD67 |
| 8086:0f38 | 8086:0f31 | Intel           | Atom Processor Z36xxx... | 81.8%  | 4.12.4   | 0A0191D0D3 |
| 8086:0f38 | 8086:7270 | Intel           | Atom Processor Z36xxx... | 93.3%  | 5.0.0    | 0A96B79D5F |
| 8086:1919 | 1025:111e | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | 2D71938FC4 |
| 8086:1919 | 1028:06e6 | Intel           | Xeon E3-1200 v5/E3-15... | 6.2%   | 5.0.0    | 1ABBA3CDA0 |
| 8086:1919 | 1028:07a4 | Intel           | Xeon E3-1200 v5/E3-15... | 33.3%  | 5.0.0    | 75F6A84286 |
| 8086:1919 | 1028:07a5 | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | 87A44EF029 |
| 8086:1919 | 103c:82cb | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | FDB567A59E |
| 8086:1919 | 144d:c135 | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | D7B5599247 |
| 8086:1919 | 152d:1182 | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | 5D3C8DA69A |
| 8086:1919 | 17aa:2241 | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | 1038A34C39 |
| 8086:1919 | 17aa:3812 | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | 57EC66B289 |
| 8086:1919 | 17aa:382f | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | 1DD80D33E5 |
| 8086:1919 | 19e5:3e00 | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | A76E9D9514 |
| 8086:1919 | 8086:1919 | Intel           | Xeon E3-1200 v5/E3-15... | 57.1%  | 5.0.0    | 707E0DB074 |
| 8086:1919 | 8086:2015 | Intel           | Xeon E3-1200 v5/E3-15... | 47.7%  | 5.0.0    | A43311F999 |
| 8086:22b8 | 1025:1021 | Intel           | Atom/Celeron/Pentium ... | 100%   |          | 663247803F |
| 8086:22b8 | 1025:106e | Intel           | Atom/Celeron/Pentium ... | 100%   |          | 425D589D65 |
| 8086:22b8 | 1025:113a | Intel           | Atom/Celeron/Pentium ... | 100%   |          | FBF9B74A34 |
| 8086:22b8 | 1028:06ea | Intel           | Atom/Celeron/Pentium ... | 60%    | 4.20.1   | 743979C6E7 |
| 8086:22b8 | 103c:813e | Intel           | Atom/Celeron/Pentium ... | 75%    | 5.0.0    | 923CBD5735 |
| 8086:22b8 | 103c:827c | Intel           | Atom/Celeron/Pentium ... | 75%    | 5.0.0    | DD16DF4133 |
| 8086:22b8 | 1043:13a0 | Intel           | Atom/Celeron/Pentium ... | 69.2%  | 5.0.0    | 1EB4640C84 |
| 8086:22b8 | 1043:1400 | Intel           | Atom/Celeron/Pentium ... | 50%    | 5.0.11   | 838DD8C3AC |
| 8086:22b8 | 1043:1c60 | Intel           | Atom/Celeron/Pentium ... | 20%    | 5.0.0    | 5FCF1662DB |
| 8086:22b8 | 1071:a126 | Intel           | Atom/Celeron/Pentium ... | 100%   |          | F2981C1775 |
| 8086:22b8 | 1297:2063 | Intel           | Atom/Celeron/Pentium ... | 50%    | 5.0.0    | 18AE13312B |
| 8086:22b8 | 17aa:222a | Intel           | Atom/Celeron/Pentium ... | 50%    | 5.0.0    | 5AF55E5191 |
| 8086:22b8 | 17aa:3809 | Intel           | Atom/Celeron/Pentium ... | 18.2%  | 5.0.0    | 85AC9B2B53 |
| 8086:22b8 | 17aa:38e3 | Intel           | Atom/Celeron/Pentium ... | 50%    | 5.0.0    | CE2895A69A |
| 8086:22b8 | 8086:7270 | Intel           | Atom/Celeron/Pentium ... | 62.4%  | 4.20.0   | AE477CA654 |
| 8086:5a88 |           | Intel           | Celeron N3350/Pentium... | 100%   |          | 0BEDF4D656 |
| 8086:9d32 |           | Intel           | Skylake-U/Y Camera IO... | 33.3%  | 5.0.0    | C596B50DF9 |
| 8086:9d32 | 1028:07a5 | Intel           | Skylake-U/Y Camera IO... | 100%   |          | 87A44EF029 |
| 8086:9d32 | 1043:1410 | Intel           | Skylake-U/Y Camera IO... | 100%   |          | 0B5AD4104E |
| 8086:9d32 | 17aa:380c | Intel           | Skylake-U/Y Camera IO... | 33.3%  | 4.18.0   | 1D220D1155 |
| 8086:9d32 | 8086:7270 | Intel           | Skylake-U/Y Camera IO... | 23.6%  | 4.18.0   | 7F3BC4B89E |
| 8086:9d32 | 8086:9d32 | Intel           | Skylake-U/Y Camera IO... | 28.6%  | 4.18.0   | 23C4F883A7 |
| dd01:0006 | dd01:0022 | Digital Devices | Cine V7                  | 100%   |          | FCF4AFE5C6 |

### Net/ethernet (PCI)

47 out of 3975 (1.18%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 0000:0200 | 002c:0200 |                 | Ethernet controller      | 100%   |          | 32AE4212DF |
| 000c:0000 | 1043:83a3 |                 | Ethernet controller      | 100%   |          | B5189C3BF2 |
| 10ec:0139 | 10bd:0320 | Realtek Semi... | RTL-8139/8139C/8139C+... | 100%   |          | 305C35F50C |
| 10ec:3000 | 1025:132d | Realtek Semi... | Killer E3000 2.5 Giga... | 100%   |          | 17674B4CBD |
| 10ec:3000 | 1025:1375 | Realtek Semi... | Killer E3000 2.5 Giga... | 66.7%  | 5.4.5    | 54109739EB |
| 10ec:3000 | 1028:08c4 | Realtek Semi... | Killer E3000 2.5 Giga... | 100%   |          | BA3ACE6663 |
| 10ec:8125 | 1043:879b | Realtek Semi... | RTL8125 2.5GbE Contro... | 100%   |          | EB051E1278 |
| 10ec:8131 | 10ec:8131 | Realtek Semi... | RTL8131 PCIe Fast Eth... | 100%   |          | 4E43962152 |
| 10ec:8136 | 1028:0555 | Realtek Semi... | RTL810xE PCI Express ... | 5%     | 4.1.15   | A7211B4E35 |
| 10ec:8136 | 103c:1484 | Realtek Semi... | RTL810xE PCI Express ... | 7.7%   | 4.9.60   | C7734FBAE0 |
| 10ec:8136 | 103c:306b | Realtek Semi... | RTL810xE PCI Express ... | 25%    | 3.14.44  | 93C0EF7223 |
| 10ec:8136 | 103c:820c | Realtek Semi... | RTL810xE PCI Express ... | 25%    | 4.1.25   | 21A7695D56 |
| 10ec:8136 | 1462:7529 | Realtek Semi... | RTL810xE PCI Express ... | 4.2%   | 3.14.44  | 99777B72F9 |
| 10ec:8136 | 17aa:381f | Realtek Semi... | RTL810xE PCI Express ... | 8%     | 4.1.34   | 1952B1CCF3 |
| 10ec:8168 | 1025:0866 | Realtek Semi... | RTL8111/8168/8411 PCI... | 3.8%   | 3.10.51  | 8B133744C1 |
| 10ec:8168 | 1025:0918 | Realtek Semi... | RTL8111/8168/8411 PCI... | 2.1%   | 4.1.19   | 8A92A65C2E |
| 10ec:8168 | 1025:125c | Realtek Semi... | RTL8111/8168/8411 PCI... | 2.8%   | 4.18.0   | 6AEFA7E06C |
| 10ec:8168 | 1028:0870 | Realtek Semi... | RTL8111/8168/8411 PCI... | 16.7%  | 4.15.0   | B0DF3027CF |
| 10ec:8168 | 103c:180d | Realtek Semi... | RTL8111/8168/8411 PCI... | 3%     | 3.10.42  | 41A6D6B87B |
| 10ec:8168 | 1043:1447 | Realtek Semi... | RTL8111/8168/8411 PCI... | 8.3%   | 3.14.44  | F23B5BF0DA |
| 10ec:8168 | 1043:1477 | Realtek Semi... | RTL8111/8168/8411 PCI... | 10%    | 4.9.60   | BEE323A814 |
| 10ec:8168 | 1043:14f7 | Realtek Semi... | RTL8111/8168/8411 PCI... | 4.9%   | 3.14.44  | CE99670CEB |
| 10ec:8168 | 1043:200f | Realtek Semi... | RTL8111/8168/8411 PCI... | 0.3%   | 3.10.34  | 91D9C778CB |
| 10ec:8168 | 10ec:8168 | Realtek Semi... | RTL8111/8168/8411 PCI... | 0.5%   | 3.10.0   | 021596F9B3 |
| 10ec:8168 | 1297:2033 | Realtek Semi... | RTL8111/8168/8411 PCI... | 7.4%   | 4.9.20   | 51273F53DF |
| 10ec:8168 | 1458:e000 | Realtek Semi... | RTL8111/8168/8411 PCI... | 0.1%   | 3.10.0   | C04DCDD5D7 |
| 10ec:8168 | 14c0:0059 | Realtek Semi... | RTL8111/8168/8411 PCI... | 100%   |          | 42B3F11A1E |
| 10ec:8168 | 1558:1323 | Realtek Semi... | RTL8111/8168/8411 PCI... | 22.2%  | 4.15.0   | 75848692B4 |
| 10ec:8168 | 1558:1550 | Realtek Semi... | RTL8111/8168/8411 PCI... | 2.2%   | 3.14.33  | A0EB5DA51A |
| 10ec:8168 | 17aa:21fe | Realtek Semi... | RTL8111/8168/8411 PCI... | 16.7%  | 3.10.0   | E17730F707 |
| 1186:4200 | 1186:1103 | D-Link System   | DFE-520TX Fast Ethern... | 100%   |          | 790E740601 |
| 14e4:16a3 | 14e4:16a3 | Broadcom Inc... | NetXtreme BCM57786 Gi... | 100%   |          | 96265D2456 |
| 14e4:16a3 | 14e4:16b4 | Broadcom Inc... | NetXtreme BCM57786 Gi... | 100%   |          | 0E94266411 |
| 14e4:52a3 | d3a6:afcd | Broadcom Lim... | Ethernet controller      | 100%   |          | 191BA97155 |
| 168c:abcd |           | Qualcomm Ath... | Osprey Emulation Wire... | 100%   |          | 76C675CD98 |
| 1a47:0003 | 0000:0200 | 3DSP            | WLAN and Bluetooth Card  | 100%   |          | 3A17145633 |
| 8086:0000 | 8086:0000 | Intel           | PROSet/Wireless WiFi ... | 100%   |          | 418C3E7B73 |
| 8086:0d4f | 17aa:2292 | Intel           | Ethernet Connection (... | 66.7%  | 5.3.0    | 1820A998EC |
| 8086:107c | 8086:1376 | Intel           | 82541PI Gigabit Ether... | 2%     | 2.6.32   | F801FAB1AD |
| 8086:10aa | 8086:0000 | Intel           | Ethernet controller      | 100%   |          | CBBE408AAC |
| 8086:1229 | 8086:0050 | Intel           | 82557/8/9/0/1 Etherne... | 15.4%  | 3.10.0   | E568C873E2 |
| 8086:15b8 | 1043:8672 | Intel           | Ethernet Connection (... | 0.4%   | 4.1.15   | 51B31F180E |
| 8086:15bc | 1028:0851 | Intel           | Ethernet Connection (... | 100%   |          | 05D6B79D2F |
| 8086:15bc | 1462:7b23 | Intel           | Ethernet Connection (... | 33.3%  | 4.18.0   | 37076CEBE8 |
| 8086:15bc | 1849:15bc | Intel           | Ethernet Connection (... | 7.7%   | 4.13.0   | BA39531B87 |
| 8086:37cc | 103c:81c7 | Intel           | Ethernet Connection X722 | 100%   |          | 931EA9A398 |
| 8086:37cc | 15d9:0000 | Intel           | Ethernet Connection X722 | 100%   |          | 2794B14FEE |

### Net/wireless (PCI)

142 out of 915 (15.52%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 104c:8400 | 1186:3b01 | Texas Instru... | ACX 100 22Mbps Wirele... | 100%   |          | E804B92A1F |
| 104c:9066 | 1086:3b04 | Texas Instru... | ACX 111 54Mbps Wirele... | 100%   |          | DBFFE622A8 |
| 104c:9066 | 1186:3b04 | Texas Instru... | ACX 111 54Mbps Wirele... | 100%   |          | 713C36EFA0 |
| 10ec:8176 | 1a3b:1139 | Realtek Semi... | RTL8188CE 802.11b/g/n... | 2.9%   | 3.14.33  | 51273F53DF |
| 10ec:8179 | 17aa:0179 | Realtek Semi... | RTL8188EE Wireless Ne... | 6.2%   | 3.14.44  | 08BB09B100 |
| 10ec:8185 | 10ec:8225 | Realtek Semi... | RTL-8185 IEEE 802.11a... | 2.1%   | 3.14.44  | E44354FF81 |
| 10ec:8190 | 10ec:8190 | Realtek Semi... | RTL8190 802.11n PCI W... | 100%   |          | 96A75ACB49 |
| 10ec:8723 | 10ec:0726 | Realtek Semi... | RTL8723AE PCIe Wirele... | 1%     | 3.18.10  | 598F621727 |
| 10ec:8723 | 10ec:0733 | Realtek Semi... | RTL8723AE PCIe Wirele... | 100%   |          | 2F246CACD8 |
| 10ec:8821 | 1a3b:2161 | Realtek Semi... | RTL8821AE 802.11ac PC... | 10%    | 3.14.44  | 5EEDC9CEE8 |
| 10ec:b723 | 1025:b734 | Realtek Semi... | RTL8723BE PCIe Wirele... | 15.4%  | 4.1.10   | DE10405623 |
| 10ec:b723 | 103c:2231 | Realtek Semi... | RTL8723BE PCIe Wirele... | 32.1%  | 3.18.11  | B301F51204 |
| 10ec:b723 | 10ec:b729 | Realtek Semi... | RTL8723BE PCIe Wirele... | 30.3%  | 3.17.4   | FD5BC52C49 |
| 10ec:b723 | 10ec:b733 | Realtek Semi... | RTL8723BE PCIe Wirele... | 14.3%  | 4.1.38   | BDAF59B6EB |
| 10ec:b723 | 11ad:1723 | Realtek Semi... | RTL8723BE PCIe Wirele... | 3.3%   | 4.9.9    | E6285FD8C3 |
| 10ec:b723 | 17aa:b728 | Realtek Semi... | RTL8723BE PCIe Wirele... | 35.3%  | 3.18.14  | 02D1977887 |
| 10ec:b723 | 17aa:b736 | Realtek Semi... | RTL8723BE PCIe Wirele... | 13.9%  | 3.18.16  | 8C16B6C71F |
| 10ec:b723 | 1a3b:2159 | Realtek Semi... | RTL8723BE PCIe Wirele... | 5.9%   | 4.1.15   | DDF48A7B95 |
| 10ec:b723 | 1b9a:2485 | Realtek Semi... | RTL8723BE PCIe Wirele... | 8.3%   | 4.3.3    | D57B5C86E0 |
| 10ec:b822 | 103c:831b | Realtek Semi... | RTL8822BE 802.11a/b/g... | 5.5%   | 4.15.0   | BAA9C6C33C |
| 10ec:b822 | 1043:8746 | Realtek Semi... | RTL8822BE 802.11a/b/g... | 2.2%   | 4.15.0   | 27EB064D7D |
| 10ec:b822 | 1a3b:2950 | Realtek Semi... | RTL8822BE 802.11a/b/g... | 3%     | 4.13.0   | B6B40DE397 |
| 10ec:c821 | 103c:831a | Realtek Semi... | RTL8821CE 802.11ac PC... | 97.6%  | 5.0.6    | B6F032A1EE |
| 10ec:c821 | 10ec:c821 | Realtek Semi... | RTL8821CE 802.11ac PC... | 100%   |          | F71EFE50CF |
| 10ec:c821 | 10ec:c827 | Realtek Semi... | RTL8821CE 802.11ac PC... | 71.4%  | 4.15.0   | C8EE1F4CA3 |
| 10ec:c821 | 17aa:c024 | Realtek Semi... | RTL8821CE 802.11ac PC... | 96.2%  | 4.9.124  | C65ABD0640 |
| 10ec:c821 | 1a3b:3040 | Realtek Semi... | RTL8821CE 802.11ac PC... | 100%   |          | DAE31E24F3 |
| 10ec:c821 | 1a3b:3041 | Realtek Semi... | RTL8821CE 802.11ac PC... | 33.3%  | 5.3.11   | F39E5E0553 |
| 11ab:1fa6 | 1043:138f | Marvell Tech... | Marvell W8300 802.11 ... | 100%   |          | E75F4538BC |
| 11ab:1fa6 | 1186:3b09 | Marvell Tech... | Marvell W8300 802.11 ... | 100%   |          | 4BDC000ABE |
| 11ab:1fa7 | 1043:138f | Marvell Tech... | 88W8310 and 88W8000G ... | 100%   |          | 436FC401D1 |
| 11ab:1faa | 11ab:1faa | Marvell Tech... | 88w8335 [Libertas] 80... | 100%   |          | A596A275D3 |
| 11ab:1faa | 1385:6b00 | Marvell Tech... | 88w8335 [Libertas] 80... | 100%   |          | F30CD368D8 |
| 14c3:7630 | 103c:197c | MEDIATEK        | MT7630e 802.11bgn Wir... | 100%   |          | A7E6CBC45B |
| 14c3:7630 | 105b:e074 | MEDIATEK        | MT7630e 802.11bgn Wir... | 100%   |          | 2F7C16AF18 |
| 14c3:7630 | 105b:e084 | MEDIATEK        | MT7630e 802.11bgn Wir... | 100%   |          | DF4413AF58 |
| 14e4:4311 | 103c:1364 | Broadcom Inc... | BCM4311 802.11b/g WLAN   | 2.1%   | 3.14.33  | 71764E2EB9 |
| 14e4:4311 | 1468:0316 | Broadcom Inc... | BCM4311 802.11b/g WLAN   | 100%   |          | 7F0BB0CC92 |
| 14e4:4315 | 103c:1508 | Broadcom Inc... | BCM4312 802.11b/g LP-PHY | 1.5%   | 3.14.44  | D0F06C8499 |
| 14e4:4318 | 1468:0312 | Broadcom Lim... | BCM4318 [AirForce One... | 19.2%  | 3.10.34  | A28F7B2623 |
| 14e4:4324 | 1028:0003 | Broadcom Inc... | BCM4309 802.11abg Wir... | 50%    | 4.15.0   | 0077E52877 |
| 14e4:4328 | 106b:0088 | Broadcom Inc... | BCM4321 802.11a/b/g/n    | 3.8%   | 4.1.15   | 985A14858E |
| 14e4:4328 | 106b:0090 | Broadcom Lim... | BCM4321 802.11a/b/g/n    | 4.8%   | 4.1.22   | 030A81E657 |
| 14e4:432b | 1028:000d | Broadcom Inc... | BCM4322 802.11a/b/g/n... | 6.2%   | 3.10.19  | 103788F3AC |
| 14e4:432b | 103c:1510 | Broadcom        | BCM4322 802.11a/b/g/n... | 100%   |          | 23C8DE7582 |
| 14e4:4353 | 1028:000e | Broadcom Inc... | BCM43224 802.11a/b/g/n   | 5.3%   | 4.1.15   | E572489472 |
| 14e4:4353 | 106b:0093 | Broadcom Inc... | BCM43224 802.11a/b/g/n   | 2.3%   | 4.1.15   | 4E11213A56 |
| 14e4:4357 | 105b:e021 | Broadcom Inc... | BCM43225 802.11b/g/n     | 2.7%   | 3.14.25  | DDD532FC51 |
| 14e4:4358 | 105b:e040 | Broadcom Inc... | BCM43227 802.11b/g/n     | 1.5%   | 3.14.33  | 9D65BC9B14 |
| 14e4:4359 | 1028:0014 | Broadcom Inc... | BCM43228 802.11a/b/g/n   | 3.4%   | 3.14.44  | 9F82A1A551 |
| 14e4:4359 | 103c:182c | Broadcom Inc... | BCM43228 802.11a/b/g/n   | 3.3%   | 4.1.25   | 10B4B2CF4D |
| 14e4:4359 | 103c:2135 | Broadcom Inc... | BCM43228 802.11a/b/g/n   | 50%    | 4.1.25   | 3E13F8A157 |
| 14e4:4359 | 1043:850c | Broadcom Inc... | BCM43228 802.11a/b/g/n   | 6.8%   | 3.14.44  | 7E0E64D8B4 |
| 14e4:4359 | 105b:e04b | Broadcom Inc... | BCM43228 802.11a/b/g/n   | 1.5%   | 3.14.44  | EAC775D35E |
| 14e4:4359 | 105b:e08b | Broadcom Lim... | BCM43228 802.11a/b/g/n   | 10%    | 4.1.34   | 0D43FC94FE |
| 14e4:4359 | 11ad:6603 | Broadcom Inc... | BCM43228 802.11a/b/g/n   | 7.7%   | 4.1.15   | C6F99AC92E |
| 14e4:4359 | 14e4:05e2 | Broadcom Inc... | BCM43228 802.11a/b/g/n   | 7.3%   | 3.10.42  | D58DD0D4E0 |
| 14e4:4365 | 1028:0016 | Broadcom Inc... | BCM43142 802.11b/g/n     | 5.9%   | 3.14.33  | 7CEA716D9E |
| 14e4:4365 | 103c:2230 | Broadcom Inc... | BCM43142 802.11b/g/n     | 37.1%  | 3.14.44  | DE0D0A86F2 |
| 14e4:4365 | 103c:804a | Broadcom Inc... | BCM43142 802.11b/g/n     | 29.2%  | 4.1.15   | 7C960F54DF |
| 14e4:4365 | 105b:e071 | Broadcom Inc... | BCM43142 802.11b/g/n     | 37.9%  | 3.14.44  | B9133671A8 |
| 14e4:4365 | 105b:e07e | Broadcom Inc... | BCM43142 802.11b/g/n     | 25%    | 3.14.44  | 95737FD2D6 |
| 14e4:4365 | 11ad:6605 | Broadcom Inc... | BCM43142 802.11b/g/n     | 4.3%   | 3.14.33  | 4E37AD043D |
| 14e4:4365 | 11ad:6645 | Broadcom Inc... | BCM43142 802.11b/g/n     | 32.7%  | 3.14.33  | 6B82A86DF6 |
| 14e4:4365 | 11ad:6655 | Broadcom Inc... | BCM43142 802.11b/g/n     | 82.4%  | 4.9.9    | 670B794189 |
| 14e4:4365 | 11ad:6675 | Broadcom Lim... | BCM43142 802.11b/g/n     | 32.8%  | 3.14.44  | ADACEBAE45 |
| 14e4:4365 | 17aa:0611 | Broadcom Inc... | BCM43142 802.11b/g/n     | 5.3%   | 3.14.25  | 82A9861AFD |
| 14e4:4365 | 17aa:0621 | Broadcom Inc... | BCM43142 802.11b/g/n     | 13.7%  | 3.14.25  | 6E6E5E6FBA |
| 14e4:4365 | 1a3b:2155 | Broadcom Inc... | BCM43142 802.11b/g/n     | 100%   |          | 1274A24ED0 |
| 14e4:4365 | 1b9a:3002 | Broadcom        | BCM43142 802.11b/g/n     | 82.4%  | 4.1.25   | 4B9E002F83 |
| 14e4:43a0 | 1043:85df | Broadcom Inc... | BCM4360 802.11ac Wire... | 14.3%  | 4.15.0   | 8CE5DB772C |
| 14e4:43a0 | 1043:8659 | Broadcom Inc... | BCM4360 802.11ac Wire... | 14.3%  | 4.15.0   | 2301984979 |
| 14e4:43a0 | 106b:0117 | Broadcom Lim... | BCM4360 802.11ac Wire... | 25%    | 4.18.0   | 3A2A390F59 |
| 14e4:43a0 | 106b:0135 | Broadcom Inc... | BCM4360 802.11ac Wire... | 75%    | 5.0.0    | 9F3D443A21 |
| 14e4:43a0 | 14e4:0619 | Broadcom Inc... | BCM4360 802.11ac Wire... | 10%    | 4.15.0   | 3AFE42946D |
| 14e4:43ae | 17aa:0622 | Broadcom Inc... | BCM43162 802.11ac Wir... | 100%   |          | C1C9DD614A |
| 14e4:43b1 | 1028:0019 | Broadcom Lim... | BCM4352 802.11ac Wire... | 60%    | 5.0.9    | BA50FFBC59 |
| 14e4:43b1 | 103c:2154 | Broadcom Lim... | BCM4352 802.11ac Wire... | 50%    | 4.18.0   | 420C7722C6 |
| 14e4:43b1 | 1043:855c | Broadcom Inc... | BCM4352 802.11ac Wire... | 50%    | 4.15.0   | A16A7137A3 |
| 14e4:43b1 | 1043:85ba | Broadcom Inc... | BCM4352 802.11ac Wire... | 75%    | 4.18.0   | C898033824 |
| 14e4:43b1 | 17aa:0623 | Broadcom Lim... | BCM4352 802.11ac Wire... | 16.7%  | 4.15.0   | FC0DC30BF0 |
| 14e4:43b1 | 1a3b:2b23 | Broadcom Inc... | BCM4352 802.11ac Wire... | 100%   |          | 14ABE97F88 |
| 14e4:43ba | 106b:014a | Broadcom Inc... | BCM43602 802.11ac Wir... | 20%    | 4.19.88  | 5984E1BBAC |
| 14e4:43ba | 106b:0173 | Broadcom Inc... | BCM43602 802.11ac Wir... | 100%   |          | 6F3816ABBD |
| 14e4:4464 | 106b:07bf | Broadcom Inc... | BCM4364 802.11ac Wire... | 100%   |          | 7F2D68A6A2 |
| 14e4:4727 | 1028:0010 | Broadcom Inc... | BCM4313 802.11bgn Wir... | 2.9%   | 4.13.0   | EFC321CCD7 |
| 14e4:4727 | 1028:0012 | Broadcom Lim... | BCM4313 802.11bgn Wir... | 60%    | 4.15.0   | 40D48C06A1 |
| 14e4:4727 | 1028:0015 | Broadcom Inc... | BCM4313 802.11bgn Wir... | 25%    | 4.15.0   | 6251A0DB90 |
| 14e4:4727 | 103c:1483 | Broadcom Inc... | BCM4313 802.11bgn Wir... | 3.8%   | 4.1.34   | EA7FCEAF2C |
| 14e4:4727 | 103c:1795 | Broadcom Inc... | BCM4313 802.11bgn Wir... | 7.7%   | 3.10.42  | 06AA196398 |
| 14e4:4727 | 105b:e042 | Broadcom Inc... | BCM4313 802.11bgn Wir... | 12.5%  | 4.15.0   | D148A20413 |
| 14e4:4727 | 144f:7175 | Broadcom Inc... | BCM4313 802.11bgn Wir... | 12.5%  | 4.15.0   | 93629DD831 |
| 14e4:4727 | 144f:7179 | Broadcom Inc... | BCM4313 802.11bgn Wir... | 4%     | 3.10.34  | A92AED714F |
| 14e4:4727 | 14e4:0510 | Broadcom Inc... | BCM4313 802.11bgn Wir... | 25%    | 4.2.6    | A911172500 |
| 14e4:4727 | 14e4:051b | Broadcom Inc... | BCM4313 802.11bgn Wir... | 3.8%   | 2.6.32   | 4437DCCAB2 |
| 14e4:4727 | 14e4:0587 | Broadcom Lim... | BCM4313 802.11bgn Wir... | 20%    | 4.15.0   | 8D6C57DC63 |
| 14e4:4727 | 14e4:0608 | Broadcom Inc... | BCM4313 802.11bgn Wir... | 20%    | 4.4.0    | 65C68A39C0 |
| 14e4:4727 | 185f:051a | Broadcom Inc... | BCM4313 802.11bgn Wir... | 5.9%   | 4.9.0    | 86A1DD9578 |
| 14e4:4727 | 1a3b:2a47 | Broadcom Lim... | BCM4313 802.11bgn Wir... | 33.3%  | 3.10.34  | 79326DA8CA |
| 167b:2116 | 340f:187e | ZyDAS Techno... | ZD1212B Wireless Adapter | 100%   |          | C399CBB5F3 |
| 168c:001c | 103c:137b | Qualcomm Ath... | AR242x / AR542x Wirel... | 1.3%   | 3.14.33  | 93C0EF7223 |
| 168c:002b | 103c:1461 | Qualcomm Ath... | AR9285 Wireless Netwo... | 0.8%   | 3.14.33  | F4DE983D96 |
| 168c:002d | 168c:0300 | Qualcomm Ath... | AR9227 Wireless Netwo... | 3%     | 3.14.33  | AA24EEDD97 |
| 168c:002e | 105b:e034 | Qualcomm Ath... | AR9287 Wireless Netwo... | 0.5%   | 3.10.19  | 8FE3AF49FB |
| 168c:0032 | 11ad:6608 | Qualcomm Ath... | AR9485 Wireless Netwo... | 2.8%   | 3.14.33  | 67009EFFAA |
| 168c:0032 | 11ad:6617 | Qualcomm Ath... | AR9485 Wireless Netwo... | 0.5%   | 3.14.25  | 86D2D3B0E1 |
| 168c:0032 | 11ad:6628 | Qualcomm Ath... | AR9485 Wireless Netwo... | 1.5%   | 3.14.44  | 469E04E0D5 |
| 168c:0036 | 11ad:0642 | Qualcomm Ath... | QCA9565 / AR9565 Wire... | 0.4%   | 3.10.51  | 8D6D195DA2 |
| 168c:0036 | 11ad:0803 | Qualcomm Ath... | QCA9565 / AR9565 Wire... | 2.2%   | 3.14.44  | 401BBED185 |
| 168c:0037 | 1a3b:1195 | Qualcomm Ath... | AR9485 Wireless Netwo... | 50%    | 4.9.20   | CE8124E5F4 |
| 168c:0037 | 1a3b:2100 | Qualcomm Ath... | AR9485 Wireless Netwo... | 3.5%   | 3.14.25  | 0F8E9B7955 |
| 168c:0042 | 11ad:0806 | Qualcomm Ath... | QCA9377 802.11ac Wire... | 13%    | 4.4.0    | ECB6A89DFC |
| 168c:0042 | 11ad:08a6 | Qualcomm Ath... | QCA9377 802.11ac Wire... | 0.3%   | 3.10.0   | E7395D0EE2 |
| 168c:0042 | 17aa:0901 | Qualcomm Ath... | QCA9377 802.11ac Wire... | 0.5%   | 4.4.0    | C23D0EF968 |
| 168c:0042 | 17aa:4035 | Qualcomm Ath... | QCA9377 802.11ac Wire... | 1%     | 4.8.0    | C3352134E9 |
| 17fe:2220 | 1468:0310 | InProComm       | IPN 2220 802.11g         | 100%   |          | E9BD04F647 |
| 1814:0301 | 1814:2561 | Ralink          | RT2561/RT61 802.11g PCI  | 3.4%   | 3.14.33  | E40B76E473 |
| 1814:3062 | 1814:3062 | Ralink          | RT3062 Wireless 802.1... | 3.7%   | 3.14.44  | 9D9E2DB550 |
| 1814:3090 | 1462:6894 | Ralink          | RT3090 Wireless 802.1... | 100%   |          | E40B76E473 |
| 1814:3290 | 103c:18ec | Ralink          | RT3290 Wireless 802.1... | 0.4%   | 3.14.15  | 434304B738 |
| 1814:539f | 103c:1637 | Ralink          | RT5390 [802.11 b/g/n ... | 2.6%   | 3.14.44  | ED2FBC90A0 |
| 1814:5592 | 1043:851a | Ralink          | RT5592 PCIe Wireless ... | 100%   |          | 08D84A1FF9 |
| 1814:5592 | 1814:5592 | Ralink          | RT5592 PCIe Wireless ... | 100%   |          | 760C31A638 |
| 8086:02f0 | 8086:0074 | Intel           | Wireless-AC 9462         | 75%    | 5.4.0    | 4EA8D503AE |
| 8086:0893 | 8086:0262 | Intel           | Centrino Wireless-N 135  | 6.2%   | 3.14.25  | 2DD89E3983 |
| 8086:08b1 | 8086:4070 | Intel           | Wireless 7260            | 0.5%   | 3.14.25  | 550460AAAC |
| 8086:08b4 | 8086:8270 | Intel           | Wireless 3160            | 2.2%   | 3.14.44  | AB6BD693BE |
| 8086:095a | 8086:5400 | Intel           | Wireless 7265            | 5.3%   | 4.1.25   | 0A99E4D896 |
| 8086:24f3 | 8086:0130 | Intel           | Wireless 8260            | 4.5%   | 4.9.9    | B612D89D47 |
| 8086:24f3 | 8086:1010 | Intel           | Wireless 8260            | 1.2%   | 4.1.15   | 43DF678BD3 |
| 8086:24f3 | 8086:1130 | Intel           | Wireless 8260            | 2.3%   | 4.4.0    | 3A43711362 |
| 8086:24fd | 8086:0010 | Intel           | Wireless 8265 / 8275     | 0.4%   | 3.10.0   | 7D7E6AD5D5 |
| 8086:24fd | 8086:9010 | Intel           | Wireless 8265 / 8275     | 1.3%   | 4.9.9    | B78B406093 |
| 8086:2526 | 8086:0014 | Intel           | Wireless-AC 9260         | 2.3%   | 4.15.0   | AA47C9C76D |
| 8086:3165 | 8086:4010 | Intel           | Wireless 3165            | 0.4%   | 4.1.15   | 5738D326F6 |
| 8086:3165 | 8086:8110 | Intel           | Wireless 3165            | 2.3%   | 4.9.20   | 48E3CC8030 |
| 8086:3166 | 8086:4210 | Intel           | Dual Band Wireless-AC... | 0.7%   | 4.1.15   | 1B722DF896 |
| 8086:4222 | 103c:135c | Intel           | PRO/Wireless 3945ABG ... | 2.4%   | 3.14.25  | 9EDB73DD0E |
| 8086:4223 | 8086:1040 | Intel           | PRO/Wireless 2915ABG ... | 50%    | 4.18.0   | 8488B3D0B9 |
| 8086:9df0 | 8086:2034 | Intel           | Cannon Point-LP CNVi ... | 12.5%  | 4.18.0   | D60073EAD5 |
| 8086:9df0 | 8086:42a4 | Intel           | Cannon Point-LP CNVi ... | 4.5%   | 4.15.0   | B6DF9FEC5F |
| 8086:a370 | 8086:0034 | Intel           | Wireless-AC 9560 [Jef... | 0.8%   | 3.10.0   | 039A05F3EB |

### Network (PCI)

34 out of 792 (4.29%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 0000:0002 | 002c:0000 |                 | Network controller       | 100%   |          | 3859A12973 |
| 0000:0210 | 002c:0000 |                 | Network controller       | 100%   |          | 3859A12973 |
| 0000:0210 | 1105:8300 |                 |                          | 100%   |          | 3859A12973 |
| 1006:3106 | 1086:1405 | Reply Group     | Reply Ethernet contro... | 100%   |          | F597A38FF5 |
| 10ec:8125 | 1458:e000 | Realtek Semi... | RTL8125 2.5GbE Contro... | 100%   |          | B51C7D1EE8 |
| 10ec:8125 | 1849:8125 | Realtek Semi... | RTL8125 2.5GbE Contro... | 33.3%  | 5.0.0    | B89B031EB9 |
| 10ec:c822 | 1a3b:3750 | Realtek Semi... | 8822CE Wireless LAN 8... | 100%   |          | 25325D332C |
| 10ec:d723 | 103c:8319 | Realtek Semi... | RTL8723DE Wireless Ne... | 98.5%  | 4.9.41   | 16EA8E9AC4 |
| 1106:1106 | 1186:1405 | VIA Technolo... | VT82C570MV               | 100%   |          | 1EF54091BE |
| 1106:3065 | 1849:3065 | VIA Technolo... | VT6102/VT6103 [Rhine-II] | 14.8%  | 3.10.0   | 6FAC734286 |
| 1106:3106 | 1106:0105 | VIA Technolo... | VT6105/VT6106S [Rhine... | 55.6%  | 4.1.16   | A6659EE127 |
| 1260:3886 | 16be:2004 | Intersil        | ISL3886 [Prism Javeli... | 20%    | 5.0.0    | ACACF55F1F |
| 12d0:2103 | 12d0:2103 | GDE Systems     | GDE Network controller   | 100%   |          | 8C5E6472B2 |
| 14e4:4488 | 106b:0870 | Broadcom Inc... | BCM4377b Wireless Net... | 100%   |          | D3A040508D |
| 14e4:5fa0 | 106b:0870 | Broadcom Inc... | Network controller       | 100%   |          | D3A040508D |
| 168c:004a | 15aa:4035 | Qualcomm Ath... | Network controller       | 100%   |          | 04F6BB6978 |
| 168c:0063 | 168c:3071 | Qualcomm Ath... | Network controller       | 100%   |          | 8F99628F42 |
| 1810:3060 | 8001:0000 | HCL Technolo... | Network controller       | 100%   |          | CFD57C3B89 |
| 8086:0082 | 8086:1321 | Intel           | Centrino Advanced-N 6... | 0.6%   | 3.14.33  | A2002798AC |
| 8086:093c | 8086:0181 | Intel           | Wireless Gigabit 1726... | 100%   |          | D33E07EEAB |
| 8086:093c | 8086:2181 | Intel           | Wireless Gigabit 1726... | 100%   |          | 3C44DE609A |
| 8086:10d3 | 8086:a01f | Intel           | 82574L Gigabit Networ... | 1.6%   | 3.10.0   | 9B75A42A1E |
| 8086:10de | 103c:3034 | Intel           | 82567LM-3 Gigabit Net... | 4.8%   | 3.14.44  | 5DC57BDE0C |
| 8086:10f0 | 1019:1324 | Intel           | 82578DC Gigabit Netwo... | 100%   |          | 50B445BA68 |
| 8086:1502 | 1028:0493 | Intel           | 82579LM Gigabit Netwo... | 1.7%   | 3.14.33  | 3F252A50FB |
| 8086:1502 | 103c:179b | Intel           | 82579LM Gigabit Netwo... | 5%     | 3.14.44  | 18835A8B6C |
| 8086:1502 | 1043:849c | Intel           | 82579LM Gigabit Netwo... | 100%   |          | 44AA7CC920 |
| 8086:1539 | 1458:e000 | Intel           | I211 Gigabit Network ... | 0.9%   | 4.9.0    | 6BEE5D9A22 |
| 8086:24fd | 8086:1010 | Intel           | Wireless 8265 / 8275     | 0.4%   | 4.8.15   | BF84028302 |
| 8086:2723 | 1a56:1654 | Intel           | Wi-Fi 6 AX200            | 20%    | 5.0.0    | D20FB61951 |
| 8086:2723 | 8086:0080 | Intel           | Wi-Fi 6 AX200            | 53.3%  | 5.0.0    | 96711602AD |
| 8086:2723 | 8086:0084 | Intel           | Wi-Fi 6 AX200            | 30.8%  | 5.0.0    | 627975DCD4 |
| 8086:2723 | 8086:008c | Intel           | Wi-Fi 6 AX200            | 100%   |          | BDD15B19B1 |
| 8086:2723 | 8086:4080 | Intel           | Wi-Fi 6 AX200            | 11.1%  | 4.15.0   | 1CE78F244C |

### Sd host controller (PCI)

43 out of 699 (6.15%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 104c:8034 | 103c:3085 | Texas Instru... | PCIxx21/PCIxx11 SD Ho... | 33.3%  | 4.19.66  | E643DE7D13 |
| 14e4:16bc | 1025:0647 | Broadcom Inc... | BCM57765/57785 SDXC/M... | 0.2%   | 3.10.34  | 86D2D3B0E1 |
| 197b:2381 | 1025:0140 | JMicron Tech... | Standard SD Host Cont... | 33.3%  | 5.3.0    | C85107D1C1 |
| 197b:2381 | 1025:0145 | JMicron Tech... | Standard SD Host Cont... | 50%    | 4.1.15   | C07C4BD9E0 |
| 197b:2381 | 1025:0260 | JMicron Tech... | Standard SD Host Cont... | 20%    | 4.15.0   | ABC5736623 |
| 197b:2381 | 1025:0275 | JMicron Tech... | Standard SD Host Cont... | 58.3%  | 4.15.0   | 09734ADC68 |
| 197b:2381 | 103c:2aa2 | JMicron Tech... | Standard SD Host Cont... | 50%    | 4.1.15   | 744EE1496B |
| 197b:2381 | 103c:30fc | JMicron Tech... | Standard SD Host Cont... | 60%    | 4.18.0   | 039F952C77 |
| 197b:2381 | 103c:3624 | JMicron Tech... | Standard SD Host Cont... | 6.7%   | 4.1.16   | FF9CED6EF0 |
| 197b:2381 | 103c:3628 | JMicron Tech... | Standard SD Host Cont... | 3.4%   | 3.14.44  | B0C685633F |
| 197b:2381 | 1043:1a07 | JMicron Tech... | Standard SD Host Cont... | 2.4%   | 3.10.34  | 83B774A0CD |
| 197b:2381 | 1071:9525 | JMicron Tech... | Standard SD Host Cont... | 100%   |          | EC12AF8F5D |
| 197b:2381 | 1179:fd30 | JMicron Tech... | Standard SD Host Cont... | 17.4%  | 3.14.33  | A9ECF36092 |
| 197b:2381 | 1297:2000 | JMicron Tech... | Standard SD Host Cont... | 41.7%  | 4.4.0    | C227E1334E |
| 197b:2381 | 1297:2008 | JMicron Tech... | Standard SD Host Cont... | 100%   |          | 8F6ED609DD |
| 197b:2381 | 1297:2020 | JMicron Tech... | Standard SD Host Cont... | 75%    | 5.0.0    | 95D754997A |
| 197b:2381 | 1297:2027 | JMicron Tech... | Standard SD Host Cont... | 69.2%  | 4.15.0   | E1D0023466 |
| 197b:2381 | 1297:2028 | JMicron Tech... | Standard SD Host Cont... | 33.3%  | 4.9.0    | 54C077FDFC |
| 197b:2381 | 1558:0801 | JMicron Tech... | Standard SD Host Cont... | 8.3%   | 4.9.20   | 0267CF3435 |
| 197b:2381 | 1558:4120 | JMicron Tech... | Standard SD Host Cont... | 50%    | 4.20.17  | 65387A2C5F |
| 197b:2381 | 17aa:3d9a | JMicron Tech... | Standard SD Host Cont... | 22.2%  | 4.1.3    | 5E896CED5E |
| 197b:2391 | 103c:1618 | JMicron Tech... | Standard SD Host Cont... | 15%    | 4.1.15   | A284E8740A |
| 197b:2391 | 103c:161c | JMicron Tech... | Standard SD Host Cont... | 22.2%  | 4.1.15   | E8BE126153 |
| 197b:2391 | 103c:161d | JMicron Tech... | Standard SD Host Cont... | 44.4%  | 4.15.0   | C49427C6A0 |
| 197b:2391 | 103c:162a | JMicron Tech... | Standard SD Host Cont... | 27.3%  | 4.15.0   | 5951373CC3 |
| 197b:2391 | 103c:1631 | JMicron Tech... | Standard SD Host Cont... | 25%    | 4.1.19   | F1C7178572 |
| 197b:2391 | 103c:167c | JMicron Tech... | Standard SD Host Cont... | 4.7%   | 4.1.4    | ED03FD8077 |
| 197b:2391 | 103c:168b | JMicron Tech... | Standard SD Host Cont... | 7.7%   | 3.14.44  | DBE13E6A5C |
| 197b:2391 | 103c:176c | JMicron Tech... | Standard SD Host Cont... | 20%    | 4.15.0   | FDBA82A5B5 |
| 197b:2391 | 103c:179b | JMicron Tech... | Standard SD Host Cont... | 20%    | 3.14.44  | 7195452FF3 |
| 197b:2391 | 103c:179c | JMicron Tech... | Standard SD Host Cont... | 10%    | 4.9.20   | 883AFD81BF |
| 197b:2391 | 103c:17a7 | JMicron Tech... | Standard SD Host Cont... | 50%    | 3.14.44  | AE6CF1B3CA |
| 197b:2391 | 103c:17ab | JMicron Tech... | Standard SD Host Cont... | 11.1%  | 4.1.25   | 4F80F9BA3C |
| 197b:2391 | 103c:17ed | JMicron Tech... | Standard SD Host Cont... | 9.1%   | 3.14.44  | 0BC7216657 |
| 197b:2391 | 103c:17f3 | JMicron Tech... | Standard SD Host Cont... | 33.3%  | 4.9.193  | B4BA23ACA0 |
| 197b:2391 | 103c:17f6 | JMicron Tech... | Standard SD Host Cont... | 6.3%   | 3.14.39  | 5CC8316A85 |
| 197b:2391 | 103c:18df | JMicron Tech... | Standard SD Host Cont... | 20%    | 3.14.44  | 02361CAE46 |
| 197b:2391 | 1179:fc30 | JMicron Tech... | Standard SD Host Cont... | 14.3%  | 4.15.0   | 673D423ADC |
| 197b:2391 | 1558:2431 | JMicron Tech... | Standard SD Host Cont... | 100%   |          | F395EB44CF |
| 197b:2391 | 1558:2450 | JMicron Tech... | Standard SD Host Cont... | 100%   |          | 450ED4C040 |
| 197b:2391 | 1558:2700 | JMicron Tech... | Standard SD Host Cont... | 100%   |          | FBD3F68C8C |
| 197b:2391 | 1558:3500 | JMicron Tech... | Standard SD Host Cont... | 100%   |          | 7434BE9250 |
| 197b:2391 | 17aa:3976 | JMicron Tech... | Standard SD Host Cont... | 6.2%   | 3.14.44  | A85C0AB7E0 |

### Sound (PCI)

138 out of 9301 (1.48%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 0045:c061 | 0045:c061 |                 | Audio device             | 100%   |          | 8D884B92FA |
| 1002:1308 | 1025:0864 | AMD             | Kaveri HDMI/DP Audio ... | 7.1%   | 3.14.44  | 8D6D195DA2 |
| 1002:1314 | 1025:0520 | AMD             | Wrestler HDMI Audio      | 6.2%   | 3.14.44  | BF118AA31C |
| 1002:4383 | 1025:0520 | AMD             | SBx00 Azalia (Intel HDA) | 6.2%   | 3.14.44  | BF118AA31C |
| 1002:4383 | 1043:836c | AMD             | SBx00 Azalia (Intel HDA) | 1%     | 3.14.44  | 75283131DD |
| 1002:4383 | 1043:8445 | AMD             | SBx00 Azalia (Intel HDA) | 0.2%   | 3.10.0   | 8A4E34A210 |
| 1002:4383 | 1043:84fb | AMD             | SBx00 Azalia (Intel HDA) | 0.7%   | 3.14.44  | D3AEFE0601 |
| 1002:4383 | 1043:8576 | AMD             | SBx00 Azalia (Intel HDA) | 1%     | 3.14.44  | 35D0F345A4 |
| 1002:9840 | 17aa:2219 | AMD             | Kabini HDMI/DP Audio     | 50%    | 4.9.60   | 94058A82CA |
| 1002:aa38 | 1462:aa38 | AMD             | RV710/730 HDMI Audio ... | 3.1%   | 3.14.44  | 51837DE98F |
| 1002:aa38 | 174b:aa38 | AMD             | RV710/730 HDMI Audio ... | 0.8%   | 3.14.25  | 45FCBC8B9A |
| 1002:aa68 | 1545:aa68 | AMD             | Cedar HDMI Audio [Rad... | 50%    | 4.19.0   | B5BA9A13DC |
| 1002:aa90 | 1179:fb41 | AMD             | Turks HDMI Audio [Rad... | 6.7%   | 3.14.44  | 67009EFFAA |
| 1002:aa98 | 1043:aa98 | AMD             | Caicos HDMI Audio [Ra... | 1.5%   | 3.0.38   | 2A34C16AB3 |
| 1002:aa98 | 174b:aa98 | AMD             | Caicos HDMI Audio [Ra... | 0.6%   | 3.14.22  | 8A4E34A210 |
| 1002:aab0 | 103c:1990 | AMD             | Oland/Hainan/Cape Ver... | 25%    | 4.18.0   | DCE9CDAF8E |
| 1002:aab0 | 1043:aab0 | AMD             | Oland/Hainan/Cape Ver... | 0.9%   | 3.14.22  | 66219C1D36 |
| 1002:aab0 | 1682:aab0 | AMD             | Oland/Hainan/Cape Ver... | 1.4%   | 3.14.22  | D3AEFE0601 |
| 1002:aac0 | 1458:aac0 | AMD             | Tobago HDMI Audio [Ra... | 4%     | 3.14.44  | 62E0E97099 |
| 1022:1457 | 1462:fa39 | AMD             | Family 17h (Models 00... | 9.1%   | 4.9.60   | 84ED791AF7 |
| 1022:1457 | 1849:2220 | AMD             | Family 17h (Models 00... | 10%    | 4.18.0   | 707960B3EC |
| 1022:2093 | 1022:2093 | AMD             | CS5536 [Geode compani... | 100%   |          | 6D9551F87E |
| 1022:780d | 1025:0864 | AMD             | FCH Azalia Controller    | 7.1%   | 3.14.44  | 8D6D195DA2 |
| 1022:780d | 1043:85cd | AMD             | FCH Azalia Controller    | 4.8%   | 3.14.44  | CDC3F83CDB |
| 1022:780d | 1043:86c7 | AMD             | FCH Azalia Controller    | 25%    | 4.9.14   | 71ABA86389 |
| 106b:1803 | 106b:1881 | Apple           | Audio Device             | 100%   |          | 7F2D68A6A2 |
| 106b:1803 | 106b:1885 | Apple           | Audio Device             | 100%   |          | D3A040508D |
| 1073:1000 | 1073:1000 | Yamaha          | SW1000XG [XG Factory]    | 100%   |          | 8225C7BB98 |
| 10de:0059 | 1043:81ae | Nvidia          | CK804 AC'97 Audio Con... | 62.5%  | 3.14.25  | A6659EE127 |
| 10de:006b | 1043:0c11 | Nvidia          | nForce Audio Processi... | 100%   |          | 543960170E |
| 10de:006b | 147b:1c00 | Nvidia          | nForce Audio Processi... | 100%   |          | CB892B4614 |
| 10de:03f0 | 1458:a002 | Nvidia          | MCP61 High Definition... | 0.5%   | 3.14.15  | 9D9E2DB550 |
| 10de:0774 | 1043:836c | Nvidia          | MCP72XE/MCP72P/MCP78U... | 7.7%   | 3.10.19  | E1B7D175A1 |
| 10de:0774 | 1462:7578 | Nvidia          | MCP72XE/MCP72P/MCP78U... | 16.7%  | 4.9.20   | 8F804041A2 |
| 10de:0be3 | 1043:8354 | Nvidia          | High Definition Audio... | 3.1%   | 3.14.44  | 67BFE1B221 |
| 10de:0be3 | 1043:8490 | Nvidia          | High Definition Audio... | 26.3%  | 4.1.38   | A6659EE127 |
| 10de:0be3 | 1462:8094 | Nvidia          | High Definition Audio... | 1.5%   | 3.14.44  | 895D8612B4 |
| 10de:0bea | 1462:2304 | Nvidia          | GF108 High Definition... | 9.1%   | 3.14.44  | ED9D8A148D |
| 10de:0bea | 1991:5584 | Nvidia          | GF108 High Definition... | 50%    | 4.1.34   | CE8124E5F4 |
| 10de:0bee |           | Nvidia          | GF116 High Definition... | 1.2%   | 3.14.39  | 77909796EC |
| 10de:0e08 |           | Nvidia          | GF119 HDMI Audio Cont... | 3.6%   | 3.14.33  | 8F9504F263 |
| 10de:0e08 | 174b:0620 | Nvidia          | GF119 HDMI Audio Cont... | 50%    | 4.9.60   | 6566319F04 |
| 10de:0e0f | 1043:84f5 | Nvidia          | GK208 HDMI/DP Audio C... | 3.8%   | 3.14.44  | 35D0F345A4 |
| 10de:0e0f | 19da:7326 | Nvidia          | GK208 HDMI/DP Audio C... | 4.5%   | 4.15.0   | 84ED791AF7 |
| 10de:0e0f | 3842:1731 | Nvidia          | GK208 HDMI/DP Audio C... | 100%   |          | 75283131DD |
| 10de:0e1b | 10de:094b | Nvidia          | GK107 HDMI Audio Cont... | 5.6%   | 4.1.15   | 949DD823D7 |
| 10de:0e1b | 1569:0fc6 | Nvidia          | GK107 HDMI Audio Cont... | 1.1%   | 3.14.33  | 8F804041A2 |
| 10de:0fb0 | 1462:3232 | Nvidia          | GM200 High Definition... | 50%    | 5.0.0    | AF58D23265 |
| 10de:0fb9 | 10de:12af | Nvidia          | GP107GL High Definiti... | 100%   |          | C11BA25134 |
| 10de:0fba | 1043:8520 | Nvidia          | GM206 High Definition... | 4.8%   | 3.14.53  | 8D2A73DD23 |
| 10de:0fba | 3842:2962 | Nvidia          | GM206 High Definition... | 100%   |          | 707960B3EC |
| 10de:0fbc | 1462:3102 | Nvidia          | GM107 High Definition... | 5.6%   | 3.14.44  | 071F922873 |
| 10de:10ef | 1462:360c | Nvidia          | GP102 HDMI Audio Cont... | 100%   |          | 816A1797C5 |
| 10de:10f0 | 1043:8597 | Nvidia          | GP104 High Definition... | 40%    | 4.15.0   | 32166A5865 |
| 10de:10f0 | 1558:0879 | Nvidia          | GP104 High Definition... | 50%    | 4.19.0   | A7DB7C544F |
| 10de:10f1 | 10de:1c03 | Nvidia          | GP106 High Definition... | 3.3%   | 4.9.20   | E996F15E3E |
| 10de:10f1 | 1458:3724 | Nvidia          | GP106 High Definition... | 4.5%   | 4.1.34   | E40B76E473 |
| 10de:10f1 | 1462:3490 | Nvidia          | GP106 High Definition... | 33.3%  | 4.15.0   | 1B722DF896 |
| 10de:10fa | 103c:8611 | Nvidia          | TU107 GeForce GTX 165... | 100%   |          | BDD15B19B1 |
| 1102:0004 | 1102:1003 | Creative Labs   | EMU10k2/CA0100/CA0102... | 10%    | 4.1.15   | D74C162548 |
| 1102:0004 | 1102:2002 | Creative Labs   | EMU10k2/CA0100/CA0102... | 2.3%   | 3.14.44  | 2B0A36F85F |
| 13f2:0111 |           | Ford Microel... |                          | 100%   |          | 95162A226D |
| 13f2:0111 | ffff:ffff | Ford Microel... | Multimedia audio cont... | 100%   |          | 95162A226D |
| 13f6:0111 | 153b:1144 | C-Media Elec... | CMI8738/CMI8768 PCI A... | 7.1%   | 4.1.25   | 86F297ED58 |
| 13f6:8788 | 1043:8427 | C-Media Elec... | CMI8788 [Oxygen HD Au... | 100%   |          | BFB822D98C |
| 13f6:8788 | 1043:8463 | C-Media Elec... | CMI8788 [Oxygen HD Au... | 100%   |          | 9E13784BB3 |
| 13f6:8788 | 1043:8521 | C-Media Elec... | CMI8788 [Oxygen HD Au... | 2.6%   | 3.14.44  | 45FCBC8B9A |
| 13f6:8788 | 1043:855e | C-Media Elec... | CMI8788 [Oxygen HD Au... | 100%   |          | 300B071850 |
| 13f6:8788 | 7284:9783 | C-Media Elec... | CMI8788 [Oxygen HD Au... | 100%   |          | 40EA4505B9 |
| 1412:1624 | 1412:2403 | VIA Technolo... | Multimedia audio cont... | 100%   |          | 2AF6424751 |
| 19fe:7000 | 0e51:0002 | ESI             | MAYA44e Controller       | 100%   |          | FFAE40F172 |
| 8086:02c8 | 1028:0954 | Intel           | Comet Lake PCH-LP cAV... | 100%   |          | 8740133E10 |
| 8086:02c8 | 1043:1a61 | Intel           | Comet Lake PCH-LP cAV... | 100%   |          | 4EA8D503AE |
| 8086:0c0c | 8086:0c0c | Intel           | Xeon E3-1200 v3/4th G... | 10%    | 4.9.60   | 77909796EC |
| 8086:0c0c | 8086:2010 | Intel           | Xeon E3-1200 v3/4th G... | 0.8%   | 2.6.32   | DFDA14135D |
| 8086:0f04 | 1043:14dd | Intel           | Atom Processor Z36xxx... | 1.7%   | 3.14.33  | 106830C1CC |
| 8086:0f04 | 17aa:3695 | Intel           | Atom Processor Z36xxx... | 50%    | 4.15.0   | 08BB09B100 |
| 8086:0f28 | 17aa:3907 | Intel           | Atom Processor Z36xxx... | 100%   |          | 6D960BD235 |
| 8086:0f28 | 8086:0f28 | Intel           | Atom Processor Z36xxx... | 100%   |          | A154D9D080 |
| 8086:0f28 | 8086:7270 | Intel           | Atom Processor Z36xxx... | 100%   |          | E5412A533C |
| 8086:160c | 1025:098a | Intel           | Broadwell-U Audio Con... | 1.1%   | 3.14.44  | 4F849E1E80 |
| 8086:160c | 17aa:390b | Intel           | Broadwell-U Audio Con... | 6.9%   | 4.9.60   | AB6BD693BE |
| 8086:1c20 | 1025:0504 | Intel           | 6 Series/C200 Series ... | 0.7%   | 3.14.25  | 8FE3AF49FB |
| 8086:1c20 | 1028:0492 | Intel           | 6 Series/C200 Series ... | 8%     | 4.9.60   | EAFEF7DB79 |
| 8086:1c20 | 1028:0493 | Intel           | 6 Series/C200 Series ... | 8.5%   | 3.14.33  | EFD71FBD61 |
| 8086:1c20 | 1043:8445 | Intel           | 6 Series/C200 Series ... | 0.3%   | 3.10.0   | 1678EE56C3 |
| 8086:1c20 | 1849:1892 | Intel           | 6 Series/C200 Series ... | 2.7%   | 3.10.0   | 895D8612B4 |
| 8086:1d20 | 1028:05d2 | Intel           | C600/X79 series chips... | 6.7%   | 4.15.0   | 949DD823D7 |
| 8086:1e20 | 1025:074f | Intel           | 7 Series/C216 Chipset... | 100%   |          | 6566319F04 |
| 8086:1e20 | 1028:052c | Intel           | 7 Series/C216 Chipset... | 7.1%   | 4.15.0   | 29A0FC6CE0 |
| 8086:1e20 | 1179:fb40 | Intel           | 7 Series/C216 Chipset... | 16.7%  | 4.1.15   | 67009EFFAA |
| 8086:1e20 | 1297:2033 | Intel           | 7 Series/C216 Chipset... | 20%    | 4.9.20   | 9137B29AFE |
| 8086:1e20 | 1458:a002 | Intel           | 7 Series/C216 Chipset... | 0.6%   | 4.15.0   | 740BF21A40 |
| 8086:1e20 | 17aa:3083 | Intel           | 7 Series/C216 Chipset... | 25%    | 4.9.111  | E3BF127788 |
| 8086:1e20 | 17aa:3977 | Intel           | 7 Series/C216 Chipset... | 0.3%   | 3.10.42  | 2DD89E3983 |
| 8086:1e20 | 8086:1e20 | Intel           | 7 Series/C216 Chipset... | 5.9%   | 4.1.34   | CE8124E5F4 |
| 8086:2284 | 1025:1009 | Intel           | Atom/Celeron/Pentium ... | 100%   |          | 401BBED185 |
| 8086:2284 | 1043:1cbd | Intel           | Atom/Celeron/Pentium ... | 16.7%  | 4.9.9    | 71CCEBC0C1 |
| 8086:22a8 | 8086:7270 | Intel           | Atom/Celeron/Pentium ... | 100%   |          | 5E59B4F83C |
| 8086:266e | 103c:3006 | Intel           | 82801FB/FBM/FR/FW/FRW... | 33.3%  | 4.9.20   | 51837DE98F |
| 8086:266e | 1179:ff00 | Intel           | 82801FB/FBM/FR/FW/FRW... | 7.7%   | 4.15.0   | 8488B3D0B9 |
| 8086:266e | 1458:ae01 | Intel           | 82801FB/FBM/FR/FW/FRW... | 8%     | 3.14.44  | FD291EB728 |
| 8086:269a | 103c:1307 | Intel           | 631xESB/632xESB High ... | 20%    | 4.1.15   | B5BA9A13DC |
| 8086:27d8 | 1019:2683 | Intel           | NM10/ICH7 Family High... | 2.5%   | 3.14.44  | EAA25586D2 |
| 8086:27d8 | 1028:0220 | Intel           | NM10/ICH7 Family High... | 8.3%   | 3.14.44  | BBA0FE2672 |
| 8086:27d8 | 1043:8290 | Intel           | NM10/ICH7 Family High... | 0.5%   | 3.14.25  | 45FCBC8B9A |
| 8086:27d8 | 1043:83d4 | Intel           | NM10/ICH7 Family High... | 1.4%   | 3.14.44  | 8807184E95 |
| 8086:27d8 | 104d:81fc | Intel           | NM10/ICH7 Family High... | 100%   |          | 7F0BB0CC92 |
| 8086:27d8 | 1458:a002 | Intel           | NM10/ICH7 Family High... | 0.2%   | 3.13.0   | D6C3BCD69B |
| 8086:27d8 | 1462:104e | Intel           | NM10/ICH7 Family High... | 20%    | 4.1.15   | 5F15F028A8 |
| 8086:27d8 | 1854:005f | Intel           | NM10/ICH7 Family High... | 100%   |          | F60C56AC42 |
| 8086:27d8 | 1b0a:0001 | Intel           | NM10/ICH7 Family High... | 5.6%   | 3.14.44  | 396BE2A324 |
| 8086:284b | 1734:1083 | Intel           | 82801H (ICH8 Family) ... | 18.2%  | 3.14.44  | BF1BADE95D |
| 8086:293e | 103c:281e | Intel           | 82801I (ICH9 Family) ... | 2.2%   | 3.14.44  | 61D1ED752A |
| 8086:293e | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 25%    | 3.14.44  | 93C0EF7223 |
| 8086:293e | 1458:a022 | Intel           | 82801I (ICH9 Family) ... | 8.3%   | 3.14.44  | 071F922873 |
| 8086:34c8 | 1028:0979 | Intel           | Smart Sound Technolog... | 22.2%  | 5.0.0    | 7F4CE08DF9 |
| 8086:3b56 | 103c:3674 | Intel           | 5 Series/3400 Series ... | 16.7%  | 4.15.0   | F4DE983D96 |
| 8086:3b56 | 1043:8375 | Intel           | 5 Series/3400 Series ... | 1.5%   | 3.14.44  | E40B76E473 |
| 8086:3b56 | 1458:a002 | Intel           | 5 Series/3400 Series ... | 0.6%   | 3.10.42  | 66219C1D36 |
| 8086:3b56 | 1849:6718 | Intel           | 5 Series/3400 Series ... | 11.1%  | 3.14.25  | 1D9934126C |
| 8086:8c20 | 1043:143f | Intel           | 8 Series/C220 Series ... | 12.5%  | 4.9.41   | A268D267B1 |
| 8086:8c20 | 1458:a002 | Intel           | 8 Series/C220 Series ... | 1.3%   | 3.10.0   | E996F15E3E |
| 8086:8c20 | 8086:8c20 | Intel           | 8 Series/C220 Series ... | 12.5%  | 4.9.124  | 77909796EC |
| 8086:8ca0 | 1462:d917 | Intel           | 9 Series Chipset Fami... | 6.2%   | 4.1.15   | 8D2A73DD23 |
| 8086:8d20 | 1458:a182 | Intel           | C610/X99 series chips... | 6.2%   | 4.1.15   | AF58D23265 |
| 8086:9ca0 | 1025:098a | Intel           | Wildcat Point-LP High... | 1.1%   | 3.14.44  | 4F849E1E80 |
| 8086:9ca0 | 17aa:390b | Intel           | Wildcat Point-LP High... | 6.9%   | 4.9.60   | AB6BD693BE |
| 8086:9d71 | 17aa:225d | Intel           | Sunrise Point-LP HD A... | 4.5%   | 4.14.35  | 7D7E6AD5D5 |
| 8086:9d72 | 1028:06e6 | Intel           | 300 Series Chipset Sm... | 100%   |          | EC07F9B3A7 |
| 8086:9dc8 | 1028:08a8 | Intel           | Cannon Point-LP High ... | 14.3%  | 4.15.0   | B6DF9FEC5F |
| 8086:a170 | 103c:8257 | Intel           | 100 Series/C230 Serie... | 50%    | 4.15.0   | D079BA6F90 |
| 8086:a2f0 | 1043:8735 | Intel           | 200 Series PCH HD Audio  | 25%    | 4.9.95   | 816A1797C5 |
| 8086:a2f0 | 1458:a182 | Intel           | 200 Series PCH HD Audio  | 2.2%   | 3.10.0   | 1A67024C19 |
| 8086:a2f0 | 1558:0879 | Intel           | 200 Series PCH HD Audio  | 33.3%  | 4.18.0   | A7DB7C544F |
| 8086:a348 | 1028:0851 | Intel           | Cannon Lake PCH cAVS     | 100%   |          | 05D6B79D2F |
| 8086:a348 | 103c:860f | Intel           | Cannon Lake PCH cAVS     | 100%   |          | BDD15B19B1 |
| 8086:a348 | 17aa:36e7 | Intel           | Cannon Lake PCH cAVS     | 25%    | 4.15.0   | 1B722DF896 |

### Storage (PCI)

56 out of 213 (26.29%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 104c:8033 | 1179:ff05 | Texas Instru... | PCIxx21/PCIxx11 Flash... | 12.5%  | 4.15.0   | 8488B3D0B9 |
| 104c:803b | 1025:011f | Texas Instru... | PCIxx12 Flash Media C... | 0.8%   | 3.14.33  | 2EE51E8201 |
| 104c:803b | 104d:81fc | Texas Instru... | PCIxx12 Flash Media C... | 100%   |          | 7F0BB0CC92 |
| 1095:3110 | 1095:7110 | Silicon Image   | SCSI storage controller  | 100%   |          | 69BD5A45B3 |
| 1106:401a | 1028:0408 | VIA Technolo... | VIA Card Reader Host ... | 100%   |          | 3125B9C83A |
| 1106:401a | 1071:9515 | VIA Technolo... | VIA Card Reader Host ... | 100%   |          | E028F277D4 |
| 1106:401a | 17aa:3608 | VIA Technolo... | VIA Card Reader Host ... | 100%   |          | EA55AE13AC |
| 117c:0064 | 117c:0064 | ATTO Technology | Celerity FC 16Gb/s Ge... | 100%   |          | 43EE2001E1 |
| 11f8:8032 | 117c:003b | PMC-Sierra      | PM8032 Tachyon QE8       | 100%   |          | 2903921AEB |
| 1217:7130 | 1019:300e | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 3C221F81A4 |
| 1217:7130 | 1025:010d | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 5A64D135B2 |
| 1217:7130 | 1025:011a | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 69380B60FC |
| 1217:7130 | 1025:0123 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | B127BEAD10 |
| 1217:7130 | 1025:0124 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 5AAFE28787 |
| 1217:7130 | 1025:012b | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 21509117BA |
| 1217:7130 | 1025:013c | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | A8E4D6D25F |
| 1217:7130 | 1028:026f | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 20788C640E |
| 1217:7130 | 1028:0273 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | C9D61D9E11 |
| 1217:7130 | 1028:0275 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | B0314C0713 |
| 1217:7130 | 1071:8258 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 98006DB3BD |
| 1217:7130 | 107b:0696 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | E9F51C8451 |
| 1217:7130 | 10cf:13c6 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 7B7919A092 |
| 1217:7130 | 10cf:143d | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 4A653FDD06 |
| 1217:7130 | 10cf:14d6 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 751064E2A2 |
| 1217:7130 | 1179:ff50 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 6108B0C47E |
| 1217:7130 | 1462:3fbb | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | FDCEAF9E02 |
| 1217:7130 | 1462:3fc1 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 278EF4A255 |
| 1217:7130 | 1462:3fe9 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 3F64CDD242 |
| 1217:7130 | 1462:3ff3 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | A249DABAD8 |
| 1217:7130 | 1462:4327 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 59A1BF0CA5 |
| 1217:7130 | 1462:63f6 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | BA35BAD99E |
| 1217:7130 | 1462:6440 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 43D96E36AB |
| 1217:7130 | 14ff:a003 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 6647A9CB02 |
| 1217:7130 | 1631:0188 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 856B9A1A68 |
| 1217:7130 | 1734:10c7 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 6E3970FC39 |
| 1217:7130 | 17aa:3a21 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 5988593465 |
| 1217:8130 | 1025:019f | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | 806ABC807D |
| 1217:8130 | 1025:038b | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | D7BF7F6352 |
| 1217:8130 | 1028:02bc | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | E1FF130D0A |
| 1217:8130 | 1028:02ea | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | EFA8CE8686 |
| 1217:8130 | 1028:02eb | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | 77B6FABE29 |
| 1217:8130 | 10cf:1568 | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | C2AA02F6B3 |
| 1217:8130 | 1179:ff50 | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | 60D901703E |
| 1217:8231 | 1028:0493 | O2 Micro        | O2Micro Integrated MS... | 100%   |          | CA779DE74C |
| 1217:8231 | 1028:04a9 | O2 Micro        | O2Micro Integrated MS... | 100%   |          | F3F87090B3 |
| 1217:8330 | 1028:04a3 | O2 Micro        | OZ600 MS/xD Controller   | 100%   |          | D8BA5B1425 |
| 1217:8330 | 1028:04a4 | O2 Micro        | OZ600 MS/xD Controller   | 100%   |          | 2A2FBFB933 |
| 1217:8330 | 10cf:16ae | O2 Micro        | OZ600 MS/xD Controller   | 100%   |          | 12ED876B92 |
| 1217:8331 | 1028:0494 | O2 Micro        | O2 Flash Memory Card     | 100%   |          | 4384225066 |
| 1217:8331 | 1028:049a | O2 Micro        | O2 Flash Memory Card     | 100%   |          | 6FD4500E86 |
| 1217:8331 | 1028:049b | O2 Micro        | O2 Flash Memory Card     | 100%   |          | 4673399116 |
| 1aed:3002 | 1014:04d3 | SanDisk         | ioMemory HHHL            | 100%   |          | FB0D0A1860 |
| 1b85:1221 | 1b85:1221 | OCZ Technolo... | OCZ 12xx SCSI Controller | 100%   |          | 323982480D |
| 9004:7178 |           | Adaptec         | AIC-7870P/7871 [AHA-2... | 33.3%  | 3.14.44  | 87BEA4712A |
| ace1:0005 | ace1:0005 |                 | Storage controller       | 100%   |          | 22F215C605 |
| ace1:0006 | ace1:0006 |                 | Storage controller       | 100%   |          | EF20304D33 |

### Storage/ata (PCI)

5 out of 4158 (0.12%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1022:43c8 | 1b21:1062 | AMD             | 400 Series Chipset SA... | 0.3%   | 4.4.0    | 21D76CDE28 |
| 1022:7901 | 1043:87c0 | AMD             | FCH SATA Controller [... | 5%     | 4.15.0   | 21D76CDE28 |
| 11ab:6141 | 1043:81d6 | Marvell Tech... | 88SE614x SATA II PCI-... | 100%   |          | 9EA64D6592 |
| 8086:2929 | 103c:306b | Intel           | 82801IBM/IEM (ICH9M/I... | 25%    | 3.14.44  | 93C0EF7223 |
| 8086:a353 | 1028:087c | Intel           | Cannon Lake Mobile PC... | 3.6%   | 4.15.0   | C917477768 |

### Storage/raid (PCI)

9 out of 575 (1.57%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1022:43bd | 1b21:1062 | AMD             | FCH RAID Controller      | 100%   |          | 2ED5B5AFC5 |
| 1028:0016 | 1028:1f24 | Dell            | PowerEdge Expandable ... | 100%   |          | 389DD308F7 |
| 103c:193f | 103c:3381 | Hewlett-Packard | Dynamic Smart Array B... | 100%   |          | 4825C12F7D |
| 1095:1114 | 1095:5114 | Silicon Image   | RAID bus controller      | 100%   |          | 126A2B0E4F |
| 1103:0611 | 1103:0611 | HighPoint Te... | RAID bus controller      | 100%   |          | E8AECFE123 |
| 1103:2840 | 1103:0000 | HighPoint Te... | RAID bus controller      | 100%   |          | 7653740066 |
| 117c:002c | 117c:002c | ATTO Technology | ExpressSAS R380          | 100%   |          | F233ABA040 |
| 1590:0045 | 1590:0045 | Hewlett-Packard | RAID bus controller      | 100%   |          | 3FAC52AF81 |
| 6883:0dd4 | 6883:0dd4 |                 | RAID bus controller      | 100%   |          | 7211932892 |

### System peripheral (PCI)

120 out of 664 (18.07%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 0e11:b203 | 103c:3305 | Compaq Computer | Integrated Lights Out... | 80%    | 4.9.60   | DF7A5AC424 |
| 103c:3306 | 103c:3309 | Hewlett-Packard | Integrated Lights-Out... | 80%    | 2.6.32   | D6C67240AC |
| 103c:3306 | 103c:3381 | Hewlett-Packard | Integrated Lights-Out... | 56.9%  | 2.6.32   | 8C7DEBB708 |
| 104c:8201 | 103c:006d | Texas Instru... | PCI1620 Firmware Load... | 100%   |          | E1BAA5BDE6 |
| 104c:8201 | 103c:08b0 | Texas Instru... | PCI1620 Firmware Load... | 100%   |          | 316E375A5C |
| 104c:8204 | 1028:0139 | Texas Instru... | PCI7410/7510/7610 PCI... | 100%   |          | 0504CC20A9 |
| 104c:8204 | 1028:014e | Texas Instru... | PCI7410/7510/7610 PCI... | 100%   |          | 0493B906A1 |
| 10b5:2065 | 10b5:9030 | PLX Technology  | System peripheral        | 100%   |          | BF5B58520E |
| 10b5:8609 | 10b5:8609 | PLX Technology  | PEX 8609 8-lane, 8-Po... | 100%   |          | E8AECFE123 |
| 1179:0805 | 1179:0001 | Toshiba Amer... | SD TypA Controller       | 40%    | 4.1.34   | 6ED70A9B46 |
| 1180:0576 | 10cf:1256 | Ricoh           | R5C576 SD Bus Host Ad... | 100%   |          | 4DCFB332DF |
| 1180:0576 | ffff:ffff | Ricoh           | R5C576 SD Bus Host Ad... | 100%   |          | 116C24A4D7 |
| 1180:0592 | 17aa:20ca | Ricoh           | R5C592 Memory Stick B... | 2.1%   | 3.14.25  | 81A4DA9481 |
| 1180:0852 | 1028:029f | Ricoh           | xD-Picture Card Contr... | 20%    | 4.1.15   | 44C743E996 |
| 1180:0852 | 1043:1877 | Ricoh           | xD-Picture Card Contr... | 3.6%   | 3.0.28   | 70CC866946 |
| 1180:0852 | 1734:10ad | Ricoh           | xD-Picture Card Contr... | 12.5%  | 4.1.33   | D6BC4ADE36 |
| 1180:0852 | 17aa:20cb | Ricoh           | xD-Picture Card Contr... | 2.1%   | 3.14.25  | 81A4DA9481 |
| 1180:e230 | 1028:02bd | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 31D62139B3 |
| 1180:e230 | 1028:02fe | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 4DA3A91131 |
| 1180:e230 | 1028:0401 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | B524E2847B |
| 1180:e230 | 1028:0402 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 400532E714 |
| 1180:e230 | 1028:0413 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | A1E1395C6F |
| 1180:e230 | 1028:0442 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 1BB8E0A4D4 |
| 1180:e230 | 103c:1455 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | C148D2D7EC |
| 1180:e230 | 103c:146d | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 45A1D9A3BA |
| 1180:e230 | 103c:1471 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 89C840D7E1 |
| 1180:e230 | 103c:1722 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 3E6CC68DC2 |
| 1180:e230 | 103c:1726 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 759D141031 |
| 1180:e230 | 103c:307e | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | C1A1180C7A |
| 1180:e230 | 1043:1f47 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | A89E10B5B7 |
| 1180:e230 | 104d:905a | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | EB4E58C4D9 |
| 1180:e230 | 104d:9060 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 05CFF66AC2 |
| 1180:e230 | 104d:9066 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 1DE544887B |
| 1180:e230 | 104d:9067 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 7412A9035D |
| 1180:e230 | 104d:9069 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | D21AA077CE |
| 1180:e230 | 104d:9071 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 90D3759348 |
| 1180:e230 | 104d:9072 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | DA9CBAC74B |
| 1180:e230 | 104d:907a | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | FF5B7BA78E |
| 1180:e230 | 1179:0001 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 9BE4F247B6 |
| 1180:e230 | 1179:ff1e | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | A98407C880 |
| 1180:e230 | 1179:ff40 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | A5D1F93E9C |
| 1180:e230 | 17aa:2134 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 9A495F134B |
| 1180:e232 | 104d:907e | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 4A2DA5DD1B |
| 1180:e232 | 104d:9081 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 9DD5AB7DF8 |
| 1180:e232 | 104d:9083 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | B4CF237F88 |
| 1180:e232 | 104d:9086 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | C1F9CF2BE3 |
| 1180:e232 | 104d:9089 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 56C1A2EF9B |
| 1180:e232 | 104d:908e | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 59BB8EC907 |
| 1180:e232 | 104d:9095 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 405F4DEF54 |
| 1180:e232 | 104d:9097 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 7685534B8E |
| 1180:e232 | 1179:0001 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 4398E73607 |
| 1217:7110 | 10cf:11c4 | O2 Micro        | OZ711Mx 4-in-1 Memory... | 100%   |          | EA732BEA27 |
| 14e4:16be | 1025:0500 | Broadcom Inc... | BCM57765/57785 MS Car... | 100%   |          | 94A0B4FAB9 |
| 14e4:16be | 1025:0504 | Broadcom Inc... | BCM57765/57785 MS Car... | 100%   |          | 832F6EF100 |
| 14e4:16be | 1025:0599 | Broadcom Lim... | BCM57765/57785 MS Car... | 100%   |          | 593ECA45A2 |
| 14e4:16be | 1025:0605 | Broadcom Lim... | BCM57765/57785 MS Car... | 100%   |          | 72878CC6E9 |
| 14e4:16be | 1025:0647 | Broadcom Inc... | BCM57765/57785 MS Car... | 100%   |          | 9084C70732 |
| 14e4:16bf | 1025:0500 | Broadcom Inc... | BCM57765/57785 xD-Pic... | 100%   |          | 94A0B4FAB9 |
| 14e4:16bf | 1025:0504 | Broadcom Inc... | BCM57765/57785 xD-Pic... | 100%   |          | 832F6EF100 |
| 14e4:16bf | 1025:0599 | Broadcom Lim... | BCM57765/57785 xD-Pic... | 100%   |          | 593ECA45A2 |
| 14e4:16bf | 1025:0605 | Broadcom Lim... | BCM57765/57785 xD-Pic... | 100%   |          | 72878CC6E9 |
| 14e4:16bf | 1025:0647 | Broadcom Inc... | BCM57765/57785 xD-Pic... | 100%   |          | 9084C70732 |
| 197b:2382 | 1297:2020 | JMicron Tech... | SD/MMC Host Controller   | 25%    | 4.15.0   | D826611187 |
| 197b:2384 | 1019:2238 | JMicron Tech... | xD Host Controller       | 100%   |          | 7E782321C8 |
| 197b:2384 | 1025:0128 | JMicron Tech... | xD Host Controller       | 100%   |          | EA94093CD5 |
| 197b:2384 | 1025:013b | JMicron Tech... | xD Host Controller       | 100%   |          | 3C347BEC2E |
| 197b:2384 | 1025:013d | JMicron Tech... | xD Host Controller       | 100%   |          | D96905F762 |
| 197b:2384 | 1025:013e | JMicron Tech... | xD Host Controller       | 100%   |          | B563FF6430 |
| 197b:2384 | 1025:0140 | JMicron Tech... | xD Host Controller       | 100%   |          | C85107D1C1 |
| 197b:2384 | 1025:0142 | JMicron Tech... | xD Host Controller       | 100%   |          | 884C33EE98 |
| 197b:2384 | 1025:0143 | JMicron Tech... | xD Host Controller       | 100%   |          | 310A169187 |
| 197b:2384 | 1025:0145 | JMicron Tech... | xD Host Controller       | 100%   |          | 542B22772F |
| 197b:2384 | 1025:0146 | JMicron Tech... | xD Host Controller       | 100%   |          | 649CB24583 |
| 197b:2384 | 1025:015b | JMicron Tech... | xD Host Controller       | 100%   |          | 75927BE93C |
| 197b:2384 | 1025:0160 | JMicron Tech... | xD Host Controller       | 100%   |          | BBCDDB4D27 |
| 197b:2384 | 1025:0200 | JMicron Tech... | xD Host Controller       | 100%   |          | 454098B840 |
| 197b:2384 | 1025:0259 | JMicron Tech... | xD Host Controller       | 100%   |          | 8C172C772A |
| 197b:2384 | 1025:0260 | JMicron Tech... | xD Host Controller       | 100%   |          | ABC5736623 |
| 197b:2384 | 1025:042f | JMicron Tech... | xD Host Controller       | 100%   |          | 1395FA2E0F |
| 197b:2384 | 103c:1489 | JMicron Tech... | xD Host Controller       | 100%   |          | A6305AD3A0 |
| 197b:2384 | 103c:2aa2 | JMicron Tech... | xD Host Controller       | 100%   |          | 744EE1496B |
| 197b:2384 | 103c:2aa6 | JMicron Tech... | xD Host Controller       | 100%   |          | 45542209AF |
| 197b:2384 | 103c:30f4 | JMicron Tech... | xD Host Controller       | 100%   |          | 01F5E9CD57 |
| 197b:2384 | 103c:30f7 | JMicron Tech... | xD Host Controller       | 100%   |          | 90DCC06EEA |
| 197b:2384 | 103c:30fb | JMicron Tech... | xD Host Controller       | 100%   |          | 762D293955 |
| 197b:2384 | 103c:30fc | JMicron Tech... | xD Host Controller       | 100%   |          | CE906A67B9 |
| 197b:2384 | 103c:3600 | JMicron Tech... | xD Host Controller       | 100%   |          | 3F857E2920 |
| 197b:2384 | 103c:3603 | JMicron Tech... | xD Host Controller       | 100%   |          | F2190D7446 |
| 197b:2384 | 103c:3610 | JMicron Tech... | xD Host Controller       | 100%   |          | F31F2EC406 |
| 197b:2384 | 103c:361b | JMicron Tech... | xD Host Controller       | 100%   |          | 500C2BCFBC |
| 197b:2384 | 103c:3624 | JMicron Tech... | xD Host Controller       | 100%   |          | 0C8D7641B2 |
| 197b:2384 | 103c:3628 | JMicron Tech... | xD Host Controller       | 100%   |          | BF5A8C1756 |
| 197b:2384 | 103c:363e | JMicron Tech... | xD Host Controller       | 100%   |          | A9E05596D5 |
| 197b:2384 | 103c:3659 | JMicron Tech... | xD Host Controller       | 100%   |          | B48F5D5FDD |
| 197b:2384 | 103c:7001 | JMicron Tech... | xD Host Controller       | 100%   |          | 2D49142FA9 |
| 197b:2384 | 103c:7010 | JMicron Tech... | xD Host Controller       | 100%   |          | 6E70B36184 |
| 197b:2384 | 1043:1a07 | JMicron Tech... | xD Host Controller       | 100%   |          | 088FFC2823 |
| 197b:2384 | 1071:9525 | JMicron Tech... | xD Host Controller       | 100%   |          | EC12AF8F5D |
| 197b:2384 | 1179:fd30 | JMicron Tech... | xD Host Controller       | 100%   |          | 59D7D4A316 |
| 197b:2384 | 1179:fdb0 | JMicron Tech... | xD Host Controller       | 100%   |          | 3BF39D603E |
| 197b:2384 | 1179:ff02 | JMicron Tech... | xD Host Controller       | 100%   |          | EF1BFF7353 |
| 197b:2384 | 1179:ff08 | JMicron Tech... | xD Host Controller       | 100%   |          | 09F5B63B0D |
| 197b:2384 | 1462:100f | JMicron Tech... | xD Host Controller       | 100%   |          | 9FEC6C5DE7 |
| 197b:2384 | 1462:6520 | JMicron Tech... | xD Host Controller       | 100%   |          | 12132D4EBD |
| 197b:2384 | 152d:0834 | JMicron Tech... | xD Host Controller       | 100%   |          | C6D0242C42 |
| 197b:2384 | 1558:0803 | JMicron Tech... | xD Host Controller       | 100%   |          | F5F1021D04 |
| 197b:2384 | 1558:0806 | JMicron Tech... | xD Host Controller       | 100%   |          | F3BF4D62C0 |
| 197b:2384 | 1734:113d | JMicron Tech... | xD Host Controller       | 100%   |          | BD5D293529 |
| 197b:2384 | 1734:113f | JMicron Tech... | xD Host Controller       | 100%   |          | 93C1102EAE |
| 197b:2384 | 17aa:2130 | JMicron Tech... | xD Host Controller       | 100%   |          | 4B5548D0BB |
| 197b:2384 | 17aa:3602 | JMicron Tech... | xD Host Controller       | 100%   |          | 55C2F8E26B |
| 197b:2384 | 17aa:3881 | JMicron Tech... | xD Host Controller       | 100%   |          | 7F669E0390 |
| 197b:2387 | 17aa:3921 | JMicron Tech... | SD/MMC Host Controller   | 100%   |          | 6CA3597271 |
| 197b:2389 | 17aa:3924 | JMicron Tech... | xD Host Controller       | 100%   |          | 6CA3597271 |
| 197b:2394 | 1028:0446 | JMicron Tech... | xD Host Controller       | 100%   |          | 3C558B4510 |
| 197b:2394 | 103c:2ac6 | JMicron Tech... | xD Host Controller       | 100%   |          | 461345008C |
| 197b:2394 | 1179:fc30 | JMicron Tech... | xD Host Controller       | 100%   |          | 2FAE738892 |
| 197b:2394 | 1462:107f | JMicron Tech... | xD Host Controller       | 100%   |          | 4D22D14A1D |
| 197b:2394 | 17aa:3976 | JMicron Tech... | xD Host Controller       | 100%   |          | 6177430B68 |
| 197b:2394 | 17aa:3977 | JMicron Tech... | xD Host Controller       | 100%   |          | AFD1938614 |

### Tv card (PCI)

8 out of 273 (2.93%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1131:7130 | 5ace:5050 | Philips Semi... | SAA7130 Video Broadca... | 3.1%   | 3.14.44  | D82F0A25EA |
| 1131:7133 | 16be:0007 | Philips Semi... | SAA7131/SAA7133/SAA71... | 100%   |          | 24A0914BA3 |
| 1131:7133 | 16be:0008 | Philips Semi... | SAA7131/SAA7133/SAA71... | 100%   |          | 24A0914BA3 |
| 11de:6057 | 1031:7efe | Zoran           | ZR36057PQC Video cutt... | 6.7%   | 3.14.44  | BEB1083A7F |
| 11de:6057 | 1031:d801 | Zoran           | ZR36057PQC Video cutt... | 100%   |          | F700FF20C6 |
| 14f1:8800 | 8922:8888 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 75%    | 4.1.25   | ADF2D5DACA |
| 14f1:8802 | 8922:8888 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 75%    | 4.1.25   | ADF2D5DACA |
| 4444:0016 | 0070:8801 | Internext Co... | iTVC16 (CX23416) Vide... | 8.3%   | 4.1.15   | 8854FD6644 |

### Usb controller (PCI)

48 out of 15775 (0.30%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1002:4397 | 1458:5004 | AMD             | SB7x0/SB8x0/SB9x0 USB... | 0.1%   | 3.10.0   | 0533339E4E |
| 1002:4399 | 1458:5004 | AMD             | SB7x0/SB8x0/SB9x0 USB... | 0.1%   | 3.10.0   | 0533339E4E |
| 1022:7807 | 103c:216f | AMD             | FCH USB OHCI Controller  | 20%    | 4.9.20   | E190391A64 |
| 1022:7807 | 1458:5004 | AMD             | FCH USB OHCI Controller  | 0.2%   | 3.14.25  | FA543553EC |
| 1022:7808 | 103c:216f | AMD             | FCH USB EHCI Controller  | 20%    | 4.9.20   | E190391A64 |
| 1022:7809 | 1458:5004 | AMD             | FCH USB OHCI Controller  | 0.2%   | 3.14.25  | FA543553EC |
| 1022:7814 | 103c:216f | AMD             | FCH USB XHCI Controller  | 20%    | 4.9.20   | E190391A64 |
| 104c:8241 | 103c:2ada | Texas Instru... | TUSB73x0 SuperSpeed U... | 33.3%  | 4.15.0   | 3BB5A2AB3E |
| 10de:005a | 1043:815a | Nvidia          | CK804 USB Controller     | 4.6%   | 3.10.19  | A6659EE127 |
| 10de:005b | 1043:815a | Nvidia          | CK804 USB Controller     | 4.6%   | 3.10.19  | A6659EE127 |
| 1106:3104 | 1106:3104 | VIA Technolo... | USB 2.0                  | 1.6%   | 3.14.22  | F3D97660A0 |
| 1106:3104 | 1106:318a | VIA Technolo... | USB 2.0                  | 20%    | 4.1.25   | E56DD30CA2 |
| 1106:3483 | 1106:3483 | VIA Technolo... | VL805 USB 3.0 Host Co... | 0.4%   | 3.14.44  | 76393E37C8 |
| 1106:3483 | 1458:5007 | VIA Technolo... | VL805 USB 3.0 Host Co... | 7.6%   | 3.10.0   | BE1C2E3D9C |
| 1912:0014 | 103c:1996 | Renesas Tech... | uPD720201 USB 3.0 Hos... | 3.8%   | 4.4.4    | 7CF6D970EC |
| 1912:0014 | 1912:0014 | Renesas Tech... | uPD720201 USB 3.0 Hos... | 4%     | 4.1.15   | E3CF1A821F |
| 1912:0015 |           | Renesas Tech... | uPD720202 USB 3.0 Hos... | 4.8%   | 3.14.25  | 740FC92339 |
| 1b21:1042 | 1043:1059 | ASMedia Tech... | ASM1042 SuperSpeed US... | 0.3%   | 3.10.34  | 6C9107BCAD |
| 1b21:1042 | 1043:8488 | ASMedia Tech... | ASM1042 SuperSpeed US... | 0.1%   | 3.10.34  | 9DB86FFBF1 |
| 1b21:1042 | 1462:7693 | ASMedia Tech... | ASM1042 SuperSpeed US... | 5.4%   | 3.14.15  | FC5F1E6327 |
| 1b21:1042 | 1849:1042 | ASMedia Tech... | ASM1042 SuperSpeed US... | 3.8%   | 3.10.0   | 101E707D3C |
| 1b73:1000 | 1043:1039 | Fresco Logic    | FL1000G USB 3.0 Host ... | 0.8%   | 3.0.28   | 0EAEBD5FCA |
| 8086:1e31 | 1028:0534 | Intel           | 7 Series/C210 Series ... | 7.3%   | 4.1.19   | EB05A0D70D |
| 8086:1e31 | 103c:1970 | Intel           | 7 Series/C210 Series ... | 6.7%   | 3.14.44  | E2F0FC675A |
| 8086:1e31 | 1043:1447 | Intel           | 7 Series/C210 Series ... | 8.3%   | 3.14.44  | F23B5BF0DA |
| 8086:1e31 | 104d:9095 | Intel           | 7 Series/C210 Series ... | 4.5%   | 3.14.25  | 2A2BD0A648 |
| 8086:1e31 | 17aa:21f3 | Intel           | 7 Series/C210 Series ... | 1.5%   | 3.14.44  | 3085B68179 |
| 8086:22b7 | 8086:7270 | Intel           | USB Synopsys Controller  | 10%    | 4.9.9    | 19F89F5D4E |
| 8086:2934 | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 25%    | 3.14.44  | 93C0EF7223 |
| 8086:2935 | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 25%    | 3.14.44  | 93C0EF7223 |
| 8086:2936 | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 25%    | 3.14.44  | 93C0EF7223 |
| 8086:2937 | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 25%    | 3.14.44  | 93C0EF7223 |
| 8086:2938 | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 25%    | 3.14.44  | 93C0EF7223 |
| 8086:2939 | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 25%    | 3.14.44  | 93C0EF7223 |
| 8086:293a | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 25%    | 3.14.44  | 93C0EF7223 |
| 8086:293c | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 25%    | 3.14.44  | 93C0EF7223 |
| 8086:3b36 | 8086:7270 | Intel           | 5 Series/3400 Series ... | 77.3%  | 3.14.44  | 4F5F07BC6E |
| 8086:3b3b | 8086:7270 | Intel           | 5 Series/3400 Series ... | 77.3%  | 3.14.44  | 4F5F07BC6E |
| 8086:8c26 | 103c:1909 | Intel           | 8 Series/C220 Series ... | 16.7%  | 4.9.0    | 196DFE92A3 |
| 8086:8c2d | 103c:1909 | Intel           | 8 Series/C220 Series ... | 16.7%  | 4.9.0    | 196DFE92A3 |
| 8086:8c31 | 8086:204a | Intel           | 8 Series/C220 Series ... | 12.5%  | 4.1.25   | 8C48173C7B |
| 8086:8d26 | 1043:8600 | Intel           | C610/X99 series chips... | 2%     | 4.1.25   | CCA78B29D4 |
| 8086:8d2d | 1043:8600 | Intel           | C610/X99 series chips... | 2%     | 4.1.25   | CCA78B29D4 |
| 8086:9ca6 | 1025:098a | Intel           | Wildcat Point-LP USB ... | 1.1%   | 3.14.44  | DE4737FCF1 |
| 8086:9ca6 | 1028:06be | Intel           | Wildcat Point-LP USB ... | 16.7%  | 4.15.0   | 1FBEE12FFE |
| 8086:9cb1 | 103c:806c | Intel           | Wildcat Point-LP USB ... | 100%   |          | 462F2D5347 |
| 8086:9d30 | 8086:7270 | Intel           | Skylake-U/Y USB Devic... | 100%   |          | 6D7A537E86 |
| 8086:9d30 | 8086:9d30 | Intel           | Skylake-U/Y USB Devic... | 33.3%  | 4.15.0   | 3E70A8DFF1 |

USB Devices
-----------

Non-100% value in the 'Missed' column indicates that the driver for a device is available
in the latest kernel versions. You can find corresponding hwinfo reports for listed devices
by a probe ID.

Missed — percentage of probes with missed driver for the device,
Linux  — the minimum Linux kernel version in which the driver was found,
Probe  — latest probe ID with missed driver for the device.

### Audio (USB)

7 out of 83 (8.43%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 046d:0a0b | Logitech        | ClearChat Pro USB        | 25%    | 4.15.0   | 56D5984A14 |
| 046d:0a87 | Logitech        | G935 Gaming Headset      | 100%   |          | 58C9748044 |
| 0644:8030 | TEAC            | US-1800                  | 100%   |          | 75C7FE6B69 |
| 0763:201a | M-Audio         | M-Audio Micro            | 100%   |          | 4AFB8F7991 |
| 0955:7002 | Nvidia          | stereo controller        | 100%   |          | BA096189BC |
| 1235:8016 | Focusrite-No... | Focusrite Scarlett 2i2   | 14.3%  | 4.9.20   | F16ADBF7F3 |
| b58e:0005 | Blue Microph... |                          | 50%    | 5.0.0    | A588768A6C |

### Bluetooth (USB)

32 out of 341 (9.38%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 044e:300c | Alps Electric   | Bluetooth Controller ... | 7.7%   | 4.1.15   | 7F0BB0CC92 |
| 0489:e036 | Foxconn / Ho... | Bluetooth USB Host Co... | 0.8%   | 3.0.28   | 69F933DD8C |
| 0489:e069 | Foxconn / Ho... | BT                       | 97.6%  | 4.9.41   | 6BA9DB05DC |
| 04ca:2006 | Lite-On Tech... | BCM43142A0 Bluetooth ... | 7.3%   | 4.0.8    | 805C7CD772 |
| 04ca:2007 | Lite-On Tech... | Broadcom BCM43142A0 B... | 9.4%   | 4.1.7    | BAA62D56E7 |
| 04ca:2009 | Lite-On Tech... | BCM43142A0               | 8.3%   | 4.0.2    | 14539CFCC1 |
| 04ca:300b | Lite-On Tech... | Lite-On Bluetooth Device | 0.3%   | 3.10.51  | 8D6D195DA2 |
| 04ca:300d | Lite-On Tech... | Atheros AR3012 Bluetooth | 3.2%   | 4.1.19   | 6D7A537E86 |
| 04ca:3014 | Lite-On Tech... | Qualcomm Atheros Blue... | 8.3%   | 4.1.25   | 401BBED185 |
| 05ac:8215 | Apple           | Built-in Bluetooth 2.... | 1.8%   | 3.14.44  | D5C9D589F2 |
| 05ac:8290 | Apple           | Bluetooth Host Contro... | 4.3%   | 4.9.9    | 91ED990D94 |
| 05e1:0100 | Syntek          | 802.11g + Bluetooth W... | 100%   |          | 0D5418F63E |
| 0930:0215 | Toshiba         | Bluetooth Device         | 12.5%  | 3.14.44  | 884E374E31 |
| 0930:0219 | Toshiba         | Bluetooth USB Host Co... | 2.1%   | 3.14.33  | 67009EFFAA |
| 0a5c:216c | Broadcom        | BCM43142A0 Bluetooth ... | 2%     | 3.14.44  | 2F3CB20593 |
| 0a5c:21e6 | Broadcom        | BCM20702 Bluetooth 4.... | 1.4%   | 3.14.15  | 867C47D444 |
| 0cf3:3002 | Qualcomm Ath... | AR3011 Bluetooth         | 5.3%   | 3.14.44  | 846CFA1057 |
| 0cf3:3004 | Qualcomm Ath... | AR3012 Bluetooth 4.0     | 0.5%   | 3.10.51  | 61287D0D21 |
| 0cf3:3005 | Qualcomm Ath... | AR3011 Bluetooth         | 0.1%   | 3.10.34  | F4DE983D96 |
| 0cf3:3008 | Qualcomm Ath... | Bluetooth (AR3011)       | 1.9%   | 3.14.25  | F430167968 |
| 0cf3:e005 | Qualcomm Ath... | Qualcomm Atheros Blue... | 3.7%   | 3.14.44  | 689DFEA547 |
| 0e8d:763e | MediaTek        | MT7630e Bluetooth Ada... | 100%   |          | A7E6CBC45B |
| 105b:e065 | Foxconn Inte... | BCM43142A0 Bluetooth ... | 13.9%  | 4.0.1    | F39685A972 |
| 13d3:3392 | IMC Networks    | Azurewave 43228+20702... | 100%   |          | 337156D639 |
| 413c:8143 | Dell            | BCM20702A0               | 85.7%  | 4.15.0   | AE4C0F8B6B |
| 413c:8197 | Dell            | Dell Wireless 380 Blu... | 2.2%   | 3.14.25  | 4E38982788 |
| 8087:0029 | Intel           | Bluetooth Device         | 0.9%   | 4.15.0   | BDD15B19B1 |
| 8087:07da | Intel           | Bluetooth Device         | 0.3%   | 4.14.141 | 2DD89E3983 |
| 8087:07dc | Intel           | Bluetooth Device         | 0.3%   | 3.10.0   | AB6BD693BE |
| 8087:0a2a | Intel           | Bluetooth Device         | 0.3%   | 3.10.0   | 69D10D1093 |
| 8087:0a2b | Intel           | Bluetooth Device         | 0.4%   | 3.10.0   | F6081D54B1 |
| 8087:0aaa | Intel           | Bluetooth Device 9460... | 0.6%   | 3.10.0   | 039A05F3EB |

### Camera (USB)

86 out of 2029 (4.24%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0402:5603 | ALi             | M5603 Video Camera Co... | 100%   |          | 775945A948 |
| 041e:400d | Creative Tec... | Webcam PD1001            | 100%   |          | 1892C5C88C |
| 041e:4039 | Creative Tec... | Webcam Live! Effects     | 100%   |          | EB3A6BB1E4 |
| 0458:702a | KYE Systems ... | WebCAM USB2.0            | 100%   |          | 3D86369A82 |
| 045e:0a00 | Microsoft       | Lumia 950 Dual SIM (R... | 50%    | 5.0.0    | 490B159371 |
| 046d:081b | Logitech        | Webcam C310              | 0.5%   | 3.14.22  | 66219C1D36 |
| 046d:0825 | Logitech        | Webcam C270              | 0.1%   | 3.10.34  | F6EB373ACA |
| 046d:09a4 | Logitech        | QuickCam E 3500          | 7.7%   | 3.14.39  | 74709A1A7B |
| 04ca:707f | Lite-On Tech... | HP Wide Vision HD Camera | 2.6%   | 4.4.0    | 06EE78EE4D |
| 04f2:b270 | Chicony Elec... | HP HD Webcam [Fixed]     | 4%     | 3.14.44  | C6E683B39B |
| 04f2:b307 | Chicony Elec... | TOSHIBA Web Camera - HD  | 2.1%   | 3.14.44  | 67009EFFAA |
| 04f2:b315 | Chicony Elec... | Integrated Camera        | 20%    | 3.14.53  | B7014678B5 |
| 04f2:b335 | Chicony Elec... | HD WebCam                | 2.4%   | 3.14.44  | 6A087DD575 |
| 04f2:b374 | Chicony Elec... | HD WebCam                | 0.8%   | 3.14.44  | 86D2D3B0E1 |
| 04f2:b3b2 | Chicony Elec... | TOSHIBA Web Camera - FHD | 16.7%  | 4.15.0   | 550460AAAC |
| 04f2:b40e | Chicony Elec... | HP Truevision HD camera  | 1.9%   | 3.14.25  | 9596ECB170 |
| 04f2:b452 | Chicony Elec... | HD WebCam                | 1%     | 3.14.25  | AF59A812BC |
| 04f2:b45a | Chicony Elec... | USB2.0 FHD Camera        | 10%    | 3.14.44  | 78D39E18EF |
| 04f2:b47f | Chicony Elec... | VGA Webcam               | 0.6%   | 3.14.44  | 401BBED185 |
| 04f2:b52b | Chicony Elec... | USB2.0 VGA UVC WebCam    | 0.8%   | 3.14.44  | 3668630E7F |
| 04f2:b59a | Chicony Elec... | XiaoMi USB 2.0 Webcam    | 20%    | 4.9.60   | B1B825395C |
| 04f2:b5f7 | Chicony Elec... | HD WebCam                | 1.2%   | 4.9.20   | 51AC6D49F9 |
| 04f2:b614 | Chicony Elec... | Integrated Camera        | 33.3%  | 5.0.0    | 4438A85B31 |
| 04f2:b615 | Chicony Elec... | Integrated IR Camera     | 33.3%  | 5.0.0    | 4438A85B31 |
| 04f2:b669 | Chicony Elec... | HP HD Camera             | 25%    | 4.19.0   | BDD15B19B1 |
| 04f2:b684 | Chicony Elec... | USB2.0 Camera            | 25%    | 4.18.0   | 5CD28E369C |
| 0547:6512 | Anchor Chips    | UCMOS05100KPA Microsc... | 100%   |          | 93BF2F1F49 |
| 058f:5608 | Alcor Micro     | USB 2.0 Web Camera       | 0.6%   | 3.14.44  | E1C0563D70 |
| 058f:a001 | Alcor Micro     | HP Webcam-101            | 2.4%   | 3.14.44  | F4DE983D96 |
| 05ac:12a8 | Apple           | iPhone5/5C/5S/6          | 1.4%   | 3.14.39  | 68E18AE90F |
| 05ac:8501 | Apple           | Built-in iSight [Micron] | 66.7%  | 4.15.0   | 6A774ADE41 |
| 05c8:038f | Cheng Uei Pr... | HP TrueVision HD         | 1.6%   | 4.9.41   | 5F80EB8AB2 |
| 05c8:03ab | Cheng Uei Pr... | HP Wide Vision HD Camera | 22.2%  | 4.9.60   | 142D7492C2 |
| 05ca:1810 | Ricoh           | Pavilion Webcam [R5U870] | 6.7%   | 4.1.15   | 92CD40AFAD |
| 05ca:1830 | Ricoh           | Visual Communication ... | 100%   |          | 047C3A9402 |
| 05ca:1834 | Ricoh           | Visual Communication ... | 100%   |          | 7DFBCB9E53 |
| 05ca:183a | Ricoh           | Visual Communication ... | 14.3%  | 3.14.44  | 7B4B0311EA |
| 05ca:1870 | Ricoh           | Webcam 1000              | 100%   |          | FB7F51216E |
| 064e:a103 | Suyin           | Acer/HP Integrated We... | 1.4%   | 3.14.33  | C2904E1345 |
| 093a:7011 | Pixart Imaging  | Digital Wireless Camera  | 100%   |          | F8FD891B32 |
| 0ac8:3420 | Z-Star Micro... | Venus USB2.0 Camera      | 0.2%   | 3.14.15  | CDC3F83CDB |
| 0ac8:3450 | Z-Star Micro... | Vimicro USB Camera (A... | 0.4%   | 3.14.22  | 3C44204AA0 |
| 0ac8:c326 | Z-Star Micro... | Namuga 1.3M Webcam       | 9.1%   | 4.1.15   | 3AD0FF0E13 |
| 0ac8:c40a | Z-Star Micro... | A4 TECH USB2.0 PC Cam... | 0.3%   | 3.10.34  | B2C845B843 |
| 0b05:200b | ASUSTek Comp... | ASUS_Z00VD               | 100%   |          | EDFAB941DF |
| 0b97:8381 | O2 Micro        | Mini S USB2.0 Camera     | 100%   |          | F1A2C19FEB |
| 0bda:5520 | Realtek Semi... | Integrated_Webcam_HD     | 8%     | 4.9.60   | 90B19AF55F |
| 0bda:564b | Realtek Semi... | WebCamera                | 50%    | 5.3.0    | 5EA0111CED |
| 0bda:5650 | Realtek Semi... | Integrated Webcam_HD     | 3.7%   | 4.4.0    | 53190BC040 |
| 0bda:58be | Realtek Semi... | Laptop_Integrated_Web... | 4.2%   | 4.1.15   | A7211B4E35 |
| 0c45:62c0 | Microdia        | Sonix USB 2.0 Camera     | 1.1%   | 2.6.32   | C1A1180C7A |
| 0c45:6350 | Microdia        | USB 2.0 Camera           | 100%   |          | 34DDCDDC0E |
| 0c45:6369 | Microdia        |                          | 100%   |          | B20E10B246 |
| 0c45:6433 | Microdia        | Laptop Integrated Web... | 22.2%  | 4.9.60   | EAFEF7DB79 |
| 0c45:643f | Microdia        | Dell Integrated HD We... | 5.2%   | 4.1.15   | 4E38982788 |
| 0c45:64d2 | Microdia        | Integrated Webcam        | 4.5%   | 4.9.60   | CE392DF9C0 |
| 0c45:671d | Microdia        | Integrated_Webcam_HD     | 7.3%   | 4.15.0   | C917477768 |
| 0e8d:200b | MediaTek        | Power                    | 100%   |          | F2CD8A3FFB |
| 0fce:0a07 | Sony Ericsso... | Xperia XA2               | 100%   |          | 20DB446598 |
| 13d3:56a6 | IMC Networks    | Integrated Camera        | 3.1%   | 4.15.0   | 7D7E6AD5D5 |
| 13d3:56e4 | IMC Networks    | USB2.0 HD IR UVC WebCam  | 50%    | 5.0.0    | 65529AFB99 |
| 13d3:5727 | IMC Networks    | Lenovo EasyCamera        | 5.9%   | 4.1.15   | AB6BD693BE |
| 13d3:5a01 | IMC Networks    | USB2.0 VGA UVC WebCam    | 0.4%   | 4.9.0    | 3923D18587 |
| 152d:0770 | JMicron Tech... | Alienware Integrated ... | 33.3%  | 5.0.0    | 7E166AFA9D |
| 174f:114f | Syntek          | Lenovo EasyCamera        | 16.7%  | 3.14.44  | 2DD89E3983 |
| 174f:14af | Syntek          | Lenovo EasyCamera        | 50%    | 4.15.0   | 08BB09B100 |
| 174f:2408 | Syntek          | EasyCamera               | 5.6%   | 4.9.60   | FA64448E42 |
| 174f:5a35 | Syntek          | Sonix 1.3MPixel USB 2... | 2%     | 3.14.33  | 0A87DE5887 |
| 174f:6a33 | Syntek          | Web Cam - Asus F3SA, ... | 100%   |          | 800F54CA3A |
| 174f:6a51 | Syntek          | 2.0MPixel Web Cam - A... | 100%   |          | 39E3030E0A |
| 1782:4011 | Spreadtrum C... | Android                  | 100%   |          | 9869646781 |
| 1871:01b0 | Aveo Technology | USB2.0 Camera            | 100%   |          | 0DB51928B9 |
| 18d1:4ee2 | Google          | Nexus Device (debug)     | 100%   |          | 104196740E |
| 18ec:3399 | Arkmicro Tec... | USB2.0 PC CAMERA         | 0.8%   | 3.14.25  | 9D9E2DB550 |
| 1b17:6111 | DarkHorse .     | USB2.0 Web Camera        | 100%   |          | 6E9BA31D2B |
| 1b3b:2938 | iPassion Tec... | PC Camera/Webcam cont... | 100%   |          | 87142BF4F1 |
| 1bbb:0170 | T & A Mobile... | VFD 529                  | 100%   |          | 875A197A28 |
| 1bcf:288a | Sunplus Inno... | 1.3M HD WebCam           | 3.1%   | 3.14.44  | 8FE3AF49FB |
| 1bcf:2c6e | Sunplus Inno... | HD WebCam                | 2.4%   | 3.14.25  | 8D6D195DA2 |
| 1bcf:2c87 | Sunplus Inno... | HP Wide Vision HD        | 4.8%   | 4.9.20   | 7BD53B3FFB |
| 2104:0124 | Tobii Techno... | EyeChip                  | 10%    | 4.9.60   | ACA7993158 |
| 2717:ff10 | Android         | Android                  | 66.7%  | 4.15.0   | D633DC9722 |
| 2970:4011 | Fly             | Life Jet                 | 100%   |          | 0C91AAB0FF |
| 5986:0143 | Acer            | HP Webcam                | 7.7%   | 4.1.16   | 0C8D7641B2 |
| 5986:1141 | Acer            | Integrated IR Camera     | 12.5%  | 4.15.0   | 6A667C9BA7 |
| 5986:2113 | Acer            | Integrated Camera        | 1.6%   | 4.13.0   | 6A667C9BA7 |

### Card reader (USB)

11 out of 15 (73.33%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 072f:9000 | Advanced Car... | ACR38 AC1038-based Sm... | 16.7%  | 4.15.0   | 870D0FE48E |
| 0b0c:003f | Todos AB        | Todos C400 smartcard ... | 100%   |          | 251D958CA9 |
| 0bda:0129 | Realtek Semi... | RTS5129 Card Reader C... | 0.1%   | 3.8.0    | 3DC7CD311B |
| 0bda:0139 | Realtek Semi... | RTS5139 Card Reader C... | 0.2%   | 3.10.34  | EF015B9C0F |
| 0bda:0150 | Realtek Semi... | USB 2.0 Card Reader      | 100%   |          | 3C44204AA0 |
| 0c45:1018 | Microdia        | Compact Flash storage... | 100%   |          | 696C2127B6 |
| 0c4b:0500 | Reiner SCT K... | cyberJack RFID standa... | 83.3%  | 4.4.4    | 2F2703FBEB |
| 0c4b:0501 | Reiner SCT K... | cyberJack RFID comfor... | 55.6%  | 5.2.13   | E0585254D8 |
| 0ca6:0010 | Castles Tech... | EZUSB PC/SC Smart Car... | 100%   |          | EF816B48E7 |
| 0d8c:5200 | C-Media Elec... | Mass Storage Controll... | 100%   |          | 24A0914BA3 |
| 17ef:3075 | Lenovo          | USB Billboard Device     | 100%   |          | 5F8373C716 |

### Chipcard (USB)

44 out of 56 (78.57%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0403:e3b4 | Future Techn... | Parsec Desktop Reader... | 100%   |          | 775160993D |
| 048d:1365 | Integrated T... | SmartCard Reader         | 100%   |          | DB4B891E15 |
| 04cc:5072 | ST-Ericsson     | Chipcard Reader          | 100%   |          | 65FD9B5315 |
| 04e6:5116 | SCM Microsys... | SCR331-LC1 / SCR3310 ... | 100%   |          | 58A23E8EFE |
| 04e6:5410 | SCM Microsys... | SCR35xx Smart Card Re... | 100%   |          | 219BC0E959 |
| 04e6:e001 | SCM Microsys... | SCR331 SmartCard Reader  | 100%   |          | D3D8B39015 |
| 0529:0620 | Aladdin Know... | Token JC                 | 88.2%  | 2.6.32   | ACFF74E0DB |
| 058f:9520 | Alcor Micro     | EMV Certified Smart C... | 88.9%  | 4.15.0   | 885EC5C180 |
| 058f:9540 | Alcor Micro     | AU9540 Smartcard Reader  | 94.3%  | 4.13.0   | 345BBA3C1F |
| 072f:90cc | Advanced Car... | ACR38 SmartCard Reader   | 36.4%  | 4.8.13   | 5D250ED2A6 |
| 072f:90de | Advanced Car... | Token USB 64K            | 50%    | 4.1.25   | 02F1FBC843 |
| 072f:b000 | Advanced Car... | ACR3901U                 | 100%   |          | A44B651190 |
| 076b:1021 | OmniKey         | CardMan 1021             | 62.5%  | 4.15.0   | 3D9E77AE8A |
| 076b:3021 | OmniKey         | CardMan 3121             | 33.3%  | 3.14.33  | B45F44A0F7 |
| 076b:4321 | OmniKey         | CardMan 4321             | 100%   |          | 3191678465 |
| 076b:5421 | OmniKey         | Smart Card Reader USB    | 100%   |          | EE4E49C4A1 |
| 08e6:3437 | Gemalto (was... | GemPC Twin SmartCard ... | 100%   |          | D2B107774B |
| 08e6:3438 | Gemalto (was... | GemPC Key SmartCard R... | 100%   |          | 4CCFEAF9AE |
| 08e6:34ec | Gemalto (was... | Compact Smart Card Re... | 93.8%  | 4.15.0   | 38A59CAFAC |
| 0a5c:5800 | Broadcom        | BCM5880 Secure Applic... | 99.2%  | 3.10.36  | 32D2083BB0 |
| 0a5c:5801 | Broadcom        | BCM5880 Secure Applic... | 99.4%  | 3.16.7   | C7F7A6189C |
| 0a5c:5802 | Broadcom        | BCM5880 Secure Applic... | 100%   |          | 3FCBB46E3F |
| 0a5c:5804 | Broadcom        | BCM5880 Secure Applic... | 100%   |          | BA50FFBC59 |
| 0a5c:5805 | Broadcom        | 5880                     | 100%   |          | 83771C3BEE |
| 0a5c:5832 | Broadcom        | 5880                     | 98.4%  | 4.15.0   | 4EF902306F |
| 0a5c:5834 | Broadcom        | 5880                     | 95.1%  | 3.10.0   | E89AA0C891 |
| 0a5c:5842 | Broadcom        | 58200                    | 100%   |          | 1FA52D766E |
| 0a5c:5843 | Broadcom        | 58200                    | 100%   |          | F576DDF5DC |
| 0a89:0025 | Aktiv           | Rutoken lite             | 50%    | 4.1.25   | 8FA80B8A39 |
| 0b97:7762 | O2 Micro        | Oz776 SmartCard Reader   | 100%   |          | 48CAE00098 |
| 0b97:7772 | O2 Micro        | OZ776 CCID Smartcard ... | 97.4%  | 4.15.0   | FF0970D119 |
| 0bda:0165 | Realtek Semi... | Smart Card Reader Int... | 71.4%  | 4.4.0    | C298C38FA6 |
| 0bf8:1006 | Fujitsu Siem... | SmartCard Reader 2A      | 100%   |          | 4CDB503B48 |
| 0c4b:0580 | Reiner SCT K... | cyberJack one            | 100%   |          | 5AB1A45C53 |
| 0c4b:9102 | Reiner SCT K... | cyberJack RFID basis ... | 100%   |          | 66EEFE25AF |
| 0ca6:00a0 | Castles Tech... | EZCCID Smart Card Reader | 100%   |          | 3DC7A36CB3 |
| 0d46:3010 | Kobil Systems   | KOBIL Class 3 Reader     | 100%   |          | CE2E3AD9AE |
| 0dc3:1004 | Athena Smart... | ASEDrive CCID            | 100%   |          | AFCF4B3764 |
| 147e:2020 | Upek            | TouchChip Fingerprint... | 100%   |          | 1949413DC7 |
| 17ef:1003 | Lenovo          | Integrated Smart Card... | 94.5%  | 3.10.0   | F3FBF8BC70 |
| 1a44:0001 | VASCO Data S... | Digipass 905 SmartCar... | 75%    | 4.15.0   | AE29C83D96 |
| 1a44:0870 | VASCO Data S... | DIGIPASS 870             | 100%   |          | 1ED6532125 |
| 23a0:0004 | BIFIT           | iBank2Key                | 100%   |          | A8A89AC09A |
| 24dc:0101 | ARDS            | JaCarta                  | 100%   |          | DA308A78C4 |

### Converter (USB)

2 out of 3 (66.67%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0403:1237 | Future Techn... | Z397 GUARD Converter     | 100%   |          | 00A5CE299A |
| 110a:1110 | Moxa Technol... | UPort 1110 1-port RS-... | 66.7%  | 4.9.124  | 3864E6C70F |

### Disk (USB)

21 out of 1549 (1.36%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 048d:1336 | Integrated T... | SD/MMC Cardreader        | 0.3%   | 3.14.22  | 7E7FB78F58 |
| 058f:6362 | Alcor Micro     | Flash Card Reader/Writer | 0.1%   | 3.8.12   | 0D4B7AD71C |
| 05e3:0723 | Genesys Logic   | GL827L SD/MMC/MS Flas... | 5%     | 3.14.33  | B09664C500 |
| 0718:069c | Imation         | TF35 USB 3.0             | 100%   |          | 92BF714334 |
| 0781:5567 | SanDisk         | Cruzer Blade 16GB        | 0.2%   | 3.14.33  | 1A7FD48C0D |
| 090c:1000 | Silicon Motion  | Flash Voyager            | 0.1%   | 2.6.32   | 0C8D7641B2 |
| 0951:1666 | Kingston Tec... | DataTraveler 100 G3/G... | 0.4%   | 3.14.44  | AF97E15AFB |
| 0984:0301 | Apricorn        | SATAWire 6G              | 22.2%  | 4.15.0   | D20CC6E64D |
| 0a89:0030 | Aktiv           | Rutoken ECP 4GB          | 33.3%  | 4.1.25   | 0F33C09E44 |
| 0bda:0184 | Realtek Semi... | RTS5182 Card Reader      | 3%     | 3.14.44  | 6566319F04 |
| 0bda:0316 | Realtek Semi... | SD/MMC 128GB             | 1.3%   | 3.14.44  | 2BD257789E |
| 0bda:0328 | Realtek Semi... | SD/MMC CRW               | 2.4%   | 3.10.0   | 4B9BEB25C2 |
| 0e8d:0002 | MediaTek        | 1030D                    | 37.5%  | 4.9.60   | E4B342382F |
| 1005:b113 | Apacer Techn... | Handy Steno/AH123 / H... | 0.3%   | 3.0.28   | 8652B8318D |
| 12d1:2590 | Huawei Techn... | ORINOQUIA Auyantepui+... | 100%   |          | BEBC187DBD |
| 1307:1171 | Transcend       | Fingerprint Reader       | 85.7%  | 4.12.14  | 35D850590E |
| 13fd:1617 | Initio          | Flash Padlock            | 100%   |          | 95CE4B3495 |
| 13fe:5500 | Kingston Tec... | Silicon-Power32G 31GB    | 1.7%   | 3.14.44  | CE392DF9C0 |
| 5136:4678 | Generic         | Flash Disk 2.0           | 22.2%  | 4.1.38   | C1841B0A29 |
| 8644:8303 | Intenso GmbG    | Supra 32GB               | 20%    | 4.9.20   | CE376CD0F4 |
| ffff:5678 | VendorCo        | ProductCode 16GB         | 6.7%   | 4.4.0    | C7F73C8073 |

### Dvb card (USB)

12 out of 51 (23.53%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 07ca:0810 | AVerMedia Te... | H810 USB Hybrid DVB-T    | 100%   |          | B46F2FEE35 |
| 07ca:0830 | AVerMedia Te... | H830 USB Hybrid DVB-T    | 100%   |          | 79A097BF6F |
| 07ca:0831 | AVerMedia Te... | H831 USB Hybrid DVB-T/T2 | 100%   |          | D5A4F195AE |
| 07ca:1334 | AVerMedia Te... | H334 MiniCard Hybrid ... | 100%   |          | 647613F22B |
| 07ca:1336 | AVerMedia Te... | A336 MiniCard Hybrid ... | 100%   |          | A2FF4426C9 |
| 07ca:4336 | AVerMedia Te... | A336 MiniCard Hybrid ... | 100%   |          | 0C3E26BCE7 |
| 0bda:2832 | Realtek Semi... | RTL2832U DVB-T           | 18.2%  | 4.1.19   | 9994FB8ABA |
| 0bda:2838 | Realtek Semi... | RTL2838 DVB-T            | 7.9%   | 3.14.25  | 032EB66625 |
| 13d3:3282 | IMC Networks    | DVB-T + GPS Minicard ... | 100%   |          | 7F0F347502 |
| 1b80:c161 | Afatech         | DVB-T 2                  | 100%   |          | 2A8FB37B8C |
| 1b80:e39a | Afatech         | DVB-T395U [af9015]       | 100%   |          | 2A8FB37B8C |
| eb1a:5013 | eMPIA Techno... | USB 2883 Device          | 100%   |          | 5DD14F9164 |

### Fingerprint reader (USB)

61 out of 62 (98.39%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0483:2016 | STMicroelect... | Fingerprint Reader       | 100%   |          | 5823C076FA |
| 04e8:730a | Samsung Elec... | Fingerprint Device       | 100%   |          | 3701BEE474 |
| 04f3:0903 | Elan Microel... | ELAN:Fingerprint         | 100%   |          | 9809687258 |
| 04f3:0c03 | Elan Microel... | ELAN:Fingerprint         | 100%   |          | BAE5A5C3DD |
| 04f3:0c1a | Elan Microel... | ELAN:Fingerprint         | 100%   |          | 4DCFEFF869 |
| 04f3:0c3a | Elan Microel... | Elan Security-WBF Fin... | 100%   |          | F3F60A5C06 |
| 05ba:0002 | DigitalPersona  | Fingerprint Scanner, ... | 100%   |          | AE361E5F23 |
| 06cb:0078 | Synaptics       | WBDI Device              | 100%   |          | 4A5BA1C902 |
| 06cb:0081 | Synaptics       | Synaptics WBDI           | 100%   |          | B0FCF85E0D |
| 06cb:0082 | Synaptics       | My Lockey                | 100%   |          | F2B50C0999 |
| 06cb:009a | Synaptics       | Synaptics WBDI           | 100%   |          | 98395B298B |
| 06cb:00a2 | Synaptics       | Synaptics WBDI           | 100%   |          | F4826C3A2A |
| 06cb:00b7 | Synaptics       | Synaptics VFS7552 Tou... | 100%   |          | 0B8C8AB6F3 |
| 06cb:00bd | Synaptics       |                          | 100%   |          | 1820A998EC |
| 08ff:1600 | AuthenTec       | AES1600                  | 100%   |          | B720D65E19 |
| 08ff:1660 | AuthenTec       | AES1660 Fingerprint S... | 100%   |          | 89EC4F0398 |
| 08ff:1686 | AuthenTec       | Fingerprint Sensor       | 100%   |          | 32C7E07A9A |
| 08ff:168a | AuthenTec       | Fingerprint Sensor       | 100%   |          | EBCFDCE11A |
| 08ff:168b | AuthenTec       | Fingerprint Sensor       | 100%   |          | 9BE4F247B6 |
| 08ff:168c | AuthenTec       | Fingerprint Sensor       | 100%   |          | DA5EB48DBB |
| 08ff:168f | AuthenTec       | AES1660 Fingerprint S... | 100%   |          | 07B13B0CD0 |
| 08ff:2500 | AuthenTec       | AES2501                  | 100%   |          | 4DCFB332DF |
| 08ff:2550 | AuthenTec       | AES2550 Fingerprint S... | 100%   |          | 09C1DFABF4 |
| 08ff:2580 | AuthenTec       | AES2501 Fingerprint S... | 100%   |          | 65DCADAC42 |
| 08ff:2665 | AuthenTec       | Fingerprint Sensor       | 100%   |          | 6A0E9D372C |
| 08ff:2683 | AuthenTec       | Fingerprint Sensor       | 100%   |          | 52882927F1 |
| 08ff:2691 | AuthenTec       | Fingerprint Sensor       | 100%   |          | 79E75DF44E |
| 08ff:2810 | AuthenTec       | AES2810                  | 100%   |          | 1A90AC4588 |
| 138a:0001 | Validity Sen... | VFS101 Fingerprint Re... | 100%   |          | F31F2EC406 |
| 138a:0005 | Validity Sen... | VFS301 Fingerprint Re... | 100%   |          | 566E1793D3 |
| 138a:0007 | Validity Sen... | VFS451 Fingerprint Re... | 99.3%  | 5.1.4    | 82CB2D5E90 |
| 138a:0008 | Validity Sen... | VFS300 Fingerprint Re... | 100%   |          | 1BB8E0A4D4 |
| 138a:0010 | Validity Sen... | VFS Fingerprint sensor   | 100%   |          | 11B6D41A9A |
| 138a:0011 | Validity Sen... | VFS5011 Fingerprint R... | 100%   |          | AFC9FC3D29 |
| 138a:0017 | Validity Sen... | VFS 5011 fingerprint ... | 99.1%  | 4.18.0   | 14015A6CDE |
| 138a:0018 | Validity Sen... | Fingerprint scanner      | 100%   |          | 56BA5D2A72 |
| 138a:003c | Validity Sen... | VFS471 Fingerprint Re... | 98%    | 5.2.5    | 3EAB448396 |
| 138a:003d | Validity Sen... | VFS491                   | 100%   |          | 57308077EE |
| 138a:003f | Validity Sen... | VFS495 Fingerprint Re... | 96.9%  | 4.15.0   | D85B25CD22 |
| 138a:0050 | Validity Sen... | Swipe Fingerprint Sensor | 100%   |          | 18D138561D |
| 138a:0090 | Validity Sen... | VFS7500 Touch Fingerp... | 97.2%  | 4.15.0   | 3504F119EA |
| 138a:0091 | Validity Sen... | VFS7552 Touch Fingerp... | 100%   |          | 14C2B3FA53 |
| 138a:0092 | Validity Sen... | Synaptics VFS7552 Tou... | 100%   |          | E9DECBC4FD |
| 138a:0094 | Validity Sen... | Synaptics WBDI           | 100%   |          | A549A39A12 |
| 138a:0097 | Validity Sen... | Synaptics WBDI           | 100%   |          | 46BFB60272 |
| 138a:009d | Validity Sen... | Synaptics WBDI           | 100%   |          | 0818236221 |
| 138a:00a6 | Validity Sen... | Synaptics VFS7552 Tou... | 100%   |          | 2687FA68FB |
| 138a:00ab | Validity Sen... | Synaptics VFS7552 Tou... | 100%   |          | 65B1EB0CA1 |
| 147e:1000 | Upek            | Biometric Touchchip/T... | 100%   |          | B7F262168C |
| 147e:1001 | Upek            | TCS5B Fingerprint sensor | 100%   |          | AAB454995E |
| 147e:1002 | Upek            | Biometric Touchchip/T... | 100%   |          | 91C9287871 |
| 147e:2016 | Upek            | Biometric Touchchip/T... | 100%   |          | 6EFC416CE0 |
| 1c7a:0570 | LighTuning T... | EgisTec Touch Fingerp... | 100%   |          | 82680EE78B |
| 1c7a:0603 | LighTuning T... | EgisTec ES603            | 100%   |          | D75C0B2DA5 |
| 1c7a:0801 | LighTuning T... | Fingerprint Reader       | 100%   |          | DF25B03899 |
| 27c6:5117 | Shenzhen Goo... | Fingerprint Reader       | 100%   |          | 53631F5F96 |
| 27c6:530c | Shenzhen Goo... | Fingerprint Reader       | 100%   |          | DAE953BAB0 |
| 27c6:538c | Goodix          | FingerPrint              | 100%   |          | 85BB9ECF3B |
| 27c6:5584 | Generic         | Goodix FingerPrint De... | 100%   |          | D1CA80EDFF |
| 27c6:55a4 | Generic         | Goodix FingerPrint De... | 100%   |          | E4301E56F9 |
| 27c6:55b4 | Generic         | Goodix FingerPrint De... | 94.1%  | 5.3.0    | B49AAC1247 |

### Hardware key (USB)

4 out of 4 (100%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0471:485d | Philips (or ... | Senselock SenseIV v2.x   | 100%   |          | E4A6E39276 |
| 0a89:0003 | Aktiv           | Guardant Stealth/Net II  | 100%   |          | 5149320E81 |
| 0a89:0020 | Aktiv           | Rutoken S                | 72.7%  | 3.14.15  | 35FB98B552 |
| 14a8:0001 | Soft protect... | Soft protection devic... | 100%   |          | 4015843475 |

### Hasp (USB)

1 out of 1 (100%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0529:0001 | Aladdin Know... | HASP copy protection ... | 100%   |          | 4015843475 |

### Hub (USB)

9 out of 376 (2.39%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 03eb:3301 | Atmel           | at43301 4-Port Hub       | 3.8%   | 3.14.44  | 8CF625BE49 |
| 0451:1446 | Texas Instru... | TUSB2040/2070 Hub        | 9.1%   | 4.15.0   | 593A72A02B |
| 0a05:7211 | Unknown Manu... | hub                      | 5.6%   | 3.14.44  | C389CF184F |
| 1a40:0101 | incomplete h... | 4-Port HUB               | 0.1%   | 3.2.0    | 9596ECB170 |
| 8087:0020 | Intel           | Integrated Rate Match... | 0%     | 3.0.28   | 57943279FE |
| 8087:0024 | Intel           | Integrated Rate Match... | 0.1%   | 3.10.0   | 269CE86EE6 |
| 8087:8000 | Intel           | Hub                      | 0%     | 2.6.32   | CE392DF9C0 |
| 8087:8001 | Intel           | Hub                      | 0.2%   | 2.6.32   | BD6F7205F3 |
| 8087:8008 | Intel           | Hub                      | 0%     | 2.6.32   | 31E99D9CEA |

### Human interface (USB)

4 out of 432 (0.93%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 044f:b10a | ThrustMaster    | T.16000M Joystick        | 9.1%   | 4.1.25   | 417453E269 |
| 04b4:fd13 | Cypress Semi... | Programmable power so... | 50%    | 4.18.0   | 7C4C7CAF9A |
| 11ff:3341 |                 | USB Joystick             | 20%    | 4.1.7    | CD7FA9B160 |
| 1770:ff00 | MSI EPF USB     | MSI EPF USB / LED con... | 0.5%   | 3.10.0   | 1C47BC90E4 |

### Imaging (USB)

1 out of 2 (50%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 04a7:04d0 | Visioneer       | Xerox DocuMate 5460      | 100%   |          | 4ABAC242CC |

### Input/keyboard (USB)

4 out of 1477 (0.27%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0624:0294 | Avocent         | Dell 03R874 KVM dongle   | 100%   |          | 97313ACF09 |
| 0a5c:4502 | Broadcom        | Keyboard (Boot Interf... | 0.6%   | 3.0.28   | 0C3E26BCE7 |
| 0b05:17fd | ASUSTek Comp... | ASUS ROG Macrokey        | 11.1%  | 3.14.44  | C5777BA928 |
| 0c45:7401 | Microdia        | TEMPer Temperature Se... | 89.5%  | 4.15.0   | 2AD366F4C0 |

### Input/mouse (USB)

12 out of 1496 (0.80%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0458:003a | KYE Systems ... | NetScroll+ Mini Trave... | 0.1%   | 3.10.0   | 5599435B69 |
| 045e:0040 | Microsoft       | Wheel Mouse Optical      | 0.6%   | 3.14.25  | BFCD766C51 |
| 046d:c06c | Logitech        | Optical Mouse            | 0.4%   | 2.6.32   | C6690BB6D9 |
| 048d:8910 | Integrated T... | ITE Device(8910)         | 5.3%   | 4.13.0   | 2D91F64A77 |
| 04b4:0033 | Cypress Semi... | Mouse                    | 0.9%   | 3.14.25  | 4BCDE0B215 |
| 0bc7:0006 | X10 Wireless... | Wireless Transceiver ... | 18.4%  | 3.14.25  | ADF2D5DACA |
| 1532:0042 | Razer USA       | Abyssus 2014             | 12.5%  | 4.9.76   | 31E99D9CEA |
| 18d1:4ee7 | Google          | ZTE A2017U               | 77.8%  | 5.0.0    | 6D14F41FBD |
| 18f8:0f97 | [Maxxter]       | USB OPTICAL MOUSE        | 0.3%   | 4.1.15   | BEADDBA484 |
| 1c4f:0034 | SiGma Micro     | Usb Mouse                | 0.2%   | 3.10.0   | 6834F4BC15 |
| 413c:8158 | Dell            | Integrated Touchpad /... | 71.4%  | 3.14.44  | FE08C422A4 |
| 413c:8162 | Dell            | Integrated Touchpad [... | 77.5%  | 3.14.33  | 73BB565F78 |

### Modem (USB)

5 out of 110 (4.55%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 04e8:6773 | Samsung Elec... | HSPA Modem               | 66.7%  | 4.15.0   | 3AD0FF0E13 |
| 0572:cb16 | Conexant Sys... | USB-ADSL Modem           | 100%   |          | 07217A2477 |
| 0baf:00ec | U.S. Robotics   | 56K Faxmodem             | 100%   |          | EF974030B3 |
| 0bdb:1926 | Ericsson Bus... | H5321 gw Mobile Broad... | 2.2%   | 3.10.0   | B2ECBDE0F2 |
| 27c6:5301 | HTMicroelect... | Goodix Fingerprint De... | 3%     | 4.4.0    | 716CB93844 |

### Net/wimax (USB)

3 out of 6 (50%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 8086:0186 | Intel           | WiMAX Connection 2400m   | 7%     | 3.14.44  | 78F773AA5C |
| 8086:1406 | Intel           | WiMAX Connection 2400m   | 3.8%   | 3.10.19  | 5971AC1B90 |
| 8087:07d6 | Intel           | Centrino WiMAX 6150      | 12.5%  | 3.10.34  | 1D59A8F384 |

### Net/wireless (USB)

78 out of 256 (30.47%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0411:0242 | BUFFALO         | RTL8811AU WI-U2-433DM... | 100%   |          | D92D4F0666 |
| 0457:0162 | Silicon Inte... | SiS162 usb Wireless L... | 100%   |          | D625F7E867 |
| 045e:0292 | Microsoft       | Xbox360 Wireless Netw... | 100%   |          | 90D3759348 |
| 050d:110a | Belkin Compo... | F9L1101v2 802.11abgn ... | 100%   |          | 506F4A7C1D |
| 050d:615a | Belkin Compo... | F7D4101 / F9L1101v1 8... | 100%   |          | 04CE720011 |
| 050d:7050 | Belkin Compo... | F5D7050 Wireless G Ad... | 100%   |          | 7AC6824CEB |
| 0586:3425 | ZyXEL Commun... | MT7610U NWD6505 802.1... | 100%   |          | 57B1BCAC00 |
| 0586:3426 | ZyXEL Commun... | ZyXEL Dual-Band Wirel... | 66.7%  | 5.3.11   | A7FCEE3095 |
| 07d1:3a0d | D-Link System   | DWA-120 802.11g Wirel... | 100%   |          | A8A7EB8824 |
| 07d1:3b01 | D-Link System   | AirPlus G DWL-G122 Wi... | 100%   |          | A55363D509 |
| 07d1:3b11 | D-Link System   | DWA-130 802.11n Wirel... | 100%   |          | 606522CEDA |
| 0846:9011 | NetGear         | BCM4323 WNDA3100v2 80... | 100%   |          | 9DA498DED3 |
| 0846:9014 | NetGear         | WNDA3100v3 802.11abgn... | 100%   |          | 96CA792DC8 |
| 0846:9020 | NetGear         | BCM43231 WNA3100(v1) ... | 100%   |          | 68CF43B792 |
| 0846:9050 | NetGear         | A6200 802.11a/b/g/n/a... | 100%   |          | B4AFED8FAD |
| 0846:9052 | NetGear         | RTL8811AU A6100 AC600... | 36%    | 4.15.0   | 1F8881A081 |
| 0a5c:bd11 | Broadcom        | BCM4320 802.11bg Wire... | 100%   |          | CA66B01DF7 |
| 0a5c:bd13 | Broadcom        | BCM4323 802.11abgn Wi... | 100%   |          | B220FD9C11 |
| 0b05:17c9 | ASUSTek Comp... | USB-AC53 802.11a/b/g/... | 100%   |          | C7951A3833 |
| 0b05:17d1 | ASUSTek Comp... | MT7610U AC51 802.11a/... | 64.7%  | 5.0.0    | 8EBA4B1357 |
| 0b05:17d2 | ASUSTek Comp... | USB-AC56 802.11a/b/g/... | 100%   |          | 2F6DFEC51C |
| 0b05:17db | ASUSTek Comp... | MT7610U USB-AC50 802.... | 100%   |          | 93C92CF446 |
| 0b05:1817 | ASUSTek Comp... | RTL8814AU USB-AC68 80... | 93.3%  | 4.15.0   | 464709685B |
| 0b05:1841 | ASUSTek Comp... | 802.11ac NIC             | 33.3%  | 4.15.0   | 4B4C28ABBC |
| 0b05:184c | ASUSTek Comp... | RTL8812BU USB-AC53 Na... | 94.1%  | 4.18.0   | BA1D0F6920 |
| 0b05:1852 | ASUSTek Comp... | 802.11ac NIC             | 100%   |          | D043FCBC96 |
| 0bda:0811 | Realtek Semi... | RTL8811AU 802.11ac WL... | 55%    | 4.15.0   | D75C0B2DA5 |
| 0bda:8176 | Realtek Semi... | RTL8188CUS 802.11n WL... | 0.6%   | 3.14.25  | 51837DE98F |
| 0bda:8179 | Realtek Semi... | RTL8188EUS 802.11n Wi... | 0.9%   | 3.14.25  | 2F2703FBEB |
| 0bda:818b | Realtek Semi... | RTL8192EU ACT-WNP-UA-... | 13.4%  | 4.9.0    | 9D85C4CA60 |
| 0bda:8812 | Realtek Semi... | RTL8812AU 802.11a/b/g... | 34%    | 4.1.38   | 71C83542C5 |
| 0bda:8813 | Realtek Semi... | RTL8814AU 802.11a/b/g... | 100%   |          | D32464D841 |
| 0bda:a811 | Realtek Semi... | RTL8811AU 802.11a/b/g... | 83.3%  | 4.15.0   | E50B6BA10C |
| 0bda:b711 | Realtek Semi... | RTL8188GU 802.11n WLA... | 100%   |          | 1E21855EB2 |
| 0bda:b812 | Realtek Semi... | RTL8812BU USB3.0 802.... | 61.7%  | 4.9.155  | B5C538F345 |
| 0bda:c811 | Realtek Semi... | RTL8811CU 802.11ac NIC   | 74.3%  | 4.4.0    | 1F9408B984 |
| 0bda:f179 | Realtek Semi... | 802.11n                  | 90%    | 4.18.0   | 7605FC1D79 |
| 0bf8:100f | Fujitsu Siem... | miniCard D2301 802.11... | 100%   |          | 40B94D516E |
| 0cde:0015 | Z-Com           | ISL3887 XG-705A 802.1... | 100%   |          | B4E374835E |
| 0cf3:9271 | Qualcomm Ath... | AR9271 802.11n           | 0.2%   | 3.14.25  | E6A7D05EF4 |
| 0e8d:760c | MediaTek        | 802.11 n WLAN            | 100%   |          | 74DFE126D0 |
| 0e8d:7610 | MediaTek        | MT7610U WiFi             | 85.7%  | 4.15.0   | F75495E252 |
| 0e8d:7612 | MediaTek        | 802.11ac WLAN            | 83.3%  | 5.0.0    | 2373345C64 |
| 13b1:0029 | Linksys         | WUSB300N 802.11bgn Wi... | 100%   |          | 18CF7C0503 |
| 13b1:003a | Linksys         | BCM43236 AE2500 802.1... | 100%   |          | 913FC75AA0 |
| 13b1:003e | Linksys         | MT7610U AE6000 802.11... | 100%   |          | 0370C48B5C |
| 13b1:003f | Linksys         | RTL8812AU WUSB6300 80... | 56.2%  | 4.1.19   | 92100B9B64 |
| 13b1:0042 | Linksys         | QCA9377 WUSB6100M 802... | 25%    | 4.15.0   | 5155142A94 |
| 148f:7601 | Ralink Techn... | MT7601U Wireless Adapter | 13.7%  | 3.14.33  | 67D2092578 |
| 148f:760b | Ralink Techn... | MT7601U Wireless Adapter | 36.4%  | 3.14.33  | D3D5F51D7A |
| 148f:761a | Ralink Techn... | MT7610U ("Archer T2U"... | 66.7%  | 4.18.0   | 667DF7FB6C |
| 1eda:2610 | AirTies Wire... | AirTies Wireless Adapter | 100%   |          | 591BDD6E15 |
| 2001:3314 | D-Link          | RTL8821AU DWA-171 802... | 39.1%  | 4.4.0    | D85422E2C1 |
| 2001:3315 | D-Link          | RTL8812AU DWA-182 Wir... | 45.5%  | 3.14.39  | 1111158623 |
| 2001:3319 | D-Link          | RTL8192EU DWA-131 Wir... | 35.6%  | 4.1.38   | 58607ACCAE |
| 2001:331c | D-Link          | 802.11ac NIC             | 50%    | 4.15.0   | 724931A3B9 |
| 2357:0101 | Realtek         | RTL8812AU Archer T4U ... | 27.3%  | 4.1.25   | 915F8EEC67 |
| 2357:0103 | Realtek         | RTL8812AU Archer T4UH... | 50%    | 3.14.44  | D804242BA9 |
| 2357:0105 | MediaTek        | MT7610U Archer T1U 80... | 88.9%  | 5.0.0    | E68759AA8E |
| 2357:0106 | TP-Link         | 802.11ac NIC             | 100%   |          | 62B0B05A66 |
| 2357:0107 | Realtek         | RTL8192EU TL-WN821N V... | 18.2%  | 4.9.155  | 6CF7359C7E |
| 2357:0109 | Realtek         | RTL8192EU TL-WN823N 8... | 7.4%   | 3.16.0   | CA04809D83 |
| 2357:010c | Realtek         | RTL8188EUS TL-WN722N v2  | 4.3%   | 4.9.41   | 90A8CF6632 |
| 2357:010d | Realtek         | RTL8812AU TP-Link Arc... | 46.7%  | 4.15.0   | C6F604105F |
| 2357:010e | Realtek         | RTL8812AU TL-WN722N v2   | 100%   |          | 40817D415E |
| 2357:0111 | TP-Link         | 802.11n NIC              | 100%   |          | 4FFA15CD0F |
| 2357:0115 | TP-Link         | 802.11ac NIC             | 50%    | 4.15.0   | 419565138F |
| 2357:011e | TP-Link         | 802.11ac WLAN Adapter    | 75%    | 4.17.0   | BA4440586C |
| 2357:011f | TP-Link         | 802.11ac WLAN Adapter    | 100%   |          | 68248270EE |
| 2357:0120 | TP-Link         | 802.11ac WLAN Adapter    | 100%   |          | 49E321F31A |
| 2357:0122 | TP-Link         | 802.11n NIC              | 50%    | 4.18.0   | 7F6510382A |
| 2357:0126 | TP-Link         | 802.11n NIC              | 66.7%  | 4.18.0   | 355D2DD10F |
| 2357:012d | TP-Link         | 802.11ac NIC             | 50%    | 4.15.0   | 0D4A781BD5 |
| 2604:0012 | Realtek         | RTL8812AU Tenda U12 8... | 83.3%  | 4.15.0   | C1F0DB0D58 |
| 2c4e:0100 | Realtek         | RTL8192EU WLAN contro... | 55.6%  | 4.9.124  | 2CE91A523F |
| 2c4e:0102 | Realtek         | 802.11n NIC              | 100%   |          | DE9CAC1509 |
| 413c:8102 | Dell            | TrueMobile 1300 802.1... | 100%   |          | 5776ED841E |
| 4317:0720 | Broadcom        | Dynex DX-BUSB            | 100%   |          | 806CA649D7 |

### Network (USB)

9 out of 234 (3.85%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 05ac:12ab | Apple           | iPad 4/Mini1             | 33.3%  | 4.10.0   | AB105D132E |
| 0846:9053 | NetGear         | A6210                    | 55%    | 4.15.0   | 31B6C12A09 |
| 0bda:8153 | Realtek Semi... | RTL8153 Gigabit Ether... | 0.4%   | 4.1.15   | 08BB09B100 |
| 0bda:b720 | Realtek Semi... | RTL8723BU 802.11n WLA... | 4.8%   | 4.4.1    | 0F4722247C |
| 2001:330f | D-Link          | RTL8188ETV DWA-125 11... | 3.2%   | 3.14.44  | 01D21EA756 |
| 2001:3318 | D-Link          | 11ac adapter             | 75%    | 4.1.34   | 22D7E30FD4 |
| 7392:a812 | Edimax Techn... | RTL8811AU AC600 USB      | 31.6%  | 3.14.25  | 0B6B3550B5 |
| 7392:a833 | Edimax Techn... | AC1750 USB               | 25%    | 4.15.0   | 4D2C5EC5BB |
| 7392:b822 | Edimax Techn... | AC1200 MU-MIMO USB2.0... | 80%    | 4.18.0   | 6C6668A1A5 |

### Sound (USB)

3 out of 455 (0.66%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 046d:0a46 | Logitech        |                          | 50%    | 5.0.0    | 46B504A53C |
| 0763:2012 | M-Audio         | M-Audio Fast Track Pro   | 33.3%  | 4.15.0   | 1D9934126C |
| 0a12:1243 | Cambridge Si... | CSRA64110 USB Audio      | 60%    | 5.2.6    | 2A3F7B30CC |

### Tv card (USB)

4 out of 100 (4%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 046d:08a2 | Logitech        | Labtec Webcam Pro        | 25%    | 3.14.44  | 51837DE98F |
| 07ca:0889 | AVerMedia Te... | AVerTV Satellite 2       | 100%   |          | 174EC665C6 |
| 0ac8:c002 | Z-Star Micro... | Visual Communication ... | 20%    | 4.9.9    | 7F0BB0CC92 |
| 0c45:6030 | Microdia        | VideoCAM ExpressII       | 100%   |          | 6F28F56C47 |

### Ups (USB)

2 out of 21 (9.52%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0592:0002 | Powerware       | UPS (X-Slot)             | 100%   |          | 049C18DB44 |
| 06da:0002 | Phoenixtec P... | UPS                      | 100%   |          | 4F5E89A87E |

### Video (USB)

5 out of 7 (71.43%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0fd9:0051 | Elgato Systems  | GameCapture HD           | 100%   |          | 05F988930D |
| 1164:1ee9 | YUAN High-Te... | Polaris AV Capture       | 100%   |          | A2613DB100 |
| 1b80:a41c | Afatech         | Polaris AV Capture       | 100%   |          | F20674C0B8 |
| 2304:0224 | Pinnacle Sys... | MovieBox Plus (710-USB)  | 100%   |          | E9365BC8D0 |
| 5555:3382 | Epiphan Systems | VGA2USB Frame Grabber    | 100%   |          | 37A831391B |

### Wireless (USB)

1 out of 30 (3.33%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 15a9:003a | Gemtek          | Modem YOTA 4G LTE        | 100%   |          | 02E0DBC8D3 |

