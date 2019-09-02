Devices with poor Linux-compatibility
=====================================

This is a project to find PCI/USB devices with poor Linux-compatibility based on the [hwinfo](https://github.com/openSUSE/hwinfo)
reports collected by Linux users at https://linux-hardware.org.

In the scope of this project, the device is considered poorly supported by Linux if driver
is not found for this device in at least one user probe on any Linux distribution.

You can find appropriate hwinfo report in this repository by a probe ID as follows:

    find . -name {PROBE ID}

Everyone can contribute to this repository by uploading probes of their computers
by the [hw-probe](https://github.com/linuxhw/hw-probe) tool:

    sudo hw-probe -all -upload

Total reports: 52030.

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
| 1814:3298 | 103c:18ec | Ralink          | RT3290 Bluetooth         | 99.5%  | 4.18.0   | A978F2CA38 |
| 1814:3298 | 103c:191c | Ralink          | RT3290 Bluetooth         | 100%   |          | 9B25B9E02E |
| 1814:3298 | 105b:e056 | Ralink          | RT3290 Bluetooth         | 100%   |          | F71E42FC3C |
| 1814:3298 | 10cf:1772 | Ralink          | RT3290 Bluetooth         | 100%   |          | 1135E21142 |
| 1814:3298 | 1814:3298 | Ralink          | RT3290 Bluetooth         | 100%   |          | FE9255E7F3 |
| 1814:3298 | 1a3b:210b | Ralink          | RT3290 Bluetooth         | 100%   |          | 2333E930AF |
| 1814:3298 | 1a3b:2787 | Ralink          | RT3290 Bluetooth         | 100%   |          | 4C67B55B77 |
| 1814:3298 | 1a3b:2987 | Ralink          | RT3290 Bluetooth         | 100%   |          | 8D13B8BFE3 |
| 1814:3298 | 1a3b:2f87 | Ralink          | RT3290 Bluetooth         | 100%   |          | 45F3B356CF |

### Card reader (PCI)

19 out of 670 (2.84%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 10ec:5227 | 1179:0001 | Realtek Semi... | RTS5227 PCI Express C... | 20%    | 4.15.0   | 550460AAAC |
| 10ec:5227 | 1462:10f4 | Realtek Semi... | RTS5227 PCI Express C... | 100%   |          | 852662BDF3 |
| 10ec:522a | 103c:806e | Realtek Semi... | RTS522A PCI Express C... | 100%   |          | 62A9EF950E |
| 10ec:522a | 103c:8079 | Realtek Semi... | RTS522A PCI Express C... | 16.7%  | 4.4.1    | 15E62C605F |
| 10ec:522a | 103c:80a4 | Realtek Semi... | RTS522A PCI Express C... | 33.3%  | 4.9.60   | B01FB51118 |
| 10ec:522a | 103c:80ff | Realtek Semi... | RTS522A PCI Express C... | 66.7%  | 4.7.2    | B7B039F46E |
| 10ec:522a | 103c:8100 | Realtek Semi... | RTS522A PCI Express C... | 100%   |          | 2B56F34E21 |
| 10ec:522a | 103c:8101 | Realtek Semi... | RTS522A PCI Express C... | 25%    | 4.9.60   | BC496704F4 |
| 10ec:522a | 103c:820c | Realtek Semi... | RTS522A PCI Express C... | 25%    | 4.9.20   | FAE1CD27F3 |
| 10ec:522a | 103c:8392 | Realtek Semi... | RTS522A PCI Express C... | 66.7%  | 4.9.20   | 142D7492C2 |
| 10ec:522a | 103c:84db | Realtek Semi... | RTS522A PCI Express C... | 50%    | 4.18.0   | 06EE78EE4D |
| 10ec:522a | 17aa:5048 | Realtek Semi... | RTS522A PCI Express C... | 33.3%  | 4.15.0   | 842B139FE7 |
| 10ec:522a | 17aa:5113 | Realtek Semi... | RTS522A PCI Express C... | 25%    | 4.15.0   | 32F7318757 |
| 10ec:5287 | 1025:0866 | Realtek Semi... | RTL8411B PCI Express ... | 1.2%   | 3.14.25  | 798177A8A9 |
| 10ec:5289 | 1043:1447 | Realtek Semi... | RTL8411 PCI Express C... | 6.7%   | 3.14.44  | F23B5BF0DA |
| 1aea:6601 | 0001:0001 | Alcor Micro     | AU6601 PCI-E Flash ca... | 60%    | 4.9.0    | 740C1D3CBF |
| 1aea:6601 | 1179:f900 | Alcor Micro     | AU6601 PCI-E Flash ca... | 100%   |          | 43A9D7922A |
| 1aea:6621 | 1aea:6621 | Alcor Micro     | Alcor Micro PCIe Card... | 81.8%  | 5.0.0    | B4ED65654C |
| 1aea:6625 | 103c:83a9 | Alcor Micro     | Alcor Micro PCIe Card... | 100%   |          | A68CD7F224 |

### Communication controller (PCI)

218 out of 2354 (9.26%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 04f1:2f20 | 04f1:200c |                 | Communication controller | 100%   |          | 6759172767 |
| 104c:8035 | 103c:0934 | Texas Instru... | PCIxx21/PCIxx11 Smart... | 100%   |          | 16F00AAE37 |
| 104c:8035 | 103c:0944 | Texas Instru... | PCIxx21/PCIxx11 Smart... | 100%   |          | 5DA5847C6D |
| 104c:8035 | 103c:099c | Texas Instru... | PCIxx21/PCIxx11 Smart... | 100%   |          | AFE75774F3 |
| 104c:8038 | 1028:0182 | Texas Instru... | PCI6515 SmartCard Con... | 100%   |          | D134258917 |
| 104c:8038 | 1028:0186 | Texas Instru... | PCI6515 SmartCard Con... | 100%   |          | DEEA511BCD |
| 104c:8038 | 1028:0187 | Texas Instru... | PCI6515 SmartCard Con... | 100%   |          | 358447EB4E |
| 104c:803d | 103c:309f | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | 5BE41E5F47 |
| 104c:803d | 103c:30a3 | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | E5523A66D5 |
| 104c:803d | 103c:30aa | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | CF41AB5F1A |
| 104c:803d | 103c:30ac | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | 3604EF7ED6 |
| 104c:803d | 103c:30ad | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | 9F51D8D813 |
| 104c:803d | 103c:30b1 | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | D4DC67EA5D |
| 104c:803d | 1071:8212 | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | 01F778FE4E |
| 1093:c801 |           | National Ins... | PCI-GPIB                 | 100%   |          | 29A0FC6CE0 |
| 11c1:0480 | 1668:0500 | LSI             | Venus Modem (V90, 56K... | 25%    | 3.14.22  | 0A61436F40 |
| 11c1:048c | 11c1:044c | LSI             | V.92 56K WinModem        | 100%   |          | 6A798F999C |
| 11c1:0620 | 11c1:0620 | LSI             | Lucent V.92 Data/Fax ... | 100%   |          | 005023EE9D |
| 11c1:0630 | 11c1:0630 | LSI             | PCI-SV92EX Soft Modem    | 100%   |          | 96600BDB45 |
| 11c1:0630 | 11c1:0631 | LSI             | PCI-SV92EX Soft Modem    | 100%   |          | A496E46CB4 |
| 125d:2838 | 125d:2838 | ESS Technology  | ES2838/2839 SuperLink... | 100%   |          | 5E6A0F1B7E |
| 127a:2015 | 127a:2015 | Rockwell Int... | HSF 56k Data/Fax/Voic... | 100%   |          | 55EC1147BA |
| 13f6:0211 | 13f6:0211 | C-Media Elec... | CM8738                   | 100%   |          | F207A07F05 |
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
| 14f1:2f00 | 14f1:2004 | Conexant Sys... | HSF 56k HSFi Modem       | 100%   |          | C78BDF01D1 |
| 14f1:2f00 | 187e:3409 | Conexant Sys... | HSF 56k HSFi Modem       | 100%   |          | C1BD1568DC |
| 14f1:2f12 | 16ec:2016 | Conexant Sys... | HSF Data/Fax/Voice (USA) | 100%   |          | 3ADDAB1A1D |
| 14f1:2f20 | 14f1:200c | Conexant Sys... | HSF 56k Data/Fax Modem   | 100%   |          | 9E3BA9F39A |
| 14f1:2f20 | 14f1:200f | Conexant Sys... | HSF 56k Data/Fax Modem   | 100%   |          | BC9F90FD94 |
| 14f1:2f30 | 14f1:200f | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | 68ADD91E03 |
| 14f1:2f30 | 14f1:2014 | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | 1930575F3E |
| 14f1:2f30 | 14f1:2051 | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | 7E932C8DF9 |
| 14f1:2f30 | 14f1:2075 | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | BBF84F3432 |
| 14f1:2f30 | 14f1:20d5 | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | 16CD9F0B26 |
| 14f1:2f40 | 14f1:2000 | Conexant Sys... | PCI CX11261 Soft Modem   | 100%   |          | 1F97EF92E1 |
| 14f1:2f50 | 14f1:207c | Conexant Sys... | Conexant SoftK56 Data... | 100%   |          | DE599FD63C |
| 14f1:2f81 | 14f1:0000 | Conexant Sys... | PCIe CX95610 Soft Modem  | 100%   |          | 4C1091E630 |
| 14f1:2f82 | 14f1:0000 | Conexant Sys... | PCIe CX95610 Soft Modem  | 100%   |          | C2AB31CCD9 |
| 1fd4:1999 | 1fd4:0101 | SUNIX           | Multiport serial cont... | 100%   |          | 4415A64795 |
| 5372:6870 | 1000:0010 |                 | Communication controller | 100%   |          | 2C1DD09A17 |
| 8086:0801 | 8086:0801 | Intel           | Moorestown SPI Ctrl 1    | 100%   |          | D1874B6708 |
| 8086:0802 | 8086:0802 | Intel           | Moorestown I2C 0         | 100%   |          | D1874B6708 |
| 8086:0803 | 8086:0803 | Intel           | Moorestown I2C 1         | 100%   |          | D1874B6708 |
| 8086:0804 | 8086:0804 | Intel           | Moorestown I2C 2         | 100%   |          | D1874B6708 |
| 8086:1c3a | 1043:11d7 | Intel           | 6 Series/C200 Series ... | 4%     | 3.10.34  | A5A0DA657B |
| 8086:1c3a | 1043:844d | Intel           | 6 Series/C200 Series ... | 0.1%   | 3.0.38   | 1678EE56C3 |
| 8086:1c3a | 17aa:3975 | Intel           | 6 Series/C200 Series ... | 0.7%   | 3.10.34  | 2239D316E8 |
| 8086:1c3a | 8086:7270 | Intel           | 6 Series/C200 Series ... | 1.6%   | 3.14.22  | D5C9D589F2 |
| 8086:1d3a | 15d9:0628 | Intel           | C600/X79 series chips... | 50%    | 3.10.0   | 99E743CA9E |
| 8086:1d3a | 15d9:0636 | Intel           | C600/X79 series chips... | 100%   |          | 100EFA1F4A |
| 8086:1d3b | 1028:048c | Intel           | C600/X79 series chips... | 100%   |          | B6374DF09A |
| 8086:1d3b | 1028:04f8 | Intel           | C600/X79 series chips... | 100%   |          | A1EFBB1BE1 |
| 8086:1d3b | 1043:84ef | Intel           | C600/X79 series chips... | 100%   |          | 996F55BB36 |
| 8086:1d3b | 15d9:0628 | Intel           | C600/X79 series chips... | 100%   |          | F7519BF7BE |
| 8086:1d3b | 15d9:062c | Intel           | C600/X79 series chips... | 100%   |          | 2B1034E588 |
| 8086:1d3b | 15d9:0636 | Intel           | C600/X79 series chips... | 100%   |          | 100EFA1F4A |
| 8086:1d3b | 15d9:0665 | Intel           | C600/X79 series chips... | 100%   |          | CEC82EF5D0 |
| 8086:1d3b | 15d9:070a | Intel           | C600/X79 series chips... | 100%   |          | B4C8ABC585 |
| 8086:1d3b | 1849:1d3b | Intel           | C600/X79 series chips... | 100%   |          | 69907BBCE0 |
| 8086:1d3b | 8086:1d3b | Intel           | C600/X79 series chips... | 100%   |          | AA487A5EDB |
| 8086:1d3b | 8086:357e | Intel           | C600/X79 series chips... | 100%   |          | F65EC09250 |
| 8086:1e3a | 1019:99f2 | Intel           | 7 Series/C216 Chipset... | 100%   |          | 45F3B356CF |
| 8086:1e3a | 1025:0647 | Intel           | 7 Series/C216 Chipset... | 0.8%   | 3.10.34  | 86D2D3B0E1 |
| 8086:1e3a | 1028:052c | Intel           | 7 Series/C216 Chipset... | 9.1%   | 4.15.0   | 29A0FC6CE0 |
| 8086:1e3a | 1028:058b | Intel           | 7 Series/C216 Chipset... | 100%   |          | 42A50DEDAB |
| 8086:1e3a | 1043:1447 | Intel           | 7 Series/C216 Chipset... | 9.1%   | 3.14.44  | F23B5BF0DA |
| 8086:1e3a | 1043:84ca | Intel           | 7 Series/C216 Chipset... | 1.5%   | 3.10.34  | 570B707FFB |
| 8086:1e3a | 17aa:21f9 | Intel           | 7 Series/C216 Chipset... | 14.3%  | 3.14.15  | B7014678B5 |
| 8086:1e3a | 17aa:21fa | Intel           | 7 Series/C216 Chipset... | 1.1%   | 3.10.42  | CEFD5E879B |
| 8086:1e3a | 17aa:3977 | Intel           | 7 Series/C216 Chipset... | 0.4%   | 3.10.42  | 2DD89E3983 |
| 8086:1e3a | 1849:1e3a | Intel           | 7 Series/C216 Chipset... | 0.9%   | 3.10.0   | 8505F4654F |
| 8086:1e3a | 8086:1e3a | Intel           | 7 Series/C216 Chipset... | 7.7%   | 3.10.34  | CE8124E5F4 |
| 8086:29d4 | 103c:281e | Intel           | 82Q33 Express MEI Con... | 3.6%   | 3.14.44  | 13EF653132 |
| 8086:2e14 | 8086:1003 | Intel           | 4 Series Chipset HECI... | 50%    | 5.0.0    | 53C6C139DA |
| 8086:2e44 | 8086:0025 | Intel           | 4 Series Chipset HECI... | 100%   |          | 8C4EFA23E2 |
| 8086:319a | 1043:1181 | Intel           | Celeron/Pentium Silve... | 23.5%  | 4.15.0   | 76D01F63C2 |
| 8086:319a | 1043:1df0 | Intel           | Celeron/Pentium Silve... | 100%   |          | 22AC5B8AE1 |
| 8086:319a | 1043:1eb0 | Intel           | Celeron/Pentium Silve... | 20%    | 4.15.0   | 00EECF27F3 |
| 8086:3b64 | 103c:3674 | Intel           | 5 Series/3400 Series ... | 25%    | 4.15.0   | F4DE983D96 |
| 8086:3b64 | 1043:1c77 | Intel           | 5 Series/3400 Series ... | 0.8%   | 3.14.25  | 7FDEE4E7BB |
| 8086:3b64 | 105b:0dd5 | Intel           | 5 Series/3400 Series ... | 20%    | 4.1.25   | 6B384CAEA8 |
| 8086:5a9a | 8086:7270 | Intel           | Celeron N3350/Pentium... | 1.9%   | 4.4.0    | 8ADD68C95A |
| 8086:5a9c | 1025:1084 | Intel           | Communication controller | 100%   |          | EB24B13C29 |
| 8086:5a9c | 1028:075f | Intel           | Communication controller | 100%   |          | 3D61CAE371 |
| 8086:5a9c | 1043:8738 | Intel           | Communication controller | 100%   |          | 82BDD3F39F |
| 8086:5a9c | 17aa:3802 | Intel           | Communication controller | 100%   |          | B02B76DC46 |
| 8086:5a9c | 17aa:3803 | Intel           | Communication controller | 100%   |          | F8913A087C |
| 8086:5a9c | 17aa:3809 | Intel           | Communication controller | 100%   |          | 2CE172A9F5 |
| 8086:5a9e | 1025:1084 | Intel           | Communication controller | 100%   |          | EB24B13C29 |
| 8086:5a9e | 1028:075f | Intel           | Communication controller | 100%   |          | 3D61CAE371 |
| 8086:5a9e | 1043:8738 | Intel           | Communication controller | 100%   |          | 82BDD3F39F |
| 8086:5a9e | 17aa:3802 | Intel           | Communication controller | 100%   |          | B02B76DC46 |
| 8086:5a9e | 17aa:3803 | Intel           | Communication controller | 100%   |          | F8913A087C |
| 8086:5a9e | 17aa:380a | Intel           | Communication controller | 100%   |          | 2CE172A9F5 |
| 8086:8c3a | 1028:0620 | Intel           | 8 Series/C220 Series ... | 100%   |          | F801FAB1AD |
| 8086:8c3a | 1043:8534 | Intel           | 8 Series/C220 Series ... | 0.2%   | 3.14.25  | 4712036FF4 |
| 8086:8c3a | 1462:7816 | Intel           | 8 Series/C220 Series ... | 6.7%   | 3.14.33  | 093472BA51 |
| 8086:8c3a | 1462:7823 | Intel           | 8 Series/C220 Series ... | 27.3%  | 3.14.25  | 4C0C5DE2E6 |
| 8086:8c3a | 15d9:0921 | Intel           | 8 Series/C220 Series ... | 100%   |          | DB25C87154 |
| 8086:8c3a | 17aa:3978 | Intel           | 8 Series/C220 Series ... | 3.3%   | 3.14.44  | 825E182B0C |
| 8086:8c3a | 8086:204a | Intel           | 8 Series/C220 Series ... | 12.5%  | 4.1.25   | 8C48173C7B |
| 8086:8c3b | 15d9:0921 | Intel           | 8 Series/C220 Series ... | 100%   |          | DB25C87154 |
| 8086:8c3b | 1849:8c3b | Intel           | 8 Series/C220 Series ... | 100%   |          | 9E52EE363E |
| 8086:8cba | 1043:8534 | Intel           | 9 Series Chipset Fami... | 1.4%   | 3.14.25  | DA88C70AB8 |
| 8086:8cba | 1458:1c3a | Intel           | 9 Series Chipset Fami... | 0.8%   | 3.14.22  | 5A77B72FE5 |
| 8086:8d3a | 1043:8600 | Intel           | C610/X99 series chips... | 2.5%   | 4.1.25   | ABB20B34F4 |
| 8086:8d3a | 15d9:0831 | Intel           | C610/X99 series chips... | 33.3%  | 4.15.0   | 52D5275C7F |
| 8086:8d3a | 8086:35c5 | Intel           | C610/X99 series chips... | 100%   |          | 08100751B7 |
| 8086:8d3a | 8086:35c9 | Intel           | C610/X99 series chips... | 100%   |          | 5F9F099F36 |
| 8086:8d3a | 8086:7270 | Intel           | C610/X99 series chips... | 33.3%  | 4.4.0    | EDE05678EF |
| 8086:8d3b | 1028:0601 | Intel           | C610/X99 series chips... | 100%   |          | AF9F6ACE3F |
| 8086:8d3b | 1028:0639 | Intel           | C610/X99 series chips... | 100%   |          | 3BA1B5FC84 |
| 8086:8d3b | 1028:063a | Intel           | C610/X99 series chips... | 100%   |          | FF3ACF2BDC |
| 8086:8d3b | 1043:85f6 | Intel           | C610/X99 series chips... | 100%   |          | FD500E59D6 |
| 8086:8d3b | 15d9:0821 | Intel           | C610/X99 series chips... | 100%   |          | 17BF7A3CBC |
| 8086:8d3b | 15d9:0824 | Intel           | C610/X99 series chips... | 100%   |          | 6C96E4A591 |
| 8086:8d3b | 15d9:0831 | Intel           | C610/X99 series chips... | 100%   |          | 52D5275C7F |
| 8086:8d3b | 15d9:0834 | Intel           | C610/X99 series chips... | 100%   |          | EEE6327556 |
| 8086:8d3b | 15d9:0835 | Intel           | C610/X99 series chips... | 100%   |          | 7479576DA8 |
| 8086:8d3b | 1d49:0a00 | Intel           | C610/X99 series chips... | 100%   |          | 817865DED6 |
| 8086:8d3b | 8086:35c5 | Intel           | C610/X99 series chips... | 100%   |          | 08100751B7 |
| 8086:8d3b | 8086:35c9 | Intel           | C610/X99 series chips... | 100%   |          | 5F9F099F36 |
| 8086:8d3b | 8086:7270 | Intel           | C610/X99 series chips... | 100%   |          | 7658F21E98 |
| 8086:9c3a | 17aa:220c | Intel           | 8 Series HECI #0         | 3%     | 4.1.15   | CB4F8A8EF2 |
| 8086:9cba | 17aa:390b | Intel           | Wildcat Point-LP MEI ... | 8.7%   | 4.9.60   | AB6BD693BE |
| 8086:9d3a | 1025:1094 | Intel           | Sunrise Point-LP CSME... | 10%    | 4.9.9    | E7D6077756 |
| 8086:9d3a | 1028:06de | Intel           | Sunrise Point-LP CSME... | 16.7%  | 4.15.0   | AE7AD1E7D9 |
| 8086:9d3a | 1028:06fd | Intel           | Sunrise Point-LP CSME... | 40%    | 4.15.0   | 98D787F0D4 |
| 8086:9d3a | 1028:0782 | Intel           | Sunrise Point-LP CSME... | 33.3%  | 4.18.0   | 49389100FC |
| 8086:9d3a | 103c:8079 | Intel           | Sunrise Point-LP CSME... | 20%    | 4.4.1    | F1A8589F00 |
| 8086:9d3a | 103c:80a4 | Intel           | Sunrise Point-LP CSME... | 33.3%  | 4.9.60   | B01FB51118 |
| 8086:9d3a | 103c:80ff | Intel           | Sunrise Point-LP CSME... | 66.7%  | 4.7.2    | B7B039F46E |
| 8086:9d3a | 103c:8100 | Intel           | Sunrise Point-LP CSME... | 100%   |          | 2B56F34E21 |
| 8086:9d3a | 103c:8101 | Intel           | Sunrise Point-LP CSME... | 25%    | 4.9.60   | BC496704F4 |
| 8086:9d3a | 103c:820c | Intel           | Sunrise Point-LP CSME... | 25%    | 4.9.20   | FAE1CD27F3 |
| 8086:9d3a | 1043:1ccd | Intel           | Sunrise Point-LP CSME... | 25%    | 4.9.20   | A4B26975E9 |
| 8086:9d3a | 1179:f820 | Intel           | Sunrise Point-LP CSME... | 25%    | 4.15.0   | B781D8419A |
| 8086:9d3a | 17aa:225c | Intel           | Sunrise Point-LP CSME... | 14.3%  | 4.18.0   | 4438A85B31 |
| 8086:9d3a | 17aa:225d | Intel           | Sunrise Point-LP CSME... | 10%    | 4.14.35  | 6F9DCA6953 |
| 8086:9d3a | 17aa:3801 | Intel           | Sunrise Point-LP CSME... | 3.1%   | 4.9.9    | 412EAC636F |
| 8086:9d3a | 17aa:3808 | Intel           | Sunrise Point-LP CSME... | 5.6%   | 4.9.20   | 9B61CC7F7F |
| 8086:9d3a | 17aa:380c | Intel           | Sunrise Point-LP CSME... | 25%    | 4.9.111  | C3352134E9 |
| 8086:9d3a | 17aa:3819 | Intel           | Sunrise Point-LP CSME... | 16.7%  | 4.9.0    | 18379EBD5C |
| 8086:9d3a | 17aa:382d | Intel           | Sunrise Point-LP CSME... | 11.1%  | 4.9.60   | 65FE9A36B5 |
| 8086:9d3a | 17aa:5048 | Intel           | Sunrise Point-LP CSME... | 33.3%  | 4.15.0   | 842B139FE7 |
| 8086:9d3a | 8086:1999 | Intel           | Sunrise Point-LP CSME... | 5.9%   | 4.9.155  | B1A55C7D69 |
| 8086:9d3e |           | Intel           | Skylake-U/Y CSME: HEC... | 69%    | 4.18.7   | 2FB15D0705 |
| 8086:9d3e | 103c:82cb | Intel           | Skylake-U/Y CSME: HEC... | 100%   |          | FDB567A59E |
| 8086:a13a | 1019:9bc9 | Intel           | 100 Series/C230 Serie... | 100%   |          | 744A3F2E54 |
| 8086:a13a | 1019:9c56 | Intel           | 100 Series/C230 Serie... | 50%    | 4.15.0   | 093E3BB0DE |
| 8086:a13a | 1028:06de | Intel           | 100 Series/C230 Serie... | 25%    | 5.0.0    | BC4C6EBBA7 |
| 8086:a13a | 1028:06f7 | Intel           | 100 Series/C230 Serie... | 66.7%  | 4.15.0   | E2D11AD2AC |
| 8086:a13a | 103c:8392 | Intel           | 100 Series/C230 Serie... | 66.7%  | 4.9.20   | 142D7492C2 |
| 8086:a13a | 1043:1080 | Intel           | 100 Series/C230 Serie... | 33.3%  | 5.0.0    | 5B1076EA3C |
| 8086:a13a | 1043:1d6d | Intel           | 100 Series/C230 Serie... | 100%   |          | 9D6C0DD372 |
| 8086:a13a | 1043:8694 | Intel           | 100 Series/C230 Serie... | 12.2%  | 4.4.0    | 89F4BB64D7 |
| 8086:a13a | 1458:1c3a | Intel           | 100 Series/C230 Serie... | 15.1%  | 4.4.0    | 53E6A4F263 |
| 8086:a13a | 1462:116e | Intel           | 100 Series/C230 Serie... | 100%   |          | 1C47BC90E4 |
| 8086:a13a | 1462:1190 | Intel           | 100 Series/C230 Serie... | 16.7%  | 4.9.9    | 2B70AAB06F |
| 8086:a13a | 1462:7970 | Intel           | 100 Series/C230 Serie... | 20%    | 4.9.20   | AC10EFBB42 |
| 8086:a13a | 1462:7977 | Intel           | 100 Series/C230 Serie... | 40%    | 4.9.60   | D1DED92F20 |
| 8086:a13a | 1462:7982 | Intel           | 100 Series/C230 Serie... | 40%    | 4.15.0   | AE97650E7C |
| 8086:a13a | 1462:7995 | Intel           | 100 Series/C230 Serie... | 100%   |          | 7D25E0B2DD |
| 8086:a13a | 1462:7996 | Intel           | 100 Series/C230 Serie... | 13.3%  | 4.9.20   | 29D13E00C3 |
| 8086:a13a | 15d9:0884 | Intel           | 100 Series/C230 Serie... | 50%    | 4.15.7   | BB8832ACBD |
| 8086:a13a | 1734:121d | Intel           | 100 Series/C230 Serie... | 25%    | 4.12.14  | 29C7E9E412 |
| 8086:a13a | 17aa:3802 | Intel           | 100 Series/C230 Serie... | 4.8%   | 4.4.16   | 25576A8571 |
| 8086:a13a | 1849:a13a | Intel           | 100 Series/C230 Serie... | 6.7%   | 4.3.3    | 9869646781 |
| 8086:a13a | 8086:1999 | Intel           | 100 Series/C230 Serie... | 25%    | 4.9.20   | 13B41B547A |
| 8086:a13b | 15d9:0884 | Intel           | 100 Series/C230 Serie... | 50%    | 4.15.7   | BB8832ACBD |
| 8086:a13b | 8086:1999 | Intel           | 100 Series/C230 Serie... | 100%   |          | 13B41B547A |
| 8086:a1ba | 8086:7270 | Intel           | C620 Series Chipset F... | 16.7%  | 4.9.60   | F823B40D84 |
| 8086:a1bb | 1028:0718 | Intel           | C620 Series Chipset F... | 100%   |          | 97313ACF09 |
| 8086:a1bb | 1028:07cb | Intel           | C620 Series Chipset F... | 100%   |          | 5B9EC879FC |
| 8086:a1bb | 1043:871e | Intel           | C620 Series Chipset F... | 100%   |          | A1916FC246 |
| 8086:a1bb | 15d9:095d | Intel           | C620 Series Chipset F... | 100%   |          | 2794B14FEE |
| 8086:a1bb | 15d9:096d | Intel           | C620 Series Chipset F... | 100%   |          | DCFB9EE48A |
| 8086:a1bb | 15d9:0987 | Intel           | C620 Series Chipset F... | 100%   |          | 893E9D69F2 |
| 8086:a1bb | 8086:35ce | Intel           | C620 Series Chipset F... | 100%   |          | 5B11F4C63C |
| 8086:a1bb | 8086:7270 | Intel           | C620 Series Chipset F... | 100%   |          | 8E73F804F5 |
| 8086:a1be | 1028:0718 | Intel           | C620 Series Chipset F... | 100%   |          | 97313ACF09 |
| 8086:a1be | 1028:07cb | Intel           | C620 Series Chipset F... | 100%   |          | 5B9EC879FC |
| 8086:a1be | 1043:871e | Intel           | C620 Series Chipset F... | 100%   |          | A1916FC246 |
| 8086:a1be | 1590:00eb | Intel           | C620 Series Chipset F... | 100%   |          | 9E91D0ED19 |
| 8086:a1be | 15d9:095d | Intel           | C620 Series Chipset F... | 100%   |          | 2794B14FEE |
| 8086:a1be | 15d9:096d | Intel           | C620 Series Chipset F... | 100%   |          | DCFB9EE48A |
| 8086:a1be | 15d9:0987 | Intel           | C620 Series Chipset F... | 100%   |          | 893E9D69F2 |
| 8086:a1be | 8086:35ce | Intel           | C620 Series Chipset F... | 100%   |          | 4391DFF8D2 |
| 8086:a1be | 8086:7270 | Intel           | C620 Series Chipset F... | 100%   |          | 8E73F804F5 |
| 8086:a2ba | 1458:1c3a | Intel           | 200 Series PCH CSME H... | 3.4%   | 3.10.0   | 1A67024C19 |
| 8086:a2ba | 1462:7a71 | Intel           | 200 Series PCH CSME H... | 33.3%  | 4.9.9    | 309262E3D6 |
| 8086:a328 | 1025:1264 | Intel           | 300 Series Chipset De... | 12.5%  | 4.15.0   | C4FA903BED |
| 8086:a328 | 1028:08a1 | Intel           | 300 Series Chipset De... | 33.3%  | 4.18.0   | AACC137FAA |
| 8086:a328 | 1849:a328 | Intel           | 300 Series Chipset De... | 100%   |          | B2FAC79AFD |
| 8086:a360 | 1025:1264 | Intel           | Cannon Lake PCH HECI ... | 12.5%  | 4.15.0   | C4FA903BED |
| 8086:a360 | 1028:0851 | Intel           | Cannon Lake PCH HECI ... | 100%   |          | 05D6B79D2F |
| 8086:a360 | 1028:086f | Intel           | Cannon Lake PCH HECI ... | 11.1%  | 4.15.0   | 2261D3C647 |
| 8086:a360 | 1028:0877 | Intel           | Cannon Lake PCH HECI ... | 16.7%  | 4.15.0   | 3FBDBB7E9C |
| 8086:a360 | 103c:84db | Intel           | Cannon Lake PCH HECI ... | 50%    | 4.18.0   | 06EE78EE4D |
| 8086:a360 | 1043:1041 | Intel           | Cannon Lake PCH HECI ... | 50%    | 4.19.1   | F38CA9409C |
| 8086:a360 | 1043:8694 | Intel           | Cannon Lake PCH HECI ... | 10.3%  | 4.15.0   | F978F464EB |
| 8086:a360 | 1458:1c3a | Intel           | Cannon Lake PCH HECI ... | 11.6%  | 4.15.0   | 29FCA206F8 |
| 8086:a360 | 1462:126a | Intel           | Cannon Lake PCH HECI ... | 100%   |          | 039A05F3EB |
| 8086:a360 | 1462:7b33 | Intel           | Cannon Lake PCH HECI ... | 25%    | 4.15.0   | F08CE9BD47 |
| 8086:a360 | 17aa:2267 | Intel           | Cannon Lake PCH HECI ... | 20%    | 4.19.11  | AAB68A3B33 |
| 8086:a360 | 17aa:36e7 | Intel           | Cannon Lake PCH HECI ... | 33.3%  | 4.18.0   | 1B722DF896 |
| 8086:a360 | 1849:a360 | Intel           | Cannon Lake PCH HECI ... | 26.1%  | 4.15.0   | B2FAC79AFD |
| 8086:a364 | 1849:a364 | Intel           | 300 Series Chipset Fa... | 100%   |          | B2FAC79AFD |
| 9710:9900 | a000:2000 | MosChip Semi... | MCS9900 Multi-I/O Con... | 100%   |          | 7D609B3954 |

### Firewire controller (PCI)

2 out of 662 (0.30%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1102:4001 | 1102:0010 | Creative Labs   | SB Audigy FireWire Port  | 2.8%   | 3.14.15  | 2A34C16AB3 |
| 11c1:5901 | 11c1:5900 | LSI             | FW643 [TrueFire] PCIe... | 0.7%   | 3.14.44  | D5C9D589F2 |

### Flash memory (PCI)

28 out of 48 (58.33%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1524:0520 | 1025:007a | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | E4219525B9 |
| 1524:0520 | 1025:0090 | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | 719BE91D02 |
| 1524:0520 | 1025:009f | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | A28F7B2623 |
| 1524:0520 | 1025:010f | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | 0E64D71097 |
| 1524:0520 | 1179:ff01 | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | C27B4CD3AF |
| 1524:0530 | 1025:007a | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | E4219525B9 |
| 1524:0530 | 1025:0090 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 719BE91D02 |
| 1524:0530 | 1025:009f | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | A28F7B2623 |
| 1524:0530 | 1025:010f | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 0E64D71097 |
| 1524:0530 | 1179:ff01 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | C27B4CD3AF |
| 1524:0530 | 14c0:0020 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 0351248973 |
| 1524:0530 | 1734:10c1 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | AAAB07D2AE |
| 1524:0530 | 1734:10d7 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | CA3AC06D30 |
| 1524:0530 | 17aa:2079 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | EDAE63A429 |
| 1524:0720 | 1025:011b | ENE Technology  | Memory Stick Card Rea... | 100%   |          | B614684231 |
| 1524:0720 | 1025:012a | ENE Technology  | Memory Stick Card Rea... | 100%   |          | C95503E7D2 |
| 1524:0720 | 1025:012e | ENE Technology  | Memory Stick Card Rea... | 100%   |          | 16BE592F4F |
| 1524:0720 | 1462:2fb3 | ENE Technology  | Memory Stick Card Rea... | 100%   |          | D6A996DA64 |
| 1524:0720 | 1462:2fbd | ENE Technology  | Memory Stick Card Rea... | 100%   |          | 6502446C70 |
| 1524:0730 | 1025:011b | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | B614684231 |
| 1524:0730 | 1025:012a | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | C95503E7D2 |
| 1524:0730 | 1025:012e | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 16BE592F4F |
| 1524:0730 | 1462:2fb3 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | D6A996DA64 |
| 1524:0730 | 1462:2fbd | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 6502446C70 |
| 1524:0730 | 1558:0664 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 51E2E84C28 |
| 1524:0730 | 1558:0668 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 41C9811E8B |
| 1524:0730 | 1558:0669 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 647FD58075 |
| 1524:0730 | 1558:0801 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | A28F10A223 |

### Graphics card (PCI)

311 out of 8931 (3.48%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1002:130f | 1849:130f | AMD             | Kaveri [Radeon R7 Gra... | 10%    | 3.14.44  | 50841878AE |
| 1002:15d8 | 103c:85ad | AMD             | Picasso                  | 100%   |          | 0D375562BD |
| 1002:15d8 | 103c:8615 | AMD             | Picasso                  | 100%   |          | 048229855F |
| 1002:15d8 | 1043:18f1 | AMD             | Picasso                  | 75%    | 5.2.0    | 123447177A |
| 1002:15d8 | 17aa:5124 | AMD             | Picasso                  | 100%   |          | 79E53D2DB5 |
| 1002:15dd | 1002:15dd | AMD             | Raven Ridge [Radeon V... | 2.4%   | 4.15.0   | 6BD3D061A7 |
| 1002:15dd | 103c:8434 | AMD             | Raven Ridge [Radeon V... | 50%    | 4.18.0   | E30D68CA01 |
| 1002:15dd | 1043:876b | AMD             | Raven Ridge [Radeon V... | 12.8%  | 4.15.0   | F48E23AB6A |
| 1002:15dd | 1458:d000 | AMD             | Raven Ridge [Radeon V... | 5.6%   | 3.10.0   | 158FB83DCC |
| 1002:15dd | 1462:7a36 | AMD             | Raven Ridge [Radeon V... | 28.6%  | 4.16.18  | 41871808C5 |
| 1002:15dd | 17aa:36f5 | AMD             | Raven Ridge [Radeon V... | 100%   |          | 7E41940C9C |
| 1002:4752 | 103c:3208 | AMD             | Rage 3 [Rage XL PCI]     | 100%   |          | 2C877CF870 |
| 1002:4752 | 8086:3439 | AMD             | Rage 3 [Rage XL PCI]     | 100%   |          | 0F21E859FA |
| 1002:4c4d | 1002:4c4d | AMD             | Rage Mobility AGP 2x ... | 100%   |          | 5C43AB36E8 |
| 1002:6600 | 103c:194d | AMD             | Mars [Radeon HD 8670A... | 20%    | 3.14.25  | 2EDF7E28BE |
| 1002:6600 | 103c:195d | AMD             | Mars [Radeon HD 8670A... | 100%   |          | 1A786FF081 |
| 1002:6600 | 144d:c706 | AMD             | Mars [Radeon HD 8670A... | 11.1%  | 3.14.44  | 21C3A8765C |
| 1002:6600 | 144d:c708 | AMD             | Mars [Radeon HD 8670A... | 33.3%  | 4.1.15   | D8F94CA15D |
| 1002:6601 | 144d:c0e8 | AMD             | Mars [Radeon HD 8730M]   | 64.3%  | 4.8.12   | 74BA47C62B |
| 1002:6604 | 103c:8150 | AMD             | Opal XT [Radeon R7 M2... | 25%    | 4.18.12  | FD1C0C441E |
| 1002:6610 | 1787:2012 | AMD             | Oland XT [Radeon HD 8... | 100%   |          | 50841878AE |
| 1002:665c | 1043:0456 | AMD             | Bonaire XT [Radeon HD... | 40%    | 4.15.0   | 8EACB4F7F2 |
| 1002:66af | 1002:081e | AMD             | Vega 20 [Radeon VII]     | 37.5%  | 4.15.0   | 0F37A61AA0 |
| 1002:6740 | 103c:3388 | AMD             | Whistler [Radeon HD 6... | 22.5%  | 3.14.44  | 17C76F0730 |
| 1002:6741 | 17aa:3976 | AMD             | Whistler [Radeon HD 6... | 5.3%   | 4.1.15   | 70A3F923C2 |
| 1002:675b | 1002:7600 | AMD             | Turks [Radeon HD 7600... | 50%    | 4.15.0   | B511052CC4 |
| 1002:6760 | 103c:1672 | AMD             | Seymour [Radeon HD 64... | 5%     | 3.14.44  | 4F9C19A9C0 |
| 1002:6760 | 106b:00e1 | AMD             | Seymour [Radeon HD 64... | 100%   |          | 772B6F3A59 |
| 1002:6761 | 1297:4012 | AMD             | Seymour LP [Radeon HD... | 100%   |          | DE0CC0AB6F |
| 1002:6770 | 17aa:3623 | AMD             | Caicos [Radeon HD 645... | 20%    | 4.1.15   | 02882EF37B |
| 1002:6778 | 1028:2120 | AMD             | Caicos XT [Radeon HD ... | 4.2%   | 3.10.0   | 8A8C155D34 |
| 1002:6779 | 1043:03da | AMD             | Caicos [Radeon HD 645... | 0.9%   | 3.10.34  | 9734ABB0D4 |
| 1002:6779 | 1043:047b | AMD             | Caicos [Radeon HD 645... | 50%    | 4.15.0   | 423A12D8A5 |
| 1002:6779 | 174b:e164 | AMD             | Caicos [Radeon HD 645... | 2.7%   | 3.14.33  | 8A4E34A210 |
| 1002:67b1 | 1002:0b00 | AMD             | Hawaii PRO [Radeon R9... | 100%   |          | 2FAE8819F7 |
| 1002:67df | 1002:0b37 | AMD             | Ellesmere [Radeon RX ... | 25%    | 4.20.5   | 5CC9EEEBFE |
| 1002:67df | 1da2:e366 | AMD             | Ellesmere [Radeon RX ... | 3.6%   | 4.9.20   | A9ED28807E |
| 1002:67ef | 174b:e344 | AMD             | Baffin [Radeon RX 460... | 20%    | 4.9.124  | 98A829DCFD |
| 1002:67ef | 174b:e348 | AMD             | Baffin [Radeon RX 460... | 10%    | 4.9.20   | 72DD80DA38 |
| 1002:67ff | 1da2:e348 | AMD             | Baffin [Radeon RX 550... | 7.7%   | 4.9.60   | CEDA0A30C3 |
| 1002:6819 | 1043:045b | AMD             | Pitcairn PRO [Radeon ... | 28.6%  | 3.14.33  | A12C16610A |
| 1002:6819 | 174b:a001 | AMD             | Pitcairn PRO [Radeon ... | 25%    | 4.9.0    | 97B72D7509 |
| 1002:6821 | 1028:05ee | AMD             | Venus XT [Radeon HD 8... | 14.3%  | 3.14.44  | 31B0BECCAB |
| 1002:6823 | 1028:05eb | AMD             | Venus PRO [Radeon HD ... | 18.2%  | 3.14.44  | A06AAF3EA2 |
| 1002:6823 | 1179:f935 | AMD             | Venus PRO [Radeon HD ... | 40%    | 4.15.0   | 35DC9BFB0B |
| 1002:682f | 1028:0572 | AMD             | Chelsea LP [Radeon HD... | 5.6%   | 3.14.44  | 609E372F78 |
| 1002:6840 | 1028:0598 | AMD             | Thames [Radeon HD 750... | 4.5%   | 3.14.25  | 988B8C4B4A |
| 1002:6840 | 103c:1840 | AMD             | Thames [Radeon HD 750... | 14.3%  | 3.14.44  | B0552C0AF2 |
| 1002:6840 | 103c:1842 | AMD             | Thames [Radeon HD 750... | 6.2%   | 3.14.44  | 2266C4AA6C |
| 1002:6840 | 144d:c0d8 | AMD             | Thames [Radeon HD 750... | 6.1%   | 3.14.22  | 935529F421 |
| 1002:6841 | 1028:057f | AMD             | Thames [Radeon HD 755... | 28.6%  | 4.15.0   | C38BDE084A |
| 1002:6841 | 103c:17f4 | AMD             | Thames [Radeon HD 755... | 18.2%  | 3.14.44  | C79BD3EFCD |
| 1002:6841 | 104d:90ac | AMD             | Thames [Radeon HD 755... | 2%     | 3.10.19  | A41A94F4F5 |
| 1002:68a1 | 1025:0475 | AMD             | Broadway PRO [Mobilit... | 100%   |          | 3B1F271BB2 |
| 1002:68e0 | 104d:9071 | AMD             | Park [Mobility Radeon... | 10.5%  | 4.1.34   | E7257D1630 |
| 1002:68e4 | 1043:1c92 | AMD             | Robson CE [Radeon HD ... | 3%     | 3.14.44  | 7FDEE4E7BB |
| 1002:68e4 | 17aa:397a | AMD             | Robson CE [Radeon HD ... | 7.4%   | 3.10.34  | AF0EC73528 |
| 1002:68f9 | 1028:2126 | AMD             | Cedar [Radeon HD 5000... | 33.3%  | 4.1.34   | D5A5261203 |
| 1002:6938 | 1043:04f5 | AMD             | Tonga XT / Amethyst X... | 33.3%  | 4.5.5    | 0E1E35C6E2 |
| 1002:6939 | 1682:9380 | AMD             | Tonga PRO [Radeon R9 ... | 100%   |          | A3F6229CAA |
| 1002:6939 | 174b:e308 | AMD             | Tonga PRO [Radeon R9 ... | 12.5%  | 4.9.60   | 77EF398855 |
| 1002:699f | 1043:0511 | AMD             | Lexa PRO [Radeon 540/... | 1.9%   | 4.15.18  | A994473A14 |
| 1002:699f | 1458:22f3 | AMD             | Lexa PRO [Radeon 540/... | 50%    | 4.15.0   | 03EEED62F1 |
| 1002:699f | 1462:8a90 | AMD             | Lexa PRO [Radeon 540/... | 50%    | 3.10.0   | 4769912443 |
| 1002:791f | 1462:6b30 | AMD             | RS690M [Radeon Xpress... | 100%   |          | 4940058A56 |
| 1002:94c3 | 1028:0402 | AMD             | RV610 [Radeon HD 2400... | 50%    | 4.15.0   | BBA0FE2672 |
| 1002:954f | 1462:1618 | AMD             | RV710 [Radeon HD 4350... | 50%    | 3.14.53  | 51837DE98F |
| 1002:9553 | 1043:1c42 | AMD             | RV710/M92 [Mobility R... | 4.8%   | 4.1.15   | 6D866DDF45 |
| 1002:9610 | 1458:d000 | AMD             | RS780 [Radeon HD 3200]   | 25%    | 4.1.38   | BC16FF7B2F |
| 1002:9616 | 1043:8388 | AMD             | RS780L [Radeon 3000]     | 1%     | 3.14.44  | 8A29337DB7 |
| 1002:9712 | 103c:1609 | AMD             | RS880M [Mobility Rade... | 28.6%  | 3.13.0   | 1DD894B330 |
| 1002:9714 | 1849:9714 | AMD             | RS880 [Radeon HD 4290]   | 50%    | 4.1.25   | CAFF866F87 |
| 1002:9807 | 1002:9807 | AMD             | Wrestler [Radeon HD 6... | 100%   |          | 3027B15C31 |
| 1002:9830 | 1043:8623 | AMD             | Kabini [Radeon HD 840... | 1.8%   | 3.14.44  | 7A3C73F361 |
| 1002:9851 | 1025:088c | AMD             | Mullins [Radeon R4/R5... | 100%   |          | D0E8E1E8D9 |
| 1002:9851 | 103c:2269 | AMD             | Mullins [Radeon R4/R5... | 10%    | 4.9.20   | 912D4C6523 |
| 1002:9851 | 103c:226b | AMD             | Mullins [Radeon R4/R5... | 20%    | 4.1.34   | 8016AF5575 |
| 1002:9851 | 103c:22cd | AMD             | Mullins [Radeon R4/R5... | 25%    | 4.15.0   | 46004F2E8E |
| 1002:9851 | 17aa:3801 | AMD             | Mullins [Radeon R4/R5... | 10.5%  | 4.1.15   | A30A019453 |
| 1002:9874 | 103c:80b6 | AMD             | Wani [Radeon R5/R6/R7... | 33.3%  | 4.18.0   | C7EEDACBF5 |
| 1002:9874 | 17aa:5113 | AMD             | Wani [Radeon R5/R6/R7... | 25%    | 4.15.0   | 32F7318757 |
| 1002:98e4 | 17aa:39f9 | AMD             | Stoney [Radeon R2/R3/... | 12.5%  | 4.9.60   | C23D0EF968 |
| 1002:9900 | 103c:1849 | AMD             | Trinity [Radeon HD 76... | 12.5%  | 3.14.44  | FE4579E9D1 |
| 1002:9996 | 1462:7721 | AMD             | Richland [Radeon HD 8... | 20%    | 3.14.44  | 373FA45C3B |
| 10de:0140 | 1458:3126 | Nvidia          | NV43 [GeForce 6600 GT]   | 100%   |          | 9F8066CA65 |
| 10de:0141 | 1043:81ee | Nvidia          | NV43 [GeForce 6600]      | 50%    | 4.1.38   | 71BC5B9631 |
| 10de:0141 | 1458:3126 | Nvidia          | NV43 [GeForce 6600]      | 33.3%  | 4.9.60   | 7E447609BE |
| 10de:0148 | 1179:0001 | Nvidia          | NV43M [GeForce Go 6600]  | 100%   |          | D5D7DAB02F |
| 10de:01d1 | 1028:0405 | Nvidia          | G72 [GeForce 7300 LE]    | 33.3%  | 3.14.13  | D866167EB1 |
| 10de:01d3 |           | Nvidia          | G72 [GeForce 7200 GS ... | 25%    | 4.1.25   | 17445004F4 |
| 10de:0244 | 103c:30b7 | Nvidia          | C51 [GeForce Go 6150]    | 8.3%   | 3.10.34  | 0CA0AF6291 |
| 10de:0292 | 105b:0f03 | Nvidia          | G71 [GeForce 7900 GS]    | 50%    | 4.1.15   | 7296E03F32 |
| 10de:0298 | 1179:ff31 | Nvidia          | G71M [GeForce Go 7900... | 100%   |          | FED8975477 |
| 10de:031a | 104d:814f | Nvidia          | NV31M [GeForce FX Go5... | 100%   |          | 88ABDEBE09 |
| 10de:0326 | 1462:911a | Nvidia          | NV34 [GeForce FX 5500]   | 33.3%  | 4.9.41   | FFD7AFA075 |
| 10de:03d0 | 1043:8234 | Nvidia          | C61 [GeForce 6150SE n... | 23.5%  | 3.14.53  | 7A7933F5D5 |
| 10de:03d1 | 1019:2609 | Nvidia          | C61 [GeForce 6100 nFo... | 10%    | 4.15.0   | 5343BC19E6 |
| 10de:03d6 | 1043:83a4 | Nvidia          | C61 [GeForce 7025 / n... | 6.2%   | 3.14.44  | DA40FFB555 |
| 10de:0402 | 1043:8258 | Nvidia          | G84 [GeForce 8600 GT]    | 33.3%  | 4.1.25   | 8CDD8FFE23 |
| 10de:0405 | 1043:15d2 | Nvidia          | G84M [GeForce 9500M GS]  | 11.1%  | 3.14.44  | 4137AC8F54 |
| 10de:040f | 10de:049a | Nvidia          | G84GL [Quadro FX 1700]   | 5%     | 4.1.25   | 092205321D |
| 10de:0426 | 104d:9018 | Nvidia          | G86M [GeForce 8400M GT]  | 100%   |          | 8A814A5779 |
| 10de:0428 | 1043:1513 | Nvidia          | G86M [GeForce 8400M G]   | 20%    | 4.1.15   | E0EEE8D1CC |
| 10de:042e | 1043:17c2 | Nvidia          | G86M [GeForce 9300M G]   | 6.7%   | 3.14.33  | 4E30CC5479 |
| 10de:0531 | 103c:30cf | Nvidia          | C67 [GeForce 7150M / ... | 22.2%  | 4.1.15   | 1184F5572B |
| 10de:0602 | 10de:057c | Nvidia          | G92 [GeForce 8800 GT]    | 75%    | 4.19.20  | DA7914FBED |
| 10de:0614 | 1043:8314 | Nvidia          | G92 [GeForce 9800 GT]    | 25%    | 3.14.44  | A3AFA44F01 |
| 10de:062f | 10de:060e | Nvidia          | G94 [GeForce 9800 S]     | 100%   |          | D677F0444F |
| 10de:06cd | 3842:1470 | Nvidia          | GF100 [GeForce GTX 470]  | 100%   |          | A0225AA660 |
| 10de:06e9 | 1043:19b2 | Nvidia          | G98M [GeForce 9300M GS]  | 1.4%   | 3.10.34  | DAADE835C6 |
| 10de:0848 | 1043:82e2 | Nvidia          | C77 [GeForce 8300]       | 12.5%  | 3.10.19  | E1B7D175A1 |
| 10de:0849 | 1043:82f2 | Nvidia          | C77 [GeForce 8200]       | 33.3%  | 3.14.44  | E3ADCE0E5E |
| 10de:0868 | 103c:2a83 | Nvidia          | C79 [nForce 760i SLI]    | 100%   |          | D677F0444F |
| 10de:0a28 | 103c:7001 | Nvidia          | GT216M [GeForce GT 230M] | 9.1%   | 3.10.34  | 2E7C7E635C |
| 10de:0a34 | 1642:3928 | Nvidia          | GT216M [GeForce GT 240M] | 100%   |          | 0921BB94E0 |
| 10de:0a65 |           | Nvidia          | GT218 [GeForce 210]      | 1.2%   | 3.14.25  | 3C2FD252E1 |
| 10de:0a65 | 1043:8490 | Nvidia          | GT218 [GeForce 210]      | 28.6%  | 4.9.9    | 2DB3C1A436 |
| 10de:0a65 | 1458:3629 | Nvidia          | GT218 [GeForce 210]      | 7.7%   | 4.1.15   | 8C3172A9F3 |
| 10de:0a65 | 1462:8094 | Nvidia          | GT218 [GeForce 210]      | 3.2%   | 3.14.44  | B7812DD3C1 |
| 10de:0a65 | 3842:1310 | Nvidia          | GT218 [GeForce 210]      | 33.3%  | 4.9.124  | 9CB0AC857A |
| 10de:0e22 | 3842:1370 | Nvidia          | GF104 [GeForce GTX 460]  | 100%   |          | 957AF816F5 |
| 10de:0f02 | 1043:84f6 | Nvidia          | GF108 [GeForce GT 730]   | 9.1%   | 3.14.44  | 309F371381 |
| 10de:0fc1 | 1043:83f3 | Nvidia          | GK107 [GeForce GT 640]   | 2.9%   | 3.14.44  | 9C1344C76E |
| 10de:0fc2 | 10de:093c | Nvidia          | GK107 [GeForce GT 630... | 50%    | 4.9.20   | 84224B6ADA |
| 10de:0fc6 | 1043:8427 | Nvidia          | GK107 [GeForce GTX 650]  | 11.8%  | 3.14.44  | 4E0DC79606 |
| 10de:0fc6 | 1462:2802 | Nvidia          | GK107 [GeForce GTX 650]  | 66.7%  | 4.18.0   | 128A90D3B7 |
| 10de:0ffa | 10de:094b | Nvidia          | GK107GL [Quadro K600]    | 20%    | 4.1.15   | 428006990E |
| 10de:100a | 1462:2983 | Nvidia          | GK110B [GeForce GTX 7... | 100%   |          | 91D43B6213 |
| 10de:107c | 10de:102f | Nvidia          | GF119 [NVS 315]          | 50%    | 4.18.0   | 9E55C4BDEE |
| 10de:1086 | 1043:8387 | Nvidia          | GF110 [GeForce GTX 57... | 16.7%  | 3.14.22  | BC8749820A |
| 10de:11c6 | 1043:8446 | Nvidia          | GK106 [GeForce GTX 65... | 25%    | 3.14.44  | 3730F9BE71 |
| 10de:11c8 | 1569:11c8 | Nvidia          | GK106 [GeForce GTX 65... | 12.5%  | 4.1.15   | CE85A9AD63 |
| 10de:1244 |           | Nvidia          | GF116 [GeForce GTX 55... | 5.8%   | 3.14.44  | 3736215480 |
| 10de:1244 | 3842:1556 | Nvidia          | GF116 [GeForce GTX 55... | 33.3%  | 4.15.0   | 4BE9CE0F72 |
| 10de:1287 | 1043:84f5 | Nvidia          | GK208B [GeForce GT 730]  | 44.4%  | 4.1.16   | 8AA494134E |
| 10de:1287 | 1043:8501 | Nvidia          | GK208B [GeForce GT 730]  | 14.3%  | 4.1.15   | 930D8056C3 |
| 10de:1287 | 1043:850c | Nvidia          | GK208B [GeForce GT 730]  | 50%    | 4.18.0   | 6CF789DF63 |
| 10de:1287 | 10de:1083 | Nvidia          | GK208B [GeForce GT 730]  | 100%   |          | 5E5919C697 |
| 10de:1287 | 10de:1287 | Nvidia          | GK208B [GeForce GT 730]  | 10%    | 4.1.25   | 8603D5BDF5 |
| 10de:1288 | 1462:8c90 | Nvidia          | GK208B [GeForce GT 720]  | 25%    | 4.1.15   | 74EDF3551E |
| 10de:1288 | 1569:1288 | Nvidia          | GK208B [GeForce GT 720]  | 50%    | 4.9.60   | 7E9CD09A5D |
| 10de:128b | 1043:8572 | Nvidia          | GK208B [GeForce GT 710]  | 8.3%   | 4.1.25   | 7902B95176 |
| 10de:128b | 1043:85f7 | Nvidia          | GK208B [GeForce GT 710]  | 25%    | 4.9.124  | 08A7929F4A |
| 10de:1380 | 1043:84bb | Nvidia          | GM107 [GeForce GTX 75... | 22.2%  | 4.4.0    | E7D55807C9 |
| 10de:1380 | 1043:84bc | Nvidia          | GM107 [GeForce GTX 75... | 16.7%  | 4.1.25   | 59CCFFE44E |
| 10de:1380 | 10de:8412 | Nvidia          | GM107 [GeForce GTX 75... | 100%   |          | 3A624021F2 |
| 10de:1380 | 1458:362d | Nvidia          | GM107 [GeForce GTX 75... | 17.6%  | 4.1.25   | C67CC4D736 |
| 10de:1380 | 1462:3102 | Nvidia          | GM107 [GeForce GTX 75... | 33.3%  | 4.1.15   | 6158505A7F |
| 10de:1381 | 1043:84f0 | Nvidia          | GM107 [GeForce GTX 750]  | 15.4%  | 4.1.15   | 8E80E31C5C |
| 10de:1381 | 10de:1073 | Nvidia          | GM107 [GeForce GTX 750]  | 16.7%  | 4.9.20   | 02666C5333 |
| 10de:1381 | 1458:362e | Nvidia          | GM107 [GeForce GTX 750]  | 57.1%  | 4.1.16   | FED7D6BB61 |
| 10de:1381 | 1458:3642 | Nvidia          | GM107 [GeForce GTX 750]  | 25%    | 4.1.15   | 8276D533D6 |
| 10de:1381 | 1462:8a9c | Nvidia          | GM107 [GeForce GTX 750]  | 38.5%  | 4.1.25   | DF2090C762 |
| 10de:13c2 | 1043:8508 | Nvidia          | GM204 [GeForce GTX 970]  | 14.3%  | 4.15.0   | 3DD9F6A674 |
| 10de:13c2 | 10de:1131 | Nvidia          | GM204 [GeForce GTX 970]  | 75%    | 4.1.15   | 675FB21B01 |
| 10de:13c2 | 1458:367a | Nvidia          | GM204 [GeForce GTX 970]  | 50%    | 4.1.15   | 3E15147646 |
| 10de:13c2 | 1458:367b | Nvidia          | GM204 [GeForce GTX 970]  | 100%   |          | 37FD9139AF |
| 10de:13c2 | 1462:3160 | Nvidia          | GM204 [GeForce GTX 970]  | 50%    | 4.15.0   | 7980C33879 |
| 10de:13c2 | 19da:1366 | Nvidia          | GM204 [GeForce GTX 970]  | 25%    | 4.18.0   | BBB6E540DE |
| 10de:13f1 | 10de:1153 | Nvidia          | GM204GL [Quadro M4000]   | 100%   |          | B8D85B966B |
| 10de:1401 | 1458:36aa | Nvidia          | GM206 [GeForce GTX 960]  | 100%   |          | 1CFE050B29 |
| 10de:1401 | 1458:36ad | Nvidia          | GM206 [GeForce GTX 960]  | 100%   |          | A8A89AC09A |
| 10de:1401 | 1458:36b0 | Nvidia          | GM206 [GeForce GTX 960]  | 100%   |          | B99D4A956B |
| 10de:1401 | 1462:3205 | Nvidia          | GM206 [GeForce GTX 960]  | 100%   |          | 7D2485C593 |
| 10de:1401 | 3842:2966 | Nvidia          | GM206 [GeForce GTX 960]  | 100%   |          | 33DA9C195D |
| 10de:1406 | 1028:072b | Nvidia          | GM206 [GeForce GTX 96... | 100%   |          | 4B9D75483A |
| 10de:17c2 | 10de:1132 | Nvidia          | GM200 [GeForce GTX TI... | 100%   |          | 2369E0376D |
| 10de:1b06 | 1043:85e2 | Nvidia          | GP102 [GeForce GTX 10... | 100%   |          | 5D1A48EE4E |
| 10de:1b06 | 3842:6696 | Nvidia          | GP102 [GeForce GTX 10... | 20%    | 4.18.0   | 35DAE7072E |
| 10de:1b80 | 1458:3717 | Nvidia          | GP104 [GeForce GTX 1080] | 100%   |          | 3F1B997D89 |
| 10de:1b80 | 1462:3367 | Nvidia          | GP104 [GeForce GTX 1080] | 100%   |          | DEE8563CD4 |
| 10de:1b81 |           | Nvidia          | GP104 [GeForce GTX 1070] | 50%    | 4.9.20   | D326BF619F |
| 10de:1b81 | 1043:8597 | Nvidia          | GP104 [GeForce GTX 1070] | 100%   |          | 90D8E62525 |
| 10de:1b81 | 1043:859f | Nvidia          | GP104 [GeForce GTX 1070] | 100%   |          | D68BCE418A |
| 10de:1b81 | 1043:85a0 | Nvidia          | GP104 [GeForce GTX 1070] | 50%    | 4.19.28  | 691E406FAF |
| 10de:1b81 | 10b0:1b81 | Nvidia          | GP104 [GeForce GTX 1070] | 100%   |          | 8FB6824328 |
| 10de:1b81 | 1458:36fc | Nvidia          | GP104 [GeForce GTX 1070] | 50%    | 4.9.20   | CD8505D488 |
| 10de:1be1 | 1462:11ff | Nvidia          | GP104BM [GeForce GTX ... | 100%   |          | C2E855B5BC |
| 10de:1c02 |           | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | A248371C4D |
| 10de:1c02 | 103c:82fc | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | 75C701DDBD |
| 10de:1c02 | 1043:85b1 | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | 39F3C43A6B |
| 10de:1c02 | 10de:1c02 | Nvidia          | GP106 [GeForce GTX 10... | 40%    | 4.18.0   | AC3662FF5F |
| 10de:1c02 | 1458:3722 | Nvidia          | GP106 [GeForce GTX 10... | 4.5%   | 4.15.0   | CC9A8D1703 |
| 10de:1c02 | 1458:3724 | Nvidia          | GP106 [GeForce GTX 10... | 40%    | 4.15.0   | 316FA5B314 |
| 10de:1c02 | 1462:3287 | Nvidia          | GP106 [GeForce GTX 10... | 16.7%  | 4.13.0   | CCB4D48D08 |
| 10de:1c02 | 1462:8c95 | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | EB775E1534 |
| 10de:1c02 | 3842:6162 | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | FCC69B7D1E |
| 10de:1c03 |           | Nvidia          | GP106 [GeForce GTX 10... | 50%    | 4.15.0   | 74B6562CCD |
| 10de:1c03 | 1043:85a4 | Nvidia          | GP106 [GeForce GTX 10... | 50%    | 4.15.0   | 725B24FE69 |
| 10de:1c03 | 1043:85a6 | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | EB6CD37E93 |
| 10de:1c03 | 1043:85ae | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | 7DC13C6D0D |
| 10de:1c03 | 1043:85e0 | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | 2C9527A545 |
| 10de:1c03 | 10de:1c03 | Nvidia          | GP106 [GeForce GTX 10... | 75%    | 5.0.0    | 186DBB4515 |
| 10de:1c03 | 1458:3716 | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | 8E3EE6F0BA |
| 10de:1c03 | 1458:3739 | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | 1DDF0EC6EC |
| 10de:1c03 | 1458:3776 | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | 28D68A2C46 |
| 10de:1c03 | 1462:3281 | Nvidia          | GP106 [GeForce GTX 10... | 50%    | 4.15.0   | E044F153CE |
| 10de:1c03 | 1462:3283 | Nvidia          | GP106 [GeForce GTX 10... | 14.3%  | 4.13.0   | 9043D81B30 |
| 10de:1c03 | 19da:1438 | Nvidia          | GP106 [GeForce GTX 10... | 33.3%  | 4.18.0   | EF4553CD64 |
| 10de:1c03 | 3842:6163 | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | D94180D023 |
| 10de:1c81 | 10de:11c0 | Nvidia          | GP107 [GeForce GTX 1050] | 80%    | 4.15.0   | 1276D33239 |
| 10de:1c81 | 10de:1c81 | Nvidia          | GP107 [GeForce GTX 1050] | 100%   |          | 6E08766029 |
| 10de:1c81 | 1458:372c | Nvidia          | GP107 [GeForce GTX 1050] | 50%    | 4.15.0   | 1A7DB52C9A |
| 10de:1c81 | 1458:372d | Nvidia          | GP107 [GeForce GTX 1050] | 75%    | 4.15.0   | CAFF866F87 |
| 10de:1c81 | 1458:3765 | Nvidia          | GP107 [GeForce GTX 1050] | 40%    | 4.15.0   | 4CA432FFE1 |
| 10de:1c81 | 1458:3766 | Nvidia          | GP107 [GeForce GTX 1050] | 100%   |          | BE505B8545 |
| 10de:1c81 | 1462:3354 | Nvidia          | GP107 [GeForce GTX 1050] | 100%   |          | 844A6EF03C |
| 10de:1c81 | 1462:8c97 | Nvidia          | GP107 [GeForce GTX 1050] | 66.7%  | 4.15.0   | 9784B3BFB0 |
| 10de:1c81 | 19da:2454 | Nvidia          | GP107 [GeForce GTX 1050] | 50%    | 4.15.0   | F67985779A |
| 10de:1c81 | 3842:6150 | Nvidia          | GP107 [GeForce GTX 1050] | 100%   |          | F2560038AF |
| 10de:1c82 | 1043:85d3 | Nvidia          | GP107 [GeForce GTX 10... | 83.3%  | 4.15.0   | B211311006 |
| 10de:1c82 | 1043:85d6 | Nvidia          | GP107 [GeForce GTX 10... | 33.3%  | 4.15.0   | E48D3747A9 |
| 10de:1c82 | 1043:85ff | Nvidia          | GP107 [GeForce GTX 10... | 20%    | 4.15.0   | 4FF6F8B306 |
| 10de:1c82 | 1043:8613 | Nvidia          | GP107 [GeForce GTX 10... | 33.3%  | 4.15.0   | 4F0A8E2C5B |
| 10de:1c82 | 1043:8627 | Nvidia          | GP107 [GeForce GTX 10... | 100%   |          | 70C1FC426A |
| 10de:1c82 | 1043:862a | Nvidia          | GP107 [GeForce GTX 10... | 100%   |          | F08CE9BD47 |
| 10de:1c82 | 10b0:1c82 | Nvidia          | GP107 [GeForce GTX 10... | 100%   |          | 85FF8C6337 |
| 10de:1c82 | 10de:11bf | Nvidia          | GP107 [GeForce GTX 10... | 10%    | 4.15.0   | 0E4E505931 |
| 10de:1c82 | 10de:1c82 | Nvidia          | GP107 [GeForce GTX 10... | 43.8%  | 4.15.0   | F2CA33243F |
| 10de:1c82 | 1458:3729 | Nvidia          | GP107 [GeForce GTX 10... | 100%   |          | D18B737840 |
| 10de:1c82 | 1458:3733 | Nvidia          | GP107 [GeForce GTX 10... | 50%    | 4.15.0   | E510EC2AB5 |
| 10de:1c82 | 1462:3351 | Nvidia          | GP107 [GeForce GTX 10... | 38.5%  | 4.15.0   | B2CD0963B2 |
| 10de:1c82 | 1462:8c96 | Nvidia          | GP107 [GeForce GTX 10... | 20%    | 4.15.0   | DF0EE54A66 |
| 10de:1c82 | 19da:2454 | Nvidia          | GP107 [GeForce GTX 10... | 50%    | 5.0.0    | 1FE17AADBB |
| 10de:1cb1 | 10de:11bc | Nvidia          | GP107GL [Quadro P1000]   | 100%   |          | 555F102847 |
| 10de:1cb6 | 1028:1264 | Nvidia          | GP107GL [Quadro P620]    | 100%   |          | AD29AF92C2 |
| 10de:1d01 | 1043:85f4 | Nvidia          | GP108 [GeForce GT 1030]  | 66.7%  | 4.18.0   | 04C0BFBF31 |
| 10de:1d01 | 1043:85f5 | Nvidia          | GP108 [GeForce GT 1030]  | 50%    | 4.15.0   | C9B3B14E25 |
| 10de:1d01 | 10de:1d01 | Nvidia          | GP108 [GeForce GT 1030]  | 100%   |          | 61F5096F4A |
| 10de:1d01 | 1458:375c | Nvidia          | GP108 [GeForce GT 1030]  | 20%    | 4.18.0   | 5E946FBF6A |
| 10de:1d01 | 1462:8c98 | Nvidia          | GP108 [GeForce GT 1030]  | 27.3%  | 4.15.0   | E244A01D83 |
| 10de:1d01 | 19da:1476 | Nvidia          | GP108 [GeForce GT 1030]  | 50%    | 4.18.0   | 2B0D032DAD |
| 10de:1e02 | 10de:12a3 | Nvidia          | TU102 [TITAN RTX]        | 100%   |          | 30502C41DE |
| 10de:1e04 | 1458:37c4 | Nvidia          | TU102 [GeForce RTX 20... | 100%   |          | 510AE49DF2 |
| 10de:1e07 | 1462:3711 | Nvidia          | TU102 [GeForce RTX 20... | 100%   |          | 62128222FA |
| 10de:1e07 | 1462:3715 | Nvidia          | TU102 [GeForce RTX 20... | 100%   |          | CE19512CBB |
| 10de:1e07 | 19da:1503 | Nvidia          | TU102 [GeForce RTX 20... | 100%   |          | C8FDC5E958 |
| 10de:1e07 | 3842:2487 | Nvidia          | TU102 [GeForce RTX 20... | 100%   |          | C3DCC51002 |
| 10de:1e82 | 1043:8676 | Nvidia          | TU104 [GeForce RTX 2080] | 100%   |          | 48041296CA |
| 10de:1e82 | 10b0:1e87 | Nvidia          | TU104 [GeForce RTX 2080] | 100%   |          | 73CF7CEE79 |
| 10de:1e82 | 1462:3722 | Nvidia          | TU104 [GeForce RTX 2080] | 100%   |          | ACBAD1E6CE |
| 10de:1e87 | 1458:37a8 | Nvidia          | TU104 [GeForce RTX 20... | 100%   |          | AAD0551E27 |
| 10de:1eb1 | 10de:12a0 | Nvidia          | TU104GL [Quadro RTX 4... | 100%   |          | B95F8101E5 |
| 10de:1f02 | 1458:37c8 | Nvidia          | TU106 [GeForce RTX 2070] | 100%   |          | 69F2264D39 |
| 10de:1f07 | 1043:8670 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | AF6DA5211E |
| 10de:1f07 | 1043:8671 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | AC29A018F8 |
| 10de:1f07 | 10de:12ad | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | 55119E58D9 |
| 10de:1f07 | 1462:3732 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | F1B7697C91 |
| 10de:1f08 | 10de:1f08 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | E28AE1AC43 |
| 10de:1f08 | 1458:3fc2 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | 8DF2C93C38 |
| 10de:1f08 | 196e:130f | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | 328F236B37 |
| 10de:1f08 | 3842:2167 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | 32073E3911 |
| 10de:1f11 | 103c:8574 | Nvidia          | TU106M [GeForce RTX 2... | 100%   |          | 29CB9464AE |
| 10de:1f82 | 1462:3800 | Nvidia          | TU117 [GeForce GTX 1650] | 100%   |          | D5F4BDB1B5 |
| 10de:1f91 | 1043:109f | Nvidia          | TU107 [GeForce GTX 1650] | 100%   |          | 123447177A |
| 10de:2182 | 10de:2182 | Nvidia          | TU116 [GeForce GTX 16... | 100%   |          | C4788779C1 |
| 10de:2182 | 1462:3750 | Nvidia          | TU116 [GeForce GTX 16... | 100%   |          | FB532E634D |
| 8086:0162 | 1028:052c | Intel           | Xeon E3-1200 v2/3rd G... | 14.3%  | 4.15.0   | 29A0FC6CE0 |
| 8086:0162 | 1043:84ca | Intel           | Xeon E3-1200 v2/3rd G... | 25%    | 3.14.44  | 570B707FFB |
| 8086:0162 | 1849:0162 | Intel           | Xeon E3-1200 v2/3rd G... | 3.4%   | 3.10.0   | 8505F4654F |
| 8086:0166 | 1025:0647 | Intel           | 3rd Gen Core processo... | 0.8%   | 3.10.34  | 86D2D3B0E1 |
| 8086:0412 | 1462:7816 | Intel           | Xeon E3-1200 v3/4th G... | 25%    | 4.9.20   | 093472BA51 |
| 8086:041a | 1462:7823 | Intel           | Xeon E3-1200 v3 Proce... | 100%   |          | 7755195EF6 |
| 8086:0f31 | 1025:0936 | Intel           | Atom Processor Z36xxx... | 12.5%  | 4.15.0   | 1718CF1D36 |
| 8086:1902 | 1043:8694 | Intel           | HD Graphics 510          | 12%    | 4.8.14   | A91734714E |
| 8086:1902 | 1462:7996 | Intel           | HD Graphics 510          | 25%    | 4.9.20   | BFAA613B9E |
| 8086:1902 | 8086:2212 | Intel           | HD Graphics 510          | 100%   |          | FF56929B10 |
| 8086:1912 | 1458:d000 | Intel           | HD Graphics 530          | 30%    | 4.9.41   | 53E6A4F263 |
| 8086:1912 | 1849:1912 | Intel           | HD Graphics 530          | 5.6%   | 4.3.3    | 5EF461260F |
| 8086:1916 | 1025:1094 | Intel           | Skylake GT2 [HD Graph... | 10%    | 4.9.9    | E7D6077756 |
| 8086:1916 | 1028:06de | Intel           | Skylake GT2 [HD Graph... | 16.7%  | 4.15.0   | AE7AD1E7D9 |
| 8086:1916 | 1028:06fd | Intel           | Skylake GT2 [HD Graph... | 25%    | 4.15.0   | 569785286A |
| 8086:1916 | 103c:8079 | Intel           | Skylake GT2 [HD Graph... | 8%     | 4.1.15   | 82F5250E0D |
| 8086:1916 | 103c:80a4 | Intel           | Skylake GT2 [HD Graph... | 33.3%  | 4.9.60   | B01FB51118 |
| 8086:1916 | 103c:80ff | Intel           | Skylake GT2 [HD Graph... | 62.5%  | 4.7.2    | B7B039F46E |
| 8086:1916 | 103c:8100 | Intel           | Skylake GT2 [HD Graph... | 100%   |          | 2B56F34E21 |
| 8086:1916 | 103c:8101 | Intel           | Skylake GT2 [HD Graph... | 9.1%   | 4.9.60   | BC496704F4 |
| 8086:1916 | 103c:820c | Intel           | Skylake GT2 [HD Graph... | 25%    | 4.9.20   | FAE1CD27F3 |
| 8086:1916 | 1043:1ccd | Intel           | Skylake GT2 [HD Graph... | 25%    | 4.9.20   | A4B26975E9 |
| 8086:1916 | 1179:f822 | Intel           | Skylake GT2 [HD Graph... | 25%    | 4.15.0   | B781D8419A |
| 8086:1916 | 17aa:3824 | Intel           | Skylake GT2 [HD Graph... | 6.2%   | 4.9.9    | 412EAC636F |
| 8086:1916 | 17aa:382c | Intel           | Skylake GT2 [HD Graph... | 25%    | 4.9.0    | 18379EBD5C |
| 8086:1916 | 17aa:5048 | Intel           | Skylake GT2 [HD Graph... | 33.3%  | 4.15.0   | 842B139FE7 |
| 8086:191b | 1028:06de | Intel           | HD Graphics 530          | 25%    | 5.0.0    | BC4C6EBBA7 |
| 8086:191b | 1043:1080 | Intel           | HD Graphics 530          | 33.3%  | 5.0.0    | 5B1076EA3C |
| 8086:191b | 1043:1d6d | Intel           | HD Graphics 530          | 100%   |          | 9D6C0DD372 |
| 8086:191b | 1462:1190 | Intel           | HD Graphics 530          | 16.7%  | 4.9.9    | 2B70AAB06F |
| 8086:1921 | 17aa:39e8 | Intel           | HD Graphics 520          | 25%    | 4.9.111  | C3352134E9 |
| 8086:22b1 | 1025:1012 | Intel           | Atom/Celeron/Pentium ... | 5.1%   | 4.9.20   | 16D1C62342 |
| 8086:22b1 | 1028:0725 | Intel           | Atom/Celeron/Pentium ... | 25%    | 4.9.20   | 92DCC778AC |
| 8086:22b1 | 1043:10c0 | Intel           | Atom/Celeron/Pentium ... | 3.7%   | 4.9.9    | E6AFAB9B56 |
| 8086:22b1 | 1558:0945 | Intel           | Atom/Celeron/Pentium ... | 7.7%   | 4.1.15   | BDAF59B6EB |
| 8086:2572 | 103c:12bc | Intel           | 82865G Integrated Gra... | 25%    | 4.1.34   | DD4DD47556 |
| 8086:2772 | 8086:464c | Intel           | 82945G/GZ Integrated ... | 12.5%  | 3.10.0   | 1B11619EC9 |
| 8086:27a2 | 104d:820f | Intel           | Mobile 945GM/GMS, 943... | 42.9%  | 3.14.44  | 811EFEE1FC |
| 8086:27a2 | 1462:0341 | Intel           | Mobile 945GM/GMS, 943... | 25%    | 4.1.15   | C71F72F074 |
| 8086:2992 | 1734:10b5 | Intel           | 82Q963/Q965 Integrate... | 25%    | 4.1.15   | BF1BADE95D |
| 8086:2e12 | 17aa:3048 | Intel           | 4 Series Chipset Inte... | 15.4%  | 4.1.15   | 4B2E86F845 |
| 8086:3e91 | 1043:8694 | Intel           | 8th Gen Core Processo... | 25%    | 4.15.0   | DA54361164 |
| 8086:3e91 | 1849:3e91 | Intel           | 8th Gen Core Processo... | 10%    | 4.15.0   | 59151791CF |
| 8086:3e92 | 1028:0851 | Intel           | UHD Graphics 630 (Des... | 100%   |          | 05D6B79D2F |
| 8086:3e98 | 1462:7b98 | Intel           | UHD Graphics 630 (Des... | 100%   |          | 297E534CF0 |
| 8086:3e9b | 1025:1264 | Intel           | UHD Graphics 630 (Mob... | 13.3%  | 4.15.0   | C4FA903BED |
| 8086:3e9b | 1462:126a | Intel           | UHD Graphics 630 (Mob... | 100%   |          | 039A05F3EB |
| 8086:5912 | 1043:8694 | Intel           | HD Graphics 630          | 1.8%   | 4.4.49   | B0DE2CBA6A |
| 8086:5912 | 1458:d000 | Intel           | HD Graphics 630          | 3.8%   | 3.10.0   | 6126E55D1A |
| 8086:5916 | 1028:0782 | Intel           | HD Graphics 620          | 33.3%  | 4.18.0   | 49389100FC |
| 8086:5916 | 17aa:39f1 | Intel           | HD Graphics 620          | 11.1%  | 4.9.60   | 65FE9A36B5 |
| 8086:5916 | 8086:2212 | Intel           | HD Graphics 620          | 5.6%   | 4.9.41   | B1A55C7D69 |
| 8086:8108 | 1028:02b1 | Intel           | US15W/US15X SCH [Poul... | 100%   |          | 7D4473A4A5 |
| 8086:a011 | 1462:104e | Intel           | Atom Processor D4xx/D... | 20%    | 4.1.15   | 5F15F028A8 |

### Modem (PCI)

38 out of 86 (44.19%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1039:7013 | 1025:0083 | Silicon Inte... | AC'97 Modem Controller   | 100%   |          | 354B6DE784 |
| 1057:3052 | 1057:3020 | Motorola        | SM56 Data Fax Modem      | 100%   |          | D3B45DE297 |
| 1057:3052 | 1631:3034 | Motorola        | SM56 Data Fax Modem      | 100%   |          | B7CEC1644D |
| 10b9:5457 | 103c:0850 | ULi Electronics | M5457 AC'97 Modem Con... | 100%   |          | 4E9D284D9C |
| 11c1:0440 | 11c1:0440 | LSI             | 56k WinModem             | 100%   |          | 6B2E5020C2 |
| 11c1:0449 | 1468:0410 | LSI             | L56xM+S [Mars-2] WinM... | 100%   |          | A8A13EFBA0 |
| 11c1:044c | 11c1:044c | LSI             | LT WinModem              | 100%   |          | E75F4538BC |
| 11c1:044e | 11c1:044e | LSI             | LT WinModem              | 100%   |          | 6203763CC5 |
| 11c1:044e | 1235:044e | LSI             | LT WinModem              | 100%   |          | 3D74179CB7 |
| 1543:3052 | 1543:3000 | SILICON Labo... | Intel 537 [Winmodem]     | 100%   |          | 75C969D54B |
| 2003:8800 | 16ef:2800 | Smart Link      | LM-I56N                  | 100%   |          | 8B4AE6CF41 |
| 2003:8800 | 1801:2800 | Smart Link      | LM-I56N                  | 100%   |          | 413AE4FF4F |
| 8086:1040 | 8086:1000 | Intel           | 536EP Data Fax Modem     | 100%   |          | 1263C61735 |
| 8086:2486 | 134d:4c21 | Intel           | 82801CA/CAM AC'97 Mod... | 100%   |          | 38C172234D |
| 8086:24c6 | 1014:0524 | Intel           | 82801DB/DBL/DBM (ICH4... | 100%   |          | BE49E35FA4 |
| 8086:24c6 | 1014:0559 | Intel           | 82801DB/DBL/DBM (ICH4... | 83.3%  | 3.14.53  | 1811B66E00 |
| 8086:24c6 | 103c:3080 | Intel           | 82801DB/DBL/DBM (ICH4... | 100%   |          | 6802B34FDD |
| 8086:24c6 | 10cf:10d1 | Intel           | 82801DB/DBL/DBM (ICH4... | 66.7%  | 3.14.25  | EA732BEA27 |
| 8086:24c6 | 1179:0001 | Intel           | 82801DB/DBL/DBM (ICH4... | 50%    | 4.9.0    | 15CFD6C8AF |
| 8086:24c6 | 1179:ff31 | Intel           | 82801DB/DBL/DBM (ICH4... | 80%    | 4.1.38   | E9BD04F647 |
| 8086:24c6 | 14f1:5422 | Intel           | 82801DB/DBL/DBM (ICH4... | 11.1%  | 3.14.44  | 0504CC20A9 |
| 8086:24c6 | 1734:103c | Intel           | 82801DB/DBL/DBM (ICH4... | 100%   |          | 6F452862B4 |
| 8086:24d6 | 1025:0045 | Intel           | 82801EB/ER (ICH5/ICH5... | 100%   |          | 41CC7EB08C |
| 8086:24d6 | 1179:0001 | Intel           | 82801EB/ER (ICH5/ICH5... | 100%   |          | A7D4DEEF9E |
| 8086:266d | 1014:0574 | Intel           | 82801FB/FBM/FR/FW/FRW... | 75%    | 4.9.41   | 4916E9EC9C |
| 8086:266d | 1014:0576 | Intel           | 82801FB/FBM/FR/FW/FRW... | 50%    | 3.14.33  | 9809E004BA |
| 8086:266d | 1025:0066 | Intel           | 82801FB/FBM/FR/FW/FRW... | 25%    | 3.14.44  | E814DA247A |
| 8086:266d | 1025:006a | Intel           | 82801FB/FBM/FR/FW/FRW... | 42.9%  | 3.14.25  | 86C81D521E |
| 8086:266d | 103c:0934 | Intel           | 82801FB/FBM/FR/FW/FRW... | 100%   |          | 16F00AAE37 |
| 8086:266d | 103c:099c | Intel           | 82801FB/FBM/FR/FW/FRW... | 14.3%  | 3.14.44  | C60AB5C121 |
| 8086:266d | 103c:3080 | Intel           | 82801FB/FBM/FR/FW/FRW... | 50%    | 4.9.9    | 0572E8425C |
| 8086:266d | 103c:3082 | Intel           | 82801FB/FBM/FR/FW/FRW... | 100%   |          | 91C7AE2180 |
| 8086:266d | 103c:309d | Intel           | 82801FB/FBM/FR/FW/FRW... | 33.3%  | 4.1.16   | 837230178B |
| 8086:266d | 103c:30c4 | Intel           | 82801FB/FBM/FR/FW/FRW... | 50%    | 4.1.25   | 87F8EF65AE |
| 8086:266d | 1179:0001 | Intel           | 82801FB/FBM/FR/FW/FRW... | 69.2%  | 3.14.44  | 45B2F7B46A |
| 8086:266d | 144d:2115 | Intel           | 82801FB/FBM/FR/FW/FRW... | 50%    | 4.1.22   | 88BAF3B388 |
| 8086:266d | 14f1:5423 | Intel           | 82801FB/FBM/FR/FW/FRW... | 40.7%  | 3.14.44  | 23F9D951DE |
| 8086:266d | 17aa:207c | Intel           | 82801FB/FBM/FR/FW/FRW... | 100%   |          | EDAE63A429 |

### Multimedia controller (PCI)

127 out of 153 (83.01%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 0002:8290 | 107d:2609 |                 | Multimedia controller    | 100%   |          | 95D420F37F |
| 1002:4d51 | 1002:b041 | AMD             | Unified AVStream Driver  | 100%   |          | 2CF316774E |
| 1002:ac12 | 1002:b539 | AMD             | Theater HD T507 (DVB-... | 100%   |          | DD5E0979B0 |
| 1002:ac12 | 12ab:0003 | AMD             | Theater HD T507 (DVB-... | 100%   |          | EA55AE13AC |
| 1002:ad18 | 1682:ad18 | AMD             | Multimedia controller    | 100%   |          | 3108FE53D3 |
| 1022:15e2 | 1022:15e2 | AMD             | Raven/Raven2/FireFlig... | 50%    | 5.0.0    | 048229855F |
| 1022:15e2 | 1025:1233 | AMD             | Raven/Raven2/FireFlig... | 100%   |          | 856A212CAA |
| 1022:15e2 | 103c:8433 | AMD             | Raven/Raven2/FireFlig... | 50%    | 5.0.0    | 2BCAD0A319 |
| 1022:15e2 | 103c:8434 | AMD             | Raven/Raven2/FireFlig... | 100%   |          | E2E650868B |
| 1022:15e2 | 103c:8496 | AMD             | Raven/Raven2/FireFlig... | 25%    | 5.0.0    | 10702AB56C |
| 1022:15e2 | 103c:84ae | AMD             | Raven/Raven2/FireFlig... | 85.3%  | 5.0.0    | E8755C7EF8 |
| 1022:15e2 | 103c:84d2 | AMD             | Raven/Raven2/FireFlig... | 100%   |          | DEFB86D43A |
| 1022:15e2 | 17aa:36f5 | AMD             | Raven/Raven2/FireFlig... | 100%   |          | 7E41940C9C |
| 1022:15e2 | 17aa:380b | AMD             | Raven/Raven2/FireFlig... | 100%   |          | 52036BD95B |
| 1022:15e2 | 17aa:3811 | AMD             | Raven/Raven2/FireFlig... | 100%   |          | 878BBF3E54 |
| 1022:15e2 | 17aa:5124 | AMD             | Raven/Raven2/FireFlig... | 100%   |          | 79E53D2DB5 |
| 1022:15e2 | 19e5:3e06 | AMD             | Raven/Raven2/FireFlig... | 100%   |          | 2CDCEA8607 |
| 1057:3410 | 1057:ffff | Motorola        | DSP56361 Digital Sign... | 100%   |          | 16A7890585 |
| 1057:3410 | 11af:eed2 | Motorola        | DSP56361 Digital Sign... | 100%   |          | 16A7890585 |
| 1057:3410 | 11af:eee1 | Motorola        | DSP56361 Digital Sign... | 100%   |          | 16A7890585 |
| 109e:0878 |           | Brooktree       | Bt878 Audio Capture      | 100%   |          | BA9CCBD3A5 |
| 109e:0878 | 0070:ff04 | Brooktree       | Bt878 Audio Capture      | 100%   |          | 2C877CF870 |
| 109e:0878 | 1047:f331 | Brooktree       | Bt878 Audio Capture      | 100%   |          | 444FFBC8A6 |
| 109e:0878 | 107d:6609 | Brooktree       | Bt878 Audio Capture      | 100%   |          | 4A6B13BAEA |
| 109e:0878 | 1461:0001 | Brooktree       | Bt878 Audio Capture      | 100%   |          | E8072B6F3A |
| 109e:0878 | 1461:0002 | Brooktree       | Bt878 Audio Capture      | 100%   |          | A22609B54B |
| 109e:0878 | 1461:0003 | Brooktree       | Bt878 Audio Capture      | 6.7%   | 3.14.25  | 7A69435C43 |
| 109e:0878 | 1461:0004 | Brooktree       | Bt878 Audio Capture      | 100%   |          | 660B28DD52 |
| 109e:0878 | 800a:763d | Brooktree       | Bt878 Audio Capture      | 100%   |          | 08DCF9AA49 |
| 109e:0878 | 800b:763d | Brooktree       | Bt878 Audio Capture      | 100%   |          | 08DCF9AA49 |
| 109e:0878 | 800c:763d | Brooktree       | Bt878 Audio Capture      | 100%   |          | 08DCF9AA49 |
| 109e:0878 | 800d:763d | Brooktree       | Bt878 Audio Capture      | 100%   |          | 08DCF9AA49 |
| 109e:0878 | bd11:4100 | Brooktree       | Bt878 Audio Capture      | 100%   |          | C20B184FC3 |
| 10b5:9056 | 1a0e:0073 | PLX Technology  | PCI9056 32-bit 66MHz ... | 50%    | 4.15.0   | 5122F7EE54 |
| 10cf:202a | 104d:81fa | Fujitsu Limi... | Integrated MPEG Encoder  | 100%   |          | 7F0BB0CC92 |
| 10cf:2030 | 104d:9062 | Fujitsu Limi... | Fujitsu Multimedia co... | 100%   |          | 2628EBE1BB |
| 1131:7160 | 1461:0455 | Philips Semi... | SAA7160                  | 100%   |          | F85808C04C |
| 1131:7160 | 1461:0555 | Philips Semi... | SAA7160                  | 100%   |          | D400943350 |
| 1131:7160 | 1461:0855 | Philips Semi... | SAA7160                  | 100%   |          | BBDA8BED86 |
| 1131:7160 | 1461:0955 | Philips Semi... | SAA7160                  | 100%   |          | 388696B306 |
| 1131:7160 | 1461:0a55 | Philips Semi... | SAA7160                  | 100%   |          | 99DDBBF195 |
| 1131:7160 | 1461:1055 | Philips Semi... | SAA7160                  | 100%   |          | 9E921922BA |
| 1131:7160 | 1461:1455 | Philips Semi... | SAA7160                  | 100%   |          | C785DD2710 |
| 1131:7160 | 1461:1855 | Philips Semi... | SAA7160                  | 100%   |          | FA070462FC |
| 1131:7160 | 1461:2355 | Philips Semi... | SAA7160                  | 100%   |          | B98B8362E0 |
| 1131:7160 | 1461:2655 | Philips Semi... | SAA7160                  | 100%   |          | A74B989748 |
| 1131:7160 | 16be:0034 | Philips Semi... | SAA7160                  | 100%   |          | 2B8D93B7EC |
| 1131:7160 | 1ae4:0700 | Philips Semi... | SAA7160                  | 100%   |          | E9FCA3B9C8 |
| 1131:7160 | 6281:0001 | Philips Semi... | SAA7160                  | 13.3%  | 4.9.76   | 30EC426B43 |
| 1131:7160 | 6928:0001 | Philips Semi... | SAA7160                  | 100%   |          | 8C8F8EFAB1 |
| 1131:7160 | 6928:0002 | Philips Semi... | SAA7160                  | 100%   |          | 47FD7AB796 |
| 1131:7162 | 11bd:0100 | Philips Semi... | SAA7162                  | 100%   |          | EF8A743A1E |
| 1131:7162 | 11bd:0101 | Philips Semi... | SAA7162                  | 100%   |          | 003EB89135 |
| 1131:7231 | 12ab:0762 | Philips Semi... | SAA7231                  | 100%   |          | A72F1BCDE6 |
| 1131:7231 | 12ab:0763 | Philips Semi... | SAA7231                  | 100%   |          | 6F6F611F59 |
| 1131:7231 | 1461:0b0f | Philips Semi... | SAA7231                  | 100%   |          | 791CA50070 |
| 1131:7231 | 1461:110f | Philips Semi... | SAA7231                  | 100%   |          | 90DFBFB6FA |
| 1131:7231 | 1461:1400 | Philips Semi... | SAA7231                  | 100%   |          | 4F99536247 |
| 1131:7231 | 1461:2a0f | Philips Semi... | SAA7231                  | 100%   |          | 4CA7976A88 |
| 1131:7231 | 1461:2b07 | Philips Semi... | SAA7231                  | 100%   |          | 8672A3F85D |
| 1131:7231 | 1461:2b0f | Philips Semi... | SAA7231                  | 100%   |          | F92CB57F54 |
| 1131:7231 | 1461:3301 | Philips Semi... | SAA7231                  | 100%   |          | 7E1176A7C2 |
| 1131:7231 | 1461:7983 | Philips Semi... | SAA7231                  | 100%   |          | 6186ACA9BB |
| 1131:7231 | 16be:0008 | Philips Semi... | SAA7231                  | 100%   |          | 1BA5C50EAD |
| 1131:7231 | 5ace:8000 | Philips Semi... | SAA7231                  | 100%   |          | FA070462FC |
| 1131:7231 | 5ace:8150 | Philips Semi... | SAA7231                  | 100%   |          | 8603D5BDF5 |
| 1131:7231 | 5ace:8201 | Philips Semi... | SAA7231                  | 100%   |          | 3D68E82C9F |
| 11bd:0040 | 11bd:0045 | Pinnacle Sys... | Royal TS Function 1      | 100%   |          | FF0A7B1FC8 |
| 11bd:0041 | 11bd:0045 | Pinnacle Sys... | RoyalTS Function 2       | 100%   |          | FF0A7B1FC8 |
| 11bd:0042 | 11bd:0045 | Pinnacle Sys... | Royal TS Function 3      | 100%   |          | FF0A7B1FC8 |
| 11bd:bede | 11bd:0022 | Pinnacle Sys... | AV/DV Studio Capture ... | 100%   |          | BC68308D9C |
| 11bd:bede | 11bd:0023 | Pinnacle Sys... | AV/DV Studio Capture ... | 100%   |          | EBD8A5801D |
| 14e4:1570 | 14e4:1570 | Broadcom Inc... | 720p FaceTime HD Camera  | 23.3%  | 4.15.0   | 49A28F87B9 |
| 14e4:1612 | 14e4:2612 | Broadcom        | BCM70012 Video Decode... | 100%   |          | 3CBFF8D8F5 |
| 14e4:1615 | 105b:0d77 | Broadcom        | BCM70015 Video Decode... | 100%   |          | B036D312E6 |
| 14e4:1615 | 14e4:1615 | Broadcom Inc... | BCM70015 Video Decode... | 100%   |          | E6CF3D7F11 |
| 14f1:8803 | 185b:e000 | Conexant Sys... | CX2388x TV Capture Chip  | 100%   |          | 5B85C2F248 |
| 14f1:8804 | 0070:1402 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | 186479593C |
| 14f1:8804 | 0070:6902 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | 556AE96F13 |
| 14f1:8804 | 0070:6906 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | B95995E16E |
| 14f1:8804 | 0070:9002 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | 8168BA11E3 |
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
| 8086:0f38 | 8086:0f31 | Intel           | Atom Processor Z36xxx... | 89.5%  | 4.12.4   | CEAC334581 |
| 8086:0f38 | 8086:7270 | Intel           | Atom Processor Z36xxx... | 92.9%  | 5.0.0    | 2D4AA64C10 |
| 8086:1919 | 1025:111e | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | D6EFA0F211 |
| 8086:1919 | 1028:06e6 | Intel           | Xeon E3-1200 v5/E3-15... | 20%    | 5.0.0    | 1ABBA3CDA0 |
| 8086:1919 | 1028:07a4 | Intel           | Xeon E3-1200 v5/E3-15... | 33.3%  | 5.0.0    | 75F6A84286 |
| 8086:1919 | 103c:82cb | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | FDB567A59E |
| 8086:1919 | 144d:c135 | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | D7B5599247 |
| 8086:1919 | 152d:1182 | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | 57487D8BF7 |
| 8086:1919 | 17aa:2241 | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | 1038A34C39 |
| 8086:1919 | 17aa:3812 | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | 57EC66B289 |
| 8086:1919 | 17aa:382f | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | 1DD80D33E5 |
| 8086:1919 | 19e5:3e00 | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | 3DD5AAE701 |
| 8086:1919 | 8086:1919 | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | 707E0DB074 |
| 8086:1919 | 8086:2015 | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | 329795002B |
| 8086:22b8 | 1025:1021 | Intel           | Atom/Celeron/Pentium ... | 100%   |          | 663247803F |
| 8086:22b8 | 1025:106e | Intel           | Atom/Celeron/Pentium ... | 100%   |          | 425D589D65 |
| 8086:22b8 | 1028:06ea | Intel           | Atom/Celeron/Pentium ... | 60%    | 4.20.1   | 743979C6E7 |
| 8086:22b8 | 103c:813e | Intel           | Atom/Celeron/Pentium ... | 100%   |          | F91E0FBE6B |
| 8086:22b8 | 103c:827c | Intel           | Atom/Celeron/Pentium ... | 100%   |          | DD16DF4133 |
| 8086:22b8 | 1043:13a0 | Intel           | Atom/Celeron/Pentium ... | 90%    | 5.1.6    | 1EB4640C84 |
| 8086:22b8 | 1043:1400 | Intel           | Atom/Celeron/Pentium ... | 63.6%  | 5.0.11   | 838DD8C3AC |
| 8086:22b8 | 1071:a126 | Intel           | Atom/Celeron/Pentium ... | 100%   |          | F2981C1775 |
| 8086:22b8 | 1297:2063 | Intel           | Atom/Celeron/Pentium ... | 83.3%  | 5.0.0    | 7B041A9627 |
| 8086:22b8 | 17aa:222a | Intel           | Atom/Celeron/Pentium ... | 50%    | 5.0.0    | 5AF55E5191 |
| 8086:22b8 | 17aa:3809 | Intel           | Atom/Celeron/Pentium ... | 33.3%  | 5.0.0    | E844699BF8 |
| 8086:22b8 | 17aa:38e3 | Intel           | Atom/Celeron/Pentium ... | 66.7%  | 5.1.15   | CE2895A69A |
| 8086:22b8 | 8086:7270 | Intel           | Atom/Celeron/Pentium ... | 81.6%  | 4.20.0   | B3104B40CE |
| 8086:5a88 |           | Intel           | Celeron N3350/Pentium... | 100%   |          | F92E526676 |
| 8086:9d32 |           | Intel           | Skylake-U/Y Camera IO... | 50%    | 5.1.0    | C596B50DF9 |
| 8086:9d32 | 1043:1410 | Intel           | Skylake-U/Y Camera IO... | 100%   |          | 0B5AD4104E |
| 8086:9d32 | 17aa:380c | Intel           | Skylake-U/Y Camera IO... | 33.3%  | 4.18.0   | 1D220D1155 |
| 8086:9d32 | 8086:7270 | Intel           | Skylake-U/Y Camera IO... | 35.3%  | 4.18.0   | 2FB15D0705 |
| 8086:9d32 | 8086:9d32 | Intel           | Skylake-U/Y Camera IO... | 50%    | 4.18.0   | 23C4F883A7 |
| dd01:0006 | dd01:0022 | Digital Devices | Cine V7                  | 100%   |          | FCF4AFE5C6 |

### Net/ethernet (PCI)

32 out of 3468 (0.92%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 0000:0200 | 002c:0200 |                 | Ethernet controller      | 100%   |          | 32AE4212DF |
| 000c:0000 | 1043:83a3 |                 | Ethernet controller      | 100%   |          | B5189C3BF2 |
| 10ec:0139 | 10bd:0320 | Realtek Semi... | RTL-8139/8139C/8139C+... | 100%   |          | 305C35F50C |
| 10ec:3000 | 1025:132d | Realtek Semi... | Killer E3000 2.5 Giga... | 100%   |          | EFD907D30F |
| 10ec:8131 | 10ec:8131 | Realtek Semi... | RTL8131 PCIe Fast Eth... | 100%   |          | 4E43962152 |
| 10ec:8136 | 1028:0555 | Realtek Semi... | RTL810xE PCI Express ... | 5%     | 4.1.15   | A7211B4E35 |
| 10ec:8136 | 103c:1484 | Realtek Semi... | RTL810xE PCI Express ... | 7.7%   | 4.9.60   | C7734FBAE0 |
| 10ec:8136 | 103c:306b | Realtek Semi... | RTL810xE PCI Express ... | 33.3%  | 3.14.44  | 93C0EF7223 |
| 10ec:8136 | 103c:820c | Realtek Semi... | RTL810xE PCI Express ... | 25%    | 4.1.25   | 21A7695D56 |
| 10ec:8136 | 1462:7529 | Realtek Semi... | RTL810xE PCI Express ... | 4.8%   | 3.14.44  | 99777B72F9 |
| 10ec:8136 | 17aa:381f | Realtek Semi... | RTL810xE PCI Express ... | 10.5%  | 4.1.34   | 1952B1CCF3 |
| 10ec:8168 | 1025:125c | Realtek Semi... | RTL8111/8168/8411 PCI... | 7.1%   | 4.18.0   | 6AEFA7E06C |
| 10ec:8168 | 103c:180d | Realtek Semi... | RTL8111/8168/8411 PCI... | 3.1%   | 3.10.42  | 41A6D6B87B |
| 10ec:8168 | 1043:1447 | Realtek Semi... | RTL8111/8168/8411 PCI... | 9.1%   | 3.14.44  | F23B5BF0DA |
| 10ec:8168 | 1043:200f | Realtek Semi... | RTL8111/8168/8411 PCI... | 0.4%   | 3.10.34  | 91D9C778CB |
| 10ec:8168 | 1297:2033 | Realtek Semi... | RTL8111/8168/8411 PCI... | 14.3%  | 4.9.20   | 51273F53DF |
| 10ec:8168 | 1458:e000 | Realtek Semi... | RTL8111/8168/8411 PCI... | 0%     | 2.6.32   | 765A1CCD27 |
| 10ec:8168 | 14c0:0059 | Realtek Semi... | RTL8111/8168/8411 PCI... | 100%   |          | 42B3F11A1E |
| 10ec:8168 | 1558:1323 | Realtek Semi... | RTL8111/8168/8411 PCI... | 28.6%  | 4.15.0   | 75848692B4 |
| 10ec:8168 | 1558:1550 | Realtek Semi... | RTL8111/8168/8411 PCI... | 2.3%   | 3.14.33  | A0EB5DA51A |
| 1186:4200 | 1186:1103 | D-Link System   | DFE-520TX Fast Ethern... | 100%   |          | 790E740601 |
| 14e4:16a3 | 14e4:16b4 | Broadcom Inc... | NetXtreme BCM57786 Gi... | 100%   |          | FECEC5C77A |
| 14e4:52a3 | d3a6:afcd | Broadcom Lim... | Ethernet controller      | 100%   |          | 191BA97155 |
| 1a47:0003 | 0000:0200 | 3DSP            | WLAN and Bluetooth Card  | 100%   |          | 3A17145633 |
| 8086:0000 | 8086:0000 | Intel           | PROSet/Wireless WiFi ... | 100%   |          | 418C3E7B73 |
| 8086:107c | 8086:1376 | Intel           | 82541PI Gigabit Ether... | 2.9%   | 2.6.32   | F801FAB1AD |
| 8086:10aa | 8086:0000 | Intel           | Ethernet controller      | 100%   |          | CBBE408AAC |
| 8086:15b8 | 1043:8672 | Intel           | Ethernet Connection (... | 0.5%   | 4.1.15   | 51B31F180E |
| 8086:15bc | 1028:0851 | Intel           | Ethernet Connection (... | 100%   |          | 05D6B79D2F |
| 8086:15bc | 1849:15bc | Intel           | Ethernet Connection (... | 13.3%  | 4.13.0   | BA39531B87 |
| 8086:37cc | 103c:81c7 | Intel           | Ethernet Connection X722 | 100%   |          | 0617E49F12 |
| 8086:37cc | 15d9:0000 | Intel           | Ethernet Connection X722 | 100%   |          | 2794B14FEE |

### Net/wireless (PCI)

114 out of 849 (13.43%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 104c:8400 | 1186:3b01 | Texas Instru... | ACX 100 22Mbps Wirele... | 100%   |          | 92B50659EB |
| 104c:9066 | 1086:3b04 | Texas Instru... | ACX 111 54Mbps Wirele... | 100%   |          | DBFFE622A8 |
| 104c:9066 | 1186:3b04 | Texas Instru... | ACX 111 54Mbps Wirele... | 100%   |          | C1E24ECC67 |
| 10ec:8176 | 1a3b:1139 | Realtek Semi... | RTL8188CE 802.11b/g/n... | 3.9%   | 3.14.33  | 51273F53DF |
| 10ec:8190 | 10ec:8190 | Realtek Semi... | RTL8190 802.11n PCI W... | 100%   |          | AE38CF07EA |
| 10ec:8723 | 10ec:0726 | Realtek Semi... | RTL8723AE PCIe Wirele... | 1%     | 3.18.10  | 598F621727 |
| 10ec:8821 | 1a3b:2161 | Realtek Semi... | RTL8821AE 802.11ac PC... | 14.3%  | 3.14.44  | 5EEDC9CEE8 |
| 10ec:b723 | 1025:b734 | Realtek Semi... | RTL8723BE PCIe Wirele... | 18.2%  | 4.1.10   | DE10405623 |
| 10ec:b723 | 103c:2231 | Realtek Semi... | RTL8723BE PCIe Wirele... | 34%    | 3.18.11  | B301F51204 |
| 10ec:b723 | 10ec:b729 | Realtek Semi... | RTL8723BE PCIe Wirele... | 31.5%  | 3.17.4   | FD5BC52C49 |
| 10ec:b723 | 10ec:b733 | Realtek Semi... | RTL8723BE PCIe Wirele... | 16.7%  | 4.1.38   | BDAF59B6EB |
| 10ec:b723 | 11ad:1723 | Realtek Semi... | RTL8723BE PCIe Wirele... | 3.9%   | 4.9.9    | E6285FD8C3 |
| 10ec:b723 | 17aa:b728 | Realtek Semi... | RTL8723BE PCIe Wirele... | 35.3%  | 3.18.14  | 02D1977887 |
| 10ec:b723 | 17aa:b736 | Realtek Semi... | RTL8723BE PCIe Wirele... | 15.5%  | 3.18.16  | 8C16B6C71F |
| 10ec:b723 | 1a3b:2159 | Realtek Semi... | RTL8723BE PCIe Wirele... | 5.9%   | 4.1.15   | DDF48A7B95 |
| 10ec:b723 | 1b9a:2485 | Realtek Semi... | RTL8723BE PCIe Wirele... | 11.1%  | 4.3.3    | D57B5C86E0 |
| 10ec:b822 | 103c:831b | Realtek Semi... | RTL8822BE 802.11a/b/g... | 9.8%   | 4.15.0   | AC62725ABE |
| 10ec:b822 | 1043:8746 | Realtek Semi... | RTL8822BE 802.11a/b/g... | 6.2%   | 4.15.0   | 27EB064D7D |
| 10ec:b822 | 1a3b:2950 | Realtek Semi... | RTL8822BE 802.11a/b/g... | 4.3%   | 4.13.0   | B6B40DE397 |
| 10ec:c821 | 103c:831a | Realtek Semi... | RTL8821CE 802.11ac PC... | 97.3%  | 5.0.6    | 4F9294F4B5 |
| 10ec:c821 | 10ec:c821 | Realtek Semi... | RTL8821CE 802.11ac PC... | 100%   |          | F71EFE50CF |
| 10ec:c821 | 10ec:c827 | Realtek Semi... | RTL8821CE 802.11ac PC... | 71.4%  | 4.15.0   | C8EE1F4CA3 |
| 10ec:c821 | 17aa:c024 | Realtek Semi... | RTL8821CE 802.11ac PC... | 90.7%  | 4.9.124  | C61C9E33F6 |
| 10ec:c821 | 1a3b:3040 | Realtek Semi... | RTL8821CE 802.11ac PC... | 100%   |          | C3F6335949 |
| 10ec:c821 | 1a3b:3041 | Realtek Semi... | RTL8821CE 802.11ac PC... | 100%   |          | 2B350FD655 |
| 11ab:1fa6 | 1043:138f | Marvell Tech... | Marvell W8300 802.11 ... | 100%   |          | E75F4538BC |
| 11ab:1fa7 | 1043:138f | Marvell Tech... | 88W8310 and 88W8000G ... | 100%   |          | 436FC401D1 |
| 11ab:1faa | 11ab:1faa | Marvell Tech... | 88w8335 [Libertas] 80... | 100%   |          | AD16215D6C |
| 11ab:1faa | 1385:6b00 | Marvell Tech... | 88w8335 [Libertas] 80... | 100%   |          | C9EEDBA4ED |
| 14c3:7630 | 103c:197c | MEDIATEK        | MT7630e 802.11bgn Wir... | 100%   |          | A7E6CBC45B |
| 14c3:7630 | 105b:e074 | MEDIATEK        | MT7630e 802.11bgn Wir... | 100%   |          | 91D9C778CB |
| 14c3:7630 | 105b:e084 | MEDIATEK        | MT7630e 802.11bgn Wir... | 100%   |          | 0E146447BF |
| 14e4:4311 | 1468:0316 | Broadcom Inc... | BCM4311 802.11b/g WLAN   | 100%   |          | 7F0BB0CC92 |
| 14e4:4315 | 103c:1508 | Broadcom Inc... | BCM4312 802.11b/g LP-PHY | 1.7%   | 3.14.44  | D0F06C8499 |
| 14e4:4318 | 1468:0312 | Broadcom Lim... | BCM4318 [AirForce One... | 20.8%  | 3.10.34  | A28F7B2623 |
| 14e4:4328 | 106b:0088 | Broadcom Inc... | BCM4321 802.11a/b/g/n    | 5.3%   | 4.1.15   | 985A14858E |
| 14e4:4328 | 106b:0090 | Broadcom Lim... | BCM4321 802.11a/b/g/n    | 5.6%   | 4.1.22   | 030A81E657 |
| 14e4:432b | 1028:000d | Broadcom Inc... | BCM4322 802.11a/b/g/n... | 7.1%   | 3.10.19  | 103788F3AC |
| 14e4:4353 | 1028:000e | Broadcom Inc... | BCM43224 802.11a/b/g/n   | 4.3%   | 4.1.15   | 68FA7AD805 |
| 14e4:4353 | 106b:0093 | Broadcom Inc... | BCM43224 802.11a/b/g/n   | 3%     | 4.1.15   | 4E11213A56 |
| 14e4:4357 | 105b:e021 | Broadcom Inc... | BCM43225 802.11b/g/n     | 3.3%   | 3.14.25  | DDD532FC51 |
| 14e4:4358 | 105b:e040 | Broadcom Inc... | BCM43227 802.11b/g/n     | 0.9%   | 3.14.33  | 4ABA261C6D |
| 14e4:4359 | 1028:0014 | Broadcom Inc... | BCM43228 802.11a/b/g/n   | 4.8%   | 3.14.44  | 9F82A1A551 |
| 14e4:4359 | 103c:2135 | Broadcom Inc... | BCM43228 802.11a/b/g/n   | 50%    | 4.1.25   | 3E13F8A157 |
| 14e4:4359 | 1043:850c | Broadcom Inc... | BCM43228 802.11a/b/g/n   | 7%     | 3.14.44  | 7E0E64D8B4 |
| 14e4:4359 | 105b:e04b | Broadcom Inc... | BCM43228 802.11a/b/g/n   | 1.6%   | 3.14.44  | EAC775D35E |
| 14e4:4359 | 105b:e08b | Broadcom Lim... | BCM43228 802.11a/b/g/n   | 10%    | 4.1.34   | 0D43FC94FE |
| 14e4:4359 | 11ad:6603 | Broadcom Inc... | BCM43228 802.11a/b/g/n   | 8.3%   | 4.1.15   | C6F99AC92E |
| 14e4:4359 | 14e4:05e2 | Broadcom Inc... | BCM43228 802.11a/b/g/n   | 8.5%   | 3.10.42  | D58DD0D4E0 |
| 14e4:4365 | 1028:0016 | Broadcom Inc... | BCM43142 802.11b/g/n     | 3.3%   | 3.14.33  | 5913B022E4 |
| 14e4:4365 | 103c:2230 | Broadcom Inc... | BCM43142 802.11b/g/n     | 30.4%  | 3.14.44  | 9F366DE52D |
| 14e4:4365 | 103c:804a | Broadcom Inc... | BCM43142 802.11b/g/n     | 28.4%  | 4.1.15   | 86CACB02C8 |
| 14e4:4365 | 105b:e071 | Broadcom Inc... | BCM43142 802.11b/g/n     | 26.1%  | 3.14.44  | E822D548D0 |
| 14e4:4365 | 105b:e07e | Broadcom Inc... | BCM43142 802.11b/g/n     | 14.3%  | 3.14.44  | C081ADAAE3 |
| 14e4:4365 | 11ad:6605 | Broadcom Inc... | BCM43142 802.11b/g/n     | 4.3%   | 3.14.33  | 4E37AD043D |
| 14e4:4365 | 11ad:6645 | Broadcom Inc... | BCM43142 802.11b/g/n     | 22.9%  | 3.14.33  | A047328A79 |
| 14e4:4365 | 11ad:6655 | Broadcom Inc... | BCM43142 802.11b/g/n     | 86.7%  | 4.9.20   | AB3369F45C |
| 14e4:4365 | 11ad:6675 | Broadcom Lim... | BCM43142 802.11b/g/n     | 20%    | 3.14.44  | 2A224752BA |
| 14e4:4365 | 17aa:0611 | Broadcom Inc... | BCM43142 802.11b/g/n     | 5.1%   | 3.14.25  | 991CC1AF7C |
| 14e4:4365 | 17aa:0621 | Broadcom Inc... | BCM43142 802.11b/g/n     | 10%    | 3.14.25  | 5C27867F6E |
| 14e4:4365 | 1a3b:2155 | Broadcom Inc... | BCM43142 802.11b/g/n     | 100%   |          | 34BE6240D1 |
| 14e4:4365 | 1b9a:3002 | Broadcom        | BCM43142 802.11b/g/n     | 72.7%  | 4.1.25   | 6020877A68 |
| 14e4:43a0 | 1043:85df | Broadcom Inc... | BCM4360 802.11ac Wire... | 20%    | 4.15.0   | 8CE5DB772C |
| 14e4:43a0 | 1043:8659 | Broadcom Inc... | BCM4360 802.11ac Wire... | 14.3%  | 4.15.0   | 2301984979 |
| 14e4:43a0 | 106b:0117 | Broadcom Lim... | BCM4360 802.11ac Wire... | 40%    | 4.18.0   | 3A2A390F59 |
| 14e4:43ae | 17aa:0622 | Broadcom Inc... | BCM43162 802.11ac Wir... | 100%   |          | ACD1BCBBC4 |
| 14e4:43b1 | 103c:2154 | Broadcom Lim... | BCM4352 802.11ac Wire... | 100%   |          | 420C7722C6 |
| 14e4:43b1 | 1043:855c | Broadcom Inc... | BCM4352 802.11ac Wire... | 50%    | 4.15.0   | D94180D023 |
| 14e4:43b1 | 1043:85ba | Broadcom Inc... | BCM4352 802.11ac Wire... | 33.3%  | 4.18.0   | 5585935586 |
| 14e4:43b1 | 17aa:0623 | Broadcom Lim... | BCM4352 802.11ac Wire... | 25%    | 4.15.0   | FC0DC30BF0 |
| 14e4:43ba | 106b:0173 | Broadcom Inc... | BCM43602 802.11ac Wir... | 100%   |          | 6F3816ABBD |
| 14e4:4727 | 1028:0010 | Broadcom Inc... | BCM4313 802.11bgn Wir... | 5.9%   | 4.13.3   | EFC321CCD7 |
| 14e4:4727 | 1028:0012 | Broadcom Lim... | BCM4313 802.11bgn Wir... | 60%    | 4.15.0   | 40D48C06A1 |
| 14e4:4727 | 1028:0015 | Broadcom Inc... | BCM4313 802.11bgn Wir... | 20%    | 4.15.0   | 6283472778 |
| 14e4:4727 | 103c:1483 | Broadcom Inc... | BCM4313 802.11bgn Wir... | 6.2%   | 4.1.34   | EA7FCEAF2C |
| 14e4:4727 | 103c:1795 | Broadcom Inc... | BCM4313 802.11bgn Wir... | 8.3%   | 3.10.42  | 06AA196398 |
| 14e4:4727 | 105b:e042 | Broadcom Inc... | BCM4313 802.11bgn Wir... | 12.5%  | 4.15.0   | D148A20413 |
| 14e4:4727 | 144f:7175 | Broadcom Inc... | BCM4313 802.11bgn Wir... | 14.3%  | 4.15.0   | 93629DD831 |
| 14e4:4727 | 144f:7179 | Broadcom Inc... | BCM4313 802.11bgn Wir... | 4%     | 3.10.34  | A92AED714F |
| 14e4:4727 | 14e4:0510 | Broadcom Inc... | BCM4313 802.11bgn Wir... | 36.4%  | 4.2.6    | EA55AE13AC |
| 14e4:4727 | 14e4:051b | Broadcom Inc... | BCM4313 802.11bgn Wir... | 5%     | 2.6.32   | 4437DCCAB2 |
| 14e4:4727 | 14e4:0587 | Broadcom Lim... | BCM4313 802.11bgn Wir... | 28.6%  | 4.15.0   | 8D6C57DC63 |
| 14e4:4727 | 14e4:0608 | Broadcom Inc... | BCM4313 802.11bgn Wir... | 33.3%  | 4.4.0    | 65C68A39C0 |
| 14e4:4727 | 185f:051a | Broadcom Inc... | BCM4313 802.11bgn Wir... | 8.3%   | 4.9.0    | 86A1DD9578 |
| 167b:2116 | 340f:187e | ZyDAS Techno... | ZD1212B Wireless Adapter | 100%   |          | C399CBB5F3 |
| 168c:001c | 103c:137b | Qualcomm Ath... | AR242x / AR542x Wirel... | 1.8%   | 3.14.33  | 93C0EF7223 |
| 168c:002b | 103c:1461 | Qualcomm Ath... | AR9285 Wireless Netwo... | 0.9%   | 3.14.33  | F4DE983D96 |
| 168c:0032 | 11ad:6617 | Qualcomm Ath... | AR9485 Wireless Netwo... | 0.6%   | 3.14.25  | 86D2D3B0E1 |
| 168c:0032 | 11ad:6628 | Qualcomm Ath... | AR9485 Wireless Netwo... | 1.6%   | 3.14.44  | 469E04E0D5 |
| 168c:0036 | 11ad:0642 | Qualcomm Ath... | QCA9565 / AR9565 Wire... | 0.4%   | 3.10.51  | 8D6D195DA2 |
| 168c:0036 | 11ad:0803 | Qualcomm Ath... | QCA9565 / AR9565 Wire... | 1.4%   | 3.14.44  | DE4737FCF1 |
| 168c:0037 | 1a3b:1195 | Qualcomm Ath... | AR9485 Wireless Netwo... | 50%    | 4.9.20   | CE8124E5F4 |
| 168c:0037 | 1a3b:2100 | Qualcomm Ath... | AR9485 Wireless Netwo... | 3.8%   | 3.14.25  | 0F8E9B7955 |
| 168c:0042 | 11ad:0806 | Qualcomm Ath... | QCA9377 802.11ac Wire... | 23.1%  | 4.4.0    | ECB6A89DFC |
| 168c:0042 | 11ad:08a6 | Qualcomm Ath... | QCA9377 802.11ac Wire... | 0.5%   | 4.9.9    | E7395D0EE2 |
| 168c:0042 | 17aa:0901 | Qualcomm Ath... | QCA9377 802.11ac Wire... | 0.9%   | 4.9.0    | C23D0EF968 |
| 168c:0042 | 17aa:4035 | Qualcomm Ath... | QCA9377 802.11ac Wire... | 1.1%   | 4.8.0    | C3352134E9 |
| 17fe:2220 | 1468:0310 | InProComm       | IPN 2220 802.11g         | 100%   |          | E9BD04F647 |
| 1814:3062 | 1814:3062 | Ralink          | RT3062 Wireless 802.1... | 4.8%   | 3.14.44  | 9D9E2DB550 |
| 1814:3290 | 103c:18ec | Ralink          | RT3290 Wireless 802.1... | 0.3%   | 3.14.15  | 5C0BCB0583 |
| 1814:539f | 103c:1637 | Ralink          | RT5390 [802.11 b/g/n ... | 3%     | 3.14.44  | ED2FBC90A0 |
| 1814:5592 | 1043:851a | Ralink          | RT5592 PCIe Wireless ... | 100%   |          | 08D84A1FF9 |
| 1814:5592 | 1814:5592 | Ralink          | RT5592 PCIe Wireless ... | 100%   |          | 760C31A638 |
| 8086:0893 | 8086:0262 | Intel           | Centrino Wireless-N 135  | 6.5%   | 3.14.25  | 2DD89E3983 |
| 8086:08b1 | 8086:4070 | Intel           | Wireless 7260            | 0.6%   | 3.14.25  | 550460AAAC |
| 8086:08b4 | 8086:8270 | Intel           | Wireless 3160            | 3.5%   | 3.14.44  | AB6BD693BE |
| 8086:095a | 8086:5400 | Intel           | Wireless 7265            | 6.2%   | 4.1.25   | 0A99E4D896 |
| 8086:24f3 | 8086:1010 | Intel           | Wireless 8260            | 1.5%   | 4.1.15   | 43DF678BD3 |
| 8086:2526 | 8086:0014 | Intel           | Wireless-AC 9260         | 3.3%   | 4.15.0   | 7DEC6AEA64 |
| 8086:3165 | 8086:4010 | Intel           | Wireless 3165            | 0.5%   | 4.1.15   | 5738D326F6 |
| 8086:3165 | 8086:8110 | Intel           | Wireless 3165            | 4%     | 4.9.20   | 48E3CC8030 |
| 8086:3166 | 8086:4210 | Intel           | Dual Band Wireless-AC... | 1.2%   | 4.1.15   | 1B722DF896 |
| 8086:4222 | 103c:135c | Intel           | PRO/Wireless 3945ABG ... | 2.6%   | 3.14.25  | 9EDB73DD0E |
| 8086:a370 | 8086:0034 | Intel           | Wireless-AC 9560 [Jef... | 1.7%   | 4.4.0    | 039A05F3EB |

### Network (PCI)

19 out of 688 (2.76%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 0000:0002 | 002c:0000 |                 | Network controller       | 100%   |          | 3859A12973 |
| 0000:0210 | 002c:0000 |                 | Network controller       | 100%   |          | 3859A12973 |
| 0000:0210 | 1105:8300 |                 |                          | 100%   |          | 3859A12973 |
| 1006:3106 | 1086:1405 | Reply Group     | Reply Ethernet contro... | 100%   |          | F597A38FF5 |
| 10ec:c822 | 1a3b:3750 | Realtek Semi... | Realtek Network contr... | 100%   |          | 123447177A |
| 10ec:d723 | 103c:8319 | Realtek Semi... | RTL8723DE Wireless Ne... | 98.3%  | 4.9.87   | D7977A3B0E |
| 1106:1106 | 1186:1405 | VIA Technolo... | VT82C570MV               | 100%   |          | 1EF54091BE |
| 1106:3065 | 1849:3065 | VIA Technolo... | VT6102/VT6103 [Rhine-II] | 8.3%   | 3.10.0   | 05A172FBB7 |
| 1260:3886 | 16be:2004 | Intersil        | ISL3886 [Prism Javeli... | 25%    | 5.0.0    | ACACF55F1F |
| 12d0:2103 | 12d0:2103 | GDE Systems     | GDE Network controller   | 100%   |          | 8C5E6472B2 |
| 168c:004a | 15aa:4035 | Qualcomm Ath... | Network controller       | 100%   |          | 04F6BB6978 |
| 1810:3060 | 8001:0000 | HCL Technolo... | Network controller       | 100%   |          | CFD57C3B89 |
| 8086:093c | 8086:0181 | Intel           | Wireless Gigabit 1726... | 100%   |          | D33E07EEAB |
| 8086:093c | 8086:2181 | Intel           | Wireless Gigabit 1726... | 100%   |          | EE5666AC16 |
| 8086:10d3 | 8086:a01f | Intel           | 82574L Gigabit Networ... | 2.6%   | 3.10.0   | 9B75A42A1E |
| 8086:10de | 103c:3034 | Intel           | 82567LM-3 Gigabit Net... | 7.7%   | 3.14.44  | 5DC57BDE0C |
| 8086:10f0 | 1019:1324 | Intel           | 82578DC Gigabit Netwo... | 100%   |          | 50B445BA68 |
| 8086:1502 | 1043:849c | Intel           | 82579LM Gigabit Netwo... | 100%   |          | 44AA7CC920 |
| 8086:24fd | 8086:1010 | Intel           | Wireless 8265 / 8275     | 0.7%   | 4.8.15   | BF84028302 |

### Sd host controller (PCI)

28 out of 636 (4.40%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 14e4:16bc | 1025:0647 | Broadcom Inc... | BCM57765/57785 SDXC/M... | 0.2%   | 3.10.34  | 86D2D3B0E1 |
| 197b:2381 | 1025:0145 | JMicron Tech... | Standard SD Host Cont... | 50%    | 4.1.15   | C07C4BD9E0 |
| 197b:2381 | 1025:0275 | JMicron Tech... | Standard SD Host Cont... | 70%    | 4.18.0   | 09734ADC68 |
| 197b:2381 | 103c:30fc | JMicron Tech... | Standard SD Host Cont... | 75%    | 4.18.0   | 039F952C77 |
| 197b:2381 | 103c:3628 | JMicron Tech... | Standard SD Host Cont... | 3.8%   | 3.14.44  | B0C685633F |
| 197b:2381 | 1043:1a07 | JMicron Tech... | Standard SD Host Cont... | 2%     | 3.10.34  | CC09C5F6B5 |
| 197b:2381 | 1179:fd30 | JMicron Tech... | Standard SD Host Cont... | 14.3%  | 3.14.33  | 6E89AF808B |
| 197b:2381 | 1297:2020 | JMicron Tech... | Standard SD Host Cont... | 100%   |          | 95D754997A |
| 197b:2381 | 1297:2027 | JMicron Tech... | Standard SD Host Cont... | 77.8%  | 4.15.0   | 7BF56A1008 |
| 197b:2381 | 1297:2028 | JMicron Tech... | Standard SD Host Cont... | 33.3%  | 4.9.0    | 54C077FDFC |
| 197b:2381 | 1558:0801 | JMicron Tech... | Standard SD Host Cont... | 11.1%  | 4.9.20   | 0267CF3435 |
| 197b:2381 | 1558:4120 | JMicron Tech... | Standard SD Host Cont... | 50%    | 4.20.17  | 65387A2C5F |
| 197b:2381 | 17aa:3d9a | JMicron Tech... | Standard SD Host Cont... | 28.6%  | 4.1.3    | 5E896CED5E |
| 197b:2391 | 103c:1618 | JMicron Tech... | Standard SD Host Cont... | 11.1%  | 4.1.15   | 46D335AC01 |
| 197b:2391 | 103c:161c | JMicron Tech... | Standard SD Host Cont... | 11.1%  | 4.1.15   | F271B8993E |
| 197b:2391 | 103c:161d | JMicron Tech... | Standard SD Host Cont... | 66.7%  | 4.15.0   | 6385FBCA24 |
| 197b:2391 | 103c:162a | JMicron Tech... | Standard SD Host Cont... | 16.7%  | 4.15.0   | 3EED0FAF40 |
| 197b:2391 | 103c:168b | JMicron Tech... | Standard SD Host Cont... | 7.7%   | 3.14.44  | DBE13E6A5C |
| 197b:2391 | 103c:176c | JMicron Tech... | Standard SD Host Cont... | 25%    | 4.15.0   | FDBA82A5B5 |
| 197b:2391 | 103c:179b | JMicron Tech... | Standard SD Host Cont... | 15.4%  | 3.14.44  | BE19F87892 |
| 197b:2391 | 103c:17a7 | JMicron Tech... | Standard SD Host Cont... | 55.6%  | 3.14.44  | AE6CF1B3CA |
| 197b:2391 | 103c:17ab | JMicron Tech... | Standard SD Host Cont... | 13%    | 4.1.25   | 42129ED417 |
| 197b:2391 | 103c:17ed | JMicron Tech... | Standard SD Host Cont... | 10%    | 3.14.44  | 0BC7216657 |
| 197b:2391 | 103c:17f3 | JMicron Tech... | Standard SD Host Cont... | 100%   |          | B4BA23ACA0 |
| 197b:2391 | 103c:18df | JMicron Tech... | Standard SD Host Cont... | 14.3%  | 3.14.44  | BDF850308B |
| 197b:2391 | 1558:2431 | JMicron Tech... | Standard SD Host Cont... | 100%   |          | F395EB44CF |
| 197b:2391 | 1558:2450 | JMicron Tech... | Standard SD Host Cont... | 100%   |          | 450ED4C040 |
| 197b:2391 | 1558:2700 | JMicron Tech... | Standard SD Host Cont... | 100%   |          | 49A16A1DB5 |

### Sound (PCI)

92 out of 8014 (1.15%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 0045:c061 | 0045:c061 |                 | Audio device             | 100%   |          | 8D884B92FA |
| 1002:1308 | 1025:0864 | AMD             | Kaveri HDMI/DP Audio ... | 8.3%   | 3.14.44  | 8D6D195DA2 |
| 1002:1314 | 1025:0520 | AMD             | Wrestler HDMI Audio      | 6.2%   | 3.14.44  | BF118AA31C |
| 1002:4383 | 1025:0520 | AMD             | SBx00 Azalia (Intel HDA) | 6.2%   | 3.14.44  | BF118AA31C |
| 1002:4383 | 1043:836c | AMD             | SBx00 Azalia (Intel HDA) | 0.6%   | 3.14.44  | C2703245E8 |
| 1002:4383 | 1043:8445 | AMD             | SBx00 Azalia (Intel HDA) | 0.2%   | 3.13.0   | 8A4E34A210 |
| 1002:9840 | 17aa:2219 | AMD             | Kabini HDMI/DP Audio     | 50%    | 4.9.60   | 94058A82CA |
| 1002:aa38 | 1462:aa38 | AMD             | RV710/730 HDMI Audio ... | 3.6%   | 3.14.44  | 51837DE98F |
| 1002:aa38 | 174b:aa38 | AMD             | RV710/730 HDMI Audio ... | 1%     | 3.14.25  | 45FCBC8B9A |
| 1002:aa98 | 1043:aa98 | AMD             | Caicos HDMI Audio [Ra... | 1.7%   | 3.0.38   | 2A34C16AB3 |
| 1002:aa98 | 174b:aa98 | AMD             | Caicos HDMI Audio [Ra... | 0.9%   | 3.14.22  | 8A4E34A210 |
| 1002:aab0 | 103c:1990 | AMD             | Oland/Hainan/Cape Ver... | 33.3%  | 4.18.0   | DCE9CDAF8E |
| 1002:aab0 | 1043:aab0 | AMD             | Oland/Hainan/Cape Ver... | 0.7%   | 3.14.22  | CDC3F83CDB |
| 1002:aac0 | 1458:aac0 | AMD             | Tobago HDMI Audio [Ra... | 4.2%   | 3.14.44  | 62E0E97099 |
| 1022:1457 | 1849:2220 | AMD             | Family 17h (Models 00... | 16.7%  | 4.18.0   | 707960B3EC |
| 1022:2093 | 1022:2093 | AMD             | CS5536 [Geode compani... | 100%   |          | 6D9551F87E |
| 1022:780d | 1025:0864 | AMD             | FCH Azalia Controller    | 8.3%   | 3.14.44  | 8D6D195DA2 |
| 1022:780d | 1043:85cd | AMD             | FCH Azalia Controller    | 5.6%   | 3.14.44  | CDC3F83CDB |
| 1022:780d | 1043:86c7 | AMD             | FCH Azalia Controller    | 33.3%  | 4.9.14   | 71ABA86389 |
| 10de:006b | 1043:0c11 | Nvidia          | nForce Audio Processi... | 100%   |          | 543960170E |
| 10de:006b | 147b:1c00 | Nvidia          | nForce Audio Processi... | 100%   |          | CB892B4614 |
| 10de:03f0 | 1458:a002 | Nvidia          | MCP61 High Definition... | 0.5%   | 3.14.15  | 9D9E2DB550 |
| 10de:0774 | 1043:836c | Nvidia          | MCP72XE/MCP72P/MCP78U... | 7.7%   | 3.10.19  | E1B7D175A1 |
| 10de:0774 | 1462:7578 | Nvidia          | MCP72XE/MCP72P/MCP78U... | 16.7%  | 4.9.20   | 8F804041A2 |
| 10de:0be3 | 1043:8354 | Nvidia          | High Definition Audio... | 3.8%   | 3.14.44  | 67BFE1B221 |
| 10de:0be3 | 1462:8094 | Nvidia          | High Definition Audio... | 1.6%   | 3.14.44  | 895D8612B4 |
| 10de:0bea | 1462:2304 | Nvidia          | GF108 High Definition... | 9.1%   | 3.14.44  | ED9D8A148D |
| 10de:0bea | 1991:5584 | Nvidia          | GF108 High Definition... | 50%    | 4.1.34   | CE8124E5F4 |
| 10de:0bee |           | Nvidia          | GF116 High Definition... | 1.3%   | 3.14.39  | 77909796EC |
| 10de:0e08 |           | Nvidia          | GF119 HDMI Audio Cont... | 4.2%   | 3.14.33  | 8F9504F263 |
| 10de:0e0f | 3842:1731 | Nvidia          | GK208 HDMI/DP Audio C... | 100%   |          | C2703245E8 |
| 10de:0e1b | 1569:0fc6 | Nvidia          | GK107 HDMI Audio Cont... | 1.1%   | 3.14.33  | 8F804041A2 |
| 10de:0fb9 | 10de:12af | Nvidia          | GP107GL High Definiti... | 100%   |          | C11BA25134 |
| 10de:0fba | 1043:8520 | Nvidia          | GM206 High Definition... | 5.9%   | 3.14.53  | 8D2A73DD23 |
| 10de:0fba | 3842:2962 | Nvidia          | GM206 High Definition... | 100%   |          | 707960B3EC |
| 10de:10ef | 1462:360c | Nvidia          | GP102 HDMI Audio Cont... | 100%   |          | 816A1797C5 |
| 10de:10f0 | 1043:8597 | Nvidia          | GP104 High Definition... | 40%    | 4.15.0   | 32166A5865 |
| 10de:10f0 | 1558:0879 | Nvidia          | GP104 High Definition... | 50%    | 4.19.0   | A7DB7C544F |
| 10de:10f1 | 1462:3490 | Nvidia          | GP106 High Definition... | 50%    | 4.18.0   | 1B722DF896 |
| 1102:0004 | 1102:1003 | Creative Labs   | EMU10k2/CA0100/CA0102... | 16.7%  | 4.1.15   | D74C162548 |
| 1102:0004 | 1102:2002 | Creative Labs   | EMU10k2/CA0100/CA0102... | 2.6%   | 3.14.44  | 2B0A36F85F |
| 13f2:0111 |           | Ford Microel... |                          | 100%   |          | 95162A226D |
| 13f2:0111 | ffff:ffff | Ford Microel... | Multimedia audio cont... | 100%   |          | 95162A226D |
| 13f6:0111 | 153b:1144 | C-Media Elec... | CMI8738/CMI8768 PCI A... | 7.1%   | 4.1.25   | 86F297ED58 |
| 13f6:8788 | 1043:8463 | C-Media Elec... | CMI8788 [Oxygen HD Au... | 100%   |          | 9E13784BB3 |
| 13f6:8788 | 1043:8521 | C-Media Elec... | CMI8788 [Oxygen HD Au... | 2.6%   | 3.14.44  | 45FCBC8B9A |
| 13f6:8788 | 1043:855e | C-Media Elec... | CMI8788 [Oxygen HD Au... | 100%   |          | EE53639037 |
| 1412:1624 | 1412:2403 | VIA Technolo... | Multimedia audio cont... | 100%   |          | 2AF6424751 |
| 8086:0c0c | 8086:0c0c | Intel           | Xeon E3-1200 v3/4th G... | 12.5%  | 4.9.60   | 77909796EC |
| 8086:0c0c | 8086:2010 | Intel           | Xeon E3-1200 v3/4th G... | 0.2%   | 2.6.32   | A268D267B1 |
| 8086:0f04 | 1043:14dd | Intel           | Atom Processor Z36xxx... | 1.9%   | 3.14.33  | 106830C1CC |
| 8086:0f28 | 17aa:3907 | Intel           | Atom Processor Z36xxx... | 100%   |          | 6D960BD235 |
| 8086:0f28 | 8086:0f28 | Intel           | Atom Processor Z36xxx... | 100%   |          | A154D9D080 |
| 8086:0f28 | 8086:7270 | Intel           | Atom Processor Z36xxx... | 100%   |          | E5412A533C |
| 8086:160c | 1025:098a | Intel           | Broadwell-U Audio Con... | 1.3%   | 3.14.44  | 4F849E1E80 |
| 8086:160c | 17aa:390b | Intel           | Broadwell-U Audio Con... | 8.7%   | 4.9.60   | AB6BD693BE |
| 8086:1c20 | 1028:0493 | Intel           | 6 Series/C200 Series ... | 11.6%  | 3.14.33  | EFD71FBD61 |
| 8086:1c20 | 1043:8445 | Intel           | 6 Series/C200 Series ... | 0.4%   | 3.10.34  | 1678EE56C3 |
| 8086:1c20 | 1849:1892 | Intel           | 6 Series/C200 Series ... | 2.9%   | 3.10.0   | 895D8612B4 |
| 8086:1e20 | 1028:052c | Intel           | 7 Series/C216 Chipset... | 9.1%   | 4.15.0   | 29A0FC6CE0 |
| 8086:1e20 | 1297:2033 | Intel           | 7 Series/C216 Chipset... | 33.3%  | 4.9.20   | 9137B29AFE |
| 8086:1e20 | 1458:a002 | Intel           | 7 Series/C216 Chipset... | 0.7%   | 3.9.10   | 740BF21A40 |
| 8086:1e20 | 17aa:3977 | Intel           | 7 Series/C216 Chipset... | 0.4%   | 3.10.42  | 2DD89E3983 |
| 8086:1e20 | 8086:1e20 | Intel           | 7 Series/C216 Chipset... | 9.1%   | 4.1.34   | CE8124E5F4 |
| 8086:22a8 | 8086:7270 | Intel           | Atom/Celeron/Pentium ... | 100%   |          | 514C494F7F |
| 8086:266e | 103c:3006 | Intel           | 82801FB/FBM/FR/FW/FRW... | 33.3%  | 4.9.20   | 51837DE98F |
| 8086:266e | 1458:ae01 | Intel           | 82801FB/FBM/FR/FW/FRW... | 9.1%   | 3.14.44  | FD291EB728 |
| 8086:27d8 | 1019:2683 | Intel           | NM10/ICH7 Family High... | 2.9%   | 3.14.44  | EAA25586D2 |
| 8086:27d8 | 1028:0220 | Intel           | NM10/ICH7 Family High... | 9.1%   | 3.14.44  | BBA0FE2672 |
| 8086:27d8 | 1043:8290 | Intel           | NM10/ICH7 Family High... | 0.5%   | 3.14.25  | 45FCBC8B9A |
| 8086:27d8 | 1043:83d4 | Intel           | NM10/ICH7 Family High... | 1.6%   | 3.14.44  | 8807184E95 |
| 8086:27d8 | 104d:81fc | Intel           | NM10/ICH7 Family High... | 100%   |          | 7F0BB0CC92 |
| 8086:27d8 | 1458:a002 | Intel           | NM10/ICH7 Family High... | 0.2%   | 3.14.25  | D6C3BCD69B |
| 8086:27d8 | 1462:104e | Intel           | NM10/ICH7 Family High... | 20%    | 4.1.15   | 5F15F028A8 |
| 8086:27d8 | 1854:005f | Intel           | NM10/ICH7 Family High... | 100%   |          | F60C56AC42 |
| 8086:27d8 | 1b0a:0001 | Intel           | NM10/ICH7 Family High... | 7.1%   | 3.14.44  | 396BE2A324 |
| 8086:284b | 1734:1083 | Intel           | 82801H (ICH8 Family) ... | 18.2%  | 3.14.44  | BF1BADE95D |
| 8086:293e | 103c:281e | Intel           | 82801I (ICH9 Family) ... | 3.6%   | 3.14.44  | 61D1ED752A |
| 8086:293e | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 33.3%  | 3.14.44  | 93C0EF7223 |
| 8086:3b56 | 103c:3674 | Intel           | 5 Series/3400 Series ... | 25%    | 4.15.0   | F4DE983D96 |
| 8086:8c20 | 1043:143f | Intel           | 8 Series/C220 Series ... | 12.5%  | 4.9.41   | A268D267B1 |
| 8086:8c20 | 8086:8c20 | Intel           | 8 Series/C220 Series ... | 16.7%  | 4.9.124  | 77909796EC |
| 8086:8ca0 | 1462:d917 | Intel           | 9 Series Chipset Fami... | 6.2%   | 4.1.15   | 8D2A73DD23 |
| 8086:9ca0 | 1025:098a | Intel           | Wildcat Point-LP High... | 1.3%   | 3.14.44  | 4F849E1E80 |
| 8086:9ca0 | 17aa:390b | Intel           | Wildcat Point-LP High... | 8.7%   | 4.9.60   | AB6BD693BE |
| 8086:9d72 | 1028:06e6 | Intel           | 300 Series Chipset Sm... | 100%   |          | C97022A8FC |
| 8086:a170 | 103c:8257 | Intel           | 100 Series/C230 Serie... | 50%    | 4.15.0   | D079BA6F90 |
| 8086:a2f0 | 1043:8735 | Intel           | 200 Series PCH HD Audio  | 33.3%  | 4.9.95   | 816A1797C5 |
| 8086:a2f0 | 1458:a182 | Intel           | 200 Series PCH HD Audio  | 3.2%   | 3.10.0   | 1A67024C19 |
| 8086:a2f0 | 1558:0879 | Intel           | 200 Series PCH HD Audio  | 33.3%  | 4.18.0   | A7DB7C544F |
| 8086:a348 | 1028:0851 | Intel           | Cannon Lake PCH cAVS     | 100%   |          | 05D6B79D2F |
| 8086:a348 | 17aa:36e7 | Intel           | Cannon Lake PCH cAVS     | 33.3%  | 4.18.0   | 1B722DF896 |

### Storage (PCI)

47 out of 225 (20.89%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 104c:803b | 104d:81fc | Texas Instru... | PCIxx12 Flash Media C... | 100%   |          | 7F0BB0CC92 |
| 1095:3110 | 1095:7110 | Silicon Image   | SCSI storage controller  | 100%   |          | 69BD5A45B3 |
| 1106:401a | 1071:9515 | VIA Technolo... | VIA Card Reader Host ... | 100%   |          | E028F277D4 |
| 1106:401a | 17aa:3608 | VIA Technolo... | VIA Card Reader Host ... | 100%   |          | EA55AE13AC |
| 1217:7130 | 1019:300e | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 3C221F81A4 |
| 1217:7130 | 1025:010d | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 5A64D135B2 |
| 1217:7130 | 1025:011a | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 69380B60FC |
| 1217:7130 | 1025:0123 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | B127BEAD10 |
| 1217:7130 | 1025:0124 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 5AAFE28787 |
| 1217:7130 | 1025:012b | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 21509117BA |
| 1217:7130 | 1025:013c | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 77E3B20E26 |
| 1217:7130 | 1028:026f | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | D6AAC94E1F |
| 1217:7130 | 1028:0273 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | C9D61D9E11 |
| 1217:7130 | 1028:0275 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | B0314C0713 |
| 1217:7130 | 1071:8258 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 98006DB3BD |
| 1217:7130 | 107b:0696 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | E9F51C8451 |
| 1217:7130 | 10cf:13c6 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 7B7919A092 |
| 1217:7130 | 10cf:143d | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 6639C529C5 |
| 1217:7130 | 10cf:14d6 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | EEFC712947 |
| 1217:7130 | 1179:ff50 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | B6017B2145 |
| 1217:7130 | 1462:3fbb | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | FDCEAF9E02 |
| 1217:7130 | 1462:3fc1 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 278EF4A255 |
| 1217:7130 | 1462:3fe9 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 3F64CDD242 |
| 1217:7130 | 1462:3ff3 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | E6FCAC8295 |
| 1217:7130 | 1462:4327 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 59A1BF0CA5 |
| 1217:7130 | 1462:63f6 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | BA35BAD99E |
| 1217:7130 | 14ff:a003 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 6647A9CB02 |
| 1217:7130 | 1631:0188 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 856B9A1A68 |
| 1217:7130 | 1734:10c7 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | A8295DF38F |
| 1217:7130 | 17aa:3a21 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 5988593465 |
| 1217:8130 | 1025:019f | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | 806ABC807D |
| 1217:8130 | 1028:02bc | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | 20F0F865AE |
| 1217:8130 | 1028:02ea | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | EFA8CE8686 |
| 1217:8130 | 1028:02eb | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | 77B6FABE29 |
| 1217:8130 | 10cf:1568 | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | C2AA02F6B3 |
| 1217:8130 | 1179:ff50 | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | 34905CB301 |
| 1217:8231 | 1028:0493 | O2 Micro        | O2Micro Integrated MS... | 100%   |          | CA6EFEBBD7 |
| 1217:8231 | 1028:04a9 | O2 Micro        | O2Micro Integrated MS... | 100%   |          | 79B2A2D980 |
| 1217:8330 | 1028:04a3 | O2 Micro        | OZ600 MS/xD Controller   | 100%   |          | 19E1CA5871 |
| 1217:8330 | 1028:04a4 | O2 Micro        | OZ600 MS/xD Controller   | 100%   |          | 370EF78297 |
| 1217:8331 | 1028:0494 | O2 Micro        | O2 Flash Memory Card     | 100%   |          | 31F0876A89 |
| 1217:8331 | 1028:049a | O2 Micro        | O2 Flash Memory Card     | 100%   |          | 5D67AE99E3 |
| 1217:8331 | 1028:049b | O2 Micro        | O2 Flash Memory Card     | 100%   |          | 26DE378A54 |
| 1b85:1221 | 1b85:1221 | OCZ Technolo... | OCZ 12xx SCSI Controller | 100%   |          | 323982480D |
| 9004:7178 |           | Adaptec         | AIC-7870P/7871 [AHA-2... | 33.3%  | 3.14.44  | 87BEA4712A |
| ace1:0005 | ace1:0005 |                 | Storage controller       | 100%   |          | 22F215C605 |
| ace1:0006 | ace1:0006 |                 | Storage controller       | 100%   |          | EF20304D33 |

### Storage/ata (PCI)

2 out of 3602 (0.06%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 11ab:6141 | 1043:81d6 | Marvell Tech... | 88SE614x SATA II PCI-... | 100%   |          | 12AE1A5665 |
| 8086:2929 | 103c:306b | Intel           | 82801IBM/IEM (ICH9M/I... | 33.3%  | 3.14.44  | 93C0EF7223 |

### Storage/raid (PCI)

7 out of 460 (1.52%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1022:43bd | 1b21:1062 | AMD             | FCH RAID Controller      | 100%   |          | 2ED5B5AFC5 |
| 1028:0016 | 1028:1f24 | Dell            | PowerEdge Expandable ... | 100%   |          | 389DD308F7 |
| 103c:193f | 103c:3381 | Hewlett-Packard | Dynamic Smart Array B... | 100%   |          | 4825C12F7D |
| 1095:1114 | 1095:5114 | Silicon Image   | RAID bus controller      | 100%   |          | 126A2B0E4F |
| 1103:2840 | 1103:0000 | HighPoint Te... | RAID bus controller      | 100%   |          | 7653740066 |
| 1590:0045 | 1590:0045 | Hewlett-Packard | RAID bus controller      | 100%   |          | 3FAC52AF81 |
| 6883:0dd4 | 6883:0dd4 |                 | RAID bus controller      | 100%   |          | 7211932892 |

### System peripheral (PCI)

109 out of 617 (17.67%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 0e11:b203 | 103c:3305 | Compaq Computer | Integrated Lights Out... | 71.4%  | 4.9.60   | 6806624961 |
| 103c:3306 | 103c:3309 | Hewlett-Packard | Integrated Lights-Out... | 75%    | 2.6.32   | 179B0500B3 |
| 103c:3306 | 103c:3381 | Hewlett-Packard | Integrated Lights-Out... | 51.2%  | 2.6.32   | 140DAF886E |
| 104c:8201 | 103c:08b0 | Texas Instru... | PCI1620 Firmware Load... | 100%   |          | 316E375A5C |
| 104c:8204 | 1028:0139 | Texas Instru... | PCI7410/7510/7610 PCI... | 100%   |          | 0504CC20A9 |
| 104c:8204 | 1028:014e | Texas Instru... | PCI7410/7510/7610 PCI... | 100%   |          | 0493B906A1 |
| 1179:0805 | 1179:0001 | Toshiba Amer... | SD TypA Controller       | 50%    | 4.1.34   | 6ED70A9B46 |
| 1180:0576 | 10cf:1256 | Ricoh           | R5C576 SD Bus Host Ad... | 100%   |          | 4DCFB332DF |
| 1180:0592 | 17aa:20ca | Ricoh           | R5C592 Memory Stick B... | 2.9%   | 3.14.25  | 81A4DA9481 |
| 1180:0852 | 1043:1877 | Ricoh           | xD-Picture Card Contr... | 3.8%   | 3.0.28   | 70CC866946 |
| 1180:0852 | 1734:10ad | Ricoh           | xD-Picture Card Contr... | 16.7%  | 4.1.33   | D6BC4ADE36 |
| 1180:0852 | 17aa:20cb | Ricoh           | xD-Picture Card Contr... | 2.9%   | 3.14.25  | 81A4DA9481 |
| 1180:e230 | 1028:02bd | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 31D62139B3 |
| 1180:e230 | 1028:02fe | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 4DA3A91131 |
| 1180:e230 | 1028:0401 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 6006F3386E |
| 1180:e230 | 1028:0402 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 9E4109323B |
| 1180:e230 | 1028:0413 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | A3F3EB5872 |
| 1180:e230 | 1028:0442 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 459C56742E |
| 1180:e230 | 103c:1455 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 1B076B60C5 |
| 1180:e230 | 103c:146d | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 801F83247C |
| 1180:e230 | 103c:1471 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 435433694F |
| 1180:e230 | 103c:1722 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 3E6CC68DC2 |
| 1180:e230 | 103c:1726 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 759D141031 |
| 1180:e230 | 103c:307e | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 943AE873F7 |
| 1180:e230 | 104d:905a | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | EB4E58C4D9 |
| 1180:e230 | 104d:9060 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 2628EBE1BB |
| 1180:e230 | 104d:9066 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | A11EA53B6C |
| 1180:e230 | 104d:9067 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 7412A9035D |
| 1180:e230 | 104d:9069 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 94C60C4371 |
| 1180:e230 | 104d:9071 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 3C5767E938 |
| 1180:e230 | 104d:9072 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | DA9CBAC74B |
| 1180:e230 | 104d:907a | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 195F0109A8 |
| 1180:e230 | 1179:0001 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 9F5E64A19A |
| 1180:e230 | 1179:ff1e | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 725958F861 |
| 1180:e230 | 1179:ff40 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | A5D1F93E9C |
| 1180:e230 | 17aa:2134 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | DA5E944C6C |
| 1180:e232 | 104d:907e | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 265BA34E71 |
| 1180:e232 | 104d:9081 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | ED39416136 |
| 1180:e232 | 104d:9083 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | DE93F78B0C |
| 1180:e232 | 104d:9086 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | C1F9CF2BE3 |
| 1180:e232 | 104d:9089 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 56C1A2EF9B |
| 1180:e232 | 104d:908e | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 59BB8EC907 |
| 1180:e232 | 104d:9095 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 3F62942EFE |
| 1180:e232 | 104d:9097 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 7685534B8E |
| 1180:e232 | 1179:0001 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 4398E73607 |
| 1217:7110 | 10cf:11c4 | O2 Micro        | OZ711Mx 4-in-1 Memory... | 100%   |          | EA732BEA27 |
| 14e4:16be | 1025:0500 | Broadcom Inc... | BCM57765/57785 MS Car... | 100%   |          | 481B67D08F |
| 14e4:16be | 1025:0504 | Broadcom Inc... | BCM57765/57785 MS Car... | 100%   |          | 8579BA1B16 |
| 14e4:16be | 1025:0599 | Broadcom Lim... | BCM57765/57785 MS Car... | 100%   |          | 593ECA45A2 |
| 14e4:16be | 1025:0605 | Broadcom Lim... | BCM57765/57785 MS Car... | 100%   |          | 4BBB490EBC |
| 14e4:16be | 1025:0647 | Broadcom Inc... | BCM57765/57785 MS Car... | 100%   |          | E67DFC255A |
| 14e4:16bf | 1025:0500 | Broadcom Inc... | BCM57765/57785 xD-Pic... | 100%   |          | 481B67D08F |
| 14e4:16bf | 1025:0504 | Broadcom Inc... | BCM57765/57785 xD-Pic... | 100%   |          | 8579BA1B16 |
| 14e4:16bf | 1025:0599 | Broadcom Lim... | BCM57765/57785 xD-Pic... | 100%   |          | 593ECA45A2 |
| 14e4:16bf | 1025:0605 | Broadcom Lim... | BCM57765/57785 xD-Pic... | 100%   |          | 4BBB490EBC |
| 14e4:16bf | 1025:0647 | Broadcom Inc... | BCM57765/57785 xD-Pic... | 100%   |          | E67DFC255A |
| 197b:2382 | 1297:2020 | JMicron Tech... | SD/MMC Host Controller   | 33.3%  | 4.15.0   | D826611187 |
| 197b:2384 | 1019:2238 | JMicron Tech... | xD Host Controller       | 100%   |          | 7E782321C8 |
| 197b:2384 | 1025:0128 | JMicron Tech... | xD Host Controller       | 100%   |          | EA94093CD5 |
| 197b:2384 | 1025:013b | JMicron Tech... | xD Host Controller       | 100%   |          | 3C347BEC2E |
| 197b:2384 | 1025:013d | JMicron Tech... | xD Host Controller       | 100%   |          | C57DDB8581 |
| 197b:2384 | 1025:013e | JMicron Tech... | xD Host Controller       | 100%   |          | B563FF6430 |
| 197b:2384 | 1025:0142 | JMicron Tech... | xD Host Controller       | 100%   |          | 884C33EE98 |
| 197b:2384 | 1025:0143 | JMicron Tech... | xD Host Controller       | 100%   |          | 310A169187 |
| 197b:2384 | 1025:0145 | JMicron Tech... | xD Host Controller       | 100%   |          | 542B22772F |
| 197b:2384 | 1025:0146 | JMicron Tech... | xD Host Controller       | 100%   |          | 2D9126A5BF |
| 197b:2384 | 1025:015b | JMicron Tech... | xD Host Controller       | 100%   |          | 75927BE93C |
| 197b:2384 | 1025:0160 | JMicron Tech... | xD Host Controller       | 100%   |          | BBCDDB4D27 |
| 197b:2384 | 1025:0200 | JMicron Tech... | xD Host Controller       | 100%   |          | 454098B840 |
| 197b:2384 | 1025:0260 | JMicron Tech... | xD Host Controller       | 100%   |          | 0D5E0790A7 |
| 197b:2384 | 1025:042f | JMicron Tech... | xD Host Controller       | 100%   |          | 1395FA2E0F |
| 197b:2384 | 103c:2aa2 | JMicron Tech... | xD Host Controller       | 100%   |          | D8AA06CBF6 |
| 197b:2384 | 103c:2aa6 | JMicron Tech... | xD Host Controller       | 100%   |          | 45542209AF |
| 197b:2384 | 103c:30f4 | JMicron Tech... | xD Host Controller       | 100%   |          | DDA054B15D |
| 197b:2384 | 103c:30f7 | JMicron Tech... | xD Host Controller       | 100%   |          | 5A1D10C2E8 |
| 197b:2384 | 103c:30fb | JMicron Tech... | xD Host Controller       | 100%   |          | 762D293955 |
| 197b:2384 | 103c:30fc | JMicron Tech... | xD Host Controller       | 100%   |          | F3A761814C |
| 197b:2384 | 103c:3600 | JMicron Tech... | xD Host Controller       | 100%   |          | 3F857E2920 |
| 197b:2384 | 103c:3603 | JMicron Tech... | xD Host Controller       | 100%   |          | 9CE29D0583 |
| 197b:2384 | 103c:361b | JMicron Tech... | xD Host Controller       | 100%   |          | 500C2BCFBC |
| 197b:2384 | 103c:3624 | JMicron Tech... | xD Host Controller       | 100%   |          | 167B3FD913 |
| 197b:2384 | 103c:3628 | JMicron Tech... | xD Host Controller       | 100%   |          | E09686C315 |
| 197b:2384 | 103c:363e | JMicron Tech... | xD Host Controller       | 100%   |          | A9E05596D5 |
| 197b:2384 | 103c:3659 | JMicron Tech... | xD Host Controller       | 100%   |          | AFAAE2AA59 |
| 197b:2384 | 103c:7001 | JMicron Tech... | xD Host Controller       | 100%   |          | 2D49142FA9 |
| 197b:2384 | 103c:7010 | JMicron Tech... | xD Host Controller       | 100%   |          | 6E70B36184 |
| 197b:2384 | 1043:1a07 | JMicron Tech... | xD Host Controller       | 100%   |          | F47F34752E |
| 197b:2384 | 1179:fd30 | JMicron Tech... | xD Host Controller       | 100%   |          | 6C04009832 |
| 197b:2384 | 1179:fdb0 | JMicron Tech... | xD Host Controller       | 100%   |          | 3BF39D603E |
| 197b:2384 | 1179:ff02 | JMicron Tech... | xD Host Controller       | 100%   |          | EE66F4DDC1 |
| 197b:2384 | 1179:ff08 | JMicron Tech... | xD Host Controller       | 100%   |          | 97D9353E2A |
| 197b:2384 | 1462:100f | JMicron Tech... | xD Host Controller       | 100%   |          | 9FEC6C5DE7 |
| 197b:2384 | 1462:6520 | JMicron Tech... | xD Host Controller       | 100%   |          | 12132D4EBD |
| 197b:2384 | 152d:0834 | JMicron Tech... | xD Host Controller       | 100%   |          | C6D0242C42 |
| 197b:2384 | 1558:0803 | JMicron Tech... | xD Host Controller       | 100%   |          | F5F1021D04 |
| 197b:2384 | 1558:0806 | JMicron Tech... | xD Host Controller       | 100%   |          | F3BF4D62C0 |
| 197b:2384 | 1734:113d | JMicron Tech... | xD Host Controller       | 100%   |          | BD5D293529 |
| 197b:2384 | 1734:113f | JMicron Tech... | xD Host Controller       | 100%   |          | 93C1102EAE |
| 197b:2384 | 17aa:2130 | JMicron Tech... | xD Host Controller       | 100%   |          | 2AFD83B0D3 |
| 197b:2384 | 17aa:3602 | JMicron Tech... | xD Host Controller       | 100%   |          | 55C2F8E26B |
| 197b:2384 | 17aa:3881 | JMicron Tech... | xD Host Controller       | 100%   |          | 7F669E0390 |
| 197b:2387 | 17aa:3921 | JMicron Tech... | SD/MMC Host Controller   | 100%   |          | 57733D4AEE |
| 197b:2389 | 17aa:3924 | JMicron Tech... | xD Host Controller       | 100%   |          | 57733D4AEE |
| 197b:2394 | 1028:0446 | JMicron Tech... | xD Host Controller       | 100%   |          | 3C558B4510 |
| 197b:2394 | 103c:2ac6 | JMicron Tech... | xD Host Controller       | 100%   |          | 461345008C |
| 197b:2394 | 1179:fc30 | JMicron Tech... | xD Host Controller       | 100%   |          | D9FC00D39E |
| 197b:2394 | 1462:107f | JMicron Tech... | xD Host Controller       | 100%   |          | 4D22D14A1D |
| 197b:2394 | 17aa:3976 | JMicron Tech... | xD Host Controller       | 100%   |          | DF1A1447C6 |
| 197b:2394 | 17aa:3977 | JMicron Tech... | xD Host Controller       | 100%   |          | 8C427755B7 |

### Tv card (PCI)

2 out of 231 (0.87%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 11de:6057 | 1031:7efe | Zoran           | ZR36057PQC Video cutt... | 14.3%  | 3.14.44  | BEB1083A7F |
| 11de:6057 | 1031:d801 | Zoran           | ZR36057PQC Video cutt... | 100%   |          | F700FF20C6 |

### Usb controller (PCI)

33 out of 14085 (0.23%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1002:4397 | 1458:5004 | AMD             | SB7x0/SB8x0/SB9x0 USB... | 0.1%   | 3.10.0   | 0533339E4E |
| 1002:4399 | 1458:5004 | AMD             | SB7x0/SB8x0/SB9x0 USB... | 0.1%   | 3.10.0   | 0533339E4E |
| 1022:7807 | 1458:5004 | AMD             | FCH USB OHCI Controller  | 0.3%   | 3.14.25  | FA543553EC |
| 1022:7809 | 1458:5004 | AMD             | FCH USB OHCI Controller  | 0.3%   | 3.14.25  | FA543553EC |
| 104c:8241 | 103c:2ada | Texas Instru... | TUSB73x0 SuperSpeed U... | 50%    | 4.15.0   | 3BB5A2AB3E |
| 1106:3104 | 1106:3104 | VIA Technolo... | USB 2.0                  | 1.9%   | 3.14.22  | F3D97660A0 |
| 1106:3104 | 1106:318a | VIA Technolo... | USB 2.0                  | 20%    | 4.1.25   | E56DD30CA2 |
| 1106:3483 | 1458:5007 | VIA Technolo... | VL805 USB 3.0 Host Co... | 5.8%   | 3.10.0   | 327D1FD20C |
| 1912:0014 | 103c:1996 | Renesas Tech... | uPD720201 USB 3.0 Hos... | 4.8%   | 4.4.4    | 7CF6D970EC |
| 1912:0014 | 1912:0014 | Renesas Tech... | uPD720201 USB 3.0 Hos... | 4.8%   | 4.1.15   | E3CF1A821F |
| 1912:0015 |           | Renesas Tech... | uPD720202 USB 3.0 Hos... | 10%    | 3.14.25  | 740FC92339 |
| 1b21:1042 | 1043:1059 | ASMedia Tech... | ASM1042 SuperSpeed US... | 0.4%   | 3.10.34  | 6C9107BCAD |
| 1b21:1042 | 1043:8488 | ASMedia Tech... | ASM1042 SuperSpeed US... | 0.1%   | 3.10.34  | 9DB86FFBF1 |
| 1b21:1042 | 1849:1042 | ASMedia Tech... | ASM1042 SuperSpeed US... | 1.7%   | 3.10.0   | F88D5A4221 |
| 8086:1e31 | 1043:1447 | Intel           | 7 Series/C210 Series ... | 9.1%   | 3.14.44  | F23B5BF0DA |
| 8086:1e31 | 104d:9095 | Intel           | 7 Series/C210 Series ... | 7.1%   | 3.14.25  | 2A2BD0A648 |
| 8086:22b7 | 8086:7270 | Intel           | USB Synopsys Controller  | 12.9%  | 4.9.9    | 19F89F5D4E |
| 8086:2934 | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 33.3%  | 3.14.44  | 93C0EF7223 |
| 8086:2935 | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 33.3%  | 3.14.44  | 93C0EF7223 |
| 8086:2936 | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 33.3%  | 3.14.44  | 93C0EF7223 |
| 8086:2937 | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 33.3%  | 3.14.44  | 93C0EF7223 |
| 8086:2938 | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 33.3%  | 3.14.44  | 93C0EF7223 |
| 8086:2939 | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 33.3%  | 3.14.44  | 93C0EF7223 |
| 8086:293a | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 33.3%  | 3.14.44  | 93C0EF7223 |
| 8086:293c | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 33.3%  | 3.14.44  | 93C0EF7223 |
| 8086:3b36 | 8086:7270 | Intel           | 5 Series/3400 Series ... | 72.2%  | 3.14.44  | 2458B122E5 |
| 8086:3b3b | 8086:7270 | Intel           | 5 Series/3400 Series ... | 72.2%  | 3.14.44  | 2458B122E5 |
| 8086:8c31 | 8086:204a | Intel           | 8 Series/C220 Series ... | 12.5%  | 4.1.25   | 8C48173C7B |
| 8086:8d26 | 1043:8600 | Intel           | C610/X99 series chips... | 2.4%   | 4.1.25   | CCA78B29D4 |
| 8086:8d2d | 1043:8600 | Intel           | C610/X99 series chips... | 2.4%   | 4.1.25   | CCA78B29D4 |
| 8086:9ca6 | 1025:098a | Intel           | Wildcat Point-LP USB ... | 1.3%   | 3.14.44  | DE4737FCF1 |
| 8086:9cb1 | 103c:806c | Intel           | Wildcat Point-LP USB ... | 100%   |          | 462F2D5347 |
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

6 out of 63 (9.52%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 046d:0a0b | Logitech        | ClearChat Pro USB        | 50%    | 4.18.0   | 56D5984A14 |
| 0644:8030 | TEAC            | US-1800                  | 100%   |          | 75C7FE6B69 |
| 0763:201a | M-Audio         | M-Audio Micro            | 100%   |          | 4AFB8F7991 |
| 0955:7002 | Nvidia          | stereo controller        | 100%   |          | A1B30D6B32 |
| 1235:8016 | Focusrite-No... | Focusrite Scarlett 2i2   | 50%    | 4.9.20   | F16ADBF7F3 |
| b58e:0005 | Blue Microph... |                          | 50%    | 5.0.0    | A588768A6C |

### Bluetooth (USB)

23 out of 320 (7.19%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 044e:300c | Alps Electric   | Bluetooth Controller ... | 11.1%  | 4.1.15   | 7F0BB0CC92 |
| 0489:e036 | Foxconn / Ho... | Bluetooth USB Host Co... | 0.9%   | 3.0.28   | 69F933DD8C |
| 0489:e069 | Foxconn / Ho... | BT                       | 97.1%  | 4.9.41   | 91D9C778CB |
| 04ca:2006 | Lite-On Tech... | BCM43142A0 Bluetooth ... | 8.5%   | 4.0.8    | 805C7CD772 |
| 04ca:2007 | Lite-On Tech... | Broadcom BCM43142A0 B... | 10.5%  | 4.1.7    | BAA62D56E7 |
| 04ca:2009 | Lite-On Tech... | BCM43142A0               | 12.9%  | 4.0.2    | 14539CFCC1 |
| 04ca:300b | Lite-On Tech... | Lite-On Bluetooth Device | 0.3%   | 3.10.51  | 8D6D195DA2 |
| 04ca:3014 | Lite-On Tech... | Qualcomm Atheros Blue... | 7.8%   | 4.1.25   | 770C1DB77C |
| 05ac:8215 | Apple           | Built-in Bluetooth 2.... | 2.4%   | 3.14.44  | D5C9D589F2 |
| 05e1:0100 | Syntek          | 802.11g + Bluetooth W... | 100%   |          | 132B7E93A3 |
| 0cf3:3004 | Qualcomm Ath... | AR3012 Bluetooth 4.0     | 0.5%   | 3.10.51  | 46D4B91CF0 |
| 0cf3:3005 | Qualcomm Ath... | AR3011 Bluetooth         | 0.1%   | 3.10.34  | F4DE983D96 |
| 0cf3:3008 | Qualcomm Ath... | Bluetooth (AR3011)       | 1.9%   | 3.14.25  | F430167968 |
| 0cf3:e005 | Qualcomm Ath... | Qualcomm Atheros Blue... | 3.9%   | 3.14.44  | BB521FFE81 |
| 0e8d:763e | MediaTek        | MT7630e Bluetooth Ada... | 100%   |          | A7E6CBC45B |
| 105b:e065 | Foxconn Inte... | BCM43142A0 Bluetooth ... | 15.7%  | 4.0.1    | F39685A972 |
| 13d3:3392 | IMC Networks    | Azurewave 43228+20702... | 100%   |          | 337156D639 |
| 413c:8143 | Dell            | BCM20702A0               | 85.7%  | 4.15.0   | AE4C0F8B6B |
| 8087:07da | Intel           | Bluetooth Device         | 0.3%   | 3.9.10   | 2DD89E3983 |
| 8087:07dc | Intel           | Bluetooth Device         | 0.4%   | 3.10.0   | AB6BD693BE |
| 8087:0a2a | Intel           | Bluetooth Device         | 0.3%   | 3.14.44  | 1B722DF896 |
| 8087:0a2b | Intel           | Bluetooth Device         | 0.1%   | 3.10.0   | 4438A85B31 |
| 8087:0aaa | Intel           | Bluetooth Device 9460... | 1.5%   | 4.1.25   | 039A05F3EB |

### Camera (USB)

53 out of 1825 (2.90%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0402:5603 | ALi             | M5603 Video Camera Co... | 100%   |          | 775945A948 |
| 041e:400d | Creative Tec... | Webcam PD1001            | 100%   |          | 1892C5C88C |
| 041e:4039 | Creative Tec... | Webcam Live! Effects     | 100%   |          | EB3A6BB1E4 |
| 0458:702a | KYE Systems ... | WebCAM USB2.0            | 100%   |          | 3D86369A82 |
| 045e:0a00 | Microsoft       | Lumia 950 Dual SIM (R... | 100%   |          | 490B159371 |
| 046d:09a4 | Logitech        | QuickCam E 3500          | 9.1%   | 3.14.39  | 74709A1A7B |
| 04ca:707f | Lite-On Tech... | HP Wide Vision HD Camera | 4.3%   | 4.4.0    | 06EE78EE4D |
| 04f2:b270 | Chicony Elec... | HP HD Webcam [Fixed]     | 5%     | 3.14.44  | C6E683B39B |
| 04f2:b315 | Chicony Elec... | Integrated Camera        | 20%    | 3.14.53  | B7014678B5 |
| 04f2:b374 | Chicony Elec... | HD WebCam                | 0.8%   | 3.14.44  | 86D2D3B0E1 |
| 04f2:b3b2 | Chicony Elec... | TOSHIBA Web Camera - FHD | 100%   |          | 550460AAAC |
| 04f2:b40e | Chicony Elec... | HP Truevision HD camera  | 2.7%   | 3.14.25  | 9596ECB170 |
| 04f2:b45a | Chicony Elec... | USB2.0 FHD Camera        | 11.1%  | 3.14.44  | 78D39E18EF |
| 04f2:b5f7 | Chicony Elec... | HD WebCam                | 2%     | 4.9.20   | 51AC6D49F9 |
| 04f2:b614 | Chicony Elec... | Integrated Camera        | 50%    | 5.1.15   | 4438A85B31 |
| 04f2:b615 | Chicony Elec... | Integrated IR Camera     | 50%    | 5.1.15   | 4438A85B31 |
| 0547:6512 | Anchor Chips    | UCMOS05100KPA Microsc... | 100%   |          | 93BF2F1F49 |
| 058f:a001 | Alcor Micro     | HP Webcam-101            | 2.7%   | 3.14.44  | F4DE983D96 |
| 05ac:8501 | Apple           | Built-in iSight [Micron] | 80%    | 4.19.52  | 6A774ADE41 |
| 05c8:03ab | Cheng Uei Pr... | HP Wide Vision HD Camera | 40%    | 4.9.60   | 142D7492C2 |
| 05ca:1810 | Ricoh           | Pavilion Webcam [R5U870] | 6.7%   | 4.1.15   | 92CD40AFAD |
| 05ca:1830 | Ricoh           | Visual Communication ... | 100%   |          | 50E5B9D6CA |
| 05ca:183a | Ricoh           | Visual Communication ... | 6.2%   | 3.14.44  | 3284C77676 |
| 05ca:1870 | Ricoh           | Webcam 1000              | 100%   |          | FB7F51216E |
| 093a:7011 | Pixart Imaging  | Digital Wireless Camera  | 100%   |          | F8FD891B32 |
| 0ac8:3420 | Z-Star Micro... | Venus USB2.0 Camera      | 0.2%   | 3.14.15  | CDC3F83CDB |
| 0ac8:3450 | Z-Star Micro... | Vimicro USB Camera (A... | 0.4%   | 3.14.22  | 3C44204AA0 |
| 0ac8:c326 | Z-Star Micro... | Namuga 1.3M Webcam       | 10%    | 4.1.15   | 3AD0FF0E13 |
| 0ac8:c40a | Z-Star Micro... | A4 TECH USB2.0 PC Cam... | 0.3%   | 3.10.34  | B2C845B843 |
| 0b05:200b | ASUSTek Comp... | ASUS_Z00VD               | 100%   |          | EDFAB941DF |
| 0b97:8381 | O2 Micro        | Mini S USB2.0 Camera     | 100%   |          | 26DC6B85FE |
| 0bda:564b | Realtek Semi... | WebCamera                | 100%   |          | 5EA0111CED |
| 0bda:58be | Realtek Semi... | Laptop_Integrated_Web... | 8.3%   | 4.1.15   | A7211B4E35 |
| 0c45:6350 | Microdia        | USB 2.0 Camera           | 100%   |          | 34DDCDDC0E |
| 0c45:6369 | Microdia        |                          | 100%   |          | B20E10B246 |
| 0c45:64d2 | Microdia        | Integrated Webcam        | 9.1%   | 4.9.60   | CE392DF9C0 |
| 0e8d:200b | MediaTek        | Power                    | 100%   |          | F2CD8A3FFB |
| 13d3:5727 | IMC Networks    | Lenovo EasyCamera        | 7.7%   | 4.1.15   | AB6BD693BE |
| 13d3:5a01 | IMC Networks    | USB2.0 VGA UVC WebCam    | 0.5%   | 4.9.9    | 3923D18587 |
| 174f:114f | Syntek          | Lenovo EasyCamera        | 16.7%  | 3.14.44  | 2DD89E3983 |
| 174f:5a35 | Syntek          | Sonix 1.3MPixel USB 2... | 2%     | 3.14.33  | 0A87DE5887 |
| 174f:6a33 | Syntek          | Web Cam - Asus F3SA, ... | 100%   |          | 800F54CA3A |
| 174f:6a51 | Syntek          | 2.0MPixel Web Cam - A... | 100%   |          | 39E3030E0A |
| 1782:4011 | Spreadtrum C... | Android                  | 100%   |          | 9869646781 |
| 18ec:3399 | Arkmicro Tec... | USB2.0 PC CAMERA         | 0.8%   | 3.14.25  | 9D9E2DB550 |
| 1b17:6111 | DarkHorse .     | USB2.0 Web Camera        | 100%   |          | 6E9BA31D2B |
| 1bcf:2c6e | Sunplus Inno... | HD WebCam                | 3.2%   | 3.14.25  | 8D6D195DA2 |
| 1bcf:2c87 | Sunplus Inno... | HP Wide Vision HD        | 7.7%   | 4.9.20   | 7BD53B3FFB |
| 2104:0124 | Tobii Techno... | EyeChip                  | 10%    | 4.9.60   | ACA7993158 |
| 2717:ff10 | Android         | Android                  | 100%   |          | D633DC9722 |
| 2970:4011 | Fly             | Life Jet                 | 100%   |          | 0C91AAB0FF |
| 5986:1141 | Acer            | Integrated IR Camera     | 16.7%  | 4.18.0   | 6A667C9BA7 |
| 5986:2113 | Acer            | Integrated Camera        | 4.3%   | 4.13.0   | 6A667C9BA7 |

### Card reader (USB)

8 out of 13 (61.54%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0b0c:003f | Todos AB        | Todos C400 smartcard ... | 100%   |          | 251D958CA9 |
| 0bda:0129 | Realtek Semi... | RTS5129 Card Reader C... | 0.1%   | 3.8.0    | 9ED6957C8B |
| 0bda:0139 | Realtek Semi... | RTS5139 Card Reader C... | 0.2%   | 3.10.34  | EF015B9C0F |
| 0bda:0150 | Realtek Semi... | USB 2.0 Card Reader      | 100%   |          | 3C44204AA0 |
| 0c4b:0500 | Reiner SCT K... | cyberJack RFID standa... | 83.3%  | 4.4.4    | 2F2703FBEB |
| 0c4b:0501 | Reiner SCT K... | cyberJack RFID comfor... | 100%   |          | 37BE65DDB4 |
| 0ca6:0010 | Castles Tech... | EZUSB PC/SC Smart Car... | 100%   |          | 21FB8F59A4 |
| 0d8c:5200 | C-Media Elec... | Mass Storage Controll... | 100%   |          | 38C8446DA8 |

### Chipcard (USB)

39 out of 45 (86.67%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0403:e3b4 | Future Techn... | Parsec Desktop Reader... | 100%   |          | 775160993D |
| 048d:1365 | Integrated T... | SmartCard Reader         | 100%   |          | DB4B891E15 |
| 04e6:5116 | SCM Microsys... | SCR331-LC1 / SCR3310 ... | 100%   |          | B511052CC4 |
| 04e6:e001 | SCM Microsys... | SCR331 SmartCard Reader  | 100%   |          | D3D8B39015 |
| 0529:0620 | Aladdin Know... | Token JC                 | 93.3%  | 3.14.25  | 0CFA900AB7 |
| 058f:9520 | Alcor Micro     | EMV Certified Smart C... | 93.8%  | 4.15.0   | 936BEEBE68 |
| 058f:9540 | Alcor Micro     | AU9540 Smartcard Reader  | 97.3%  | 4.13.0   | 0F9287651D |
| 072f:90cc | Advanced Car... | ACR38 SmartCard Reader   | 35.3%  | 4.18.0   | 7F0F347502 |
| 072f:90de | Advanced Car... | Token USB 64K            | 33.3%  | 4.1.25   | A8A89AC09A |
| 072f:b000 | Advanced Car... | ACR3901U                 | 100%   |          | A44B651190 |
| 076b:1021 | OmniKey         | CardMan 1021             | 71.4%  | 4.15.0   | 3D9E77AE8A |
| 076b:3021 | OmniKey         | CardMan 3121             | 50%    | 3.14.33  | B45F44A0F7 |
| 076b:4321 | OmniKey         | CardMan 4321             | 100%   |          | 3191678465 |
| 076b:5421 | OmniKey         | Smart Card Reader USB    | 100%   |          | EE4E49C4A1 |
| 08e6:3437 | Gemalto (was... | GemPC Twin SmartCard ... | 100%   |          | BB385761F8 |
| 08e6:3438 | Gemalto (was... | GemPC Key SmartCard R... | 100%   |          | 6BDD8BE020 |
| 08e6:34ec | Gemalto (was... | Compact Smart Card Re... | 93.3%  | 4.15.0   | 85B9549CFF |
| 0a5c:5800 | Broadcom        | BCM5880 Secure Applic... | 99.2%  | 3.10.36  | CA6EFEBBD7 |
| 0a5c:5801 | Broadcom        | BCM5880 Secure Applic... | 99.3%  | 3.16.7   | FFEF7E12D0 |
| 0a5c:5802 | Broadcom        | BCM5880 Secure Applic... | 100%   |          | 4D67416D5E |
| 0a5c:5804 | Broadcom        | BCM5880 Secure Applic... | 100%   |          | 4926835893 |
| 0a5c:5805 | Broadcom        | 5880                     | 100%   |          | 5E0DC6DFA3 |
| 0a5c:5832 | Broadcom        | 5880                     | 97.1%  | 4.15.0   | B9281326D7 |
| 0a5c:5834 | Broadcom        | 5880                     | 90%    | 3.10.0   | 90E9F8DFAD |
| 0a5c:5842 | Broadcom        | 58200                    | 100%   |          | 8FB4429DD6 |
| 0a89:0025 | Aktiv           | Rutoken lite             | 50%    | 4.1.25   | 8FA80B8A39 |
| 0b97:7762 | O2 Micro        | Oz776 SmartCard Reader   | 100%   |          | BF8ACC676E |
| 0b97:7772 | O2 Micro        | OZ776 CCID Smartcard ... | 96.5%  | 4.15.0   | F40C3D18FB |
| 0bda:0165 | Realtek Semi... | Smart Card Reader Int... | 100%   |          | 7B99FD4C95 |
| 0bf8:1006 | Fujitsu Siem... | SmartCard Reader 2A      | 100%   |          | D7D5245A1A |
| 0c4b:9102 | Reiner SCT K... | cyberJack RFID basis ... | 100%   |          | 66EEFE25AF |
| 0ca6:00a0 | Castles Tech... | EZCCID Smart Card Reader | 100%   |          | 3DC7A36CB3 |
| 0dc3:1004 | Athena Smart... | ASEDrive CCID            | 100%   |          | FB13C4ACE3 |
| 147e:2020 | Upek            | TouchChip Fingerprint... | 100%   |          | DF1FD87B87 |
| 17ef:1003 | Lenovo          | Integrated Smart Card... | 92.9%  | 3.10.0   | 037CAC7A3D |
| 1a44:0001 | VASCO Data S... | Digipass 905 SmartCar... | 100%   |          | AE29C83D96 |
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

15 out of 1361 (1.10%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 048d:1336 | Integrated T... | SD/MMC Cardreader        | 0.3%   | 3.14.22  | 7E7FB78F58 |
| 058f:6362 | Alcor Micro     | Flash Card Reader/Writer | 0.1%   | 3.8.12   | 0D4B7AD71C |
| 05e3:0723 | Genesys Logic   | GL827L SD/MMC/MS Flas... | 3.2%   | 3.14.33  | DEE7D959CC |
| 0718:069c | Imation         | TF35 USB 3.0             | 100%   |          | 92BF714334 |
| 0984:0301 | Apricorn        | SATAWire 6G              | 25%    | 4.15.0   | D20CC6E64D |
| 0a89:0030 | Aktiv           | Rutoken ECP 4GB          | 33.3%  | 4.1.25   | 0F33C09E44 |
| 0bda:0328 | Realtek Semi... | SD/MMC CRW               | 4.3%   | 4.18.0   | 4B9BEB25C2 |
| 0e8d:0002 | MediaTek        | 1030D                    | 37.5%  | 4.9.60   | E4B342382F |
| 1005:b113 | Apacer Techn... | Handy Steno/AH123 / H... | 0.4%   | 3.0.28   | 8652B8318D |
| 12d1:2590 | Huawei Techn... | ORINOQUIA Auyantepui+... | 100%   |          | BEBC187DBD |
| 13fd:1617 | Initio          | Flash Padlock            | 100%   |          | 95CE4B3495 |
| 13fe:5500 | Kingston Tec... | Silicon-Power32G 31GB    | 2.1%   | 3.14.44  | CE392DF9C0 |
| 5136:4678 | Generic         | Flash Disk 2.0           | 33.3%  | 4.1.38   | C1841B0A29 |
| 8644:8303 | Intenso GmbG    | Supra 32GB               | 20%    | 4.9.20   | CE376CD0F4 |
| ffff:5678 | VendorCo        | ProductCode 16GB         | 10.3%  | 4.4.0    | C7F73C8073 |

### Dvb card (USB)

10 out of 42 (23.81%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 07ca:0810 | AVerMedia Te... | H810 USB Hybrid DVB-T    | 100%   |          | B46F2FEE35 |
| 07ca:0830 | AVerMedia Te... | H830 USB Hybrid DVB-T    | 100%   |          | 79A097BF6F |
| 07ca:0831 | AVerMedia Te... | H831 USB Hybrid DVB-T/T2 | 100%   |          | D5A4F195AE |
| 07ca:1334 | AVerMedia Te... | H334 MiniCard Hybrid ... | 100%   |          | 3EBFFF7DAD |
| 07ca:1336 | AVerMedia Te... | A336 MiniCard Hybrid ... | 100%   |          | A2FF4426C9 |
| 07ca:4336 | AVerMedia Te... | A336 MiniCard Hybrid ... | 100%   |          | 0C3E26BCE7 |
| 0bda:2832 | Realtek Semi... | RTL2832U DVB-T           | 33.3%  | 4.1.19   | 9994FB8ABA |
| 0bda:2838 | Realtek Semi... | RTL2838 DVB-T            | 7%     | 3.14.25  | F3FC00F966 |
| 13d3:3282 | IMC Networks    | DVB-T + GPS Minicard ... | 100%   |          | 7F0F347502 |
| eb1a:5013 | eMPIA Techno... | USB 2883 Device          | 100%   |          | 5DD14F9164 |

### Fingerprint reader (USB)

43 out of 44 (97.73%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0483:2016 | STMicroelect... | Fingerprint Reader       | 100%   |          | 7F41843359 |
| 04f3:0903 | Elan Microel... | ELAN:Fingerprint         | 100%   |          | 632AA405C1 |
| 04f3:0c03 | Elan Microel... | ELAN:Fingerprint         | 100%   |          | E6C392B427 |
| 04f3:0c1a | Elan Microel... | ELAN:Fingerprint         | 100%   |          | A159026F22 |
| 05ba:0002 | DigitalPersona  | Fingerprint Scanner, ... | 100%   |          | AE361E5F23 |
| 06cb:0078 | Synaptics       | WBDI Device              | 100%   |          | 4CED599618 |
| 06cb:0082 | Synaptics       | My Lockey                | 100%   |          | 3E9DFA313B |
| 06cb:00b7 | Synaptics       | Synaptics VFS7552 Tou... | 100%   |          | 0D375562BD |
| 08ff:1600 | AuthenTec       | AES1600                  | 100%   |          | 4A6A073320 |
| 08ff:1660 | AuthenTec       | AES1660 Fingerprint S... | 100%   |          | 89EC4F0398 |
| 08ff:1686 | AuthenTec       | Fingerprint Sensor       | 100%   |          | 73CAFC58A2 |
| 08ff:168a | AuthenTec       | Fingerprint Sensor       | 100%   |          | 9A145A3041 |
| 08ff:168b | AuthenTec       | Fingerprint Sensor       | 100%   |          | 4398E73607 |
| 08ff:168c | AuthenTec       | Fingerprint Sensor       | 100%   |          | 7C26C8530E |
| 08ff:168f | AuthenTec       | AES1660 Fingerprint S... | 100%   |          | 801A0452F8 |
| 08ff:2500 | AuthenTec       | AES2501                  | 100%   |          | 4DCFB332DF |
| 08ff:2550 | AuthenTec       | AES2550 Fingerprint S... | 100%   |          | EEFC712947 |
| 08ff:2580 | AuthenTec       | AES2501 Fingerprint S... | 100%   |          | 084F7E13DA |
| 08ff:2665 | AuthenTec       | Fingerprint Sensor       | 100%   |          | 42DF53B120 |
| 08ff:2683 | AuthenTec       | Fingerprint Sensor       | 100%   |          | 0A5A3C6337 |
| 08ff:2691 | AuthenTec       | Fingerprint Sensor       | 100%   |          | 79E75DF44E |
| 08ff:2810 | AuthenTec       | AES2810                  | 100%   |          | A23E000798 |
| 138a:0001 | Validity Sen... | VFS101 Fingerprint Re... | 100%   |          | 500C2BCFBC |
| 138a:0005 | Validity Sen... | VFS301 Fingerprint Re... | 100%   |          | DDF30C670A |
| 138a:0007 | Validity Sen... | VFS451 Fingerprint Re... | 99%    | 5.1.4    | E2C04796A0 |
| 138a:0008 | Validity Sen... | VFS300 Fingerprint Re... | 100%   |          | 6722706FA2 |
| 138a:0010 | Validity Sen... | VFS Fingerprint sensor   | 100%   |          | 467F389FCE |
| 138a:0011 | Validity Sen... | VFS5011 Fingerprint R... | 100%   |          | 10FB53EFCA |
| 138a:0017 | Validity Sen... | VFS 5011 fingerprint ... | 98.5%  | 4.18.0   | 7637F3DE5F |
| 138a:0018 | Validity Sen... | Fingerprint scanner      | 100%   |          | D2006E7A87 |
| 138a:003c | Validity Sen... | VFS471 Fingerprint Re... | 100%   |          | A31B1E8E5E |
| 138a:003d | Validity Sen... | VFS491                   | 100%   |          | 68A86E6E3F |
| 138a:003f | Validity Sen... | VFS495 Fingerprint Re... | 98.5%  | 4.17.0   | AC96DD45F9 |
| 138a:0050 | Validity Sen... | Swipe Fingerprint Sensor | 100%   |          | 734FCAFBD7 |
| 138a:0090 | Validity Sen... | VFS7500 Touch Fingerp... | 100%   |          | 7E4A6B2354 |
| 138a:0091 | Validity Sen... | VFS7552 Touch Fingerp... | 100%   |          | 200F73880C |
| 147e:1000 | Upek            | Biometric Touchchip/T... | 100%   |          | C15AB53D21 |
| 147e:1001 | Upek            | TCS5B Fingerprint sensor | 100%   |          | 2AFD83B0D3 |
| 147e:1002 | Upek            | Biometric Touchchip/T... | 100%   |          | 7C0CD24986 |
| 147e:2016 | Upek            | Biometric Touchchip/T... | 100%   |          | C28241E4F0 |
| 1c7a:0570 | LighTuning T... | EgisTec Touch Fingerp... | 100%   |          | 376C2CCA98 |
| 1c7a:0603 | LighTuning T... | EgisTec ES603            | 100%   |          | 47C94E2F61 |
| 1c7a:0801 | LighTuning T... | Fingerprint Reader       | 100%   |          | E1D809E15F |

### Hardware key (USB)

4 out of 4 (100%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0471:485d | Philips (or ... | Senselock SenseIV v2.x   | 100%   |          | E4A6E39276 |
| 0a89:0003 | Aktiv           | Guardant Stealth/Net II  | 100%   |          | 5149320E81 |
| 0a89:0020 | Aktiv           | Rutoken S                | 70%    | 3.14.15  | 07802CEC21 |
| 14a8:0001 | Soft protect... | Soft protection devic... | 100%   |          | 568CDC2D31 |

### Hasp (USB)

1 out of 1 (100%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0529:0001 | Aladdin Know... | HASP copy protection ... | 100%   |          | 920F49F96C |

### Hub (USB)

9 out of 333 (2.70%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 03eb:3301 | Atmel           | at43301 4-Port Hub       | 4.5%   | 3.14.44  | 8CF625BE49 |
| 0451:1446 | Texas Instru... | TUSB2040/2070 Hub        | 11.1%  | 4.15.0   | 593A72A02B |
| 0a05:7211 | Unknown Manu... | hub                      | 7.1%   | 3.14.44  | C389CF184F |
| 1a40:0101 | incomplete h... | 4-Port HUB               | 0.1%   | 3.2.0    | 9596ECB170 |
| 8087:0020 | Intel           | Integrated Rate Match... | 0%     | 3.0.28   | 57943279FE |
| 8087:0024 | Intel           | Integrated Rate Match... | 0%     | 2.6.32   | B2ECBDE0F2 |
| 8087:8000 | Intel           | Hub                      | 0.1%   | 2.6.32   | CE392DF9C0 |
| 8087:8001 | Intel           | Hub                      | 0.3%   | 2.6.32   | BD6F7205F3 |
| 8087:8008 | Intel           | Hub                      | 0%     | 2.6.32   | 31E99D9CEA |

### Human interface (USB)

3 out of 356 (0.84%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 04b4:fd13 | Cypress Semi... | Programmable power so... | 50%    | 4.18.0   | 7C4C7CAF9A |
| 11ff:3341 |                 | USB Joystick             | 20%    | 4.1.7    | CD7FA9B160 |
| 1770:ff00 | MSI EPF USB     | MSI EPF USB / LED con... | 0.8%   | 3.14.39  | 1C47BC90E4 |

### Imaging (USB)

1 out of 2 (50%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 04a7:04d0 | Visioneer       | Xerox DocuMate 5460      | 100%   |          | 4ABAC242CC |

### Input/keyboard (USB)

4 out of 1304 (0.31%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0624:0294 | Avocent         | Dell 03R874 KVM dongle   | 100%   |          | 97313ACF09 |
| 0a5c:4502 | Broadcom        | Keyboard (Boot Interf... | 0.7%   | 3.0.28   | 0C3E26BCE7 |
| 0b05:17fd | ASUSTek Comp... | ASUS ROG Macrokey        | 16.7%  | 3.14.44  | C5777BA928 |
| 0c45:7401 | Microdia        | TEMPer Temperature Se... | 88.9%  | 4.19.7   | 0818F19E7A |

### Input/mouse (USB)

8 out of 1260 (0.63%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0458:003a | KYE Systems ... | NetScroll+ Mini Trave... | 0.1%   | 3.10.0   | 5599435B69 |
| 045e:0040 | Microsoft       | Wheel Mouse Optical      | 0.8%   | 3.14.25  | BFCD766C51 |
| 046d:c06c | Logitech        | Optical Mouse            | 0.4%   | 2.6.32   | C6690BB6D9 |
| 048d:8910 | Integrated T... | ITE Device(8910)         | 12.5%  | 4.13.0   | 2D91F64A77 |
| 04b4:0033 | Cypress Semi... | Mouse                    | 1%     | 3.14.25  | 4BCDE0B215 |
| 1532:0042 | Razer USA       | Abyssus 2014             | 12.5%  | 4.9.76   | 31E99D9CEA |
| 413c:8158 | Dell            | Integrated Touchpad /... | 83.3%  | 3.14.44  | ABDBB02998 |
| 413c:8162 | Dell            | Integrated Touchpad [... | 77.2%  | 3.14.33  | 6722706FA2 |

### Modem (USB)

4 out of 95 (4.21%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 04e8:6773 | Samsung Elec... | HSPA Modem               | 66.7%  | 4.15.0   | 3AD0FF0E13 |
| 0572:cb16 | Conexant Sys... | USB-ADSL Modem           | 100%   |          | 07217A2477 |
| 0baf:00ec | U.S. Robotics   | 56K Faxmodem             | 100%   |          | EF974030B3 |
| 0bdb:1926 | Ericsson Bus... | H5321 gw Mobile Broad... | 3.1%   | 3.10.0   | B2ECBDE0F2 |

### Net/wimax (USB)

3 out of 5 (60%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 8086:0186 | Intel           | WiMAX Connection 2400m   | 6.5%   | 3.14.44  | 195F0109A8 |
| 8086:1406 | Intel           | WiMAX Connection 2400m   | 3.9%   | 3.10.19  | 5971AC1B90 |
| 8087:07d6 | Intel           | Centrino WiMAX 6150      | 14.3%  | 3.10.34  | 1D59A8F384 |

### Net/wireless (USB)

63 out of 217 (29.03%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0411:0242 | BUFFALO         | RTL8811AU WI-U2-433DM... | 100%   |          | D92D4F0666 |
| 0457:0162 | Silicon Inte... | SiS162 usb Wireless L... | 100%   |          | D625F7E867 |
| 050d:110a | Belkin Compo... | F9L1101v2 802.11abgn ... | 100%   |          | 506F4A7C1D |
| 050d:615a | Belkin Compo... | F7D4101 / F9L1101v1 8... | 100%   |          | 04CE720011 |
| 050d:7050 | Belkin Compo... | F5D7050 Wireless G Ad... | 100%   |          | 7AC6824CEB |
| 0586:3425 | ZyXEL Commun... | MT7610U NWD6505 802.1... | 100%   |          | 57B1BCAC00 |
| 0586:3426 | ZyXEL Commun... | ZyXEL Dual-Band Wirel... | 100%   |          | C9F28A9B22 |
| 07d1:3a0d | D-Link System   | DWA-120 802.11g Wirel... | 100%   |          | A8A7EB8824 |
| 07d1:3b01 | D-Link System   | AirPlus G DWL-G122 Wi... | 100%   |          | A55363D509 |
| 0846:9011 | NetGear         | BCM4323 WNDA3100v2 80... | 100%   |          | E1F01EA189 |
| 0846:9014 | NetGear         | WNDA3100v3 802.11abgn... | 100%   |          | AB3D7D926D |
| 0846:9020 | NetGear         | BCM43231 WNA3100(v1) ... | 100%   |          | 68CF43B792 |
| 0846:9052 | NetGear         | RTL8811AU A6100 AC600... | 42.9%  | 4.15.0   | 758924E4F2 |
| 0b05:17c9 | ASUSTek Comp... | USB-AC53 802.11a/b/g/... | 100%   |          | B5A179344E |
| 0b05:17d1 | ASUSTek Comp... | MT7610U AC51 802.11a/... | 100%   |          | 48E75D806A |
| 0b05:17d2 | ASUSTek Comp... | USB-AC56 802.11a/b/g/... | 100%   |          | 2F6DFEC51C |
| 0b05:17db | ASUSTek Comp... | MT7610U USB-AC50 802.... | 100%   |          | 93C92CF446 |
| 0b05:1817 | ASUSTek Comp... | RTL8814AU USB-AC68 80... | 100%   |          | D172D2F44B |
| 0b05:184c | ASUSTek Comp... | RTL8812BU USB-AC53 Na... | 96.6%  | 5.0.0    | 3E165AC0A4 |
| 0bda:0811 | Realtek Semi... | RTL8811AU 802.11ac WL... | 57.7%  | 4.15.0   | 5D65FDCE91 |
| 0bda:8176 | Realtek Semi... | RTL8188CUS 802.11n WL... | 0.7%   | 3.14.25  | 51837DE98F |
| 0bda:8179 | Realtek Semi... | RTL8188EUS 802.11n Wi... | 1.3%   | 3.14.25  | 2F2703FBEB |
| 0bda:818b | Realtek Semi... | RTL8192EU ACT-WNP-UA-... | 16.1%  | 4.9.0    | 52A6238F08 |
| 0bda:8812 | Realtek Semi... | RTL8812AU 802.11a/b/g... | 34.6%  | 4.1.38   | C3052C67D6 |
| 0bda:8813 | Realtek Semi... | RTL8814AU 802.11a/b/g... | 100%   |          | DF9651B2B8 |
| 0bda:a811 | Realtek Semi... | RTL8811AU 802.11a/b/g... | 90%    | 4.18.0   | 96B4E832EE |
| 0bda:b711 | Realtek Semi... | RTL8188GU 802.11n WLA... | 100%   |          | 10AA216491 |
| 0bda:b812 | Realtek Semi... | RTL8812BU USB3.0 802.... | 75.4%  | 4.9.155  | 1A0DF24D87 |
| 0bda:c811 | Realtek Semi... | RTL8811CU 802.11ac NIC   | 65%    | 4.4.0    | 37460463A1 |
| 0bda:f179 | Realtek Semi... | 802.11n                  | 94.7%  | 4.18.0   | CCE7F9292D |
| 0bf8:100f | Fujitsu Siem... | miniCard D2301 802.11... | 100%   |          | FEDA3B155D |
| 0cde:0015 | Z-Com           | ISL3887 XG-705A 802.1... | 100%   |          | B4E374835E |
| 0cf3:9271 | Qualcomm Ath... | AR9271 802.11n           | 0.3%   | 3.14.25  | E6A7D05EF4 |
| 0e8d:760c | MediaTek        | 802.11 n WLAN            | 100%   |          | 74DFE126D0 |
| 0e8d:7610 | MediaTek        | MT7610U WiFi             | 92.3%  | 4.15.0   | F75495E252 |
| 0e8d:7612 | MediaTek        | 802.11ac WLAN            | 100%   |          | DC6C804E81 |
| 13b1:003a | Linksys         | BCM43236 AE2500 802.1... | 100%   |          | B703E66C25 |
| 13b1:003e | Linksys         | MT7610U AE6000 802.11... | 100%   |          | 6F68EDE0BD |
| 13b1:003f | Linksys         | RTL8812AU WUSB6300 80... | 60%    | 4.1.19   | FDC986FDE7 |
| 13b1:0042 | Linksys         | QCA9377 WUSB6100M 802... | 25%    | 4.15.0   | 5155142A94 |
| 148f:7601 | Ralink Techn... | MT7601U Wireless Adapter | 15.4%  | 3.14.33  | AB4926FDFF |
| 148f:760b | Ralink Techn... | MT7601U Wireless Adapter | 36.4%  | 3.14.33  | D3D5F51D7A |
| 148f:761a | Ralink Techn... | MT7610U ("Archer T2U"... | 88.2%  | 4.18.0   | F940B41C82 |
| 2001:3314 | D-Link          | RTL8821AU DWA-171 802... | 31.2%  | 4.15.0   | 10BA468B45 |
| 2001:3315 | D-Link          | RTL8812AU DWA-182 Wir... | 40%    | 3.14.39  | CA162546EE |
| 2001:3319 | D-Link          | RTL8192EU DWA-131 Wir... | 48.5%  | 4.1.38   | 58607ACCAE |
| 2357:0101 | Realtek         | RTL8812AU Archer T4U ... | 30%    | 4.1.25   | 915F8EEC67 |
| 2357:0103 | Realtek         | RTL8812AU Archer T4UH... | 50%    | 3.14.44  | D804242BA9 |
| 2357:0105 | MediaTek        | MT7610U Archer T1U 80... | 85.7%  | 5.0.0    | DB3BBECDD0 |
| 2357:0106 | TP-Link         | 802.11ac NIC             | 100%   |          | 62B0B05A66 |
| 2357:0107 | Realtek         | RTL8192EU TL-WN821N V... | 28.6%  | 4.15.0   | 6CF7359C7E |
| 2357:0109 | Realtek         | RTL8192EU TL-WN823N 8... | 6.7%   | 3.16.0   | 8DE11EB42D |
| 2357:010c | Realtek         | RTL8188EUS TL-WN722N v2  | 4%     | 4.9.41   | 27F51AD07D |
| 2357:010d | Realtek         | RTL8812AU TP-Link Arc... | 50%    | 4.15.0   | 80EEC2D2C0 |
| 2357:010e | Realtek         | RTL8812AU TL-WN722N v2   | 100%   |          | 40817D415E |
| 2357:0115 | TP-Link         | 802.11ac NIC             | 58.8%  | 4.15.0   | 26D6C60AD5 |
| 2357:011e | TP-Link         | 802.11ac WLAN Adapter    | 100%   |          | 4CCD035532 |
| 2357:0122 | TP-Link         | 802.11n NIC              | 50%    | 4.18.0   | 7F6510382A |
| 2357:012d | TP-Link         | 802.11ac NIC             | 100%   |          | F733910E90 |
| 2604:0012 | Realtek         | RTL8812AU Tenda U12 8... | 83.3%  | 4.15.0   | C1F0DB0D58 |
| 2c4e:0100 | Realtek         | RTL8192EU WLAN contro... | 55.6%  | 4.9.124  | 2CE91A523F |
| 413c:8102 | Dell            | TrueMobile 1300 802.1... | 100%   |          | 5776ED841E |
| 4317:0720 | Broadcom        | Dynex DX-BUSB            | 100%   |          | 806CA649D7 |

### Network (USB)

5 out of 204 (2.45%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0846:9053 | NetGear         | A6210                    | 69.2%  | 4.18.0   | AC6AA4CE59 |
| 0bda:b720 | Realtek Semi... | RTL8723BU 802.11n WLA... | 3.3%   | 4.4.1    | 6135515DEB |
| 2001:330f | D-Link          | RTL8188ETV DWA-125 11... | 3.2%   | 3.14.44  | 01D21EA756 |
| 2001:3318 | D-Link          | 11ac adapter             | 71.4%  | 4.1.34   | ADF45BCCC3 |
| 7392:a812 | Edimax Techn... | RTL8811AU AC600 USB      | 31.6%  | 3.14.25  | 0B6B3550B5 |

### Sound (USB)

1 out of 346 (0.29%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0a12:1243 | Cambridge Si... | CSRA64110 USB Audio      | 100%   |          | 2A3F7B30CC |

### Tv card (USB)

3 out of 89 (3.37%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 046d:08a2 | Logitech        | Labtec Webcam Pro        | 25%    | 3.14.44  | 51837DE98F |
| 07ca:0889 | AVerMedia Te... | AVerTV Satellite 2       | 100%   |          | 174EC665C6 |
| 0ac8:c002 | Z-Star Micro... | Visual Communication ... | 25%    | 4.9.9    | 7F0BB0CC92 |

### Ups (USB)

2 out of 20 (10%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0592:0002 | Powerware       | UPS (X-Slot)             | 100%   |          | 049C18DB44 |
| 06da:0002 | Phoenixtec P... | UPS                      | 100%   |          | 4F5E89A87E |

### Video (USB)

5 out of 6 (83.33%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0fd9:0051 | Elgato Systems  | GameCapture HD           | 100%   |          | 05F988930D |
| 1164:1ee9 | YUAN High-Te... | Polaris AV Capture       | 100%   |          | 741E3E3C76 |
| 1b80:a41c | Afatech         | Polaris AV Capture       | 100%   |          | F20674C0B8 |
| 2304:0224 | Pinnacle Sys... | MovieBox Plus (710-USB)  | 100%   |          | E9365BC8D0 |
| 5555:3382 | Epiphan Systems | VGA2USB Frame Grabber    | 100%   |          | 37A831391B |

### Wireless (USB)

1 out of 20 (5%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 15a9:003a | Gemtek          | Modem YOTA 4G LTE        | 100%   |          | 02E0DBC8D3 |

