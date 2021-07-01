Devices with bad Linux-compatibility
====================================

This is a project to find PCI/USB devices with bad Linux-compatibility based on the [hwinfo](https://github.com/openSUSE/hwinfo)
reports collected by Linux users at https://linux-hardware.org for the last year.

In the scope of this project, the device is considered badly supported by Linux if driver
is not found for this device in at least one user probe on any Linux distribution.

You can find appropriate hwinfo report in this repository by a probe ID as follows:

    find . -name {PROBE ID}

Everyone can contribute to this repository by uploading probes of their computers
by the [hw-probe](https://github.com/linuxhw/hw-probe) tool:

    sudo -E hw-probe -all -upload

Total reports: 103415.

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
   * [ Storage/ide ](#storageide-pci)
   * [ Storage/nvme ](#storagenvme-pci)
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
   * [ Net/ethernet ](#netethernet-usb)
   * [ Net/wimax ](#netwimax-usb)
   * [ Net/wireless ](#netwireless-usb)
   * [ Network ](#network-usb)
   * [ Sound ](#sound-usb)
   * [ Tv card ](#tv-card-usb)
   * [ Ups ](#ups-usb)
   * [ Video ](#video-usb)
   * [ Wireless ](#wireless-usb)
4. [ Usage of Outdated Kernels ](#usage-of-outdated-kernels)

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
| 1814:3298 | 103c:18ec | Ralink          | RT3290 Bluetooth         | 96.4%  | 4.15.0   | 0FD7A7FA6C |
| 1814:3298 | 103c:191c | Ralink          | RT3290 Bluetooth         | 93.3%  | 5.4.0    | 9B4D6E18AF |
| 1814:3298 | 105b:e056 | Ralink          | RT3290 Bluetooth         | 98.7%  | 5.3.0    | 504FC006B1 |
| 1814:3298 | 10cf:1772 | Ralink          | RT3290 Bluetooth         | 100%   |          | 1135E21142 |
| 1814:3298 | 1814:3298 | Ralink          | RT3290 Bluetooth         | 100%   |          | F11C251D38 |
| 1814:3298 | 1a3b:210b | Ralink          | RT3290 Bluetooth         | 100%   |          | 2333E930AF |
| 1814:3298 | 1a3b:2787 | Ralink          | RT3290 Bluetooth         | 100%   |          | E90A6748C4 |
| 1814:3298 | 1a3b:2987 | Ralink          | RT3290 Bluetooth         | 100%   |          | 1F5B5C1D86 |
| 1814:3298 | 1a3b:2f87 | Ralink          | RT3290 Bluetooth         | 100%   |          | 329190E939 |

### Card reader (PCI)

54 out of 1052 (5.13%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 10ec:5209 | 17aa:21fe | Realtek Semi... | RTS5209 PCI Express C... | 9.1%   | 3.10.0   | 33F0BF2A69 |
| 10ec:5227 | 103c:1940 | Realtek Semi... | RTS5227 PCI Express C... | 12.5%  | 4.15.0   | F440B0000D |
| 10ec:5227 | 103c:2209 | Realtek Semi... | RTS5227 PCI Express C... | 4.8%   | 4.9.20   | 9751D299AD |
| 10ec:5227 | 1179:0001 | Realtek Semi... | RTS5227 PCI Express C... | 3.6%   | 4.15.0   | 550460AAAC |
| 10ec:5227 | 1462:10f4 | Realtek Semi... | RTS5227 PCI Express C... | 100%   |          | 852662BDF3 |
| 10ec:5227 | 17aa:220c | Realtek Semi... | RTS5227 PCI Express C... | 1.1%   | 4.1.15   | 54B33D56BB |
| 10ec:5227 | 17aa:5034 | Realtek Semi... | RTS5227 PCI Express C... | 1.3%   | 4.14.72  | 27139478FF |
| 10ec:5229 | 10ec:5229 | Realtek Semi... | RTS5229 PCI Express C... | 0.9%   | 3.10.51  | 13AB4D878D |
| 10ec:5229 | 8086:2072 | Realtek Semi... | RTS5229 PCI Express C... | 3.1%   | 4.15.0   | 70FA214165 |
| 10ec:522a | 103c:806e | Realtek Semi... | RTS522A PCI Express C... | 100%   |          | 62A9EF950E |
| 10ec:522a | 103c:8079 | Realtek Semi... | RTS522A PCI Express C... | 6.2%   | 4.4.1    | 15E62C605F |
| 10ec:522a | 103c:80a4 | Realtek Semi... | RTS522A PCI Express C... | 7.1%   | 4.9.60   | B01FB51118 |
| 10ec:522a | 103c:80ff | Realtek Semi... | RTS522A PCI Express C... | 31.6%  | 4.7.2    | B7B039F46E |
| 10ec:522a | 103c:8100 | Realtek Semi... | RTS522A PCI Express C... | 12.5%  | 4.15.0   | 2B56F34E21 |
| 10ec:522a | 103c:8101 | Realtek Semi... | RTS522A PCI Express C... | 10.5%  | 4.9.60   | BC496704F4 |
| 10ec:522a | 103c:820c | Realtek Semi... | RTS522A PCI Express C... | 25%    | 4.9.20   | FAE1CD27F3 |
| 10ec:522a | 103c:8392 | Realtek Semi... | RTS522A PCI Express C... | 66.7%  | 4.9.20   | 142D7492C2 |
| 10ec:522a | 103c:84db | Realtek Semi... | RTS522A PCI Express C... | 16.7%  | 4.15.0   | 06EE78EE4D |
| 10ec:522a | 103c:85dd | Realtek Semi... | RTS522A PCI Express C... | 2.8%   | 5.0.0    | 1169B084AC |
| 10ec:522a | 17aa:5048 | Realtek Semi... | RTS522A PCI Express C... | 18.8%  | 4.15.0   | A549AED5B4 |
| 10ec:522a | 17aa:5113 | Realtek Semi... | RTS522A PCI Express C... | 20%    | 4.15.0   | 32F7318757 |
| 10ec:522a | 1854:0325 | Realtek Semi... | RTS522A PCI Express C... | 16.7%  | 4.15.0   | BF08AA9738 |
| 10ec:5249 | 103c:2253 | Realtek Semi... | RTS5249 PCI Express C... | 10.5%  | 5.3.0    | 2B62BC6C8A |
| 10ec:5249 | 17aa:3801 | Realtek Semi... | RTS5249 PCI Express C... | 3.6%   | 3.14.44  | 39A9917502 |
| 10ec:5250 | 1462:11b1 | Realtek Semi... | RTS5250 PCI Express C... | 100%   |          | 99E70D86E2 |
| 10ec:525a | 1028:06de | Realtek Semi... | RTS525A PCI Express C... | 4.5%   | 4.1.25   | 9BAD86D9C9 |
| 10ec:525a | 1028:06df | Realtek Semi... | RTS525A PCI Express C... | 4%     | 4.15.0   | 4C46B3C18D |
| 10ec:525a | 1028:075b | Realtek Semi... | RTS525A PCI Express C... | 2.1%   | 4.4.0    | 6695D2A05E |
| 10ec:525a | 1028:079f | Realtek Semi... | RTS525A PCI Express C... | 10.5%  | 4.15.0   | F6081D54B1 |
| 10ec:525a | 1028:081b | Realtek Semi... | RTS525A PCI Express C... | 9.1%   | 3.10.0   | 05CDC89A9D |
| 10ec:525a | 1028:0905 | Realtek Semi... | RTS525A PCI Express C... | 3.8%   | 4.15.0   | 293A792A22 |
| 10ec:525a | 103c:83ba | Realtek Semi... | RTS525A PCI Express C... | 33.3%  | 4.19.7   | FE8F29171D |
| 10ec:525a | 103c:860f | Realtek Semi... | RTS525A PCI Express C... | 33.3%  | 5.3.0    | BDD15B19B1 |
| 10ec:525a | 17aa:229f | Realtek Semi... | RTS525A PCI Express C... | 5.6%   | 5.0.0    | 72F3E05699 |
| 10ec:5287 | 1025:0866 | Realtek Semi... | RTL8411B PCI Express ... | 3.6%   | 3.14.25  | 5CB1980643 |
| 10ec:5287 | 1025:1264 | Realtek Semi... | RTL8411B PCI Express ... | 2.6%   | 4.1.25   | AAAA4C011C |
| 10ec:5287 | 1558:6509 | Realtek Semi... | RTL8411B PCI Express ... | 20%    | 5.0.0    | 13AB4D878D |
| 10ec:5289 | 1025:0724 | Realtek Semi... | RTL8411 PCI Express C... | 2.3%   | 3.14.53  | 6A087DD575 |
| 10ec:5289 | 1043:1447 | Realtek Semi... | RTL8411 PCI Express C... | 5.3%   | 3.14.44  | F23B5BF0DA |
| 1aea:6601 | 0001:0001 | Alcor Micro     | AU6601 PCI-E Flash ca... | 46.2%  | 4.9.0    | E7400380E1 |
| 1aea:6601 | 1179:f900 | Alcor Micro     | AU6601 PCI-E Flash ca... | 50%    | 5.0.0    | 43A9D7922A |
| 1aea:6621 | 1aea:6621 | Alcor Micro     | AU6621 PCI-E Flash ca... | 34.9%  | 5.0.0    | F872407CA5 |
| 1aea:6625 | 103c:8349 | Alcor Micro     | AU6625 PCI-E Flash ca... | 100%   |          | 1DEE29768A |
| 1aea:6625 | 103c:834b | Alcor Micro     | AU6625 PCI-E Flash ca... | 100%   |          | BD086AB21D |
| 1aea:6625 | 103c:83a9 | Alcor Micro     | AU6625 PCI-E Flash ca... | 100%   |          | 08A47BB260 |
| 1aea:6625 | 103c:8477 | Alcor Micro     | AU6625 PCI-E Flash ca... | 100%   |          | 511D5A39C8 |
| 1aea:6625 | 103c:8478 | Alcor Micro     | AU6625 PCI-E Flash ca... | 90%    | 5.6.0    | 683B19BA25 |
| 1aea:6625 | 103c:8479 | Alcor Micro     | AU6625 PCI-E Flash ca... | 100%   |          | D3980912E7 |
| 1aea:6625 | 103c:85fa | Alcor Micro     | AU6625 PCI-E Flash ca... | 50%    | 5.7.6    | 992E2074FF |
| 1aea:6625 | 103c:85fb | Alcor Micro     | AU6625 PCI-E Flash ca... | 100%   |          | 4EA2E33944 |
| 1aea:6625 | 103c:85fc | Alcor Micro     | AU6625 PCI-E Flash ca... | 66.7%  | 5.6.0    | D3EEB872B9 |
| 1aea:6625 | 103c:85fd | Alcor Micro     | AU6625 PCI-E Flash ca... | 100%   |          | 5986AC405A |
| 1aea:6625 | 103c:85fe | Alcor Micro     | AU6625 PCI-E Flash ca... | 50%    | 5.6.11   | D23BC12452 |
| 1aea:6625 | 103c:85ff | Alcor Micro     | AU6625 PCI-E Flash ca... | 100%   |          | 5240A97FEB |

### Communication controller (PCI)

411 out of 3752 (10.95%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 04f1:2f20 | 04f1:200c |                 | Communication controller | 100%   |          | 6759172767 |
| 104c:8035 | 103c:0934 | Texas Instru... | PCIxx21/PCIxx11 Smart... | 100%   |          | 453696FF5E |
| 104c:8035 | 103c:0938 | Texas Instru... | PCIxx21/PCIxx11 Smart... | 100%   |          | 27E013BC5F |
| 104c:8035 | 103c:0944 | Texas Instru... | PCIxx21/PCIxx11 Smart... | 100%   |          | 0D21AAC1C0 |
| 104c:8035 | 103c:099c | Texas Instru... | PCIxx21/PCIxx11 Smart... | 100%   |          | 2673B46EA2 |
| 104c:8038 | 1028:0182 | Texas Instru... | PCI6515 SmartCard Con... | 100%   |          | C8B1912169 |
| 104c:8038 | 1028:0186 | Texas Instru... | PCI6515 SmartCard Con... | 100%   |          | 7391F06281 |
| 104c:8038 | 1028:0187 | Texas Instru... | PCI6515 SmartCard Con... | 100%   |          | 358447EB4E |
| 104c:803d | 103c:309f | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | 9F80EA24A6 |
| 104c:803d | 103c:30a3 | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | 6B7E7301AE |
| 104c:803d | 103c:30aa | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | 2262B2D7BC |
| 104c:803d | 103c:30ac | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | 3604EF7ED6 |
| 104c:803d | 103c:30ad | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | F950094FF1 |
| 104c:803d | 103c:30b1 | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | AB6D76493B |
| 104c:803d | 1071:8212 | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | 01F778FE4E |
| 1093:c801 |           | National Ins... | PCI-GPIB                 | 100%   |          | 29A0FC6CE0 |
| 11c1:0480 | 1668:0500 | LSI             | Venus Modem (V90, 56K... | 25%    | 3.14.22  | 0A61436F40 |
| 11c1:048c | 11c1:044c | LSI             | V.92 56K WinModem        | 100%   |          | 9D1640A3A7 |
| 11c1:0620 | 11c1:0620 | LSI             | Lucent V.92 Data/Fax ... | 100%   |          | 8CC73D5FD3 |
| 11c1:0620 | 11c1:0621 | LSI             | Lucent V.92 Data/Fax ... | 100%   |          | 5622763899 |
| 11c1:0630 | 11c1:0630 | LSI             | PCI-SV92EX Soft Modem    | 100%   |          | 40B18069A6 |
| 11c1:0630 | 11c1:0631 | LSI             | PCI-SV92EX Soft Modem    | 100%   |          | 2F857AB9C3 |
| 125d:2838 | 125d:2838 | ESS Technology  | ES2838/2839 SuperLink... | 100%   |          | 7F8C6DBB44 |
| 127a:2013 | 1436:2113 | Rockwell Int... | HSF 56k Data/Fax Modem   | 100%   |          | B701C37D96 |
| 127a:2015 | 127a:2015 | Rockwell Int... | HSF 56k Data/Fax/Voic... | 100%   |          | 55EC1147BA |
| 13f6:0211 | 13f6:0211 | C-Media Elec... | CM8738                   | 100%   |          | A23FF13FE0 |
| 14f1:1033 | 1092:0abf | Conexant Sys... | HCF 56k Data/Fax Modem   | 100%   |          | 729981A4D2 |
| 14f1:1033 | 13e0:020d | Conexant Sys... | HCF 56k Data/Fax Modem   | 100%   |          | 87F8B4B22A |
| 14f1:1035 | 148d:1035 | Conexant Sys... | HCF 56k Data/Fax/Voic... | 100%   |          | 36CC45E684 |
| 14f1:1056 | 14f1:1056 | Conexant Sys... | HCF 56k Data/Fax/Voic... | 100%   |          | 9F48604FF2 |
| 14f1:10b6 | 14f1:10b6 | Conexant Sys... | CX06834-11 HCF V.92 5... | 100%   |          | 151D253025 |
| 14f1:10b6 | 1b28:c1e0 | Conexant Sys... | CX06834-11 HCF V.92 5... | 100%   |          | 092AE3A8CA |
| 14f1:10b6 | a0a0:00c2 | Conexant Sys... | CX06834-11 HCF V.92 5... | 100%   |          | D491BA4166 |
| 14f1:2013 | 13e0:0212 | Conexant Sys... | HSF 56k Data/Fax Modem   | 100%   |          | 3ED411EF5C |
| 14f1:2014 | 1048:1540 | Conexant Sys... | HSF 56k Data/Fax/Voic... | 100%   |          | 8BF298A811 |
| 14f1:2014 | 14f1:2014 | Conexant Sys... | HSF 56k Data/Fax/Voic... | 100%   |          | 445429C65F |
| 14f1:2702 | 1028:8d88 | Conexant Sys... | HSFi modem RD01-D270     | 100%   |          | F11822D259 |
| 14f1:2702 | 1043:8d88 | Conexant Sys... | HSFi modem RD01-D270     | 100%   |          | D83C8DDEDF |
| 14f1:2702 | 14f1:2007 | Conexant Sys... | HSFi modem RD01-D270     | 100%   |          | 83629CDF01 |
| 14f1:2f00 | 122d:8d88 | Conexant Sys... | HSF 56k HSFi Modem       | 100%   |          | E29EC46FD7 |
| 14f1:2f00 | 14f1:2002 | Conexant Sys... | HSF 56k HSFi Modem       | 100%   |          | 20D5A3BD6A |
| 14f1:2f00 | 14f1:2003 | Conexant Sys... | HSF 56k HSFi Modem       | 100%   |          | AF474622B9 |
| 14f1:2f00 | 14f1:2004 | Conexant Sys... | HSF 56k HSFi Modem       | 100%   |          | AE1BDB128C |
| 14f1:2f00 | 187e:3409 | Conexant Sys... | HSF 56k HSFi Modem       | 100%   |          | C1BD1568DC |
| 14f1:2f00 | a0a0:02b0 | Conexant Sys... | HSF 56k HSFi Modem       | 100%   |          | B3AA6162D7 |
| 14f1:2f02 | 1767:000b | Conexant Sys... | HSF 56k HSFi Data/Fax    | 100%   |          | DFC83A3DB4 |
| 14f1:2f12 | 16ec:2016 | Conexant Sys... | HSF Data/Fax/Voice (USA) | 100%   |          | 3ADDAB1A1D |
| 14f1:2f20 | 14f1:2000 | Conexant Sys... | HSF 56k Data/Fax Modem   | 100%   |          | B7C39A3C3D |
| 14f1:2f20 | 14f1:200c | Conexant Sys... | HSF 56k Data/Fax Modem   | 100%   |          | 25C2C665B7 |
| 14f1:2f20 | 14f1:200f | Conexant Sys... | HSF 56k Data/Fax Modem   | 100%   |          | AE95B58668 |
| 14f1:2f20 | 14f1:2014 | Conexant Sys... | HSF 56k Data/Fax Modem   | 100%   |          | 18C81B7E8B |
| 14f1:2f30 | 14f1:2004 | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | 457AB9CF46 |
| 14f1:2f30 | 14f1:200f | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | 6126EB96B3 |
| 14f1:2f30 | 14f1:2014 | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | 1930575F3E |
| 14f1:2f30 | 14f1:2030 | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | B6380B40C3 |
| 14f1:2f30 | 14f1:2051 | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | 01318BF092 |
| 14f1:2f30 | 14f1:205d | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | A8BD4F87A5 |
| 14f1:2f30 | 14f1:2075 | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | B4164233B1 |
| 14f1:2f30 | 14f1:20d5 | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | EE28268ECD |
| 14f1:2f40 | 14f1:2000 | Conexant Sys... | PCI CX11261 Soft Modem   | 100%   |          | 7ECB1C4220 |
| 14f1:2f50 | 14f1:207c | Conexant Sys... | Conexant SoftK56 Data... | 100%   |          | 9D6E0760C5 |
| 14f1:2f81 | 14f1:0000 | Conexant Sys... | PCIe CX95610 Soft Modem  | 100%   |          | E35C61490A |
| 14f1:2f82 | 14f1:0000 | Conexant Sys... | PCIe CX95610 Soft Modem  | 100%   |          | 039AFB9C35 |
| 1556:1111 | 1556:1111 | PLDA            | XpressRich-AXI Ref De... | 50%    | 4.14.0   | 93785932DD |
| 1fd4:1999 | 1fd4:0101 | SUNIX           | Multiport serial cont... | 33.3%  | 5.3.0    | 4415A64795 |
| 5372:6870 | 1000:0010 |                 | Communication controller | 100%   |          | 9F8D495876 |
| 8086:02e0 | 1028:0950 | Intel           | Comet Lake Management... | 50%    | 5.3.0    | 20ABB6DE72 |
| 8086:02e0 | 1028:0954 | Intel           | Comet Lake Management... | 100%   |          | 8740133E10 |
| 8086:02e0 | 1028:0955 | Intel           | Comet Lake Management... | 9.1%   | 5.0.0    | 79CBBE0DFF |
| 8086:02e0 | 1028:0962 | Intel           | Comet Lake Management... | 16%    | 5.3.0    | CE1FE203D8 |
| 8086:02e0 | 103c:863f | Intel           | Comet Lake Management... | 14.3%  | 5.3.0    | F10553E785 |
| 8086:02e0 | 103c:866e | Intel           | Comet Lake Management... | 33.3%  | 5.3.0    | 8FF42ABD82 |
| 8086:02e0 | 103c:86b0 | Intel           | Comet Lake Management... | 20%    | 5.0.0    | 43BF3AF429 |
| 8086:02e0 | 1043:1c71 | Intel           | Comet Lake Management... | 66.7%  | 5.3.0    | AE5936BB68 |
| 8086:02e0 | 1462:1279 | Intel           | Comet Lake Management... | 33.3%  | 5.3.0    | 01B30270AD |
| 8086:02e0 | 1462:129c | Intel           | Comet Lake Management... | 7.7%   | 5.3.0    | 754F3C176F |
| 8086:02e0 | 1558:1404 | Intel           | Comet Lake Management... | 9.1%   | 5.3.0    | 24222EF94C |
| 8086:02e0 | 17aa:3803 | Intel           | Comet Lake Management... | 4%     | 5.3.0    | 2BD6E7B668 |
| 8086:02e0 | 17aa:3804 | Intel           | Comet Lake Management... | 33.3%  | 5.4.23   | CA529580D5 |
| 8086:02e0 | 17aa:3806 | Intel           | Comet Lake Management... | 10.5%  | 5.3.0    | A1D4CF77BC |
| 8086:02e0 | 17aa:382f | Intel           | Comet Lake Management... | 28.6%  | 5.3.0    | E454A0B006 |
| 8086:02e0 | 17aa:5078 | Intel           | Comet Lake Management... | 16.7%  | 5.0.0    | 6625FCDF3B |
| 8086:02e0 | 17aa:5079 | Intel           | Comet Lake Management... | 5.3%   | 5.3.0    | 25CC0D4B7B |
| 8086:02e0 | 1d72:1901 | Intel           | Comet Lake Management... | 16.7%  | 5.3.0    | 4D4D89C508 |
| 8086:02e0 | 8086:2081 | Intel           | Comet Lake Management... | 16.7%  | 5.3.0    | F2BFE6BFB3 |
| 8086:06e0 | 8086:7270 | Intel           | Comet Lake HECI Contr... | 100%   |          | 9BFAB5575C |
| 8086:0801 | 8086:0801 | Intel           | Moorestown SPI Ctrl 1    | 100%   |          | D1874B6708 |
| 8086:0802 | 8086:0802 | Intel           | Moorestown I2C 0         | 100%   |          | D1874B6708 |
| 8086:0803 | 8086:0803 | Intel           | Moorestown I2C 1         | 100%   |          | D1874B6708 |
| 8086:0804 | 8086:0804 | Intel           | Moorestown I2C 2         | 100%   |          | D1874B6708 |
| 8086:1197 |           | Intel           | Communication controller | 100%   |          | D1F5E15D8C |
| 8086:19d3 | 8086:19d3 | Intel           | Atom Processor C3000 ... | 100%   |          | 50B6A72C0C |
| 8086:1c3a | 1025:0504 | Intel           | 6 Series/C200 Series ... | 0.5%   | 3.10.0   | 8FE3AF49FB |
| 8086:1c3a | 1028:0493 | Intel           | 6 Series/C200 Series ... | 0.8%   | 3.14.33  | F33530C32A |
| 8086:1c3a | 1028:04a3 | Intel           | 6 Series/C200 Series ... | 2.4%   | 3.10.0   | B88C9F527C |
| 8086:1c3a | 1028:04b8 | Intel           | 6 Series/C200 Series ... | 14.3%  | 4.15.0   | A993CB7099 |
| 8086:1c3a | 103c:1659 | Intel           | 6 Series/C200 Series ... | 6.7%   | 4.1.15   | 119A35F980 |
| 8086:1c3a | 1043:11d7 | Intel           | 6 Series/C200 Series ... | 2.9%   | 3.10.34  | A5A0DA657B |
| 8086:1c3a | 1043:844d | Intel           | 6 Series/C200 Series ... | 0.3%   | 3.0.38   | 07EF877C6B |
| 8086:1c3a | 10cf:1611 | Intel           | 6 Series/C200 Series ... | 1.8%   | 4.1.34   | 958D094890 |
| 8086:1c3a | 17aa:3975 | Intel           | 6 Series/C200 Series ... | 0.9%   | 3.10.34  | 81A1579081 |
| 8086:1c3a | 8086:7270 | Intel           | 6 Series/C200 Series ... | 0.5%   | 3.14.22  | D5C9D589F2 |
| 8086:1c3b | 15d9:0631 | Intel           | 6 Series/C200 Series ... | 100%   |          | CAFF8A66F8 |
| 8086:1c3b | 1734:11cb | Intel           | 6 Series/C200 Series ... | 100%   |          | 4B6AB99884 |
| 8086:1d3a | 1028:048c | Intel           | C600/X79 series chips... | 20%    | 4.15.0   | 77A5A8BF12 |
| 8086:1d3a | 1028:04ce | Intel           | C600/X79 series chips... | 20%    | 4.15.0   | A673017516 |
| 8086:1d3a | 1028:05d2 | Intel           | C600/X79 series chips... | 4.2%   | 4.12.14  | 949DD823D7 |
| 8086:1d3a | 1028:05d4 | Intel           | C600/X79 series chips... | 25%    | 4.15.0   | 19FB02CA4E |
| 8086:1d3a | 15d9:0628 | Intel           | C600/X79 series chips... | 50%    | 3.10.0   | 99E743CA9E |
| 8086:1d3a | 15d9:062b | Intel           | C600/X79 series chips... | 100%   |          | A897C366A9 |
| 8086:1d3a | 15d9:0636 | Intel           | C600/X79 series chips... | 100%   |          | 53FB02A9EF |
| 8086:1d3a | 15d9:0709 | Intel           | C600/X79 series chips... | 50%    | 5.3.0    | 9F3D443A21 |
| 8086:1d3a | 17aa:1026 | Intel           | C600/X79 series chips... | 12.5%  | 4.15.0   | 21286AF23B |
| 8086:1d3a | 1849:1d3a | Intel           | C600/X79 series chips... | 23.5%  | 4.12.14  | CF5FE3DBCE |
| 8086:1d3a | 8086:3582 | Intel           | C600/X79 series chips... | 100%   |          | 9F6D925B73 |
| 8086:1d3b | 1028:048c | Intel           | C600/X79 series chips... | 100%   |          | 77A5A8BF12 |
| 8086:1d3b | 1028:04ce | Intel           | C600/X79 series chips... | 100%   |          | A673017516 |
| 8086:1d3b | 1028:04dc | Intel           | C600/X79 series chips... | 100%   |          | 2A0D285524 |
| 8086:1d3b | 1028:04f7 | Intel           | C600/X79 series chips... | 100%   |          | 6839F6245C |
| 8086:1d3b | 1028:04f8 | Intel           | C600/X79 series chips... | 100%   |          | E8BE4F8032 |
| 8086:1d3b | 1028:04fa | Intel           | C600/X79 series chips... | 100%   |          | CC50EA63F1 |
| 8086:1d3b | 1028:0528 | Intel           | C600/X79 series chips... | 100%   |          | 5A372D2A35 |
| 8086:1d3b | 1043:84ef | Intel           | C600/X79 series chips... | 100%   |          | 6100C873A3 |
| 8086:1d3b | 15d9:0626 | Intel           | C600/X79 series chips... | 100%   |          | 0C9DFEB831 |
| 8086:1d3b | 15d9:0628 | Intel           | C600/X79 series chips... | 100%   |          | F7519BF7BE |
| 8086:1d3b | 15d9:062b | Intel           | C600/X79 series chips... | 100%   |          | A897C366A9 |
| 8086:1d3b | 15d9:062c | Intel           | C600/X79 series chips... | 100%   |          | F2D07088C6 |
| 8086:1d3b | 15d9:0630 | Intel           | C600/X79 series chips... | 100%   |          | E48BEE9611 |
| 8086:1d3b | 15d9:0636 | Intel           | C600/X79 series chips... | 100%   |          | 53FB02A9EF |
| 8086:1d3b | 15d9:0660 | Intel           | C600/X79 series chips... | 100%   |          | 521882E396 |
| 8086:1d3b | 15d9:0665 | Intel           | C600/X79 series chips... | 100%   |          | CEC82EF5D0 |
| 8086:1d3b | 15d9:066b | Intel           | C600/X79 series chips... | 100%   |          | 1FF0EE8759 |
| 8086:1d3b | 15d9:0702 | Intel           | C600/X79 series chips... | 100%   |          | E1213C0B05 |
| 8086:1d3b | 15d9:0703 | Intel           | C600/X79 series chips... | 100%   |          | 8C793BB137 |
| 8086:1d3b | 15d9:0705 | Intel           | C600/X79 series chips... | 100%   |          | B3D08DD227 |
| 8086:1d3b | 15d9:0709 | Intel           | C600/X79 series chips... | 100%   |          | C1586CA94E |
| 8086:1d3b | 15d9:070a | Intel           | C600/X79 series chips... | 100%   |          | B4C8ABC585 |
| 8086:1d3b | 17aa:1026 | Intel           | C600/X79 series chips... | 100%   |          | 21286AF23B |
| 8086:1d3b | 1849:1d3b | Intel           | C600/X79 series chips... | 100%   |          | CF5FE3DBCE |
| 8086:1d3b | 8086:1d3b | Intel           | C600/X79 series chips... | 100%   |          | AA487A5EDB |
| 8086:1d3b | 8086:357e | Intel           | C600/X79 series chips... | 100%   |          | 0FADD1EBE3 |
| 8086:1d3b | 8086:3582 | Intel           | C600/X79 series chips... | 100%   |          | 9F6D925B73 |
| 8086:1d3b | 8086:358c | Intel           | C600/X79 series chips... | 100%   |          | D15B8F8758 |
| 8086:1d3b | 8086:3594 | Intel           | C600/X79 series chips... | 100%   |          | FBDCC4D1F5 |
| 8086:1d3b | 8086:35a0 | Intel           | C600/X79 series chips... | 100%   |          | FE1E6CFF79 |
| 8086:1d3b | 8086:35b0 | Intel           | C600/X79 series chips... | 100%   |          | 30CFD7BC18 |
| 8086:1e3a | 1019:99f2 | Intel           | 7 Series/C216 Chipset... | 50%    | 5.0.0    | 45F3B356CF |
| 8086:1e3a | 1025:0647 | Intel           | 7 Series/C216 Chipset... | 0.7%   | 3.10.34  | 86D2D3B0E1 |
| 8086:1e3a | 1025:064b | Intel           | 7 Series/C216 Chipset... | 0.7%   | 3.14.33  | 3290540C34 |
| 8086:1e3a | 1025:0724 | Intel           | 7 Series/C216 Chipset... | 11.1%  | 4.1.16   | 6A087DD575 |
| 8086:1e3a | 1025:074f | Intel           | 7 Series/C216 Chipset... | 66.7%  | 5.4.0    | 6566319F04 |
| 8086:1e3a | 1028:052c | Intel           | 7 Series/C216 Chipset... | 7.4%   | 4.15.0   | 779B6B3344 |
| 8086:1e3a | 1028:058b | Intel           | 7 Series/C216 Chipset... | 100%   |          | 4A80FC5AF7 |
| 8086:1e3a | 103c:1845 | Intel           | 7 Series/C216 Chipset... | 16.7%  | 3.14.44  | 2E60620A98 |
| 8086:1e3a | 103c:3396 | Intel           | 7 Series/C216 Chipset... | 3.8%   | 4.15.0   | 59E4E46994 |
| 8086:1e3a | 1043:1447 | Intel           | 7 Series/C216 Chipset... | 6.7%   | 3.14.44  | F23B5BF0DA |
| 8086:1e3a | 1043:1477 | Intel           | 7 Series/C216 Chipset... | 1.4%   | 3.14.15  | 731932629B |
| 8086:1e3a | 1043:84ca | Intel           | 7 Series/C216 Chipset... | 1.8%   | 3.10.34  | E214784D20 |
| 8086:1e3a | 1179:fb41 | Intel           | 7 Series/C216 Chipset... | 2.9%   | 3.10.42  | 67009EFFAA |
| 8086:1e3a | 1458:1c3a | Intel           | 7 Series/C216 Chipset... | 0.2%   | 3.10.0   | C900D7A6E2 |
| 8086:1e3a | 17aa:21f9 | Intel           | 7 Series/C216 Chipset... | 4.5%   | 3.14.15  | B7014678B5 |
| 8086:1e3a | 17aa:21fa | Intel           | 7 Series/C216 Chipset... | 1.3%   | 3.10.42  | 2EBE6149B7 |
| 8086:1e3a | 17aa:21fb | Intel           | 7 Series/C216 Chipset... | 8%     | 4.9.20   | 55427995B5 |
| 8086:1e3a | 17aa:3083 | Intel           | 7 Series/C216 Chipset... | 9.1%   | 4.9.111  | E3BF127788 |
| 8086:1e3a | 17aa:3977 | Intel           | 7 Series/C216 Chipset... | 0.3%   | 3.10.42  | 2DD89E3983 |
| 8086:1e3a | 1849:1e3a | Intel           | 7 Series/C216 Chipset... | 0.9%   | 3.10.0   | 46D7FB23B0 |
| 8086:1e3a | 1ae0:c000 | Intel           | 7 Series/C216 Chipset... | 100%   |          | 33F0BF2A69 |
| 8086:1e3a | 8086:1e3a | Intel           | 7 Series/C216 Chipset... | 4.8%   | 3.10.34  | CE8124E5F4 |
| 8086:1e3a | 8086:2035 | Intel           | 7 Series/C216 Chipset... | 20%    | 5.0.0    | DEE8F8ADAA |
| 8086:29b4 | 1028:0211 | Intel           | 82Q35 Express MEI Con... | 1.3%   | 3.14.44  | C1582B3202 |
| 8086:29b4 | 103c:2819 | Intel           | 82Q35 Express MEI Con... | 5.6%   | 3.14.25  | 1208F22123 |
| 8086:29d4 | 103c:281e | Intel           | 82Q33 Express MEI Con... | 1.7%   | 3.14.44  | 13EF653132 |
| 8086:2a45 |           | Intel           | Mobile 4 Series Chips... | 100%   |          | 55FB907088 |
| 8086:2e14 | 103c:3034 | Intel           | 4 Series Chipset HECI... | 3.7%   | 3.14.44  | A40772FC80 |
| 8086:2e14 | 103c:3048 | Intel           | 4 Series Chipset HECI... | 2.9%   | 3.10.34  | 97B51B0912 |
| 8086:2e14 | 8086:1003 | Intel           | 4 Series Chipset HECI... | 11.1%  | 4.4.0    | 53C6C139DA |
| 8086:2e44 | 8086:0025 | Intel           | 4 Series Chipset HECI... | 100%   |          | 8C4EFA23E2 |
| 8086:319a | 1043:1181 | Intel           | Celeron/Pentium Silve... | 14.8%  | 4.15.0   | 76D01F63C2 |
| 8086:319a | 1043:1df0 | Intel           | Celeron/Pentium Silve... | 44.4%  | 5.3.0    | 5D4E6E95F1 |
| 8086:319a | 1043:1eb0 | Intel           | Celeron/Pentium Silve... | 12.5%  | 4.15.0   | 47BF81F534 |
| 8086:319a | 8086:7270 | Intel           | Celeron/Pentium Silve... | 4.3%   | 4.14.71  | 7DBCB914B3 |
| 8086:34e0 | 1028:0979 | Intel           | Ice Lake-LP Managemen... | 10.5%  | 5.0.0    | 7F4CE08DF9 |
| 8086:34e0 | 1028:097c | Intel           | Ice Lake-LP Managemen... | 14.3%  | 5.0.0    | 90B19AF55F |
| 8086:34e0 | 103c:86c8 | Intel           | Ice Lake-LP Managemen... | 14.3%  | 5.3.11   | 16DBE6C7CF |
| 8086:34e4 | 1414:0039 | Intel           | Communication controller | 100%   |          | 6BF45407B9 |
| 8086:34e4 | 1414:0041 | Intel           | Communication controller | 100%   |          | 79D77CFE11 |
| 8086:3b64 | 103c:3674 | Intel           | 5 Series/3400 Series ... | 9.1%   | 4.15.0   | F4DE983D96 |
| 8086:3b64 | 103c:7008 | Intel           | 5 Series/3400 Series ... | 2.2%   | 3.10.34  | 5DD7A5FCE1 |
| 8086:3b64 | 1043:1c77 | Intel           | 5 Series/3400 Series ... | 0.5%   | 3.14.25  | 7FDEE4E7BB |
| 8086:3b64 | 105b:0dd5 | Intel           | 5 Series/3400 Series ... | 20%    | 4.1.25   | 6B384CAEA8 |
| 8086:5a9a | 1849:5a9a | Intel           | Celeron N3350/Pentium... | 2.6%   | 4.9.0    | 633A8B8ADF |
| 8086:5a9a | 8086:7270 | Intel           | Celeron N3350/Pentium... | 2.9%   | 4.4.0    | 685FD2AB95 |
| 8086:5a9c |           | Intel           | Communication controller | 100%   |          | 598FED24AD |
| 8086:5a9c | 1025:1084 | Intel           | Communication controller | 100%   |          | EB24B13C29 |
| 8086:5a9c | 1028:075f | Intel           | Communication controller | 100%   |          | 3D61CAE371 |
| 8086:5a9c | 103c:832e | Intel           | Communication controller | 100%   |          | 321E6EB4AC |
| 8086:5a9c | 1043:8738 | Intel           | Communication controller | 100%   |          | 82BDD3F39F |
| 8086:5a9c | 1297:4045 | Intel           | Communication controller | 100%   |          | 340CD4222F |
| 8086:5a9c | 17aa:3802 | Intel           | Communication controller | 100%   |          | 62D04B32F4 |
| 8086:5a9c | 17aa:3803 | Intel           | Communication controller | 100%   |          | A2C5FD1F80 |
| 8086:5a9c | 17aa:3809 | Intel           | Communication controller | 100%   |          | 1331DBAD16 |
| 8086:5a9c | 8086:7270 | Intel           | Communication controller | 100%   |          | 1C82BD39F0 |
| 8086:5a9e |           | Intel           | Communication controller | 100%   |          | 340CD4222F |
| 8086:5a9e | 1025:1084 | Intel           | Communication controller | 100%   |          | EB24B13C29 |
| 8086:5a9e | 1028:075f | Intel           | Communication controller | 100%   |          | 3D61CAE371 |
| 8086:5a9e | 103c:832e | Intel           | Communication controller | 100%   |          | 321E6EB4AC |
| 8086:5a9e | 1043:8738 | Intel           | Communication controller | 100%   |          | 82BDD3F39F |
| 8086:5a9e | 17aa:3802 | Intel           | Communication controller | 100%   |          | 62D04B32F4 |
| 8086:5a9e | 17aa:3803 | Intel           | Communication controller | 100%   |          | A2C5FD1F80 |
| 8086:5a9e | 17aa:380a | Intel           | Communication controller | 100%   |          | 1331DBAD16 |
| 8086:5a9e | 8086:7270 | Intel           | Communication controller | 100%   |          | 1C82BD39F0 |
| 8086:8c3a | 1028:05a4 | Intel           | 8 Series/C220 Series ... | 1.2%   | 3.10.0   | 541846E7D7 |
| 8086:8c3a | 1028:0620 | Intel           | 8 Series/C220 Series ... | 33.3%  | 5.3.0    | F801FAB1AD |
| 8086:8c3a | 1028:0623 | Intel           | 8 Series/C220 Series ... | 100%   |          | 29D0AD2441 |
| 8086:8c3a | 103c:2253 | Intel           | 8 Series/C220 Series ... | 5.3%   | 5.3.0    | 191021F74E |
| 8086:8c3a | 1043:8534 | Intel           | 8 Series/C220 Series ... | 0.1%   | 3.14.25  | 4712036FF4 |
| 8086:8c3a | 1458:1c3a | Intel           | 8 Series/C220 Series ... | 0.2%   | 3.10.0   | E996F15E3E |
| 8086:8c3a | 1462:7816 | Intel           | 8 Series/C220 Series ... | 2.9%   | 3.14.33  | 093472BA51 |
| 8086:8c3a | 1462:7823 | Intel           | 8 Series/C220 Series ... | 16.7%  | 3.14.25  | 4C0C5DE2E6 |
| 8086:8c3a | 1558:0250 | Intel           | 8 Series/C220 Series ... | 100%   |          | 46B44D2D1F |
| 8086:8c3a | 15d9:0921 | Intel           | 8 Series/C220 Series ... | 33.3%  | 4.15.0   | DB25C87154 |
| 8086:8c3a | 17aa:3978 | Intel           | 8 Series/C220 Series ... | 2.9%   | 3.14.44  | 39A9917502 |
| 8086:8c3a | 1849:8c3a | Intel           | 8 Series/C220 Series ... | 0.4%   | 3.10.0   | 5A36CE2620 |
| 8086:8c3a | 8086:204a | Intel           | 8 Series/C220 Series ... | 7.1%   | 4.1.25   | 8C48173C7B |
| 8086:8c3b | 1025:0790 | Intel           | 8 Series/C220 Series ... | 100%   |          | CD73F91550 |
| 8086:8c3b | 15d9:0803 | Intel           | 8 Series/C220 Series ... | 100%   |          | 869444ACF6 |
| 8086:8c3b | 15d9:086d | Intel           | 8 Series/C220 Series ... | 100%   |          | 0F21786840 |
| 8086:8c3b | 15d9:0921 | Intel           | 8 Series/C220 Series ... | 100%   |          | 34DBD86F7B |
| 8086:8c3b | 15d9:092d | Intel           | 8 Series/C220 Series ... | 100%   |          | 54CBEA6BB1 |
| 8086:8c3b | 1849:8c3b | Intel           | 8 Series/C220 Series ... | 100%   |          | 9E52EE363E |
| 8086:8c3b | 8086:7270 | Intel           | 8 Series/C220 Series ... | 100%   |          | 06197CCB84 |
| 8086:8cba | 1043:8534 | Intel           | 9 Series Chipset Fami... | 1.2%   | 3.14.25  | 1523E8F4A8 |
| 8086:8cba | 1458:1c3a | Intel           | 9 Series Chipset Fami... | 1.5%   | 3.14.22  | 9EE0D24E00 |
| 8086:8d3a | 1043:8600 | Intel           | C610/X99 series chips... | 3.7%   | 3.10.0   | 8212CC8601 |
| 8086:8d3a | 1458:7270 | Intel           | C610/X99 series chips... | 7.1%   | 4.1.15   | 6AFD8A5657 |
| 8086:8d3a | 1462:7885 | Intel           | C610/X99 series chips... | 4.3%   | 4.4.0    | 32D5183912 |
| 8086:8d3a | 15d9:0831 | Intel           | C610/X99 series chips... | 16.7%  | 3.10.0   | 52D5275C7F |
| 8086:8d3a | 15d9:0852 | Intel           | C610/X99 series chips... | 100%   |          | 2E6D79F345 |
| 8086:8d3a | 19e5:2061 | Intel           | C610/X99 series chips... | 100%   |          | 5EB4DFC951 |
| 8086:8d3a | 8086:35c5 | Intel           | C610/X99 series chips... | 100%   |          | 08100751B7 |
| 8086:8d3a | 8086:35c9 | Intel           | C610/X99 series chips... | 100%   |          | 5F9F099F36 |
| 8086:8d3a | 8086:7270 | Intel           | C610/X99 series chips... | 15.4%  | 3.10.0   | 0F42B6C827 |
| 8086:8d3b | 1028:0600 | Intel           | C610/X99 series chips... | 100%   |          | FB8C0A4C3A |
| 8086:8d3b | 1028:0601 | Intel           | C610/X99 series chips... | 100%   |          | C436F9E67A |
| 8086:8d3b | 1028:0639 | Intel           | C610/X99 series chips... | 100%   |          | 3BA1B5FC84 |
| 8086:8d3b | 1028:063a | Intel           | C610/X99 series chips... | 100%   |          | FF3ACF2BDC |
| 8086:8d3b | 1028:063b | Intel           | C610/X99 series chips... | 100%   |          | 031D1E0BEC |
| 8086:8d3b | 1043:85f6 | Intel           | C610/X99 series chips... | 100%   |          | 7426FBDF05 |
| 8086:8d3b | 1458:1000 | Intel           | C610/X99 series chips... | 100%   |          | 0EA40336C5 |
| 8086:8d3b | 15d9:0821 | Intel           | C610/X99 series chips... | 100%   |          | 17BF7A3CBC |
| 8086:8d3b | 15d9:0824 | Intel           | C610/X99 series chips... | 100%   |          | 6C96E4A591 |
| 8086:8d3b | 15d9:0831 | Intel           | C610/X99 series chips... | 100%   |          | 64918C950D |
| 8086:8d3b | 15d9:0834 | Intel           | C610/X99 series chips... | 100%   |          | 3DA0A0E196 |
| 8086:8d3b | 15d9:0835 | Intel           | C610/X99 series chips... | 100%   |          | 7479576DA8 |
| 8086:8d3b | 15d9:0852 | Intel           | C610/X99 series chips... | 100%   |          | 2E6D79F345 |
| 8086:8d3b | 15d9:7270 | Intel           | C610/X99 series chips... | 100%   |          | 5F6D0233A8 |
| 8086:8d3b | 19e5:2061 | Intel           | C610/X99 series chips... | 100%   |          | 5EB4DFC951 |
| 8086:8d3b | 1d49:0a00 | Intel           | C610/X99 series chips... | 100%   |          | 817865DED6 |
| 8086:8d3b | 8086:35c5 | Intel           | C610/X99 series chips... | 100%   |          | 08100751B7 |
| 8086:8d3b | 8086:35c9 | Intel           | C610/X99 series chips... | 100%   |          | 5F9F099F36 |
| 8086:8d3b | 8086:7270 | Intel           | C610/X99 series chips... | 100%   |          | 3BD676846B |
| 8086:8d3b | 8086:8d3b | Intel           | C610/X99 series chips... | 100%   |          | 2903921AEB |
| 8086:9c3a | 1025:0918 | Intel           | 8 Series HECI #0         | 3.1%   | 4.1.19   | F970FF6696 |
| 8086:9c3a | 1028:05e0 | Intel           | 8 Series HECI #0         | 3.3%   | 4.9.9    | 8EA71BA2AE |
| 8086:9c3a | 103c:2249 | Intel           | 8 Series HECI #0         | 12.5%  | 4.1.25   | 8DCBD3C2B1 |
| 8086:9c3a | 1043:13bd | Intel           | 8 Series HECI #0         | 33.3%  | 4.15.0   | 4BABC87322 |
| 8086:9c3a | 17aa:220c | Intel           | 8 Series HECI #0         | 6.6%   | 4.1.15   | BAD560A772 |
| 8086:9cba | 1025:0962 | Intel           | Wildcat Point-LP MEI ... | 25%    | 4.4.0    | 259BFFF741 |
| 8086:9cba | 1028:0675 | Intel           | Wildcat Point-LP MEI ... | 50%    | 4.1.25   | 30ED2641C4 |
| 8086:9cba | 17aa:390b | Intel           | Wildcat Point-LP MEI ... | 4.5%   | 4.9.60   | AB6BD693BE |
| 8086:9d3a | 1025:1094 | Intel           | Sunrise Point-LP CSME... | 3.6%   | 4.9.9    | E7D6077756 |
| 8086:9d3a | 1028:06de | Intel           | Sunrise Point-LP CSME... | 4.3%   | 4.12.14  | AE7AD1E7D9 |
| 8086:9d3a | 1028:06fd | Intel           | Sunrise Point-LP CSME... | 33.3%  | 4.15.0   | 98D787F0D4 |
| 8086:9d3a | 1028:075b | Intel           | Sunrise Point-LP CSME... | 8%     | 4.4.0    | 014FCD25D4 |
| 8086:9d3a | 1028:0782 | Intel           | Sunrise Point-LP CSME... | 12.5%  | 4.18.0   | 49389100FC |
| 8086:9d3a | 1028:079f | Intel           | Sunrise Point-LP CSME... | 21.1%  | 4.15.0   | D18E59C26A |
| 8086:9d3a | 1028:07a7 | Intel           | Sunrise Point-LP CSME... | 5.3%   | 4.9.76   | D0D56FBB1D |
| 8086:9d3a | 1028:081b | Intel           | Sunrise Point-LP CSME... | 18.2%  | 3.10.0   | D1454B26C6 |
| 8086:9d3a | 103c:8079 | Intel           | Sunrise Point-LP CSME... | 7.6%   | 4.4.1    | F1A8589F00 |
| 8086:9d3a | 103c:80a4 | Intel           | Sunrise Point-LP CSME... | 7.1%   | 4.9.60   | B01FB51118 |
| 8086:9d3a | 103c:80ff | Intel           | Sunrise Point-LP CSME... | 31.6%  | 4.7.2    | B7B039F46E |
| 8086:9d3a | 103c:8100 | Intel           | Sunrise Point-LP CSME... | 12.5%  | 4.15.0   | 2B56F34E21 |
| 8086:9d3a | 103c:8101 | Intel           | Sunrise Point-LP CSME... | 10.5%  | 4.9.60   | BC496704F4 |
| 8086:9d3a | 103c:820c | Intel           | Sunrise Point-LP CSME... | 25%    | 4.9.20   | FAE1CD27F3 |
| 8086:9d3a | 103c:83ba | Intel           | Sunrise Point-LP CSME... | 33.3%  | 4.19.7   | FE8F29171D |
| 8086:9d3a | 1043:1ccd | Intel           | Sunrise Point-LP CSME... | 8%     | 4.9.20   | A4B26975E9 |
| 8086:9d3a | 1043:1e30 | Intel           | Sunrise Point-LP CSME... | 20%    | 4.15.0   | D3B1CF2698 |
| 8086:9d3a | 1043:8744 | Intel           | Sunrise Point-LP CSME... | 100%   |          | 12D0EDEC81 |
| 8086:9d3a | 1179:f820 | Intel           | Sunrise Point-LP CSME... | 25%    | 4.15.0   | B781D8419A |
| 8086:9d3a | 17aa:225c | Intel           | Sunrise Point-LP CSME... | 2.3%   | 3.10.0   | 4438A85B31 |
| 8086:9d3a | 17aa:225d | Intel           | Sunrise Point-LP CSME... | 4.4%   | 4.14.35  | 7D7E6AD5D5 |
| 8086:9d3a | 17aa:3801 | Intel           | Sunrise Point-LP CSME... | 1.3%   | 4.9.9    | 412EAC636F |
| 8086:9d3a | 17aa:3808 | Intel           | Sunrise Point-LP CSME... | 3.2%   | 4.9.20   | 9B61CC7F7F |
| 8086:9d3a | 17aa:380c | Intel           | Sunrise Point-LP CSME... | 14.3%  | 4.9.111  | C3352134E9 |
| 8086:9d3a | 17aa:3819 | Intel           | Sunrise Point-LP CSME... | 14.3%  | 4.9.0    | 1AD9E416A0 |
| 8086:9d3a | 17aa:382d | Intel           | Sunrise Point-LP CSME... | 7.5%   | 4.9.60   | 759E13AFC4 |
| 8086:9d3a | 17aa:384e | Intel           | Sunrise Point-LP CSME... | 2.1%   | 4.9.0    | 71BECA8605 |
| 8086:9d3a | 17aa:5048 | Intel           | Sunrise Point-LP CSME... | 12.5%  | 4.15.0   | 842B139FE7 |
| 8086:9d3a | 1b0a:229f | Intel           | Sunrise Point-LP CSME... | 50%    | 4.15.0   | B857F2B82D |
| 8086:9d3a | 1d72:1808 | Intel           | Sunrise Point-LP CSME... | 50%    | 5.6.2    | 8D36FC215C |
| 8086:9d3a | 8086:1999 | Intel           | Sunrise Point-LP CSME... | 1.9%   | 4.9.155  | B1A55C7D69 |
| 8086:9d3e |           | Intel           | Skylake-U/Y CSME: HEC... | 80.9%  | 4.18.7   | E983B6A381 |
| 8086:9d3e | 103c:82cb | Intel           | Skylake-U/Y CSME: HEC... | 100%   |          | FDB567A59E |
| 8086:9da8 | 1043:16f1 | Intel           | Cannon Point-LP Seria... | 11.1%  | 4.18.0   | DBDCCC5696 |
| 8086:9de0 | 1028:089d | Intel           | Cannon Point-LP MEI C... | 11.1%  | 4.15.0   | DAF389F21B |
| 8086:9de0 | 1028:08a8 | Intel           | Cannon Point-LP MEI C... | 11.1%  | 4.15.0   | B6DF9FEC5F |
| 8086:9de0 | 1028:08bc | Intel           | Cannon Point-LP MEI C... | 18.2%  | 4.15.0   | 0787585D2E |
| 8086:9de0 | 103c:857f | Intel           | Cannon Point-LP MEI C... | 25%    | 5.3.0    | A838427772 |
| 8086:9de0 | 1043:16f1 | Intel           | Cannon Point-LP MEI C... | 11.1%  | 4.18.0   | DBDCCC5696 |
| 8086:9de0 | 1558:1325 | Intel           | Cannon Point-LP MEI C... | 9.1%   | 4.18.0   | 7C4E814D03 |
| 8086:9de0 | 17aa:2286 | Intel           | Cannon Point-LP MEI C... | 4.8%   | 4.18.0   | 12B5E06A49 |
| 8086:a13a | 1019:9bc9 | Intel           | 100 Series/C230 Serie... | 100%   |          | 744A3F2E54 |
| 8086:a13a | 1019:9c56 | Intel           | 100 Series/C230 Serie... | 50%    | 4.15.0   | 093E3BB0DE |
| 8086:a13a | 1028:06de | Intel           | 100 Series/C230 Serie... | 18.2%  | 4.15.0   | 568A079F29 |
| 8086:a13a | 1028:06f7 | Intel           | 100 Series/C230 Serie... | 14.3%  | 4.15.0   | E2D11AD2AC |
| 8086:a13a | 1028:0764 | Intel           | 100 Series/C230 Serie... | 100%   |          | 530CC43BE2 |
| 8086:a13a | 103c:8392 | Intel           | 100 Series/C230 Serie... | 66.7%  | 4.9.20   | 142D7492C2 |
| 8086:a13a | 1043:1080 | Intel           | 100 Series/C230 Serie... | 16.7%  | 4.15.0   | 5B1076EA3C |
| 8086:a13a | 1043:1d6d | Intel           | 100 Series/C230 Serie... | 20%    | 5.4.0    | 9D6C0DD372 |
| 8086:a13a | 1043:8694 | Intel           | 100 Series/C230 Serie... | 8%     | 4.4.0    | 57643353CE |
| 8086:a13a | 1458:1c3a | Intel           | 100 Series/C230 Serie... | 6.7%   | 3.10.0   | 53E6A4F263 |
| 8086:a13a | 1462:116e | Intel           | 100 Series/C230 Serie... | 50%    | 5.4.0    | 1C47BC90E4 |
| 8086:a13a | 1462:1190 | Intel           | 100 Series/C230 Serie... | 14.3%  | 4.9.9    | 2B70AAB06F |
| 8086:a13a | 1462:7970 | Intel           | 100 Series/C230 Serie... | 16.7%  | 4.9.20   | AC10EFBB42 |
| 8086:a13a | 1462:7977 | Intel           | 100 Series/C230 Serie... | 12.5%  | 4.9.60   | D1DED92F20 |
| 8086:a13a | 1462:7982 | Intel           | 100 Series/C230 Serie... | 14.3%  | 4.15.0   | AE97650E7C |
| 8086:a13a | 1462:7995 | Intel           | 100 Series/C230 Serie... | 50%    | 4.15.0   | 7D25E0B2DD |
| 8086:a13a | 1462:7996 | Intel           | 100 Series/C230 Serie... | 7.2%   | 4.4.0    | 9B9C670167 |
| 8086:a13a | 15d9:0884 | Intel           | 100 Series/C230 Serie... | 50%    | 4.15.7   | BB8832ACBD |
| 8086:a13a | 1734:121d | Intel           | 100 Series/C230 Serie... | 5.9%   | 4.4.0    | 19202ED9BC |
| 8086:a13a | 17aa:3802 | Intel           | 100 Series/C230 Serie... | 2.4%   | 4.4.16   | 25576A8571 |
| 8086:a13a | 1849:a13a | Intel           | 100 Series/C230 Serie... | 6.2%   | 4.3.3    | 1AD0702A1C |
| 8086:a13a | 8086:1999 | Intel           | 100 Series/C230 Serie... | 14.3%  | 4.9.20   | F8A23904A0 |
| 8086:a13b | 15d9:0884 | Intel           | 100 Series/C230 Serie... | 50%    | 4.15.7   | BB8832ACBD |
| 8086:a13b | 8086:1999 | Intel           | 100 Series/C230 Serie... | 33.3%  | 5.0.0    | 13B41B547A |
| 8086:a1ba | 17aa:7808 | Intel           | C620 Series Chipset F... | 38.5%  | 4.15.0   | CEE7ED2CE9 |
| 8086:a1ba | 8086:7270 | Intel           | C620 Series Chipset F... | 13.3%  | 4.9.60   | D29E79D2C5 |
| 8086:a1bb | 1028:0715 | Intel           | C620 Series Chipset F... | 100%   |          | FF29BCC418 |
| 8086:a1bb | 1028:0716 | Intel           | C620 Series Chipset F... | 100%   |          | 6CD5E5C480 |
| 8086:a1bb | 1028:0718 | Intel           | C620 Series Chipset F... | 100%   |          | 1CCB5D67C2 |
| 8086:a1bb | 1028:07cb | Intel           | C620 Series Chipset F... | 100%   |          | 5B9EC879FC |
| 8086:a1bb | 1043:871e | Intel           | C620 Series Chipset F... | 100%   |          | 61BF6587D2 |
| 8086:a1bb | 15d9:091c | Intel           | C620 Series Chipset F... | 100%   |          | 748FB8054B |
| 8086:a1bb | 15d9:0941 | Intel           | C620 Series Chipset F... | 100%   |          | 76299BB9FF |
| 8086:a1bb | 15d9:095d | Intel           | C620 Series Chipset F... | 100%   |          | 0DFD787765 |
| 8086:a1bb | 15d9:0962 | Intel           | C620 Series Chipset F... | 100%   |          | 57460AA45B |
| 8086:a1bb | 15d9:096d | Intel           | C620 Series Chipset F... | 100%   |          | F9D0B2BC99 |
| 8086:a1bb | 15d9:0987 | Intel           | C620 Series Chipset F... | 100%   |          | 893E9D69F2 |
| 8086:a1bb | 17aa:7808 | Intel           | C620 Series Chipset F... | 100%   |          | CEE7ED2CE9 |
| 8086:a1bb | 8086:35ce | Intel           | C620 Series Chipset F... | 100%   |          | D373AF93CD |
| 8086:a1bb | 8086:7270 | Intel           | C620 Series Chipset F... | 100%   |          | E9A2314525 |
| 8086:a1be | 1028:0715 | Intel           | C620 Series Chipset F... | 100%   |          | FF29BCC418 |
| 8086:a1be | 1028:0716 | Intel           | C620 Series Chipset F... | 100%   |          | 6CD5E5C480 |
| 8086:a1be | 1028:0718 | Intel           | C620 Series Chipset F... | 100%   |          | 1CCB5D67C2 |
| 8086:a1be | 1028:07cb | Intel           | C620 Series Chipset F... | 100%   |          | 5B9EC879FC |
| 8086:a1be | 1043:871e | Intel           | C620 Series Chipset F... | 100%   |          | 61BF6587D2 |
| 8086:a1be | 1590:00eb | Intel           | C620 Series Chipset F... | 100%   |          | 326E6F0067 |
| 8086:a1be | 15d9:091c | Intel           | C620 Series Chipset F... | 100%   |          | 748FB8054B |
| 8086:a1be | 15d9:0941 | Intel           | C620 Series Chipset F... | 100%   |          | 76299BB9FF |
| 8086:a1be | 15d9:095d | Intel           | C620 Series Chipset F... | 100%   |          | 0DFD787765 |
| 8086:a1be | 15d9:0962 | Intel           | C620 Series Chipset F... | 100%   |          | 57460AA45B |
| 8086:a1be | 15d9:096d | Intel           | C620 Series Chipset F... | 100%   |          | F9D0B2BC99 |
| 8086:a1be | 15d9:0987 | Intel           | C620 Series Chipset F... | 100%   |          | 893E9D69F2 |
| 8086:a1be | 17aa:7808 | Intel           | C620 Series Chipset F... | 100%   |          | CEE7ED2CE9 |
| 8086:a1be | 8086:35ce | Intel           | C620 Series Chipset F... | 100%   |          | D373AF93CD |
| 8086:a1be | 8086:7270 | Intel           | C620 Series Chipset F... | 100%   |          | E9A2314525 |
| 8086:a2ba | 1043:8694 | Intel           | 200 Series PCH CSME H... | 0.6%   | 4.4.0    | C30A3E0DDD |
| 8086:a2ba | 1458:1c3a | Intel           | 200 Series PCH CSME H... | 1.5%   | 3.10.0   | 26018540A4 |
| 8086:a2ba | 1462:7a71 | Intel           | 200 Series PCH CSME H... | 20%    | 4.9.9    | 309262E3D6 |
| 8086:a328 | 1025:1264 | Intel           | Cannon Lake PCH Seria... | 4.3%   | 4.15.0   | AAAA4C011C |
| 8086:a328 | 1028:0890 | Intel           | Cannon Lake PCH Seria... | 100%   |          | 9D14FAEDEF |
| 8086:a328 | 1028:08a1 | Intel           | Cannon Lake PCH Seria... | 25%    | 4.18.0   | AACC137FAA |
| 8086:a328 | 103c:843c | Intel           | Cannon Lake PCH Seria... | 14.3%  | 5.0.0    | E5E15DF58D |
| 8086:a328 | 17aa:229f | Intel           | Cannon Lake PCH Seria... | 2.8%   | 5.0.0    | 72F3E05699 |
| 8086:a328 | 1849:a328 | Intel           | Cannon Lake PCH Seria... | 80%    | 5.4.0    | B2FAC79AFD |
| 8086:a360 | 1019:a4a5 | Intel           | Cannon Lake PCH HECI ... | 33.3%  | 4.18.16  | 3028547DA1 |
| 8086:a360 | 1025:1264 | Intel           | Cannon Lake PCH HECI ... | 4.3%   | 4.15.0   | AAAA4C011C |
| 8086:a360 | 1025:126c | Intel           | Cannon Lake PCH HECI ... | 100%   |          | C1339E884A |
| 8086:a360 | 1028:0818 | Intel           | Cannon Lake PCH HECI ... | 10%    | 4.15.0   | F861E71F84 |
| 8086:a360 | 1028:0851 | Intel           | Cannon Lake PCH HECI ... | 100%   |          | 05D6B79D2F |
| 8086:a360 | 1028:086f | Intel           | Cannon Lake PCH HECI ... | 2.9%   | 4.15.0   | 2261D3C647 |
| 8086:a360 | 1028:0877 | Intel           | Cannon Lake PCH HECI ... | 9.1%   | 4.15.0   | 3FBDBB7E9C |
| 8086:a360 | 1028:0890 | Intel           | Cannon Lake PCH HECI ... | 100%   |          | 9D14FAEDEF |
| 8086:a360 | 1028:0905 | Intel           | Cannon Lake PCH HECI ... | 3.8%   | 4.15.0   | 293A792A22 |
| 8086:a360 | 1028:0930 | Intel           | Cannon Lake PCH HECI ... | 33.3%  | 4.15.0   | C2BF735906 |
| 8086:a360 | 103c:843c | Intel           | Cannon Lake PCH HECI ... | 14.3%  | 5.0.0    | E5E15DF58D |
| 8086:a360 | 103c:84db | Intel           | Cannon Lake PCH HECI ... | 16.7%  | 4.15.0   | 06EE78EE4D |
| 8086:a360 | 103c:860f | Intel           | Cannon Lake PCH HECI ... | 50%    | 5.3.0    | BDD15B19B1 |
| 8086:a360 | 1043:1041 | Intel           | Cannon Lake PCH HECI ... | 9.5%   | 4.19.1   | F38CA9409C |
| 8086:a360 | 1043:8694 | Intel           | Cannon Lake PCH HECI ... | 3%     | 4.12.14  | 0B771C098E |
| 8086:a360 | 1458:1c3a | Intel           | Cannon Lake PCH HECI ... | 6.6%   | 4.12.14  | 880C83AF4F |
| 8086:a360 | 1462:126a | Intel           | Cannon Lake PCH HECI ... | 50%    | 5.4.0    | 3CEF0087AA |
| 8086:a360 | 1462:7b23 | Intel           | Cannon Lake PCH HECI ... | 25%    | 4.18.0   | 37076CEBE8 |
| 8086:a360 | 1462:7b33 | Intel           | Cannon Lake PCH HECI ... | 14.3%  | 4.15.0   | F08CE9BD47 |
| 8086:a360 | 1558:67c1 | Intel           | Cannon Lake PCH HECI ... | 100%   |          | 6A8C040FBB |
| 8086:a360 | 17aa:225f | Intel           | Cannon Lake PCH HECI ... | 15%    | 4.15.0   | 2902BB9460 |
| 8086:a360 | 17aa:2267 | Intel           | Cannon Lake PCH HECI ... | 4.2%   | 4.19.11  | AAB68A3B33 |
| 8086:a360 | 17aa:2297 | Intel           | Cannon Lake PCH HECI ... | 4%     | 4.18.0   | 8376F889C2 |
| 8086:a360 | 17aa:229f | Intel           | Cannon Lake PCH HECI ... | 2.8%   | 5.0.0    | 72F3E05699 |
| 8086:a360 | 17aa:3135 | Intel           | Cannon Lake PCH HECI ... | 25%    | 4.15.0   | AA1BE9CBEC |
| 8086:a360 | 17aa:3136 | Intel           | Cannon Lake PCH HECI ... | 33.3%  | 5.0.0    | 02ECA27578 |
| 8086:a360 | 17aa:36e7 | Intel           | Cannon Lake PCH HECI ... | 25%    | 4.15.0   | 1B722DF896 |
| 8086:a360 | 17aa:3810 | Intel           | Cannon Lake PCH HECI ... | 5.3%   | 5.0.0    | 748A1EA384 |
| 8086:a360 | 1849:a360 | Intel           | Cannon Lake PCH HECI ... | 11.7%  | 4.15.0   | E64653B77C |
| 8086:a360 | 8086:7270 | Intel           | Cannon Lake PCH HECI ... | 2.9%   | 4.15.0   | 4F08E906CA |
| 8086:a361 | 15d9:1a1b | Intel           | 300 Series Chipset HE... | 100%   |          | 33FF6DBAD9 |
| 8086:a361 | 15d9:1b0f | Intel           | 300 Series Chipset HE... | 100%   |          | D9DA751F0F |
| 8086:a361 | 1849:a361 | Intel           | 300 Series Chipset HE... | 100%   |          | C6E1FF1BED |
| 8086:a364 | 1028:0890 | Intel           | Cannon Lake PCH HECI ... | 100%   |          | 9D14FAEDEF |
| 8086:a364 | 1849:a364 | Intel           | Cannon Lake PCH HECI ... | 80%    | 5.4.0    | B2FAC79AFD |
| 9710:9900 | a000:2000 | MosChip Semi... | MCS9900 Multi-I/O Con... | 100%   |          | 7D609B3954 |

### Firewire controller (PCI)

17 out of 862 (1.97%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 01c1:5811 | 0043:8294 |                 | FireWire (IEEE 1394)     | 100%   |          | 44D8BC1D36 |
| 104c:8023 | 1297:5106 | Texas Instru... | TSB43AB22A IEEE-1394a... | 16.7%  | 4.12.14  | 35D850590E |
| 1102:4001 | 1102:0010 | Creative Labs   | SB Audigy FireWire Port  | 1.6%   | 3.14.15  | 2A34C16AB3 |
| 1106:3044 | 1043:81fe | VIA Technolo... | VT6306/7/8 [Fire II(M... | 0.2%   | 3.0.28   | 781F2CDA04 |
| 1106:3044 | 1458:1000 | VIA Technolo... | VT6306/7/8 [Fire II(M... | 0.3%   | 3.14.33  | 746ED0F095 |
| 1106:3403 | 1025:0158 | VIA Technolo... | VT6315 Series Firewir... | 12.5%  | 4.9.95   | F558E48348 |
| 1106:3403 | 1849:3403 | VIA Technolo... | VT6315 Series Firewir... | 2%     | 3.14.44  | C9529F922D |
| 1180:0832 | 103c:7008 | Ricoh           | R5C832 IEEE 1394 Cont... | 6.8%   | 3.10.34  | 5DD7A5FCE1 |
| 1180:0832 | 17aa:20c7 | Ricoh           | R5C832 IEEE 1394 Cont... | 0.7%   | 3.10.19  | 28EA2CFCFB |
| 1180:e832 | 1028:040c | Ricoh           | R5C832 PCIe IEEE 1394... | 9.1%   | 4.9.60   | 919212E67C |
| 1180:e832 | 17aa:21ce | Ricoh           | R5C832 PCIe IEEE 1394... | 4%     | 3.14.25  | 8BDBED7F50 |
| 1180:e832 | 17aa:21cf | Ricoh           | R5C832 PCIe IEEE 1394... | 2.4%   | 3.10.34  | 6C0368DFEB |
| 11c1:5811 | 103c:130a | LSI             | FW322/323 [TrueFire] ... | 5.3%   | 4.9.60   | 4EF026497F |
| 11c1:5811 | 103c:130b | LSI             | FW322/323 [TrueFire] ... | 18.2%  | 5.0.0    | A1B7A080A8 |
| 11c1:5901 | 11c1:5900 | LSI             | FW643 [TrueFire] PCIe... | 1.1%   | 3.14.44  | 42636A47B1 |
| 1217:00f7 | 1217:00f7 | O2 Micro        | Firewire (IEEE 1394)     | 2.1%   | 3.13.0   | B851103D78 |
| 197b:2380 | 103c:17a7 | JMicron Tech... | IEEE 1394 Host Contro... | 3.2%   | 3.14.44  | 261BB9DE80 |

### Flash memory (PCI)

39 out of 70 (55.71%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1524:0500 | 1524:0500 | ENE Technology  | FLASH memory             | 100%   |          | 1312407631 |
| 1524:0520 | 1025:007a | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | E4219525B9 |
| 1524:0520 | 1025:007f | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | 246BC5476B |
| 1524:0520 | 1025:0090 | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | 95DB700F93 |
| 1524:0520 | 1025:009f | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | 481320CDB6 |
| 1524:0520 | 1025:010f | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | 0C4DE1A1A1 |
| 1524:0520 | 1179:ff01 | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | 89C7F0F25E |
| 1524:0520 | 1179:ff10 | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | 4375F8C26E |
| 1524:0530 | 1025:007a | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | E4219525B9 |
| 1524:0530 | 1025:007f | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 246BC5476B |
| 1524:0530 | 1025:0090 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 95DB700F93 |
| 1524:0530 | 1025:009f | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 481320CDB6 |
| 1524:0530 | 1025:010f | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 0C4DE1A1A1 |
| 1524:0530 | 1179:ff01 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 89C7F0F25E |
| 1524:0530 | 1179:ff10 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 4375F8C26E |
| 1524:0530 | 14c0:0020 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 41FD098E10 |
| 1524:0530 | 1558:5401 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 8CF7873695 |
| 1524:0530 | 1734:10c1 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 5AA1642777 |
| 1524:0530 | 1734:10d7 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | CA3AC06D30 |
| 1524:0530 | 17aa:2079 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | EDAE63A429 |
| 1524:0720 | 1025:011b | ENE Technology  | Memory Stick Card Rea... | 100%   |          | CD287A7C40 |
| 1524:0720 | 1025:012a | ENE Technology  | Memory Stick Card Rea... | 100%   |          | C95503E7D2 |
| 1524:0720 | 1025:012e | ENE Technology  | Memory Stick Card Rea... | 100%   |          | 08ABC8A867 |
| 1524:0720 | 1462:2fb3 | ENE Technology  | Memory Stick Card Rea... | 100%   |          | 4DA6B718EE |
| 1524:0720 | 1462:2fbd | ENE Technology  | Memory Stick Card Rea... | 100%   |          | 6502446C70 |
| 1524:0730 | 1025:011b | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | CD287A7C40 |
| 1524:0730 | 1025:012a | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | C95503E7D2 |
| 1524:0730 | 1025:012e | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 08ABC8A867 |
| 1524:0730 | 1462:2fb3 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 4DA6B718EE |
| 1524:0730 | 1462:2fbd | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 6502446C70 |
| 1524:0730 | 1558:0573 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 95780C2963 |
| 1524:0730 | 1558:0664 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 51E2E84C28 |
| 1524:0730 | 1558:0668 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 41C9811E8B |
| 1524:0730 | 1558:0669 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 66E0793D5B |
| 1524:0730 | 1558:0721 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 4F4A5860A1 |
| 1524:0730 | 1558:0801 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 8C6849BD5F |
| 1524:0730 | 1558:0802 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | C86682FC32 |
| 1524:0730 | 1558:5408 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | C3A0F0B364 |
| 1524:0730 | 1558:5409 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 88AB93CA71 |

### Graphics card (PCI)

673 out of 12983 (5.18%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1002:130f | 1849:130f | AMD             | Kaveri [Radeon R7 Gra... | 5.9%   | 3.14.44  | 50841878AE |
| 1002:15d8 | 1002:15d8 | AMD             | Picasso                  | 24%    | 5.0.0    | 6E23D82E88 |
| 1002:15d8 | 1025:134d | AMD             | Picasso                  | 5.3%   | 5.0.0    | 5537E9D247 |
| 1002:15d8 | 1025:134f | AMD             | Picasso                  | 11.1%  | 5.0.0    | 7721B3FB75 |
| 1002:15d8 | 103c:85ad | AMD             | Picasso                  | 22.2%  | 5.3.0    | 0D375562BD |
| 1002:15d8 | 103c:85b3 | AMD             | Picasso                  | 22.7%  | 5.0.0    | 89171F1740 |
| 1002:15d8 | 103c:85ea | AMD             | Picasso                  | 17.4%  | 5.0.0    | D81C93199C |
| 1002:15d8 | 103c:8615 | AMD             | Picasso                  | 11.1%  | 5.0.0    | 7BB8688560 |
| 1002:15d8 | 1043:1831 | AMD             | Picasso                  | 28.6%  | 5.3.0    | F1B9FA59EC |
| 1002:15d8 | 1043:18f1 | AMD             | Picasso                  | 8.9%   | 5.0.0    | 9C797156F9 |
| 1002:15d8 | 1043:876b | AMD             | Picasso                  | 20%    | 5.0.0    | 27DA19BC5D |
| 1002:15d8 | 1458:d000 | AMD             | Picasso                  | 25%    | 5.4.0    | 1BC1F63A04 |
| 1002:15d8 | 1462:7b87 | AMD             | Picasso                  | 33.3%  | 5.3.11   | 5BCFE2F1CE |
| 1002:15d8 | 17aa:3801 | AMD             | Picasso                  | 8.8%   | 4.19.97  | 7B350A4E79 |
| 1002:15d8 | 17aa:3808 | AMD             | Picasso                  | 2.2%   | 5.0.0    | 74AB3EBC38 |
| 1002:15d8 | 17aa:5124 | AMD             | Picasso                  | 7.4%   | 5.0.0    | 7B7D62D2A5 |
| 1002:15d8 | 17aa:5126 | AMD             | Picasso                  | 6.7%   | 5.0.0    | 44939F005D |
| 1002:15d8 | 19e5:3e0d | AMD             | Picasso                  | 12.5%  | 5.4.0    | 9F6E79326E |
| 1002:15dd | 1002:15dd | AMD             | Raven Ridge [Radeon V... | 3.8%   | 4.12.14  | 5D0A45B944 |
| 1002:15dd | 103c:8434 | AMD             | Raven Ridge [Radeon V... | 42.9%  | 4.18.0   | E30D68CA01 |
| 1002:15dd | 1043:876b | AMD             | Raven Ridge [Radeon V... | 5.5%   | 4.12.14  | F48E23AB6A |
| 1002:15dd | 1458:d000 | AMD             | Raven Ridge [Radeon V... | 5.6%   | 3.10.0   | 1F49F312CB |
| 1002:15dd | 1462:7a36 | AMD             | Raven Ridge [Radeon V... | 15.4%  | 4.15.0   | 41871808C5 |
| 1002:15dd | 1462:7c02 | AMD             | Raven Ridge [Radeon V... | 9.1%   | 4.15.0   | AD51164983 |
| 1002:15dd | 17aa:36f5 | AMD             | Raven Ridge [Radeon V... | 75%    | 5.5.9    | 7E41940C9C |
| 1002:1636 | 103c:8730 | AMD             | Renoir                   | 50%    | 5.6.16   | 92527E490F |
| 1002:1636 | 103c:876e | AMD             | Renoir                   | 50%    | 5.6.15   | 8C7CFCEB3C |
| 1002:1636 | 1043:16cf | AMD             | Renoir                   | 33.3%  | 5.6.0    | 2DFF24F03C |
| 1002:1636 | 1043:16ef | AMD             | Renoir                   | 100%   |          | 00373C3EE0 |
| 1002:1636 | 1043:1e21 | AMD             | Renoir                   | 100%   |          | 8D8B69EF00 |
| 1002:1636 | 1043:1f11 | AMD             | Renoir                   | 33.3%  | 5.6.15   | 645EF14CB4 |
| 1002:1636 | 17aa:381b | AMD             | Renoir                   | 43.8%  | 5.6.16   | 1AB20B09B6 |
| 1002:1636 | 17aa:381c | AMD             | Renoir                   | 100%   |          | F48BFBD65A |
| 1002:1636 | 17aa:3f1a | AMD             | Renoir                   | 16.7%  | 5.6.12   | D54D0A697B |
| 1002:1636 | 1d72:1953 | AMD             | Renoir                   | 50%    | 5.7.0    | A47F088685 |
| 1002:4354 |           | AMD             | 215CT [Mach64 CT PCI]    | 100%   |          | C0709972A2 |
| 1002:4752 | 103c:3208 | AMD             | Rage 3 [Rage XL PCI]     | 100%   |          | 2C877CF870 |
| 1002:4752 | 8086:341a | AMD             | Rage 3 [Rage XL PCI]     | 100%   |          | 37AA8C0E8E |
| 1002:4752 | 8086:3439 | AMD             | Rage 3 [Rage XL PCI]     | 100%   |          | 0F21E859FA |
| 1002:4752 | 8086:345e | AMD             | Rage 3 [Rage XL PCI]     | 100%   |          | 97CC3C4274 |
| 1002:4756 | 1002:4756 | AMD             | Rage 2 [3D Rage IIC PCI] | 100%   |          | 0B5D843F10 |
| 1002:4c4d | 1002:4c4d | AMD             | Rage Mobility AGP 2x ... | 100%   |          | 5C43AB36E8 |
| 1002:4c4d | 10cf:1074 | AMD             | Rage Mobility AGP 2x ... | 100%   |          | 66D6816956 |
| 1002:4c66 | 1028:011d | AMD             | RV250/M9 GL [Mobility... | 25%    | 3.14.44  | 680157DC8E |
| 1002:515e | 103c:31fb | AMD             | ES1000                   | 6.1%   | 2.6.32   | 2AF0FAD914 |
| 1002:5446 | 1002:0408 | AMD             | Rage 128 PRO Ultra AG... | 100%   |          | F254B75397 |
| 1002:5b60 | 1462:0320 | AMD             | RV370 [Radeon X300]      | 16.7%  | 3.10.0   | 0E8942ECAD |
| 1002:6600 | 103c:194d | AMD             | Mars [Radeon HD 8670A... | 15.4%  | 3.14.25  | 2EDF7E28BE |
| 1002:6600 | 103c:195d | AMD             | Mars [Radeon HD 8670A... | 100%   |          | 1A786FF081 |
| 1002:6601 | 103c:1990 | AMD             | Mars [Radeon HD 8730M]   | 10%    | 4.18.0   | 86ABE3D6C2 |
| 1002:6604 | 1028:066f | AMD             | Opal XT [Radeon R7 M2... | 14.3%  | 4.1.25   | C0697E8F13 |
| 1002:6604 | 103c:8150 | AMD             | Opal XT [Radeon R7 M2... | 16.7%  | 4.15.0   | FD1C0C441E |
| 1002:6610 | 1028:2120 | AMD             | Oland XT [Radeon HD 8... | 26.3%  | 4.15.0   | F81756BB21 |
| 1002:6610 | 1043:0462 | AMD             | Oland XT [Radeon HD 8... | 7.4%   | 3.14.44  | 996842CD08 |
| 1002:6610 | 1787:2012 | AMD             | Oland XT [Radeon HD 8... | 100%   |          | 50841878AE |
| 1002:6611 | 1028:1002 | AMD             | Oland [Radeon HD 8570... | 20%    | 5.0.0    | 21ADB8FC36 |
| 1002:6658 | 174b:e258 | AMD             | Bonaire XTX [Radeon R... | 4.3%   | 3.14.44  | 607681A346 |
| 1002:6658 | 1787:200f | AMD             | Bonaire XTX [Radeon R... | 50%    | 5.3.0    | 28E3ED12EF |
| 1002:665c | 1043:0456 | AMD             | Bonaire XT [Radeon HD... | 40%    | 4.15.0   | 8EACB4F7F2 |
| 1002:665f | 1682:7360 | AMD             | Tobago PRO [Radeon R7... | 12.5%  | 3.10.0   | A4E8642513 |
| 1002:66af | 1002:081e | AMD             | Vega 20 [Radeon VII]     | 9.1%   | 4.15.0   | 6F3E76F9C3 |
| 1002:6739 | 1462:2441 | AMD             | Barts PRO [Radeon HD ... | 18.2%  | 4.4.0    | 20AE6B771A |
| 1002:6740 | 103c:1657 | AMD             | Whistler [Radeon HD 6... | 5.3%   | 3.14.44  | D0C6C442EA |
| 1002:6740 | 103c:165a | AMD             | Whistler [Radeon HD 6... | 5.9%   | 4.1.15   | 0261873B10 |
| 1002:6740 | 103c:3388 | AMD             | Whistler [Radeon HD 6... | 19.7%  | 3.14.44  | 5F74F374A8 |
| 1002:6741 | 1028:04c5 | AMD             | Whistler [Radeon HD 6... | 15.4%  | 4.15.0   | 2C70B99951 |
| 1002:6741 | 1028:04cd | AMD             | Whistler [Radeon HD 6... | 10%    | 4.1.13   | 093E631BFB |
| 1002:6741 | 106b:00e8 | AMD             | Whistler [Radeon HD 6... | 28.6%  | 4.9.9    | F5BB829DBB |
| 1002:6741 | 17aa:21ef | AMD             | Whistler [Radeon HD 6... | 14.3%  | 4.18.0   | A8D9E5EF41 |
| 1002:6741 | 17aa:3976 | AMD             | Whistler [Radeon HD 6... | 3.6%   | 4.1.15   | 70A3F923C2 |
| 1002:6759 | 1787:2308 | AMD             | Turks PRO [Radeon HD ... | 1.8%   | 4.1.34   | 1B7D670A36 |
| 1002:675b | 1002:7600 | AMD             | Turks [Radeon HD 7600... | 20%    | 4.15.0   | B511052CC4 |
| 1002:6760 | 103c:161e | AMD             | Seymour [Radeon HD 64... | 7.7%   | 4.1.15   | BE8865F154 |
| 1002:6760 | 103c:1672 | AMD             | Seymour [Radeon HD 64... | 4%     | 3.14.44  | 4F9C19A9C0 |
| 1002:6760 | 103c:3581 | AMD             | Seymour [Radeon HD 64... | 10.5%  | 4.15.0   | CF65FE653A |
| 1002:6760 | 106b:00e1 | AMD             | Seymour [Radeon HD 64... | 33.3%  | 5.4.0    | 772B6F3A59 |
| 1002:6760 | 144d:c625 | AMD             | Seymour [Radeon HD 64... | 9.1%   | 3.14.44  | EEA7A5432D |
| 1002:6761 | 1297:4012 | AMD             | Seymour LP [Radeon HD... | 100%   |          | DE0CC0AB6F |
| 1002:6770 | 17aa:3623 | AMD             | Caicos [Radeon HD 645... | 20%    | 4.1.15   | 02882EF37B |
| 1002:6778 | 1028:2120 | AMD             | Caicos XT [Radeon HD ... | 5.8%   | 3.10.0   | 50650DB6E3 |
| 1002:6779 | 103c:2128 | AMD             | Caicos [Radeon HD 645... | 8.3%   | 4.1.13   | FE2C73039A |
| 1002:6779 | 1043:03da | AMD             | Caicos [Radeon HD 645... | 0.8%   | 3.10.34  | 9734ABB0D4 |
| 1002:6779 | 1043:047b | AMD             | Caicos [Radeon HD 645... | 25%    | 4.15.0   | 423A12D8A5 |
| 1002:6779 | 174b:e164 | AMD             | Caicos [Radeon HD 645... | 1.1%   | 3.14.33  | 8A4E34A210 |
| 1002:67b1 | 1002:0b00 | AMD             | Hawaii PRO [Radeon R9... | 20%    | 4.19.66  | 2FAE8819F7 |
| 1002:67df | 1002:0b37 | AMD             | Ellesmere [Radeon RX ... | 6.7%   | 4.20.5   | 5CC9EEEBFE |
| 1002:67df | 1043:0557 | AMD             | Ellesmere [Radeon RX ... | 50%    | 4.15.0   | A82798AEA1 |
| 1002:67df | 1462:3413 | AMD             | Ellesmere [Radeon RX ... | 6.5%   | 4.9.87   | 3F7E1BB390 |
| 1002:67df | 148c:2391 | AMD             | Ellesmere [Radeon RX ... | 12.5%  | 5.4.0    | F61EE20F03 |
| 1002:67df | 1da2:e366 | AMD             | Ellesmere [Radeon RX ... | 1.5%   | 4.9.20   | 935B673683 |
| 1002:67ef | 1682:9460 | AMD             | Baffin [Radeon RX 460... | 7.1%   | 4.15.0   | 8212CC8601 |
| 1002:67ef | 174b:e344 | AMD             | Baffin [Radeon RX 460... | 14.3%  | 4.9.124  | 98A829DCFD |
| 1002:67ef | 174b:e348 | AMD             | Baffin [Radeon RX 460... | 7.7%   | 4.9.20   | 72DD80DA38 |
| 1002:67ff | 1043:052d | AMD             | Baffin [Radeon RX 550... | 9.1%   | 4.15.0   | 0219C1DC48 |
| 1002:67ff | 1da2:e348 | AMD             | Baffin [Radeon RX 550... | 4%     | 4.9.60   | CEDA0A30C3 |
| 1002:6800 | 1558:7102 | AMD             | Wimbledon XT [Radeon ... | 100%   |          | B70E28F8B3 |
| 1002:6810 | 174b:e271 | AMD             | Curacao XT / Trinidad... | 2.9%   | 3.14.44  | E84363FB9C |
| 1002:6819 | 1043:042c | AMD             | Pitcairn PRO [Radeon ... | 8%     | 3.14.22  | EBBD83B0CA |
| 1002:6819 | 1043:045b | AMD             | Pitcairn PRO [Radeon ... | 11.8%  | 3.14.33  | A12C16610A |
| 1002:6819 | 174b:a001 | AMD             | Pitcairn PRO [Radeon ... | 16.7%  | 4.9.0    | 97B72D7509 |
| 1002:6819 | 1787:2320 | AMD             | Pitcairn PRO [Radeon ... | 3.7%   | 3.14.44  | 56653049B3 |
| 1002:6821 | 1028:05ee | AMD             | Venus XT [Radeon HD 8... | 13.3%  | 3.14.44  | 31B0BECCAB |
| 1002:6823 | 1028:05eb | AMD             | Venus PRO [Radeon HD ... | 15.8%  | 3.14.44  | E52F291884 |
| 1002:682f | 1028:0572 | AMD             | Chelsea LP [Radeon HD... | 4.5%   | 3.14.44  | F62BE8057A |
| 1002:6840 | 1028:056a | AMD             | Thames [Radeon HD 750... | 3.6%   | 3.14.44  | BC62335D67 |
| 1002:6840 | 1028:0598 | AMD             | Thames [Radeon HD 750... | 18.4%  | 3.14.25  | 76052EA0FD |
| 1002:6840 | 103c:183e | AMD             | Thames [Radeon HD 750... | 2.1%   | 3.14.15  | 5965DBF803 |
| 1002:6840 | 103c:1840 | AMD             | Thames [Radeon HD 750... | 12.5%  | 3.14.44  | B0552C0AF2 |
| 1002:6840 | 103c:1842 | AMD             | Thames [Radeon HD 750... | 5.3%   | 3.14.44  | 2266C4AA6C |
| 1002:6840 | 104d:9096 | AMD             | Thames [Radeon HD 750... | 3.6%   | 3.14.25  | 8677002BB3 |
| 1002:6840 | 1179:fb81 | AMD             | Thames [Radeon HD 750... | 12.5%  | 3.14.33  | 611479F524 |
| 1002:6840 | 144d:c0d8 | AMD             | Thames [Radeon HD 750... | 4.7%   | 3.14.22  | 935529F421 |
| 1002:6841 | 1028:057f | AMD             | Thames [Radeon HD 755... | 31.6%  | 4.15.0   | 00E45A225D |
| 1002:6841 | 103c:179d | AMD             | Thames [Radeon HD 755... | 22.6%  | 3.14.44  | D07E5AEF54 |
| 1002:6841 | 103c:17f4 | AMD             | Thames [Radeon HD 755... | 9.3%   | 3.14.44  | C79BD3EFCD |
| 1002:6841 | 104d:90ac | AMD             | Thames [Radeon HD 755... | 6.1%   | 3.10.19  | F5C5B94EB8 |
| 1002:68a1 | 1025:0475 | AMD             | Broadway PRO [Mobilit... | 100%   |          | 3B1F271BB2 |
| 1002:68ba | 1043:0414 | AMD             | Juniper XT [Radeon HD... | 25%    | 4.9.124  | 38709AEC79 |
| 1002:68be | 174b:e138 | AMD             | Juniper PRO [Radeon H... | 6.7%   | 4.9.20   | 6C4DA588EA |
| 1002:68c1 | 103c:1448 | AMD             | Madison [Mobility Rad... | 11.8%  | 3.10.34  | 75BB7F58F7 |
| 1002:68d8 | 1462:2201 | AMD             | Redwood XT [Radeon HD... | 20%    | 4.15.0   | DDF9D08A22 |
| 1002:68d8 | 174b:e152 | AMD             | Redwood XT [Radeon HD... | 5.9%   | 4.1.15   | D67A015497 |
| 1002:68e0 | 103c:143a | AMD             | Park [Mobility Radeon... | 6.1%   | 3.10.51  | EE5B5B6CD3 |
| 1002:68e0 | 1043:1bf2 | AMD             | Park [Mobility Radeon... | 1.3%   | 3.14.44  | A092284909 |
| 1002:68e0 | 104d:9071 | AMD             | Park [Mobility Radeon... | 6.1%   | 4.1.34   | F28BA85F16 |
| 1002:68e4 | 1043:1c92 | AMD             | Robson CE [Radeon HD ... | 2.4%   | 3.14.44  | 7FDEE4E7BB |
| 1002:68e4 | 17aa:397a | AMD             | Robson CE [Radeon HD ... | 6.8%   | 3.10.34  | AF0EC73528 |
| 1002:68f9 | 1028:2126 | AMD             | Cedar [Radeon HD 5000... | 4.5%   | 4.1.34   | D5A5261203 |
| 1002:68f9 | 1462:2127 | AMD             | Cedar [Radeon HD 5000... | 3.4%   | 4.15.0   | 3E9F988A30 |
| 1002:68f9 | 1462:2133 | AMD             | Cedar [Radeon HD 5000... | 20%    | 5.0.0    | E6AC4BAD03 |
| 1002:68f9 | 1462:2181 | AMD             | Cedar [Radeon HD 5000... | 10%    | 5.2.17   | DA73296417 |
| 1002:68f9 | 1462:2340 | AMD             | Cedar [Radeon HD 5000... | 8.3%   | 4.1.22   | 75CAA3FF6A |
| 1002:68f9 | 1682:3030 | AMD             | Cedar [Radeon HD 5000... | 9.5%   | 4.9.0    | 761DD67D16 |
| 1002:6901 | 103c:224a | AMD             | Topaz PRO [Radeon R5 ... | 11.1%  | 4.9.155  | 00E2C13F56 |
| 1002:6938 | 1043:04f5 | AMD             | Tonga XT / Amethyst X... | 33.3%  | 4.5.5    | 0E1E35C6E2 |
| 1002:6939 | 1682:9380 | AMD             | Tonga PRO [Radeon R9 ... | 14.3%  | 4.15.0   | A3F6229CAA |
| 1002:6939 | 174b:e308 | AMD             | Tonga PRO [Radeon R9 ... | 5.3%   | 4.9.60   | 77EF398855 |
| 1002:6981 | 1028:0926 | AMD             | Lexa XT [Radeon PRO W... | 33.3%  | 5.4.13   | 218EFD739A |
| 1002:699f | 1043:0511 | AMD             | Lexa PRO [Radeon 540/... | 1.6%   | 4.12.14  | A994473A14 |
| 1002:699f | 1458:22f3 | AMD             | Lexa PRO [Radeon 540/... | 20%    | 4.15.0   | 03EEED62F1 |
| 1002:699f | 1462:8a90 | AMD             | Lexa PRO [Radeon 540/... | 12.5%  | 3.10.0   | 28B8E9271B |
| 1002:699f | 148c:2380 | AMD             | Lexa PRO [Radeon 540/... | 14.3%  | 4.15.0   | F48405DCFD |
| 1002:71c5 | 1033:8816 | AMD             | RV530/M56-P [Mobility... | 50%    | 4.18.16  | 76BEC35362 |
| 1002:731f | 1458:2313 | AMD             | Navi 10 [Radeon RX 56... | 7.7%   | 5.3.0    | 2B1062016D |
| 1002:731f | 1458:2316 | AMD             | Navi 10 [Radeon RX 56... | 18.2%  | 5.4.0    | BE903F651A |
| 1002:731f | 1462:3810 | AMD             | Navi 10 [Radeon RX 56... | 20%    | 5.3.6    | 9C6D1E2A61 |
| 1002:731f | 1462:3811 | AMD             | Navi 10 [Radeon RX 56... | 50%    | 5.4.0    | 84D8CC558D |
| 1002:731f | 1da2:e409 | AMD             | Navi 10 [Radeon RX 56... | 6.2%   | 5.3.0    | 40061999CC |
| 1002:7340 | 1043:04e6 | AMD             | Navi 14 [Radeon RX 55... | 100%   |          | A53152418D |
| 1002:7340 | 1458:2319 | AMD             | Navi 14 [Radeon RX 55... | 42.9%  | 5.4.0    | 6C7CCE8852 |
| 1002:7340 | 1462:3820 | AMD             | Navi 14 [Radeon RX 55... | 100%   |          | D56B0B5DA7 |
| 1002:7340 | 1462:3822 | AMD             | Navi 14 [Radeon RX 55... | 7.7%   | 5.4.0    | D3F4F31B29 |
| 1002:7340 | 1682:5501 | AMD             | Navi 14 [Radeon RX 55... | 100%   |          | B7550DC9FC |
| 1002:7340 | 1da2:e421 | AMD             | Navi 14 [Radeon RX 55... | 12.5%  | 5.4.0    | 11405DE424 |
| 1002:791f | 1462:6b30 | AMD             | RS690M [Radeon Xpress... | 100%   |          | 4940058A56 |
| 1002:944a | 106b:00b5 | AMD             | RV770/M98L [Mobility ... | 66.7%  | 4.16.12  | D90C44B813 |
| 1002:9480 | 1025:017e | AMD             | RV730/M96 [Mobility R... | 100%   |          | 8596529915 |
| 1002:9498 | 174b:9498 | AMD             | RV730 PRO [Radeon HD ... | 22.2%  | 3.14.44  | 5A0B34CAC9 |
| 1002:94c3 | 1028:0402 | AMD             | RV610 [Radeon HD 2400... | 33.3%  | 4.15.0   | 9434F7214C |
| 1002:954f | 1043:02ca | AMD             | RV710 [Radeon HD 4350... | 50%    | 3.14.33  | 32406D5DB9 |
| 1002:954f | 1462:1618 | AMD             | RV710 [Radeon HD 4350... | 50%    | 3.14.53  | 51837DE98F |
| 1002:9552 | 103c:3074 | AMD             | RV710/M92 [Mobility R... | 6.1%   | 3.14.25  | 764886854E |
| 1002:9553 | 103c:3628 | AMD             | RV710/M92 [Mobility R... | 5.6%   | 4.1.38   | 5A2F390FC9 |
| 1002:9553 | 1043:1c42 | AMD             | RV710/M92 [Mobility R... | 3.8%   | 4.1.15   | 6D866DDF45 |
| 1002:9553 | 1179:ff82 | AMD             | RV710/M92 [Mobility R... | 60%    | 3.14.44  | 4B659DFE57 |
| 1002:95c0 | 1028:3243 | AMD             | RV620 PRO [Radeon HD ... | 75%    | 4.15.0   | BEA8F18224 |
| 1002:9610 | 1458:d000 | AMD             | RS780 [Radeon HD 3200]   | 17.9%  | 3.10.0   | 52F139CC1C |
| 1002:9614 | 1462:7550 | AMD             | RS780D [Radeon HD 3300]  | 100%   |          | 0B976BCE4C |
| 1002:9616 | 1043:8388 | AMD             | RS780L [Radeon 3000]     | 0.9%   | 3.10.0   | 9D92E8ED9D |
| 1002:9647 | 1179:fc80 | AMD             | Sumo [Radeon HD 6520G]   | 100%   |          | 82C4813A13 |
| 1002:9647 | 144d:c625 | AMD             | Sumo [Radeon HD 6520G]   | 50%    | 4.15.0   | EEA7A5432D |
| 1002:9710 | 1458:d000 | AMD             | RS880 [Radeon HD 4200]   | 3.8%   | 4.1.25   | 9FF481D661 |
| 1002:9712 | 103c:1609 | AMD             | RS880M [Mobility Rade... | 15.4%  | 3.10.0   | 1DD894B330 |
| 1002:9714 | 1849:9714 | AMD             | RS880 [Radeon HD 4290]   | 25%    | 4.1.25   | CAFF866F87 |
| 1002:9802 | 17aa:3619 | AMD             | Wrestler [Radeon HD 6... | 100%   |          | 79C67392D7 |
| 1002:9806 | 1025:0690 | AMD             | Wrestler [Radeon HD 6... | 100%   |          | 5AAA403DEE |
| 1002:9807 | 1002:9807 | AMD             | Wrestler [Radeon HD 6... | 100%   |          | 3027B15C31 |
| 1002:9808 | 17aa:397b | AMD             | Wrestler [Radeon HD 7... | 33.3%  | 5.3.0    | 1EB94811FC |
| 1002:9830 | 1043:8623 | AMD             | Kabini [Radeon HD 840... | 1.5%   | 3.14.44  | 7A3C73F361 |
| 1002:9838 | 1025:0800 | AMD             | Kabini [Radeon HD 824... | 9.1%   | 4.18.0   | 108386F622 |
| 1002:9838 | 103c:8133 | AMD             | Kabini [Radeon HD 824... | 28.6%  | 4.15.0   | 9311532F56 |
| 1002:9850 | 17aa:3804 | AMD             | Mullins [Radeon R3 Gr... | 50%    | 5.3.0    | 2D8AAC7989 |
| 1002:9851 | 1025:088c | AMD             | Mullins [Radeon R4/R5... | 100%   |          | D0E8E1E8D9 |
| 1002:9851 | 103c:2269 | AMD             | Mullins [Radeon R4/R5... | 8.3%   | 4.9.20   | 912D4C6523 |
| 1002:9851 | 103c:226b | AMD             | Mullins [Radeon R4/R5... | 11.1%  | 4.1.34   | 8016AF5575 |
| 1002:9851 | 103c:22cd | AMD             | Mullins [Radeon R4/R5... | 5.6%   | 4.15.0   | 46004F2E8E |
| 1002:9851 | 17aa:3801 | AMD             | Mullins [Radeon R4/R5... | 4.5%   | 4.1.15   | A30A019453 |
| 1002:9853 | 1028:0657 | AMD             | Mullins [Radeon R2 Gr... | 100%   |          | FDA4EB0499 |
| 1002:9853 | 17aa:3801 | AMD             | Mullins [Radeon R2 Gr... | 3.6%   | 4.1.16   | 18EDCF9CC0 |
| 1002:9874 | 103c:80b6 | AMD             | Wani [Radeon R5/R6/R7... | 33.3%  | 4.18.0   | C7EEDACBF5 |
| 1002:9874 | 1458:d000 | AMD             | Wani [Radeon R5/R6/R7... | 11.1%  | 4.15.0   | EF2A18EF64 |
| 1002:9874 | 17aa:5113 | AMD             | Wani [Radeon R5/R6/R7... | 25%    | 4.15.0   | 32F7318757 |
| 1002:98e4 | 1002:1eb0 | AMD             | Stoney [Radeon R2/R3/... | 100%   |          | F2E466A41D |
| 1002:98e4 | 1025:1087 | AMD             | Stoney [Radeon R2/R3/... | 14.3%  | 4.15.0   | AF870DDF65 |
| 1002:98e4 | 103c:84ac | AMD             | Stoney [Radeon R2/R3/... | 1.5%   | 4.15.0   | 4F1105BCA0 |
| 1002:98e4 | 17aa:39f9 | AMD             | Stoney [Radeon R2/R3/... | 7.7%   | 4.9.60   | C23D0EF968 |
| 1002:9900 | 103c:1849 | AMD             | Trinity [Radeon HD 76... | 10%    | 3.14.44  | FE4579E9D1 |
| 1002:9908 | 103c:193b | AMD             | Trinity [Radeon HD 76... | 71.4%  | 4.15.0   | B7C9817495 |
| 1002:990d | 17aa:3804 | AMD             | Richland [Radeon HD 8... | 2.7%   | 3.16.0   | BCE345B263 |
| 1002:9991 | 103c:1850 | AMD             | Trinity 2 [Radeon HD ... | 25%    | 4.9.60   | 898F2B7197 |
| 1002:9993 | 103c:1850 | AMD             | Trinity 2 [Radeon HD ... | 33.3%  | 5.4.0    | 2CC6A94D41 |
| 1002:9996 | 1462:7721 | AMD             | Richland [Radeon HD 8... | 16.7%  | 3.14.44  | 373FA45C3B |
| 1002:9998 | 1462:7721 | AMD             | Richland [Radeon HD 8... | 40%    | 4.1.19   | 64E88CC13B |
| 10de:00cd | 10de:029b | Nvidia          | NV42GL [Quadro FX 345... | 40%    | 3.14.25  | E4D149FE76 |
| 10de:0140 | 1458:3126 | Nvidia          | NV43 [GeForce 6600 GT]   | 50%    | 4.9.155  | 9F8066CA65 |
| 10de:0141 | 1043:81ee | Nvidia          | NV43 [GeForce 6600]      | 50%    | 4.1.38   | 71BC5B9631 |
| 10de:0141 | 1458:3126 | Nvidia          | NV43 [GeForce 6600]      | 16.7%  | 4.9.60   | 7E447609BE |
| 10de:0148 | 1179:0001 | Nvidia          | NV43M [GeForce Go 6600]  | 100%   |          | D5D7DAB02F |
| 10de:0161 |           | Nvidia          | NV44 [GeForce 6200 Tu... | 25%    | 4.9.60   | 10788B7DD6 |
| 10de:0163 | 1043:827b | Nvidia          | NV44 [GeForce 6200 LE]   | 100%   |          | 92059B060A |
| 10de:0181 | 10de:016e | Nvidia          | NV18 [GeForce4 MX 440... | 100%   |          | D25A89846D |
| 10de:0191 | 10de:039c | Nvidia          | G80 [GeForce 8800 GTX]   | 20%    | 5.0.0    | F62172105C |
| 10de:01d1 | 1028:0405 | Nvidia          | G72 [GeForce 7300 LE]    | 14.3%  | 3.14.13  | D866167EB1 |
| 10de:01d3 |           | Nvidia          | G72 [GeForce 7200 GS ... | 6.2%   | 4.1.25   | 17445004F4 |
| 10de:01d3 | 1682:227e | Nvidia          | G72 [GeForce 7200 GS ... | 13.3%  | 3.14.44  | A06909608C |
| 10de:01d3 | 19da:5001 | Nvidia          | G72 [GeForce 7200 GS ... | 100%   |          | 7F950EC2F7 |
| 10de:01d7 | 1043:1101 | Nvidia          | G72M [Quadro NVS 110M... | 50%    | 5.3.0    | F68C00B849 |
| 10de:0241 | 1028:01ec | Nvidia          | C51 [GeForce 6150 LE]    | 25%    | 3.14.44  | 9F87C05C90 |
| 10de:0244 | 103c:30b7 | Nvidia          | C51 [GeForce Go 6150]    | 5.9%   | 3.10.34  | 0CA0AF6291 |
| 10de:0244 | 103c:30bf | Nvidia          | C51 [GeForce Go 6150]    | 12.5%  | 4.15.0   | 5F8A15817C |
| 10de:0291 | 1682:4000 | Nvidia          | G71 [GeForce 7900 GT/... | 100%   |          | C48FFB770E |
| 10de:0292 | 105b:0f03 | Nvidia          | G71 [GeForce 7900 GS]    | 50%    | 4.1.15   | 7296E03F32 |
| 10de:0298 | 1028:019b | Nvidia          | G71M [GeForce Go 7900... | 57.1%  | 4.15.0   | D04B1D869E |
| 10de:0298 | 1179:ff31 | Nvidia          | G71M [GeForce Go 7900... | 100%   |          | FED8975477 |
| 10de:029d | 10de:032b | Nvidia          | G71GL [Quadro FX 3500]   | 11.1%  | 3.14.44  | 22179970F5 |
| 10de:029e | 10de:032c | Nvidia          | G71GL [Quadro FX 1500]   | 42.9%  | 4.9.60   | 727097891C |
| 10de:031a | 104d:814f | Nvidia          | NV31M [GeForce FX Go5... | 100%   |          | 88ABDEBE09 |
| 10de:0326 |           | Nvidia          | NV34 [GeForce FX 5500]   | 3.7%   | 3.18.16  | 427DFF8FF9 |
| 10de:0326 | 1462:911a | Nvidia          | NV34 [GeForce FX 5500]   | 33.3%  | 4.9.41   | FFD7AFA075 |
| 10de:0392 |           | Nvidia          | G73 [GeForce 7600 GS]    | 13.8%  | 3.14.25  | 1764897053 |
| 10de:0398 | 1025:006c | Nvidia          | G73M [GeForce Go 7600]   | 33.3%  | 5.3.0    | 2D3698DEC2 |
| 10de:0398 | 103c:30bb | Nvidia          | G73M [GeForce Go 7600]   | 50%    | 4.15.0   | 1FF804F5C8 |
| 10de:0398 | 1179:0001 | Nvidia          | G73M [GeForce Go 7600]   | 100%   |          | 0BAD664989 |
| 10de:0398 | 14c0:0020 | Nvidia          | G73M [GeForce Go 7600]   | 16.7%  | 4.1.38   | 41FD098E10 |
| 10de:03d0 | 1025:0153 | Nvidia          | C61 [GeForce 6150SE n... | 50%    | 5.1.0    | 2B0BCD5BE1 |
| 10de:03d0 | 103c:2a6c | Nvidia          | C61 [GeForce 6150SE n... | 3.4%   | 4.1.15   | 52991F9A5A |
| 10de:03d0 | 1043:8234 | Nvidia          | C61 [GeForce 6150SE n... | 14.3%  | 3.14.53  | 7A7933F5D5 |
| 10de:03d0 | 1458:d000 | Nvidia          | C61 [GeForce 6150SE n... | 10.5%  | 4.1.15   | B9E294218B |
| 10de:03d0 | 1462:7309 | Nvidia          | C61 [GeForce 6150SE n... | 13.6%  | 3.14.44  | 68013DAC14 |
| 10de:03d1 | 1019:2609 | Nvidia          | C61 [GeForce 6100 nFo... | 6.2%   | 4.4.0    | 5343BC19E6 |
| 10de:03d1 | 1565:1404 | Nvidia          | C61 [GeForce 6100 nFo... | 12.5%  | 4.9.60   | C071FA24D8 |
| 10de:03d6 | 1043:83a4 | Nvidia          | C61 [GeForce 7025 / n... | 11.6%  | 3.14.44  | 9065FDC5CF |
| 10de:03d6 | 1565:1405 | Nvidia          | C61 [GeForce 7025 / n... | 42.9%  | 4.9.20   | 3D289FD6D2 |
| 10de:03d6 | 1849:03d6 | Nvidia          | C61 [GeForce 7025 / n... | 6%     | 3.14.44  | D9FCBBBA59 |
| 10de:0400 | 3842:c765 | Nvidia          | G84 [GeForce 8600 GTS]   | 50%    | 5.3.0    | 9E38311ABE |
| 10de:0402 | 1043:8258 | Nvidia          | G84 [GeForce 8600 GT]    | 33.3%  | 4.1.25   | 8CDD8FFE23 |
| 10de:0402 | 10de:050e | Nvidia          | G84 [GeForce 8600 GT]    | 83.3%  | 4.9.124  | 87142BF4F1 |
| 10de:0402 | 3842:c755 | Nvidia          | G84 [GeForce 8600 GT]    | 100%   |          | C7DBE1E979 |
| 10de:0405 | 1043:15d2 | Nvidia          | G84M [GeForce 9500M GS]  | 11.1%  | 3.14.44  | 4137AC8F54 |
| 10de:0407 | 1028:01f2 | Nvidia          | G84M [GeForce 8600M GT]  | 20%    | 4.1.15   | 5BBAB2BC27 |
| 10de:0407 | 106b:00a4 | Nvidia          | G84M [GeForce 8600M GT]  | 33.3%  | 5.4.0    | 8FA09C0988 |
| 10de:0407 | 1462:3fad | Nvidia          | G84M [GeForce 8600M GT]  | 50%    | 4.1.15   | DF24AE7647 |
| 10de:040f | 10de:049a | Nvidia          | G84GL [Quadro FX 1700]   | 3.3%   | 4.1.25   | 092205321D |
| 10de:0421 | 1acc:0857 | Nvidia          | G86 [GeForce 8500 GT]    | 50%    | 4.18.0   | 629F7B490A |
| 10de:0425 | 1043:1514 | Nvidia          | G86M [GeForce 8600M GS]  | 40%    | 4.1.19   | 785A42EB5B |
| 10de:0426 | 104d:9005 | Nvidia          | G86M [GeForce 8400M GT]  | 100%   |          | 9B1280E7FC |
| 10de:0426 | 104d:9018 | Nvidia          | G86M [GeForce 8400M GT]  | 100%   |          | 8A814A5779 |
| 10de:0427 | 103c:30cd | Nvidia          | G86M [GeForce 8400M GS]  | 50%    | 3.14.44  | 109CAEF651 |
| 10de:0427 | 103c:30cf | Nvidia          | G86M [GeForce 8400M GS]  | 16.7%  | 3.14.53  | 5EDC5F1DD9 |
| 10de:0427 | 104d:9008 | Nvidia          | G86M [GeForce 8400M GS]  | 100%   |          | 207757FC14 |
| 10de:0428 | 1043:1513 | Nvidia          | G86M [GeForce 8400M G]   | 20%    | 4.1.15   | E0EEE8D1CC |
| 10de:0428 | 1631:c103 | Nvidia          | G86M [GeForce 8400M G]   | 100%   |          | AFDAAF53BA |
| 10de:042e | 1043:17c2 | Nvidia          | G86M [GeForce 9300M G]   | 6.7%   | 3.14.33  | 4E30CC5479 |
| 10de:0531 | 103c:30cf | Nvidia          | C67 [GeForce 7150M / ... | 54.5%  | 4.1.15   | A53258F04C |
| 10de:0533 | 1025:0126 | Nvidia          | C67 [GeForce 7000M / ... | 10%    | 4.1.34   | 590A68AE68 |
| 10de:0533 | 1631:c106 | Nvidia          | C67 [GeForce 7000M / ... | 100%   |          | 2E57D2A609 |
| 10de:053b | 1565:1406 | Nvidia          | C68 [GeForce 7050 PV ... | 50%    | 4.15.0   | 0B8A392B30 |
| 10de:05e2 | 3842:1255 | Nvidia          | GT200 [GeForce GTX 260]  | 100%   |          | 947267E711 |
| 10de:0602 | 10de:057c | Nvidia          | G92 [GeForce 8800 GT]    | 60%    | 4.15.0   | DA7914FBED |
| 10de:0611 | 3842:c802 | Nvidia          | G92 [GeForce 8800 GT]    | 100%   |          | D342FEF56E |
| 10de:0614 | 1043:8314 | Nvidia          | G92 [GeForce 9800 GT]    | 20%    | 3.14.44  | A3AFA44F01 |
| 10de:0614 | 1acc:913c | Nvidia          | G92 [GeForce 9800 GT]    | 100%   |          | 530D99F1D6 |
| 10de:0615 | 19da:1103 | Nvidia          | G92 [GeForce GTS 250]    | 33.3%  | 3.14.44  | 5534D6517F |
| 10de:0618 | 1028:02a1 | Nvidia          | G92M [GeForce GTX 260M]  | 100%   |          | 4A26920858 |
| 10de:061a | 10de:055f | Nvidia          | G92GL [Quadro FX 3700]   | 33.3%  | 5.3.0    | 2C436DD9BF |
| 10de:0622 | 10de:058f | Nvidia          | G94 [GeForce 9600 GT]    | 33.3%  | 4.9.60   | 43C2648D7F |
| 10de:062f | 10de:060e | Nvidia          | G94 [GeForce 9800 S]     | 100%   |          | D677F0444F |
| 10de:0638 | 10de:062c | Nvidia          | G94GL [Quadro FX 1800]   | 16.7%  | 3.14.44  | 2162A4B852 |
| 10de:0640 |           | Nvidia          | G96C [GeForce 9500 GT]   | 2.1%   | 3.14.44  | 5BFCEDE830 |
| 10de:0641 |           | Nvidia          | G96C [GeForce 9400 GT]   | 1.9%   | 4.1.15   | 761D76FE04 |
| 10de:0641 | 196d:0000 | Nvidia          | G96C [GeForce 9400 GT]   | 100%   |          | 9E63F07AED |
| 10de:065b | 1682:236d | Nvidia          | G96C [GeForce 9400 GT]   | 25%    | 5.0.0    | 5B28B44909 |
| 10de:06cd | 3842:1470 | Nvidia          | GF100 [GeForce GTX 470]  | 50%    | 4.15.0   | A0225AA660 |
| 10de:06d1 | 10de:0771 | Nvidia          | GF100GL [Tesla C2050 ... | 100%   |          | 1BEF5D0065 |
| 10de:06e4 | 1043:82bc | Nvidia          | G98 [GeForce 8400 GS ... | 50%    | 4.15.0   | 0220656F77 |
| 10de:06e8 | 103c:3603 | Nvidia          | G98M [GeForce 9200M GS]  | 33.3%  | 4.9.20   | 009A4AED18 |
| 10de:06e9 | 1043:19b2 | Nvidia          | G98M [GeForce 9300M GS]  | 2.6%   | 3.10.34  | 914F5D7BD7 |
| 10de:06e9 | 144d:c520 | Nvidia          | G98M [GeForce 9300M GS]  | 100%   |          | F9CD84FA75 |
| 10de:06ef | 103c:306a | Nvidia          | G98M [GeForce G 103M]    | 20%    | 4.1.34   | 7393752623 |
| 10de:07e1 | 1025:0158 | Nvidia          | C73 [GeForce 7100 / n... | 11.1%  | 4.9.20   | BEB70C1FC5 |
| 10de:07e1 | 103c:2a65 | Nvidia          | C73 [GeForce 7100 / n... | 16.7%  | 3.14.44  | E35C61490A |
| 10de:0848 | 1043:82e2 | Nvidia          | C77 [GeForce 8300]       | 8.3%   | 3.10.19  | E1B7D175A1 |
| 10de:0849 | 1043:82f2 | Nvidia          | C77 [GeForce 8200]       | 25%    | 3.14.44  | E3ADCE0E5E |
| 10de:084b | 1025:0153 | Nvidia          | C77 [GeForce 8200]       | 50%    | 4.15.0   | 9E32F34F8E |
| 10de:0862 | 1028:02a1 | Nvidia          | C79 [GeForce 9400M G]    | 100%   |          | 4A26920858 |
| 10de:0863 | 106b:00bd | Nvidia          | C79 [GeForce 9400M]      | 10%    | 4.1.16   | CC45A41950 |
| 10de:0868 | 103c:2a83 | Nvidia          | C79 [nForce 760i SLI]    | 100%   |          | D677F0444F |
| 10de:0869 | 106b:00b4 | Nvidia          | MCP7A [GeForce 9400]     | 11.1%  | 3.14.44  | FF93728268 |
| 10de:086c | 1043:8356 | Nvidia          | C79 [GeForce 9300 / n... | 50%    | 4.9.20   | AAF6FAFAD6 |
| 10de:0a20 | 1043:830f | Nvidia          | GT216 [GeForce GT 220]   | 18.2%  | 3.14.22  | 73DDC0D056 |
| 10de:0a28 | 103c:7001 | Nvidia          | GT216M [GeForce GT 230M] | 9.1%   | 3.10.34  | 2E7C7E635C |
| 10de:0a2c | 103c:1521 | Nvidia          | GT216M [NVS 5100M]       | 16.7%  | 4.15.0   | 2C00474A77 |
| 10de:0a2d | 1025:036d | Nvidia          | GT216M [GeForce GT 320M] | 25%    | 3.14.44  | 2A4C7DD1D5 |
| 10de:0a34 | 1642:3928 | Nvidia          | GT216M [GeForce GT 240M] | 100%   |          | 0921BB94E0 |
| 10de:0a65 |           | Nvidia          | GT218 [GeForce 210]      | 1.8%   | 3.14.25  | E82B578DAD |
| 10de:0a65 | 1043:8354 | Nvidia          | GT218 [GeForce 210]      | 2.9%   | 3.14.44  | 11CCF345FC |
| 10de:0a65 | 1043:847f | Nvidia          | GT218 [GeForce 210]      | 12.5%  | 4.18.16  | F195015CF8 |
| 10de:0a65 | 1043:8490 | Nvidia          | GT218 [GeForce 210]      | 46.7%  | 4.9.9    | A6659EE127 |
| 10de:0a65 | 1043:852d | Nvidia          | GT218 [GeForce 210]      | 4%     | 4.4.0    | A242B5B90B |
| 10de:0a65 | 1458:34d5 | Nvidia          | GT218 [GeForce 210]      | 20%    | 4.1.15   | 83BD0D970C |
| 10de:0a65 | 1458:3525 | Nvidia          | GT218 [GeForce 210]      | 6.9%   | 4.1.25   | EA3398787C |
| 10de:0a65 | 1458:3629 | Nvidia          | GT218 [GeForce 210]      | 7.7%   | 4.1.15   | 8C3172A9F3 |
| 10de:0a65 | 1462:229d | Nvidia          | GT218 [GeForce 210]      | 100%   |          | 4C42FB5573 |
| 10de:0a65 | 1462:8094 | Nvidia          | GT218 [GeForce 210]      | 4.1%   | 3.14.44  | 22A293BC9F |
| 10de:0a65 | 19da:7214 | Nvidia          | GT218 [GeForce 210]      | 25%    | 4.9.0    | 5127F7350B |
| 10de:0a65 | 3842:1310 | Nvidia          | GT218 [GeForce 210]      | 71.4%  | 4.9.124  | 9FE1C71EC5 |
| 10de:0a65 | 3842:1313 | Nvidia          | GT218 [GeForce 210]      | 2.6%   | 4.1.15   | CA8A437958 |
| 10de:0a66 | 1b0a:9060 | Nvidia          | GT218 [GeForce 310]      | 40%    | 4.15.0   | 5C7E0A86DF |
| 10de:0a6c | 1028:040a | Nvidia          | GT218M [NVS 3100M]       | 5.7%   | 4.1.22   | 2DC4747689 |
| 10de:0a6c | 1028:040b | Nvidia          | GT218M [NVS 3100M]       | 40%    | 4.9.0    | CA17782E8F |
| 10de:0a74 | 1025:0296 | Nvidia          | GT218M [GeForce G210M]   | 60%    | 4.18.0   | 64727A44DB |
| 10de:0a7a | 1179:fc90 | Nvidia          | GT218M [GeForce 315M]    | 11.1%  | 3.14.44  | 38C32074A0 |
| 10de:0ca3 | 1043:8326 | Nvidia          | GT215 [GeForce GT 240]   | 11.1%  | 4.1.25   | E0C0BA9CF1 |
| 10de:0ca5 |           | Nvidia          | GT215 [GeForce GT 220]   | 5.6%   | 3.14.33  | 2B809785CB |
| 10de:0caf | 1028:0443 | Nvidia          | GT215M [GeForce GT 335M] | 18.2%  | 4.1.25   | 931486D93C |
| 10de:0dc6 | 1462:2362 | Nvidia          | GF106 [GeForce GTS 45... | 50%    | 4.1.16   | 3FEACD8F08 |
| 10de:0dd1 | 1043:2048 | Nvidia          | GF106M [GeForce GTX 4... | 100%   |          | E738441ADB |
| 10de:0dd8 | 103c:084a | Nvidia          | GF106GL [Quadro 2000]    | 20%    | 4.9.41   | CED13A5341 |
| 10de:0de0 |           | Nvidia          | GF108 [GeForce GT 440]   | 1.5%   | 3.14.44  | 412BBB55C4 |
| 10de:0de0 | 1043:83b7 | Nvidia          | GF108 [GeForce GT 440]   | 20%    | 3.14.44  | C24FEBEB28 |
| 10de:0de1 | 10de:0828 | Nvidia          | GF108 [GeForce GT 430]   | 16.7%  | 3.14.33  | 0ADB0B5B10 |
| 10de:0de1 | 3842:1335 | Nvidia          | GF108 [GeForce GT 430]   | 50%    | 4.18.0   | 3036B319AB |
| 10de:0df0 | 104d:907a | Nvidia          | GF108M [GeForce GT 425M] | 22.2%  | 4.15.0   | 961089FAB7 |
| 10de:0df8 | 103c:0835 | Nvidia          | GF108GL [Quadro 600]     | 11.1%  | 4.9.60   | 8ABFAE9D0B |
| 10de:0df8 | 10de:0835 | Nvidia          | GF108GL [Quadro 600]     | 11.1%  | 3.10.0   | AF1ECD5263 |
| 10de:0dfa | 1028:04a3 | Nvidia          | GF108GLM [Quadro 1000M]  | 25%    | 4.18.0   | C7991B7F27 |
| 10de:0dfc | 1028:0534 | Nvidia          | GF108GLM [NVS 5200M]     | 80%    | 4.19.0   | 303A078ABD |
| 10de:0dfc | 1028:0535 | Nvidia          | GF108GLM [NVS 5200M]     | 25%    | 3.14.25  | 059C31B683 |
| 10de:0e22 | 10de:0804 | Nvidia          | GF104 [GeForce GTX 460]  | 100%   |          | CB7598899F |
| 10de:0e22 | 3842:1370 | Nvidia          | GF104 [GeForce GTX 460]  | 100%   |          | 6D5E184D8B |
| 10de:0f00 |           | Nvidia          | GF108 [GeForce GT 630]   | 7.7%   | 3.14.25  | 0B48CEFE24 |
| 10de:0f00 | 19da:5199 | Nvidia          | GF108 [GeForce GT 630]   | 11.1%  | 4.1.15   | 0EEE02F427 |
| 10de:0f01 | 1043:83fe | Nvidia          | GF108 [GeForce GT 620]   | 16.7%  | 3.14.44  | E12E8BD518 |
| 10de:0f02 | 1043:84d9 | Nvidia          | GF108 [GeForce GT 730]   | 25%    | 3.14.44  | 88C289D589 |
| 10de:0f02 | 1043:84f6 | Nvidia          | GF108 [GeForce GT 730]   | 9.1%   | 3.14.44  | 309F371381 |
| 10de:0f02 | 10de:8399 | Nvidia          | GF108 [GeForce GT 730]   | 100%   |          | 3CC8E9E496 |
| 10de:0fc1 | 1043:83f3 | Nvidia          | GK107 [GeForce GT 640]   | 4.2%   | 3.14.44  | 3B6F246900 |
| 10de:0fc2 | 10de:093c | Nvidia          | GK107 [GeForce GT 630... | 50%    | 4.9.20   | 84224B6ADA |
| 10de:0fc6 | 1043:8427 | Nvidia          | GK107 [GeForce GTX 650]  | 10%    | 3.14.44  | 4E0DC79606 |
| 10de:0fc6 | 1462:2802 | Nvidia          | GK107 [GeForce GTX 650]  | 40%    | 4.18.0   | 128A90D3B7 |
| 10de:0fc6 | 3842:2650 | Nvidia          | GK107 [GeForce GTX 650]  | 50%    | 4.15.0   | 9E45B155AC |
| 10de:0fcd | 17aa:3800 | Nvidia          | GK107M [GeForce GT 755M] | 16.7%  | 5.0.0    | 01CCFAFE86 |
| 10de:0ffa | 10de:094b | Nvidia          | GK107GL [Quadro K600]    | 23.1%  | 4.1.15   | 949DD823D7 |
| 10de:100a | 1462:2983 | Nvidia          | GK110B [GeForce GTX 7... | 100%   |          | 91D43B6213 |
| 10de:1040 | 10de:0915 | Nvidia          | GF119 [GeForce GT 520]   | 20%    | 4.15.0   | C05FF50573 |
| 10de:1040 | 174b:3214 | Nvidia          | GF119 [GeForce GT 520]   | 18.2%  | 4.9.60   | 610EB308AC |
| 10de:104a |           | Nvidia          | GF119 [GeForce GT 610]   | 12.5%  | 4.9.60   | A3A64A4645 |
| 10de:104a | 19da:2219 | Nvidia          | GF119 [GeForce GT 610]   | 100%   |          | 6E35626719 |
| 10de:104a | 19da:5228 | Nvidia          | GF119 [GeForce GT 610]   | 100%   |          | 810897C666 |
| 10de:107c | 10de:102f | Nvidia          | GF119 [NVS 315]          | 16.7%  | 4.18.0   | 9E55C4BDEE |
| 10de:1086 | 1043:8387 | Nvidia          | GF110 [GeForce GTX 57... | 16.7%  | 3.14.22  | BC8749820A |
| 10de:10d8 | 103c:0862 | Nvidia          | GT218 [NVS 300]          | 40%    | 4.15.0   | 4F9670DA15 |
| 10de:1184 | 3842:3778 | Nvidia          | GK104 [GeForce GTX 770]  | 100%   |          | C22EF5B009 |
| 10de:119e | 106b:0121 | Nvidia          | GK104M [GeForce GTX 7... | 100%   |          | D53F359250 |
| 10de:119f | 1043:213e | Nvidia          | GK104M [GeForce GTX 7... | 100%   |          | 30FBA8E75C |
| 10de:11c0 | 1043:8422 | Nvidia          | GK106 [GeForce GTX 660]  | 4.2%   | 3.14.33  | 4C444B85D5 |
| 10de:11c6 | 1043:8446 | Nvidia          | GK106 [GeForce GTX 65... | 25%    | 3.14.44  | 3730F9BE71 |
| 10de:11c8 | 1569:11c8 | Nvidia          | GK106 [GeForce GTX 65... | 6.2%   | 4.1.15   | CE85A9AD63 |
| 10de:11e0 | 1043:21bb | Nvidia          | GK106M [GeForce GTX 7... | 100%   |          | E10390E908 |
| 10de:1200 | 1043:838b | Nvidia          | GF114 [GeForce GTX 56... | 18.2%  | 3.14.44  | 5C1D6C3562 |
| 10de:1200 | 1043:83ac | Nvidia          | GF114 [GeForce GTX 56... | 75%    | 4.18.0   | A2755006BE |
| 10de:1200 | 10b0:0801 | Nvidia          | GF114 [GeForce GTX 56... | 100%   |          | D07ABA1F9C |
| 10de:1200 | 3842:1568 | Nvidia          | GF114 [GeForce GTX 56... | 100%   |          | A623E40CE4 |
| 10de:1208 | 1462:232a | Nvidia          | GF114 [GeForce GTX 56... | 50%    | 4.9.60   | BAEFCCEA96 |
| 10de:1210 | 1462:10bd | Nvidia          | GF114M [GeForce GTX 5... | 14.3%  | 4.1.15   | 7CEA76DF9B |
| 10de:1244 |           | Nvidia          | GF116 [GeForce GTX 55... | 5.3%   | 3.14.44  | 3736215480 |
| 10de:1244 | 1458:351a | Nvidia          | GF116 [GeForce GTX 55... | 20%    | 3.14.44  | FA6E6CF47B |
| 10de:1244 | 196e:089c | Nvidia          | GF116 [GeForce GTX 55... | 100%   |          | A757A049E9 |
| 10de:1244 | 1b0a:90a2 | Nvidia          | GF116 [GeForce GTX 55... | 33.3%  | 4.1.16   | 1F9450CF86 |
| 10de:1244 | 3842:1556 | Nvidia          | GF116 [GeForce GTX 55... | 20%    | 4.15.0   | 4BE9CE0F72 |
| 10de:1244 | 3842:1557 | Nvidia          | GF116 [GeForce GTX 55... | 100%   |          | 09D6286C74 |
| 10de:1244 | 3842:2059 | Nvidia          | GF116 [GeForce GTX 55... | 100%   |          | 5DD4529689 |
| 10de:1251 | 10de:0000 | Nvidia          | GF116M [GeForce GT 560M] | 100%   |          | BBF8BA233B |
| 10de:1284 | 1043:8461 | Nvidia          | GK208 [GeForce GT 630... | 10%    | 3.14.44  | 9B458CFF70 |
| 10de:1287 | 1043:84f5 | Nvidia          | GK208B [GeForce GT 730]  | 38.5%  | 4.1.16   | 5D93D067D7 |
| 10de:1287 | 1043:8501 | Nvidia          | GK208B [GeForce GT 730]  | 11.1%  | 4.1.15   | 930D8056C3 |
| 10de:1287 | 1043:850c | Nvidia          | GK208B [GeForce GT 730]  | 50%    | 4.18.0   | 6CF789DF63 |
| 10de:1287 | 1043:858b | Nvidia          | GK208B [GeForce GT 730]  | 100%   |          | 60C99711B8 |
| 10de:1287 | 10de:1083 | Nvidia          | GK208B [GeForce GT 730]  | 50%    | 4.9.60   | 5E5919C697 |
| 10de:1287 | 10de:1287 | Nvidia          | GK208B [GeForce GT 730]  | 4.3%   | 4.1.25   | 8603D5BDF5 |
| 10de:1287 | 1642:3e56 | Nvidia          | GK208B [GeForce GT 730]  | 20%    | 4.9.60   | 2F126B4841 |
| 10de:1288 | 1462:8c90 | Nvidia          | GK208B [GeForce GT 720]  | 26.7%  | 4.1.15   | 665E2E1F1B |
| 10de:1288 | 1569:1288 | Nvidia          | GK208B [GeForce GT 720]  | 50%    | 4.9.60   | 7E9CD09A5D |
| 10de:1288 | 19da:720a | Nvidia          | GK208B [GeForce GT 720]  | 66.7%  | 4.15.0   | AD88B9D524 |
| 10de:128b | 1043:8572 | Nvidia          | GK208B [GeForce GT 710]  | 4.9%   | 4.1.25   | 7902B95176 |
| 10de:128b | 1043:85f7 | Nvidia          | GK208B [GeForce GT 710]  | 20%    | 4.9.60   | 08A7929F4A |
| 10de:1380 | 1043:84bb | Nvidia          | GM107 [GeForce GTX 75... | 16%    | 4.4.0    | 6400689A90 |
| 10de:1380 | 1043:84bc | Nvidia          | GM107 [GeForce GTX 75... | 16.7%  | 4.1.25   | 59CCFFE44E |
| 10de:1380 | 10de:8412 | Nvidia          | GM107 [GeForce GTX 75... | 100%   |          | 3A624021F2 |
| 10de:1380 | 1458:362d | Nvidia          | GM107 [GeForce GTX 75... | 12%    | 4.1.25   | C67CC4D736 |
| 10de:1380 | 1458:3667 | Nvidia          | GM107 [GeForce GTX 75... | 50%    | 4.9.20   | EEB7663AF0 |
| 10de:1380 | 1462:3102 | Nvidia          | GM107 [GeForce GTX 75... | 18.8%  | 4.1.15   | 6158505A7F |
| 10de:1380 | 1642:3e32 | Nvidia          | GM107 [GeForce GTX 75... | 25%    | 4.15.0   | E5BFC5E8A5 |
| 10de:1380 | 1acc:752e | Nvidia          | GM107 [GeForce GTX 75... | 100%   |          | 356C1804FA |
| 10de:1381 | 1043:84f0 | Nvidia          | GM107 [GeForce GTX 750]  | 12.5%  | 4.1.15   | 8E80E31C5C |
| 10de:1381 | 10de:1073 | Nvidia          | GM107 [GeForce GTX 750]  | 14.3%  | 4.9.20   | 02666C5333 |
| 10de:1381 | 1458:362e | Nvidia          | GM107 [GeForce GTX 750]  | 50%    | 4.1.16   | FED7D6BB61 |
| 10de:1381 | 1458:3642 | Nvidia          | GM107 [GeForce GTX 750]  | 16.7%  | 4.1.15   | 8276D533D6 |
| 10de:1381 | 1462:8a9c | Nvidia          | GM107 [GeForce GTX 750]  | 29.4%  | 4.1.25   | DF2090C762 |
| 10de:13b6 | 1028:17b0 | Nvidia          | GM107GLM [Quadro M120... | 100%   |          | 9C4C70327E |
| 10de:13bb | 10de:1098 | Nvidia          | GM107GL [Quadro K620]    | 10%    | 4.13.0   | 840133169F |
| 10de:13c0 | 1043:8506 | Nvidia          | GM204 [GeForce GTX 980]  | 100%   |          | 3063855C7C |
| 10de:13c2 | 1019:1029 | Nvidia          | GM204 [GeForce GTX 970]  | 100%   |          | F39DBBFB9A |
| 10de:13c2 | 1043:8508 | Nvidia          | GM204 [GeForce GTX 970]  | 5.9%   | 4.15.0   | 3DD9F6A674 |
| 10de:13c2 | 10de:1131 | Nvidia          | GM204 [GeForce GTX 970]  | 80%    | 4.1.15   | 4CC243C7EF |
| 10de:13c2 | 1458:367a | Nvidia          | GM204 [GeForce GTX 970]  | 8.3%   | 4.1.15   | 3E15147646 |
| 10de:13c2 | 1458:367b | Nvidia          | GM204 [GeForce GTX 970]  | 50%    | 5.4.0    | 37FD9139AF |
| 10de:13c2 | 1462:3160 | Nvidia          | GM204 [GeForce GTX 970]  | 12.5%  | 4.15.0   | 7980C33879 |
| 10de:13c2 | 19da:1366 | Nvidia          | GM204 [GeForce GTX 970]  | 28.6%  | 4.15.0   | F3869139DC |
| 10de:13c2 | 3842:2974 | Nvidia          | GM204 [GeForce GTX 970]  | 25%    | 4.15.0   | 3251848CE3 |
| 10de:13c2 | 3842:2978 | Nvidia          | GM204 [GeForce GTX 970]  | 20%    | 4.1.15   | 3251848CE3 |
| 10de:13f1 | 10de:1153 | Nvidia          | GM204GL [Quadro M4000]   | 50%    | 5.4.0    | B8D85B966B |
| 10de:1401 | 1043:8526 | Nvidia          | GM206 [GeForce GTX 960]  | 100%   |          | 05A4F713EA |
| 10de:1401 | 1458:36aa | Nvidia          | GM206 [GeForce GTX 960]  | 100%   |          | 1CFE050B29 |
| 10de:1401 | 1458:36ad | Nvidia          | GM206 [GeForce GTX 960]  | 50%    | 5.0.0    | A8A89AC09A |
| 10de:1401 | 1458:36b0 | Nvidia          | GM206 [GeForce GTX 960]  | 100%   |          | B99D4A956B |
| 10de:1401 | 1462:3202 | Nvidia          | GM206 [GeForce GTX 960]  | 25%    | 4.1.15   | 1532D55BA0 |
| 10de:1401 | 1462:3205 | Nvidia          | GM206 [GeForce GTX 960]  | 50%    | 5.0.0    | 7D2485C593 |
| 10de:1401 | 3842:2966 | Nvidia          | GM206 [GeForce GTX 960]  | 50%    | 5.4.0    | 33DA9C195D |
| 10de:1406 | 1028:072b | Nvidia          | GM206 [GeForce GTX 96... | 100%   |          | 4B9D75483A |
| 10de:1617 | 1043:1ced | Nvidia          | GM204M [GeForce GTX 9... | 100%   |          | 6BCCA7D246 |
| 10de:17c2 | 10de:1132 | Nvidia          | GM200 [GeForce GTX TI... | 100%   |          | 2369E0376D |
| 10de:1b06 | 1043:85e2 | Nvidia          | GP102 [GeForce GTX 10... | 33.3%  | 5.5.15   | 5D1A48EE4E |
| 10de:1b06 | 3842:6696 | Nvidia          | GP102 [GeForce GTX 10... | 20%    | 4.18.0   | 35DAE7072E |
| 10de:1b80 | 1043:8592 | Nvidia          | GP104 [GeForce GTX 1080] | 50%    | 4.15.0   | 974C88BAC1 |
| 10de:1b80 | 10de:1b80 | Nvidia          | GP104 [GeForce GTX 1080] | 25%    | 4.18.0   | F7D08CE703 |
| 10de:1b80 | 1458:3717 | Nvidia          | GP104 [GeForce GTX 1080] | 33.3%  | 4.15.0   | 3F1B997D89 |
| 10de:1b80 | 1462:3367 | Nvidia          | GP104 [GeForce GTX 1080] | 30.8%  | 4.12.14  | A81EFB1774 |
| 10de:1b80 | 3842:5180 | Nvidia          | GP104 [GeForce GTX 1080] | 100%   |          | 31BF3FAE67 |
| 10de:1b81 |           | Nvidia          | GP104 [GeForce GTX 1070] | 50%    | 4.9.20   | D326BF619F |
| 10de:1b81 | 1043:8597 | Nvidia          | GP104 [GeForce GTX 1070] | 100%   |          | 90D8E62525 |
| 10de:1b81 | 1043:859f | Nvidia          | GP104 [GeForce GTX 1070] | 100%   |          | D68BCE418A |
| 10de:1b81 | 1043:85a0 | Nvidia          | GP104 [GeForce GTX 1070] | 16.7%  | 4.15.0   | 691E406FAF |
| 10de:1b81 | 10b0:1b81 | Nvidia          | GP104 [GeForce GTX 1070] | 100%   |          | 8FB6824328 |
| 10de:1b81 | 1458:36fc | Nvidia          | GP104 [GeForce GTX 1070] | 33.3%  | 4.9.20   | CD8505D488 |
| 10de:1b81 | 3842:6276 | Nvidia          | GP104 [GeForce GTX 1070] | 75%    | 4.15.0   | 2162A4B852 |
| 10de:1b82 | 1043:861d | Nvidia          | GP104 [GeForce GTX 10... | 100%   |          | B03C78FE4F |
| 10de:1b82 | 1043:8623 | Nvidia          | GP104 [GeForce GTX 10... | 33.3%  | 5.0.0    | 510B031CE9 |
| 10de:1b82 | 1462:c307 | Nvidia          | GP104 [GeForce GTX 10... | 100%   |          | 17BCC983CA |
| 10de:1b82 | 19da:2445 | Nvidia          | GP104 [GeForce GTX 10... | 33.3%  | 5.2.4    | B499AA651F |
| 10de:1b82 | 3842:5671 | Nvidia          | GP104 [GeForce GTX 10... | 33.3%  | 4.15.0   | BFDE779CB2 |
| 10de:1be1 | 103c:846a | Nvidia          | GP104BM [GeForce GTX ... | 100%   |          | 28EE5CFE8C |
| 10de:1be1 | 1462:11ff | Nvidia          | GP104BM [GeForce GTX ... | 50%    | 5.3.0    | C2E855B5BC |
| 10de:1be1 | 1558:67a4 | Nvidia          | GP104BM [GeForce GTX ... | 33.3%  | 4.18.0   | ADFAFBA25E |
| 10de:1c02 |           | Nvidia          | GP106 [GeForce GTX 10... | 70%    | 4.15.0   | A248371C4D |
| 10de:1c02 | 103c:82fc | Nvidia          | GP106 [GeForce GTX 10... | 66.7%  | 4.15.0   | B084532F5D |
| 10de:1c02 | 1043:85b1 | Nvidia          | GP106 [GeForce GTX 10... | 33.3%  | 4.15.0   | 39F3C43A6B |
| 10de:1c02 | 10de:11c2 | Nvidia          | GP106 [GeForce GTX 10... | 22.2%  | 4.15.0   | 391C431DE9 |
| 10de:1c02 | 10de:1c02 | Nvidia          | GP106 [GeForce GTX 10... | 33.3%  | 4.15.0   | AC3662FF5F |
| 10de:1c02 | 1458:3722 | Nvidia          | GP106 [GeForce GTX 10... | 3.4%   | 4.15.0   | CC9A8D1703 |
| 10de:1c02 | 1458:3724 | Nvidia          | GP106 [GeForce GTX 10... | 11.1%  | 4.15.0   | 4736EC35EF |
| 10de:1c02 | 1462:3287 | Nvidia          | GP106 [GeForce GTX 10... | 5.9%   | 4.13.0   | CCB4D48D08 |
| 10de:1c02 | 1462:8c95 | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | 778D35D82D |
| 10de:1c02 | 3842:6162 | Nvidia          | GP106 [GeForce GTX 10... | 50%    | 4.18.16  | FCC69B7D1E |
| 10de:1c03 |           | Nvidia          | GP106 [GeForce GTX 10... | 18.2%  | 4.15.0   | 8FC4603F6C |
| 10de:1c03 | 1043:85a4 | Nvidia          | GP106 [GeForce GTX 10... | 25%    | 4.15.0   | 725B24FE69 |
| 10de:1c03 | 1043:85a6 | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | EB6CD37E93 |
| 10de:1c03 | 1043:85ae | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | 5385F57036 |
| 10de:1c03 | 1043:85e0 | Nvidia          | GP106 [GeForce GTX 10... | 28.6%  | 4.18.16  | 2C9527A545 |
| 10de:1c03 | 10de:0401 | Nvidia          | GP106 [GeForce GTX 10... | 50%    | 5.3.0    | 54D159FE98 |
| 10de:1c03 | 10de:1c03 | Nvidia          | GP106 [GeForce GTX 10... | 30%    | 4.15.0   | 186DBB4515 |
| 10de:1c03 | 1458:3716 | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | 8E3EE6F0BA |
| 10de:1c03 | 1458:371a | Nvidia          | GP106 [GeForce GTX 10... | 11.1%  | 4.15.0   | 740AB53EE9 |
| 10de:1c03 | 1458:3739 | Nvidia          | GP106 [GeForce GTX 10... | 50%    | 4.15.0   | 1DDF0EC6EC |
| 10de:1c03 | 1458:3776 | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | 28D68A2C46 |
| 10de:1c03 | 1462:3281 | Nvidia          | GP106 [GeForce GTX 10... | 33.3%  | 4.15.0   | E044F153CE |
| 10de:1c03 | 1462:3283 | Nvidia          | GP106 [GeForce GTX 10... | 7.1%   | 4.13.0   | 9043D81B30 |
| 10de:1c03 | 196e:119f | Nvidia          | GP106 [GeForce GTX 10... | 50%    | 5.0.0    | B7F1DC4760 |
| 10de:1c03 | 19da:1438 | Nvidia          | GP106 [GeForce GTX 10... | 40%    | 4.18.0   | F3869139DC |
| 10de:1c03 | 3842:6163 | Nvidia          | GP106 [GeForce GTX 10... | 20%    | 4.15.0   | D94180D023 |
| 10de:1c81 | 103c:8338 | Nvidia          | GP107 [GeForce GTX 1050] | 11.8%  | 4.15.0   | 3673691CB2 |
| 10de:1c81 | 10de:11c0 | Nvidia          | GP107 [GeForce GTX 1050] | 57.1%  | 4.15.0   | 1276D33239 |
| 10de:1c81 | 10de:1c81 | Nvidia          | GP107 [GeForce GTX 1050] | 50%    | 4.18.0   | 6E08766029 |
| 10de:1c81 | 1458:372c | Nvidia          | GP107 [GeForce GTX 1050] | 50%    | 4.15.0   | 1A7DB52C9A |
| 10de:1c81 | 1458:372d | Nvidia          | GP107 [GeForce GTX 1050] | 42.9%  | 4.15.0   | CAFF866F87 |
| 10de:1c81 | 1458:3765 | Nvidia          | GP107 [GeForce GTX 1050] | 21.1%  | 4.15.0   | 2FEBF6828E |
| 10de:1c81 | 1458:3766 | Nvidia          | GP107 [GeForce GTX 1050] | 42.9%  | 4.15.0   | 98EFC397D8 |
| 10de:1c81 | 1462:3354 | Nvidia          | GP107 [GeForce GTX 1050] | 33.3%  | 5.3.0    | 844A6EF03C |
| 10de:1c81 | 1462:8c97 | Nvidia          | GP107 [GeForce GTX 1050] | 30.8%  | 4.15.0   | 9784B3BFB0 |
| 10de:1c81 | 174b:5454 | Nvidia          | GP107 [GeForce GTX 1050] | 50%    | 4.15.0   | 42EF2AA13B |
| 10de:1c81 | 19da:2454 | Nvidia          | GP107 [GeForce GTX 1050] | 50%    | 4.15.0   | F67985779A |
| 10de:1c81 | 3842:6150 | Nvidia          | GP107 [GeForce GTX 1050] | 100%   |          | F2560038AF |
| 10de:1c82 | 1043:85d3 | Nvidia          | GP107 [GeForce GTX 10... | 75%    | 4.15.0   | 79B1E21D1A |
| 10de:1c82 | 1043:85d6 | Nvidia          | GP107 [GeForce GTX 10... | 25%    | 4.15.0   | E48D3747A9 |
| 10de:1c82 | 1043:85fb | Nvidia          | GP107 [GeForce GTX 10... | 100%   |          | 16C69C53FF |
| 10de:1c82 | 1043:85ff | Nvidia          | GP107 [GeForce GTX 10... | 14.3%  | 4.15.0   | 4FF6F8B306 |
| 10de:1c82 | 1043:8613 | Nvidia          | GP107 [GeForce GTX 10... | 20%    | 4.15.0   | 4F0A8E2C5B |
| 10de:1c82 | 1043:8627 | Nvidia          | GP107 [GeForce GTX 10... | 50%    | 4.15.0   | 70C1FC426A |
| 10de:1c82 | 1043:862a | Nvidia          | GP107 [GeForce GTX 10... | 25%    | 4.15.0   | F08CE9BD47 |
| 10de:1c82 | 10b0:1c82 | Nvidia          | GP107 [GeForce GTX 10... | 100%   |          | 85FF8C6337 |
| 10de:1c82 | 10de:11bf | Nvidia          | GP107 [GeForce GTX 10... | 8.7%   | 4.15.0   | CAAC292542 |
| 10de:1c82 | 10de:1c82 | Nvidia          | GP107 [GeForce GTX 10... | 28%    | 4.15.0   | F2CA33243F |
| 10de:1c82 | 1458:3729 | Nvidia          | GP107 [GeForce GTX 10... | 66.7%  | 4.15.0   | D18B737840 |
| 10de:1c82 | 1458:3733 | Nvidia          | GP107 [GeForce GTX 10... | 25%    | 4.15.0   | E510EC2AB5 |
| 10de:1c82 | 1462:3351 | Nvidia          | GP107 [GeForce GTX 10... | 20.8%  | 4.12.14  | B2CD0963B2 |
| 10de:1c82 | 1462:8c96 | Nvidia          | GP107 [GeForce GTX 10... | 13.3%  | 4.15.0   | 51D1991329 |
| 10de:1c82 | 19da:2454 | Nvidia          | GP107 [GeForce GTX 10... | 20%    | 4.15.0   | 1FE17AADBB |
| 10de:1c8d | 1043:11d1 | Nvidia          | GP107M [GeForce GTX 1... | 20%    | 4.15.0   | C2FD6ACB71 |
| 10de:1c91 | 103c:86d4 | Nvidia          | GP107M [GeForce GTX 1... | 50%    | 5.5.3    | 9E3950795E |
| 10de:1cb1 | 10de:11bc | Nvidia          | GP107GL [Quadro P1000]   | 100%   |          | 555F102847 |
| 10de:1cb6 | 1028:1264 | Nvidia          | GP107GL [Quadro P620]    | 100%   |          | AD29AF92C2 |
| 10de:1cbb | 103c:842f | Nvidia          | GP107GLM [Quadro P100... | 100%   |          | 93F2B3D9A8 |
| 10de:1d01 | 1043:85f4 | Nvidia          | GP108 [GeForce GT 1030]  | 23.5%  | 4.15.0   | 04C0BFBF31 |
| 10de:1d01 | 1043:85f5 | Nvidia          | GP108 [GeForce GT 1030]  | 50%    | 4.15.0   | C9B3B14E25 |
| 10de:1d01 | 1043:8642 | Nvidia          | GP108 [GeForce GT 1030]  | 100%   |          | 1AD00E6974 |
| 10de:1d01 | 10de:1d01 | Nvidia          | GP108 [GeForce GT 1030]  | 21.4%  | 4.15.0   | C97547ED2D |
| 10de:1d01 | 1458:375c | Nvidia          | GP108 [GeForce GT 1030]  | 21.4%  | 4.15.0   | 1D55DAA69C |
| 10de:1d01 | 1462:8c98 | Nvidia          | GP108 [GeForce GT 1030]  | 18.4%  | 4.15.0   | C854817725 |
| 10de:1d01 | 19da:1476 | Nvidia          | GP108 [GeForce GT 1030]  | 50%    | 4.18.0   | 2B0D032DAD |
| 10de:1e02 | 10de:12a3 | Nvidia          | TU102 [TITAN RTX]        | 50%    | 5.6.10   | 30502C41DE |
| 10de:1e04 | 1458:37c4 | Nvidia          | TU102 [GeForce RTX 20... | 100%   |          | 931EA9A398 |
| 10de:1e07 | 1462:3711 | Nvidia          | TU102 [GeForce RTX 20... | 100%   |          | 62128222FA |
| 10de:1e07 | 1462:3715 | Nvidia          | TU102 [GeForce RTX 20... | 100%   |          | CE19512CBB |
| 10de:1e07 | 19da:1503 | Nvidia          | TU102 [GeForce RTX 20... | 100%   |          | C8FDC5E958 |
| 10de:1e07 | 3842:2487 | Nvidia          | TU102 [GeForce RTX 20... | 100%   |          | C3DCC51002 |
| 10de:1e30 | 1028:12ba | Nvidia          | TU102GL [Quadro RTX 6... | 20%    | 5.3.0    | 71F7A877F7 |
| 10de:1e81 | 3842:3287 | Nvidia          | TU104 [GeForce RTX 20... | 100%   |          | 3DA3A9D9AD |
| 10de:1e82 | 1043:8676 | Nvidia          | TU104 [GeForce RTX 2080] | 100%   |          | 48041296CA |
| 10de:1e82 | 10b0:1e87 | Nvidia          | TU104 [GeForce RTX 2080] | 100%   |          | 73CF7CEE79 |
| 10de:1e82 | 1462:3722 | Nvidia          | TU104 [GeForce RTX 2080] | 100%   |          | ACBAD1E6CE |
| 10de:1e87 | 1458:37a8 | Nvidia          | TU104 [GeForce RTX 20... | 100%   |          | AAD0551E27 |
| 10de:1eb1 | 1028:12a0 | Nvidia          | TU104GL [Quadro RTX 4... | 100%   |          | 0015ED3AE7 |
| 10de:1eb1 | 10de:12a0 | Nvidia          | TU104GL [Quadro RTX 4... | 100%   |          | B95F8101E5 |
| 10de:1f02 | 10de:1f02 | Nvidia          | TU106 [GeForce RTX 2070] | 100%   |          | C8C1A01026 |
| 10de:1f02 | 1458:37c8 | Nvidia          | TU106 [GeForce RTX 2070] | 100%   |          | 69F2264D39 |
| 10de:1f06 | 7377:0000 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | 82D130EB39 |
| 10de:1f07 | 1043:8670 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | AF6DA5211E |
| 10de:1f07 | 1043:8671 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | AC29A018F8 |
| 10de:1f07 | 10de:12ad | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | 55119E58D9 |
| 10de:1f07 | 1462:3732 | Nvidia          | TU106 [GeForce RTX 20... | 42.9%  | 5.0.0    | 95EB08349E |
| 10de:1f08 | 10de:1f08 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | 3CF95EC244 |
| 10de:1f08 | 1458:37d9 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | 364918C615 |
| 10de:1f08 | 1458:3fc2 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | 8DF2C93C38 |
| 10de:1f08 | 1458:3fd1 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | 4BF53BD278 |
| 10de:1f08 | 196e:130f | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | 328F236B37 |
| 10de:1f08 | 3842:2167 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | 32073E3911 |
| 10de:1f11 | 103c:8574 | Nvidia          | TU106M [GeForce RTX 2... | 100%   |          | 29CB9464AE |
| 10de:1f11 | 1043:140f | Nvidia          | TU106M [GeForce RTX 2... | 50%    | 5.3.0    | EFC1AC12C7 |
| 10de:1f47 | 10de:13ad | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | E0192EBFC1 |
| 10de:1f50 | 103c:8574 | Nvidia          | TU106BM [GeForce RTX ... | 100%   |          | E31EFEB24C |
| 10de:1f50 | 103c:8603 | Nvidia          | TU106BM [GeForce RTX ... | 100%   |          | 8295B3DB5F |
| 10de:1f82 | 10de:1320 | Nvidia          | TU117 [GeForce GTX 1650] | 100%   |          | CF74B1C03F |
| 10de:1f82 | 1462:3800 | Nvidia          | TU117 [GeForce GTX 1650] | 100%   |          | 9C0406B489 |
| 10de:1f91 | 103c:86d5 | Nvidia          | TU117M [GeForce GTX 1... | 75%    | 5.3.0    | B8F65D2C87 |
| 10de:1f91 | 1043:109f | Nvidia          | TU117M [GeForce GTX 1... | 71.4%  | 5.3.0    | D028A90A2A |
| 10de:1f91 | 17aa:3ffb | Nvidia          | TU117M [GeForce GTX 1... | 50%    | 5.3.0    | 642E6B2B6A |
| 10de:1f95 | 1043:16df | Nvidia          | TU117M [GeForce GTX 1... | 100%   |          | 326D9506FD |
| 10de:1fb9 | 103c:860e | Nvidia          | TU117GLM [Quadro T100... | 100%   |          | DC6E4DA9DE |
| 10de:2182 | 1043:86a3 | Nvidia          | TU116 [GeForce GTX 16... | 100%   |          | E891AAE560 |
| 10de:2182 | 10de:2182 | Nvidia          | TU116 [GeForce GTX 16... | 66.7%  | 5.6.15   | BC6B5804C2 |
| 10de:2182 | 1458:3fbe | Nvidia          | TU116 [GeForce GTX 16... | 100%   |          | F50C460937 |
| 10de:2182 | 1462:3750 | Nvidia          | TU116 [GeForce GTX 16... | 100%   |          | 9E2420DAD2 |
| 10de:2182 | 1462:375a | Nvidia          | TU116 [GeForce GTX 16... | 16.7%  | 5.3.0    | CA561AA481 |
| 10de:2184 | 10de:1324 | Nvidia          | TU116 [GeForce GTX 1660] | 100%   |          | 72F0115ACA |
| 10de:2184 | 10de:1366 | Nvidia          | TU116 [GeForce GTX 1660] | 100%   |          | 2F657D538C |
| 10de:2184 | 1458:3fc7 | Nvidia          | TU116 [GeForce GTX 1660] | 100%   |          | C4C123186E |
| 10de:2184 | 1462:3792 | Nvidia          | TU116 [GeForce GTX 1660] | 10%    | 5.3.0    | 705949F6E0 |
| 10de:2184 | 1462:8d91 | Nvidia          | TU116 [GeForce GTX 1660] | 50%    | 5.3.11   | C38867C0EF |
| 10de:2184 | 7377:150a | Nvidia          | TU116 [GeForce GTX 1660] | 100%   |          | 30939907C1 |
| 10de:2187 | 3842:1357 | Nvidia          | TU116 [GeForce GTX 16... | 100%   |          | F36075AAA0 |
| 10de:2191 | 103c:8574 | Nvidia          | TU116M [GeForce GTX 1... | 100%   |          | A85470AC70 |
| 10de:2191 | 1043:10af | Nvidia          | TU116M [GeForce GTX 1... | 50%    | 5.6.7    | 9C797156F9 |
| 10de:2191 | 1043:16cf | Nvidia          | TU116M [GeForce GTX 1... | 100%   |          | 2DFF24F03C |
| 8086:0042 | 1849:0042 | Intel           | Core Processor Integr... | 7.1%   | 3.14.33  | 1D9934126C |
| 8086:0102 | 17aa:3078 | Intel           | 2nd Generation Core P... | 7.1%   | 4.15.0   | 735EE0A048 |
| 8086:0106 | 1025:0504 | Intel           | 2nd Generation Core P... | 3%     | 4.1.38   | 8FE3AF49FB |
| 8086:0152 | 1043:84ca | Intel           | Xeon E3-1200 v2/3rd G... | 1.1%   | 3.10.34  | 44E0CE8FC8 |
| 8086:0162 | 1028:052c | Intel           | Xeon E3-1200 v2/3rd G... | 10%    | 4.15.0   | 29A0FC6CE0 |
| 8086:0162 | 1043:84ca | Intel           | Xeon E3-1200 v2/3rd G... | 10%    | 3.14.44  | C7C6CD6D36 |
| 8086:0166 | 1025:0647 | Intel           | 3rd Gen Core processo... | 0.6%   | 3.10.34  | 86D2D3B0E1 |
| 8086:0166 | 17aa:21fb | Intel           | 3rd Gen Core processo... | 11.1%  | 4.15.0   | 55427995B5 |
| 8086:0412 | 1462:7816 | Intel           | Xeon E3-1200 v3/4th G... | 11.1%  | 4.9.20   | 093472BA51 |
| 8086:041a | 1462:7823 | Intel           | Xeon E3-1200 v3 Proce... | 100%   |          | 7755195EF6 |
| 8086:0be2 | 8086:2012 | Intel           | Atom Processor D2xxx/... | 16.7%  | 3.14.44  | DB58FCA753 |
| 8086:0f31 | 1025:0936 | Intel           | Atom Processor Z36xxx... | 4%     | 4.12.14  | 1718CF1D36 |
| 8086:0f31 | 1458:d000 | Intel           | Atom Processor Z36xxx... | 9.1%   | 3.10.0   | D4999D1DCD |
| 8086:0f31 | 17aa:3695 | Intel           | Atom Processor Z36xxx... | 50%    | 4.15.0   | 08BB09B100 |
| 8086:1616 | 1025:1019 | Intel           | HD Graphics 5500         | 100%   |          | 5DBE9649A7 |
| 8086:1902 | 1043:8694 | Intel           | HD Graphics 510          | 7.9%   | 4.8.14   | A91734714E |
| 8086:1902 | 1462:7996 | Intel           | HD Graphics 510          | 11.1%  | 4.9.20   | BFAA613B9E |
| 8086:1902 | 8086:2212 | Intel           | HD Graphics 510          | 100%   |          | FF56929B10 |
| 8086:1912 | 1043:8694 | Intel           | HD Graphics 530          | 6.2%   | 4.4.0    | 81DBEC3DF4 |
| 8086:1912 | 1458:d000 | Intel           | HD Graphics 530          | 17.1%  | 4.9.41   | 53E6A4F263 |
| 8086:1912 | 1734:121c | Intel           | HD Graphics 530          | 25%    | 4.12.14  | 19202ED9BC |
| 8086:1912 | 1849:1912 | Intel           | HD Graphics 530          | 4.5%   | 4.3.3    | 42FACB50D6 |
| 8086:1916 | 1025:0985 | Intel           | Skylake GT2 [HD Graph... | 50%    | 5.3.0    | 01210C0B0E |
| 8086:1916 | 1025:1094 | Intel           | Skylake GT2 [HD Graph... | 3.6%   | 4.9.9    | E7D6077756 |
| 8086:1916 | 1028:06de | Intel           | Skylake GT2 [HD Graph... | 4.3%   | 4.12.14  | AE7AD1E7D9 |
| 8086:1916 | 1028:06fd | Intel           | Skylake GT2 [HD Graph... | 20%    | 4.15.0   | 569785286A |
| 8086:1916 | 103c:8079 | Intel           | Skylake GT2 [HD Graph... | 3%     | 4.1.15   | 82F5250E0D |
| 8086:1916 | 103c:80a4 | Intel           | Skylake GT2 [HD Graph... | 7.1%   | 4.9.60   | B01FB51118 |
| 8086:1916 | 103c:80ff | Intel           | Skylake GT2 [HD Graph... | 33.3%  | 4.7.2    | B7B039F46E |
| 8086:1916 | 103c:8100 | Intel           | Skylake GT2 [HD Graph... | 12.5%  | 4.15.0   | 2B56F34E21 |
| 8086:1916 | 103c:8101 | Intel           | Skylake GT2 [HD Graph... | 3%     | 4.9.60   | BC496704F4 |
| 8086:1916 | 103c:820c | Intel           | Skylake GT2 [HD Graph... | 25%    | 4.9.20   | FAE1CD27F3 |
| 8086:1916 | 1043:1ccd | Intel           | Skylake GT2 [HD Graph... | 8%     | 4.9.20   | A4B26975E9 |
| 8086:1916 | 1179:f822 | Intel           | Skylake GT2 [HD Graph... | 25%    | 4.15.0   | B781D8419A |
| 8086:1916 | 17aa:3824 | Intel           | Skylake GT2 [HD Graph... | 3.7%   | 4.9.9    | 412EAC636F |
| 8086:1916 | 17aa:382c | Intel           | Skylake GT2 [HD Graph... | 10%    | 4.9.0    | 18379EBD5C |
| 8086:1916 | 17aa:5048 | Intel           | Skylake GT2 [HD Graph... | 20%    | 4.15.0   | 842B139FE7 |
| 8086:191b | 1028:06de | Intel           | HD Graphics 530          | 4.5%   | 4.15.0   | BC4C6EBBA7 |
| 8086:191b | 1043:1080 | Intel           | HD Graphics 530          | 16.7%  | 4.15.0   | 5B1076EA3C |
| 8086:191b | 1043:1d6d | Intel           | HD Graphics 530          | 20%    | 5.4.0    | 9D6C0DD372 |
| 8086:191b | 1462:1190 | Intel           | HD Graphics 530          | 14.3%  | 4.9.9    | 2B70AAB06F |
| 8086:1921 | 17aa:39e8 | Intel           | HD Graphics 520          | 20%    | 4.9.111  | C3352134E9 |
| 8086:22b1 | 1025:1012 | Intel           | Atom/Celeron/Pentium ... | 3.8%   | 4.9.20   | 16D1C62342 |
| 8086:22b1 | 1028:0725 | Intel           | Atom/Celeron/Pentium ... | 12.5%  | 4.9.20   | 92DCC778AC |
| 8086:22b1 | 1043:10c0 | Intel           | Atom/Celeron/Pentium ... | 2%     | 4.9.9    | E6AFAB9B56 |
| 8086:22b1 | 1558:0945 | Intel           | Atom/Celeron/Pentium ... | 4.5%   | 4.1.15   | BDAF59B6EB |
| 8086:2572 | 103c:12bc | Intel           | 82865G Integrated Gra... | 11.1%  | 4.1.34   | DD4DD47556 |
| 8086:2772 | 8086:464c | Intel           | 82945G/GZ Integrated ... | 32.3%  | 3.10.0   | 947354716F |
| 8086:27a2 | 1025:0107 | Intel           | Mobile 945GM/GMS, 943... | 50%    | 4.1.34   | 290DB67DA7 |
| 8086:27a2 | 104d:820f | Intel           | Mobile 945GM/GMS, 943... | 33.3%  | 3.14.44  | 811EFEE1FC |
| 8086:27a2 | 1462:0341 | Intel           | Mobile 945GM/GMS, 943... | 22.2%  | 4.1.15   | C71F72F074 |
| 8086:2992 | 1734:10b5 | Intel           | 82Q963/Q965 Integrate... | 15.4%  | 4.1.15   | BF1BADE95D |
| 8086:29b2 | 1028:0211 | Intel           | 82Q35 Express Integra... | 2%     | 3.14.44  | C1582B3202 |
| 8086:2a12 | 103c:3618 | Intel           | Mobile GME965/GLE960 ... | 10.5%  | 3.14.44  | 13824A2872 |
| 8086:2a42 | 1631:018b | Intel           | Mobile 4 Series Chips... | 14.3%  | 5.0.0    | 96A6F21797 |
| 8086:2e12 | 1025:0151 | Intel           | 4 Series Chipset Inte... | 33.3%  | 5.3.0    | 96ED3B9CA2 |
| 8086:2e12 | 1028:027f | Intel           | 4 Series Chipset Inte... | 1.1%   | 3.14.44  | BDF53B02DC |
| 8086:2e12 | 17aa:3048 | Intel           | 4 Series Chipset Inte... | 22.2%  | 4.1.15   | 53336C3457 |
| 8086:2e32 | 1025:0390 | Intel           | 4 Series Chipset Inte... | 12.5%  | 4.15.0   | 112E50B08C |
| 8086:2e32 | 8086:d612 | Intel           | 4 Series Chipset Inte... | 33.3%  | 4.15.0   | 48AB47DFE5 |
| 8086:3e90 | 1458:d000 | Intel           | CoffeeLake-S GT1 [UHD... | 30.8%  | 4.15.0   | A174DA5BA2 |
| 8086:3e91 | 1043:8694 | Intel           | CoffeeLake-S GT2 [UHD... | 10%    | 4.15.0   | DA54361164 |
| 8086:3e91 | 1849:3e91 | Intel           | CoffeeLake-S GT2 [UHD... | 7.7%   | 4.15.0   | 59151791CF |
| 8086:3e92 | 1025:126c | Intel           | CometLake-S GT2 [UHD ... | 100%   |          | C1339E884A |
| 8086:3e92 | 1028:0851 | Intel           | CometLake-S GT2 [UHD ... | 100%   |          | 05D6B79D2F |
| 8086:3e92 | 1028:0930 | Intel           | CometLake-S GT2 [UHD ... | 33.3%  | 4.15.0   | C2BF735906 |
| 8086:3e92 | 103c:843c | Intel           | CometLake-S GT2 [UHD ... | 50%    | 5.1.3    | E5E15DF58D |
| 8086:3e92 | 1043:8694 | Intel           | CometLake-S GT2 [UHD ... | 2%     | 4.15.0   | 0B771C098E |
| 8086:3e92 | 1458:d000 | Intel           | CometLake-S GT2 [UHD ... | 1.6%   | 4.14.0   | DA58706E3D |
| 8086:3e98 | 1043:8694 | Intel           | CoffeeLake-S GT2 [UHD... | 2.9%   | 4.18.0   | 50FB2D34F9 |
| 8086:3e98 | 1462:7b98 | Intel           | CoffeeLake-S GT2 [UHD... | 50%    | 5.3.0    | 297E534CF0 |
| 8086:3e9b | 1025:1264 | Intel           | CoffeeLake-H GT2 [UHD... | 1.8%   | 4.15.0   | C4FA903BED |
| 8086:3e9b | 1462:126a | Intel           | CoffeeLake-H GT2 [UHD... | 25%    | 3.10.0   | 039A05F3EB |
| 8086:3ea0 | 1028:08a8 | Intel           | WhiskeyLake-U GT2 [UH... | 11.1%  | 4.15.0   | B6DF9FEC5F |
| 8086:5902 | 1849:5902 | Intel           | HD Graphics 610          | 7.7%   | 4.9.60   | 9E7024131D |
| 8086:5912 | 1028:0764 | Intel           | HD Graphics 630          | 100%   |          | 530CC43BE2 |
| 8086:5912 | 1043:8694 | Intel           | HD Graphics 630          | 0.8%   | 4.4.0    | B0DE2CBA6A |
| 8086:5912 | 1458:d000 | Intel           | HD Graphics 630          | 1.6%   | 3.10.0   | 6126E55D1A |
| 8086:5916 | 1028:075b | Intel           | HD Graphics 620          | 2.9%   | 4.4.0    | 6695D2A05E |
| 8086:5916 | 1028:0768 | Intel           | HD Graphics 620          | 4.8%   | 4.9.9    | 2BB9B79D2E |
| 8086:5916 | 1028:0782 | Intel           | HD Graphics 620          | 12.5%  | 4.18.0   | 49389100FC |
| 8086:5916 | 17aa:39f1 | Intel           | HD Graphics 620          | 5.9%   | 4.9.60   | 32F19AB04D |
| 8086:5916 | 8086:2212 | Intel           | HD Graphics 620          | 3.2%   | 4.9.41   | B1A55C7D69 |
| 8086:5917 | 17aa:225e | Intel           | UHD Graphics 620         | 7.1%   | 4.15.0   | 7D7E6AD5D5 |
| 8086:591b | 1028:07bf | Intel           | HD Graphics 630          | 5.9%   | 4.15.0   | 26DBEC9F3A |
| 8086:5a85 | 8086:7270 | Intel           | HD Graphics 500          | 20%    | 4.4.59   | 622CED4019 |
| 8086:8108 | 1028:02b1 | Intel           | US15W/US15X SCH [Poul... | 100%   |          | 7D4473A4A5 |
| 8086:8a52 | 1028:097c | Intel           | Iris Plus Graphics G7    | 50%    | 5.3.0    | 66554C2B07 |
| 8086:8a52 | 17aa:3ff1 | Intel           | Iris Plus Graphics G7    | 40%    | 5.3.0    | 3F4D79EA3B |
| 8086:8a56 | 1025:1422 | Intel           | Iris Plus Graphics G1... | 100%   |          | 69AEFC61B7 |
| 8086:8a56 | 1028:0979 | Intel           | Iris Plus Graphics G1... | 11.1%  | 5.0.0    | 7F4CE08DF9 |
| 8086:8a5a | 103c:86c8 | Intel           | Iris Plus Graphics G4... | 50%    | 5.4.8    | 16DBE6C7CF |
| 8086:9b41 | 1028:0954 | Intel           | CometLake-U GT2 [UHD ... | 100%   |          | 8740133E10 |
| 8086:9b41 | 17aa:382f | Intel           | CometLake-U GT2 [UHD ... | 14.3%  | 5.3.0    | E6E2F26ADE |
| 8086:9bca | 1462:129c | Intel           | Comet Lake UHD Graphics  | 7.7%   | 5.3.0    | 754F3C176F |
| 8086:9bca | 8086:2081 | Intel           | Comet Lake UHD Graphics  | 30%    | 5.3.0    | F2BFE6BFB3 |
| 8086:a001 | 1043:83e6 | Intel           | Atom Processor D4xx/D... | 37.5%  | 4.18.13  | 47E870B0B9 |
| 8086:a001 | 1458:d000 | Intel           | Atom Processor D4xx/D... | 23.1%  | 3.10.0   | 2ECE09C60B |
| 8086:a001 | 8086:4f4d | Intel           | Atom Processor D4xx/D... | 3.3%   | 3.10.0   | E20797F817 |
| 8086:a011 | 1462:104e | Intel           | Atom Processor D4xx/D... | 20%    | 4.1.15   | 5F15F028A8 |

### Modem (PCI)

63 out of 119 (52.94%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1002:4378 | 103c:3085 | AMD             | IXP SB400 AC'97 Modem... | 50%    | 5.0.0    | 31A6AA1E70 |
| 1039:7013 | 1025:0082 | Silicon Inte... | AC'97 Modem Controller   | 100%   |          | F8F0BBDD75 |
| 1039:7013 | 1025:0083 | Silicon Inte... | AC'97 Modem Controller   | 100%   |          | D131965BA5 |
| 1039:7013 | 1043:1696 | Silicon Inte... | AC'97 Modem Controller   | 100%   |          | D385784B22 |
| 1039:7013 | 1043:1816 | Silicon Inte... | AC'97 Modem Controller   | 58.3%  | 3.14.25  | AA92B168C5 |
| 1039:7013 | 104d:814e | Silicon Inte... | AC'97 Modem Controller   | 50%    | 3.14.44  | 11D39BBA01 |
| 1039:7013 | 1558:4201 | Silicon Inte... | AC'97 Modem Controller   | 100%   |          | 5B191FE82E |
| 1039:7013 | 1734:106c | Silicon Inte... | AC'97 Modem Controller   | 100%   |          | B66AF54651 |
| 1057:3052 | 1057:3020 | Motorola        | SM56 Data Fax Modem      | 100%   |          | 5198626553 |
| 1057:3052 | 1631:3034 | Motorola        | SM56 Data Fax Modem      | 100%   |          | B7CEC1644D |
| 10b9:5457 | 103c:0850 | ULi Electronics | M5457 AC'97 Modem Con... | 100%   |          | 4E9D284D9C |
| 10b9:5457 | 104d:8158 | ULi Electronics | M5457 AC'97 Modem Con... | 100%   |          | 7E4F74E16A |
| 10de:00d9 | 103c:006d | Nvidia          | nForce3 Audio            | 100%   |          | 10266A11DF |
| 10de:00d9 | 1043:1856 | Nvidia          | nForce3 Audio            | 50%    | 4.9.60   | 0A302BFAFD |
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
| 2003:8800 | 1801:2800 | Smart Link      | LM-I56N                  | 100%   |          | 62AFB6C0F6 |
| 8086:1040 | 8086:1000 | Intel           | 536EP Data Fax Modem     | 100%   |          | 279C8E8873 |
| 8086:2446 | 1025:1027 | Intel           | 82801BA/BAM AC'97 Mod... | 100%   |          | E0A83557FF |
| 8086:2486 | 1014:0223 | Intel           | 82801CA/CAM AC'97 Mod... | 50%    | 4.9.0    | B6D0B8758E |
| 8086:2486 | 1043:1496 | Intel           | 82801CA/CAM AC'97 Mod... | 100%   |          | 1E7DA431AF |
| 8086:2486 | 134d:4c21 | Intel           | 82801CA/CAM AC'97 Mod... | 100%   |          | F56665D93F |
| 8086:2486 | 14f1:5421 | Intel           | 82801CA/CAM AC'97 Mod... | 100%   |          | 4F9273C63C |
| 8086:24c6 | 1014:0524 | Intel           | 82801DB/DBL/DBM (ICH4... | 100%   |          | 8716809D07 |
| 8086:24c6 | 1014:0559 | Intel           | 82801DB/DBL/DBM (ICH4... | 85.7%  | 3.14.53  | 58F9CE5671 |
| 8086:24c6 | 1014:055a | Intel           | 82801DB/DBL/DBM (ICH4... | 16.7%  | 3.14.44  | 190737F754 |
| 8086:24c6 | 103c:3080 | Intel           | 82801DB/DBL/DBM (ICH4... | 50%    | 4.19.0   | 6802B34FDD |
| 8086:24c6 | 103c:3084 | Intel           | 82801DB/DBL/DBM (ICH4... | 100%   |          | 24A093E347 |
| 8086:24c6 | 107b:0360 | Intel           | 82801DB/DBL/DBM (ICH4... | 100%   |          | 53EC93715E |
| 8086:24c6 | 10cf:10d1 | Intel           | 82801DB/DBL/DBM (ICH4... | 66.7%  | 3.14.25  | EA732BEA27 |
| 8086:24c6 | 1179:0001 | Intel           | 82801DB/DBL/DBM (ICH4... | 66.7%  | 4.9.0    | B36ADF3084 |
| 8086:24c6 | 1179:ff31 | Intel           | 82801DB/DBL/DBM (ICH4... | 80%    | 4.1.38   | E9BD04F647 |
| 8086:24c6 | 14f1:5422 | Intel           | 82801DB/DBL/DBM (ICH4... | 30.8%  | 3.14.44  | 1629FF31A1 |
| 8086:24c6 | 1584:4007 | Intel           | 82801DB/DBL/DBM (ICH4... | 100%   |          | F13A21C874 |
| 8086:24c6 | 1734:103c | Intel           | 82801DB/DBL/DBM (ICH4... | 100%   |          | 6F452862B4 |
| 8086:24d6 | 1025:0045 | Intel           | 82801EB/ER (ICH5/ICH5... | 100%   |          | 41CC7EB08C |
| 8086:24d6 | 1179:0001 | Intel           | 82801EB/ER (ICH5/ICH5... | 100%   |          | A7D4DEEF9E |
| 8086:266d | 1014:0574 | Intel           | 82801FB/FBM/FR/FW/FRW... | 88.9%  | 4.9.41   | 5DB408D966 |
| 8086:266d | 1014:0576 | Intel           | 82801FB/FBM/FR/FW/FRW... | 50%    | 3.14.33  | 9809E004BA |
| 8086:266d | 1025:0066 | Intel           | 82801FB/FBM/FR/FW/FRW... | 63.6%  | 3.14.44  | 50122B9E8E |
| 8086:266d | 1025:006a | Intel           | 82801FB/FBM/FR/FW/FRW... | 61.5%  | 3.14.25  | 93DAE491F3 |
| 8086:266d | 103c:0934 | Intel           | 82801FB/FBM/FR/FW/FRW... | 100%   |          | 453696FF5E |
| 8086:266d | 103c:0944 | Intel           | 82801FB/FBM/FR/FW/FRW... | 40%    | 3.14.44  | 0D21AAC1C0 |
| 8086:266d | 103c:099c | Intel           | 82801FB/FBM/FR/FW/FRW... | 12.5%  | 3.14.44  | C60AB5C121 |
| 8086:266d | 103c:3080 | Intel           | 82801FB/FBM/FR/FW/FRW... | 50%    | 4.9.9    | 0572E8425C |
| 8086:266d | 103c:3081 | Intel           | 82801FB/FBM/FR/FW/FRW... | 40%    | 5.3.0    | DC4B912BFC |
| 8086:266d | 103c:3082 | Intel           | 82801FB/FBM/FR/FW/FRW... | 100%   |          | 34CDD00D12 |
| 8086:266d | 103c:309d | Intel           | 82801FB/FBM/FR/FW/FRW... | 33.3%  | 4.1.16   | 837230178B |
| 8086:266d | 103c:30c4 | Intel           | 82801FB/FBM/FR/FW/FRW... | 50%    | 4.1.25   | 87F8EF65AE |
| 8086:266d | 107b:0460 | Intel           | 82801FB/FBM/FR/FW/FRW... | 100%   |          | B62ECA10E8 |
| 8086:266d | 1179:0001 | Intel           | 82801FB/FBM/FR/FW/FRW... | 85.3%  | 3.14.44  | 0B1D1EC461 |
| 8086:266d | 144d:2115 | Intel           | 82801FB/FBM/FR/FW/FRW... | 40%    | 4.1.22   | 88BAF3B388 |
| 8086:266d | 14f1:5423 | Intel           | 82801FB/FBM/FR/FW/FRW... | 60.9%  | 3.14.44  | B171C8B34D |
| 8086:266d | 1631:c00b | Intel           | 82801FB/FBM/FR/FW/FRW... | 100%   |          | CCD46D5757 |
| 8086:266d | 17aa:207c | Intel           | 82801FB/FBM/FR/FW/FRW... | 100%   |          | EDAE63A429 |

### Multimedia controller (PCI)

219 out of 291 (75.26%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 0002:8290 | 107d:2609 |                 | Multimedia controller    | 100%   |          | 95D420F37F |
| 1002:4d51 | 1002:b041 | AMD             | Unified AVStream         | 100%   |          | E0EE188631 |
| 1002:4d52 | 1002:a346 | AMD             | Theater 550 PRO PCI [... | 100%   |          | FDE418F259 |
| 1002:ac12 | 1002:b539 | AMD             | Theater HD T507 (DVB-... | 100%   |          | 6D32273098 |
| 1002:ac12 | 12ab:0003 | AMD             | Theater HD T507 (DVB-... | 100%   |          | D9801ADC43 |
| 1002:ad18 | 1682:ad18 | AMD             | Multimedia controller    | 100%   |          | 3108FE53D3 |
| 1022:15e2 | 1022:15e2 | AMD             | Raven/Raven2/FireFlig... | 51.4%  | 4.19.8   | 326B11F044 |
| 1022:15e2 | 1025:1233 | AMD             | Raven/Raven2/FireFlig... | 62.5%  | 5.0.0    | 856A212CAA |
| 1022:15e2 | 1025:134d | AMD             | Raven/Raven2/FireFlig... | 10%    | 5.0.0    | C8AD593834 |
| 1022:15e2 | 1025:134f | AMD             | Raven/Raven2/FireFlig... | 22.2%  | 5.0.0    | 84EB1C787C |
| 1022:15e2 | 1025:1378 | AMD             | Raven/Raven2/FireFlig... | 16.7%  | 5.3.0    | 0255FCB566 |
| 1022:15e2 | 103c:8433 | AMD             | Raven/Raven2/FireFlig... | 20%    | 5.0.0    | 9C77CCAA74 |
| 1022:15e2 | 103c:8434 | AMD             | Raven/Raven2/FireFlig... | 85.7%  | 5.0.0    | E2E650868B |
| 1022:15e2 | 103c:8496 | AMD             | Raven/Raven2/FireFlig... | 25%    | 5.0.0    | 53B6114671 |
| 1022:15e2 | 103c:84a3 | AMD             | Raven/Raven2/FireFlig... | 100%   |          | 6A706DA421 |
| 1022:15e2 | 103c:84ae | AMD             | Raven/Raven2/FireFlig... | 58.1%  | 5.0.0    | 82B33EB923 |
| 1022:15e2 | 103c:84d2 | AMD             | Raven/Raven2/FireFlig... | 80%    | 5.3.0    | BEFFBD7414 |
| 1022:15e2 | 103c:85b3 | AMD             | Raven/Raven2/FireFlig... | 50%    | 5.0.0    | A3E0E0B6C7 |
| 1022:15e2 | 103c:85dd | AMD             | Raven/Raven2/FireFlig... | 8.3%   | 5.0.0    | 99A3D955A1 |
| 1022:15e2 | 103c:85e0 | AMD             | Raven/Raven2/FireFlig... | 25%    | 5.0.0    | BB8A4C9967 |
| 1022:15e2 | 103c:85ea | AMD             | Raven/Raven2/FireFlig... | 25%    | 5.0.0    | D81C93199C |
| 1022:15e2 | 103c:86d4 | AMD             | Raven/Raven2/FireFlig... | 40%    | 5.4.0    | 31D470AF54 |
| 1022:15e2 | 103c:86d5 | AMD             | Raven/Raven2/FireFlig... | 14.3%  | 5.3.0    | F08BA4BE83 |
| 1022:15e2 | 103c:86d6 | AMD             | Raven/Raven2/FireFlig... | 50%    | 5.5.5    | 48487463EB |
| 1022:15e2 | 103c:8706 | AMD             | Raven/Raven2/FireFlig... | 100%   |          | 270ACBB2D4 |
| 1022:15e2 | 17aa:36f5 | AMD             | Raven/Raven2/FireFlig... | 75%    | 5.5.9    | 7E41940C9C |
| 1022:15e2 | 17aa:380b | AMD             | Raven/Raven2/FireFlig... | 61.5%  | 5.3.0    | 932B22C52A |
| 1022:15e2 | 17aa:3811 | AMD             | Raven/Raven2/FireFlig... | 66.7%  | 5.0.0    | 8CFF91E24B |
| 1022:15e2 | 17aa:3812 | AMD             | Raven/Raven2/FireFlig... | 26.5%  | 5.0.0    | 654460DA6F |
| 1022:15e2 | 17aa:3813 | AMD             | Raven/Raven2/FireFlig... | 40%    | 5.0.0    | B98809B4F8 |
| 1022:15e2 | 17aa:3814 | AMD             | Raven/Raven2/FireFlig... | 34.8%  | 5.0.0    | 05E6C3C6BC |
| 1022:15e2 | 17aa:381b | AMD             | Raven/Raven2/FireFlig... | 16.7%  | 5.4.0    | 73DF23B815 |
| 1022:15e2 | 17aa:381f | AMD             | Raven/Raven2/FireFlig... | 66.7%  | 5.4.0    | F48BFBD65A |
| 1022:15e2 | 17aa:3821 | AMD             | Raven/Raven2/FireFlig... | 31.2%  | 5.4.0    | 73C01BEF24 |
| 1022:15e2 | 17aa:5124 | AMD             | Raven/Raven2/FireFlig... | 25.9%  | 5.0.0    | DEBE15CBE6 |
| 1022:15e2 | 17aa:5126 | AMD             | Raven/Raven2/FireFlig... | 33.3%  | 5.0.0    | D8E43B34CC |
| 1022:15e2 | 17aa:5127 | AMD             | Raven/Raven2/FireFlig... | 45.5%  | 5.4.0    | FD09B801B7 |
| 1022:15e2 | 19e5:3e06 | AMD             | Raven/Raven2/FireFlig... | 47.8%  | 5.0.0    | C3EB69A876 |
| 1022:15e2 | 19e5:3e10 | AMD             | Raven/Raven2/FireFlig... | 12.5%  | 5.3.0    | 042C4B3C5A |
| 1022:15e2 | 19e5:3e18 | AMD             | Raven/Raven2/FireFlig... | 18.2%  | 5.3.0    | 1EF79C4312 |
| 1022:15e2 | 1d72:1953 | AMD             | Raven/Raven2/FireFlig... | 100%   |          | E38BDAE28D |
| 1022:15e2 | 1e21:1043 | AMD             | Raven/Raven2/FireFlig... | 16.7%  | 5.0.0    | CCEC718F4B |
| 102b:8350 | 102b:9000 | Matrox Elect... | Matrox Multimedia con... | 100%   |          | B3EE98B7CC |
| 1057:1801 |           | Motorola        | DSP56301 Digital Sign... | 100%   |          | 13CA73B9A3 |
| 1057:3410 | 1057:ffff | Motorola        | DSP56361 Digital Sign... | 100%   |          | 16A7890585 |
| 1057:3410 | 11af:eed2 | Motorola        | DSP56361 Digital Sign... | 100%   |          | 16A7890585 |
| 1057:3410 | 11af:eee1 | Motorola        | DSP56361 Digital Sign... | 100%   |          | 16A7890585 |
| 109e:0878 |           | Brooktree       | Bt878 Audio Capture      | 97.7%  | 5.3.0    | B55D1DAEA5 |
| 109e:0878 | 0070:ff02 | Brooktree       | Bt878 Audio Capture      | 100%   |          | 84495E0FB8 |
| 109e:0878 | 0070:ff04 | Brooktree       | Bt878 Audio Capture      | 100%   |          | 2C877CF870 |
| 109e:0878 | 1002:0003 | Brooktree       | Bt878 Audio Capture      | 100%   |          | 74635460A2 |
| 109e:0878 | 1047:f331 | Brooktree       | Bt878 Audio Capture      | 100%   |          | 444FFBC8A6 |
| 109e:0878 | 107d:6607 | Brooktree       | Bt878 Audio Capture      | 75%    | 4.9.20   | 502C4EB91B |
| 109e:0878 | 107d:6609 | Brooktree       | Bt878 Audio Capture      | 100%   |          | E29BC9AC9D |
| 109e:0878 | 11bd:0012 | Brooktree       | Bt878 Audio Capture      | 25%    | 4.1.34   | ECA8E2E768 |
| 109e:0878 | 1461:0001 | Brooktree       | Bt878 Audio Capture      | 100%   |          | E8072B6F3A |
| 109e:0878 | 1461:0002 | Brooktree       | Bt878 Audio Capture      | 100%   |          | A22609B54B |
| 109e:0878 | 1461:0003 | Brooktree       | Bt878 Audio Capture      | 4.3%   | 3.14.25  | 7A69435C43 |
| 109e:0878 | 1461:0004 | Brooktree       | Bt878 Audio Capture      | 100%   |          | F2B7867CAA |
| 109e:0878 | 153b:1118 | Brooktree       | Bt878 Audio Capture      | 100%   |          | DDFD3CC319 |
| 109e:0878 | 800a:763d | Brooktree       | Bt878 Audio Capture      | 100%   |          | 08DCF9AA49 |
| 109e:0878 | 800b:763d | Brooktree       | Bt878 Audio Capture      | 100%   |          | 08DCF9AA49 |
| 109e:0878 | 800c:763d | Brooktree       | Bt878 Audio Capture      | 100%   |          | 08DCF9AA49 |
| 109e:0878 | 800d:763d | Brooktree       | Bt878 Audio Capture      | 100%   |          | 08DCF9AA49 |
| 109e:0878 | aa03:1433 | Brooktree       | Bt878 Audio Capture      | 100%   |          | ABDBF93DB4 |
| 109e:0878 | aaff:1431 | Brooktree       | Bt878 Audio Capture      | 100%   |          | ABDBF93DB4 |
| 109e:0878 | bd11:4100 | Brooktree       | Bt878 Audio Capture      | 100%   |          | 34BC4E6EF8 |
| 109e:0878 | ffff:ffff | Brooktree       | Bt878 Audio Capture      | 100%   |          | A4B2A57CC3 |
| 10b5:9056 | 1a0e:006f | PLX Technology  | PCI9056 32-bit 66MHz ... | 100%   |          | C6B09D560F |
| 10b5:9056 | 1a0e:0073 | PLX Technology  | PCI9056 32-bit 66MHz ... | 50%    | 4.15.0   | 5122F7EE54 |
| 10cf:202a | 104d:81fa | Fujitsu Limi... | Integrated MPEG Encoder  | 100%   |          | 7F0BB0CC92 |
| 10cf:2030 | 104d:9053 | Fujitsu Limi... | Fujitsu Multimedia co... | 100%   |          | CFDCAC5734 |
| 10cf:2030 | 104d:9062 | Fujitsu Limi... | Fujitsu Multimedia co... | 100%   |          | 2628EBE1BB |
| 10cf:2036 | 10fc:d05f | Fujitsu Limi... | DT-XXX                   | 100%   |          | 2485335459 |
| 10cf:2036 | 1718:190d | Fujitsu Limi... | DT-XXX                   | 100%   |          | 15202A6CAE |
| 1131:5402 | 4954:5434 | Philips Semi... | TriMedia TM1300          | 100%   |          | 64A9C1D635 |
| 1131:7160 | 107d:6686 | Philips Semi... | SAA7160                  | 100%   |          | 5BA05AC282 |
| 1131:7160 | 1131:0002 | Philips Semi... | SAA7160                  | 100%   |          | 26B6AC3832 |
| 1131:7160 | 1461:0455 | Philips Semi... | SAA7160                  | 100%   |          | F85808C04C |
| 1131:7160 | 1461:0555 | Philips Semi... | SAA7160                  | 100%   |          | C47AD5ED50 |
| 1131:7160 | 1461:0655 | Philips Semi... | SAA7160                  | 100%   |          | 58A8ECB02A |
| 1131:7160 | 1461:0855 | Philips Semi... | SAA7160                  | 100%   |          | BBDA8BED86 |
| 1131:7160 | 1461:0955 | Philips Semi... | SAA7160                  | 100%   |          | A24FCCA14F |
| 1131:7160 | 1461:0a55 | Philips Semi... | SAA7160                  | 100%   |          | 6F6DE0E938 |
| 1131:7160 | 1461:0e55 | Philips Semi... | SAA7160                  | 100%   |          | 7669D59151 |
| 1131:7160 | 1461:0f55 | Philips Semi... | SAA7160                  | 100%   |          | ED65E40A12 |
| 1131:7160 | 1461:1055 | Philips Semi... | SAA7160                  | 100%   |          | 10708BAA81 |
| 1131:7160 | 1461:1455 | Philips Semi... | SAA7160                  | 100%   |          | 3D49020A7B |
| 1131:7160 | 1461:1855 | Philips Semi... | SAA7160                  | 100%   |          | FA070462FC |
| 1131:7160 | 1461:2355 | Philips Semi... | SAA7160                  | 100%   |          | B98B8362E0 |
| 1131:7160 | 1461:2655 | Philips Semi... | SAA7160                  | 100%   |          | A74B989748 |
| 1131:7160 | 1461:7561 | Philips Semi... | SAA7160                  | 100%   |          | A010F0A8F5 |
| 1131:7160 | 1461:7992 | Philips Semi... | SAA7160                  | 100%   |          | 3ACD33354F |
| 1131:7160 | 16be:0034 | Philips Semi... | SAA7160                  | 100%   |          | 2B8D93B7EC |
| 1131:7160 | 17de:7542 | Philips Semi... | SAA7160                  | 100%   |          | 4B00918B63 |
| 1131:7160 | 185b:e750 | Philips Semi... | SAA7160                  | 100%   |          | 891F7E03D0 |
| 1131:7160 | 1ae4:0700 | Philips Semi... | SAA7160                  | 100%   |          | 0E34CA887E |
| 1131:7160 | 6281:0001 | Philips Semi... | SAA7160                  | 11.1%  | 4.9.76   | 30EC426B43 |
| 1131:7160 | 6928:0001 | Philips Semi... | SAA7160                  | 100%   |          | 8C8F8EFAB1 |
| 1131:7160 | 6928:0002 | Philips Semi... | SAA7160                  | 100%   |          | 885E9722DE |
| 1131:7160 | e517:12ab | Philips Semi... | SAA7160                  | 100%   |          | 786069DE60 |
| 1131:7160 | e519:12ab | Philips Semi... | SAA7160                  | 100%   |          | 786069DE60 |
| 1131:7162 | 11bd:0100 | Philips Semi... | SAA7162                  | 100%   |          | D495DD5272 |
| 1131:7162 | 11bd:0101 | Philips Semi... | SAA7162                  | 100%   |          | CBDA057D39 |
| 1131:7164 | 0070:8851 | Philips Semi... | SAA7164                  | 16.7%  | 3.14.22  | 9E32F34F8E |
| 1131:7231 | 0070:0810 | Philips Semi... | SAA7231                  | 100%   |          | 6AC7D4C49F |
| 1131:7231 | 12ab:0762 | Philips Semi... | SAA7231                  | 100%   |          | 6D27B996FD |
| 1131:7231 | 12ab:0763 | Philips Semi... | SAA7231                  | 100%   |          | 20768D0E33 |
| 1131:7231 | 1461:0b0f | Philips Semi... | SAA7231                  | 100%   |          | 254FB0C969 |
| 1131:7231 | 1461:110f | Philips Semi... | SAA7231                  | 100%   |          | 90DFBFB6FA |
| 1131:7231 | 1461:1400 | Philips Semi... | SAA7231                  | 100%   |          | 70C319B3C6 |
| 1131:7231 | 1461:2a0f | Philips Semi... | SAA7231                  | 100%   |          | 8D3C2E38D3 |
| 1131:7231 | 1461:2b07 | Philips Semi... | SAA7231                  | 100%   |          | 8672A3F85D |
| 1131:7231 | 1461:2b0f | Philips Semi... | SAA7231                  | 100%   |          | 6E0B7C86D5 |
| 1131:7231 | 1461:3301 | Philips Semi... | SAA7231                  | 100%   |          | 7E1176A7C2 |
| 1131:7231 | 1461:7981 | Philips Semi... | SAA7231                  | 100%   |          | 4E796E1984 |
| 1131:7231 | 1461:7983 | Philips Semi... | SAA7231                  | 100%   |          | 6186ACA9BB |
| 1131:7231 | 1461:890f | Philips Semi... | SAA7231                  | 100%   |          | 4C97361FFD |
| 1131:7231 | 16be:0002 | Philips Semi... | SAA7231                  | 100%   |          | 650300C6BF |
| 1131:7231 | 16be:0008 | Philips Semi... | SAA7231                  | 100%   |          | 6B4999F818 |
| 1131:7231 | 16be:0013 | Philips Semi... | SAA7231                  | 100%   |          | 065A4D0713 |
| 1131:7231 | 1b0a:3001 | Philips Semi... | SAA7231                  | 100%   |          | 5EFEDE21E2 |
| 1131:7231 | 5ace:8000 | Philips Semi... | SAA7231                  | 100%   |          | FA070462FC |
| 1131:7231 | 5ace:8150 | Philips Semi... | SAA7231                  | 100%   |          | 8603D5BDF5 |
| 1131:7231 | 5ace:8201 | Philips Semi... | SAA7231                  | 100%   |          | 75F255A4E2 |
| 11bd:0040 | 11bd:0045 | Pinnacle Sys... | Royal TS Function 1      | 100%   |          | FF0A7B1FC8 |
| 11bd:0041 | 11bd:0045 | Pinnacle Sys... | RoyalTS Function 2       | 100%   |          | FF0A7B1FC8 |
| 11bd:0042 | 11bd:0045 | Pinnacle Sys... | Royal TS Function 3      | 100%   |          | FF0A7B1FC8 |
| 11bd:bede | 11bd:0022 | Pinnacle Sys... | AV/DV Studio Capture ... | 100%   |          | 5D59A83BEC |
| 11bd:bede | 11bd:0023 | Pinnacle Sys... | AV/DV Studio Capture ... | 100%   |          | 17C83CBEEC |
| 11bd:bede | 11bd:0024 | Pinnacle Sys... | AV/DV Studio Capture ... | 100%   |          | D6BD28C216 |
| 123f:8120 | 10de:01e1 | LSI Logic       | DVxplore Codec           | 100%   |          | BF588FC977 |
| 127e:0010 | 127e:0010 | Winnov, L.P.    | Videum 1000 Plus         | 100%   |          | 37BC71433C |
| 12ab:0371 | 1cfa:000b | YUAN High-Te... | Game Capture 4K60 Pro    | 100%   |          | F7FB56CA93 |
| 12ab:0371 | 1cfa:000c | YUAN High-Te... | Game Capture 4K60 Pro    | 100%   |          | F7FB56CA93 |
| 12ab:0380 | 1cfa:0006 | YUAN High-Te... | Game Capture 4K60 Pro    | 100%   |          | CF5CF7D297 |
| 12ab:0710 | f718:0001 | YUAN High-Te... | Multimedia controller    | 100%   |          | 4E0D80B779 |
| 14b5:0200 |           | Creamware       | Scope                    | 100%   |          | 0FB4C2BDDA |
| 14b5:0300 |           | Creamware       | Pulsar                   | 100%   |          | 0FB4C2BDDA |
| 14b5:0600 | 14b5:0600 | Creamware       | Pulsar2                  | 100%   |          | 0FB4C2BDDA |
| 14e4:1570 | 14e4:1570 | Broadcom        | 720p FaceTime HD Camera  | 25.6%  | 4.15.0   | 4D62DBBF1A |
| 14e4:1612 | 14e4:2612 | Broadcom        | BCM70012 Video Decode... | 100%   |          | 5495F2E86E |
| 14e4:1615 | 1028:048b | Broadcom Lim... | BCM70015 Video Decode... | 100%   |          | 8081C2D2D3 |
| 14e4:1615 | 105b:0d77 | Broadcom        | BCM70015 Video Decode... | 100%   |          | B036D312E6 |
| 14e4:1615 | 14e4:1615 | Broadcom        | BCM70015 Video Decode... | 93.3%  | 5.3.0    | 580DBABC2C |
| 14f1:8002 | 14f1:0084 | Conexant Sys... | Conexant Multimedia c... | 100%   |          | 380140EB8D |
| 14f1:8803 | 185b:e000 | Conexant Sys... | CX2388x TV Capture Chip  | 100%   |          | 5B85C2F248 |
| 14f1:8804 | 0070:1402 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | BD036704BD |
| 14f1:8804 | 0070:6902 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | B4A53FAFC1 |
| 14f1:8804 | 0070:6906 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | BCEE476272 |
| 14f1:8804 | 0070:9002 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | 1351C7B098 |
| 14f1:8804 | 0070:9202 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | 3005D3D129 |
| 14f1:8804 | 0070:9402 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | 38EA92C05C |
| 14f1:8804 | 1822:0023 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | AB36F565A4 |
| 1745:2100 | 1043:48b0 | ViXS Systems    | XCode 2100 Series        | 100%   |          | AD1D92439F |
| 1745:2100 | 1043:48d1 | ViXS Systems    | XCode 2100 Series        | 100%   |          | 4B00918B63 |
| 1745:3000 | 0070:d180 | ViXS Systems    | Colossus Encoder         | 100%   |          | 669767B92E |
| 1745:3000 | 104d:9049 | ViXS Systems    | Colossus Encoder         | 100%   |          | 2628EBE1BB |
| 1797:6805 |           | Intersil Tec... | HV4000 DVR card          | 100%   |          | B2C845B843 |
| 1797:6805 | 1797:6804 | Intersil Tec... | HV4000 DVR card          | 100%   |          | B2C845B843 |
| 1797:6814 | 000a:6814 | Intersil Tec... | TW6816 multimedia vid... | 100%   |          | D455CC3322 |
| 1797:6815 | 000a:6815 | Intersil Tec... | TW6816 multimedia vid... | 100%   |          | D455CC3322 |
| 1797:6816 | 000a:6816 | Intersil Tec... | TW6816 multimedia vid... | 100%   |          | D455CC3322 |
| 1797:6817 | 000a:6817 | Intersil Tec... | TW6816 multimedia vid... | 100%   |          | D455CC3322 |
| 1822:4e35 | 1822:0048 | Twinhan Tech... | Mantis DTV PCI Bridge... | 100%   |          | CB1A0D9CDD |
| 1a00:0001 | 1a00:0001 |                 | Multimedia controller    | 100%   |          | 16A7890585 |
| 544d:6178 | 6205:0001 | TBS Technolo... | DVB Tuner PCIe Card      | 100%   |          | AFAA3A3830 |
| 544d:6178 | 6209:0001 | TBS Technolo... | DVB Tuner PCIe Card      | 100%   |          | C7E1E32971 |
| 544d:6178 | 6902:0002 | TBS Technolo... | DVB Tuner PCIe Card      | 100%   |          | B58CD9FD67 |
| 8086:0f38 | 8086:0f31 | Intel           | Atom Processor Z36xxx... | 66.7%  | 4.12.4   | 0A0191D0D3 |
| 8086:0f38 | 8086:7270 | Intel           | Atom Processor Z36xxx... | 93.3%  | 5.0.0    | 0A96B79D5F |
| 8086:1919 | 1025:111e | Intel           | Xeon E3-1200 v5/E3-15... | 80%    | 5.4.11   | 2D71938FC4 |
| 8086:1919 | 1028:06e6 | Intel           | Xeon E3-1200 v5/E3-15... | 5.3%   | 5.0.0    | 1ABBA3CDA0 |
| 8086:1919 | 1028:07a4 | Intel           | Xeon E3-1200 v5/E3-15... | 23.1%  | 5.0.0    | AA661DFC05 |
| 8086:1919 | 1028:07a5 | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | 87A44EF029 |
| 8086:1919 | 1028:081d | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | B1CC9FA911 |
| 8086:1919 | 103c:80fc | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | C0F3526E69 |
| 8086:1919 | 103c:8146 | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | 3C4E95F3C6 |
| 8086:1919 | 103c:828b | Intel           | Xeon E3-1200 v5/E3-15... | 60%    | 5.3.0    | 4EEA42AD05 |
| 8086:1919 | 103c:82cb | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | FDB567A59E |
| 8086:1919 | 144d:c135 | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | D7B5599247 |
| 8086:1919 | 144d:c14f | Intel           | Xeon E3-1200 v5/E3-15... | 20%    | 5.0.0    | F9D5F8F1CD |
| 8086:1919 | 152d:1182 | Intel           | Xeon E3-1200 v5/E3-15... | 40%    | 5.0.0    | 5D3C8DA69A |
| 8086:1919 | 17aa:2241 | Intel           | Xeon E3-1200 v5/E3-15... | 33.3%  | 5.5.4    | 1038A34C39 |
| 8086:1919 | 17aa:3812 | Intel           | Xeon E3-1200 v5/E3-15... | 66.7%  | 5.3.0    | AAEF1C5AE7 |
| 8086:1919 | 17aa:382f | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | 1DD80D33E5 |
| 8086:1919 | 19e5:3e00 | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | A76E9D9514 |
| 8086:1919 | 8086:1919 | Intel           | Xeon E3-1200 v5/E3-15... | 38.5%  | 5.0.0    | 422797E8D2 |
| 8086:1919 | 8086:2015 | Intel           | Xeon E3-1200 v5/E3-15... | 48%    | 5.0.0    | CAAF2A34B9 |
| 8086:22b8 | 1025:1021 | Intel           | Atom/Celeron/Pentium ... | 50%    | 5.0.0    | 663247803F |
| 8086:22b8 | 1025:106e | Intel           | Atom/Celeron/Pentium ... | 100%   |          | 425D589D65 |
| 8086:22b8 | 1025:113a | Intel           | Atom/Celeron/Pentium ... | 100%   |          | FBF9B74A34 |
| 8086:22b8 | 1028:06ea | Intel           | Atom/Celeron/Pentium ... | 60%    | 4.20.1   | 743979C6E7 |
| 8086:22b8 | 103c:813e | Intel           | Atom/Celeron/Pentium ... | 17.6%  | 5.0.0    | 923CBD5735 |
| 8086:22b8 | 103c:827c | Intel           | Atom/Celeron/Pentium ... | 41.2%  | 5.0.0    | 163F3173C7 |
| 8086:22b8 | 1043:13a0 | Intel           | Atom/Celeron/Pentium ... | 34.6%  | 5.0.0    | 1EB4640C84 |
| 8086:22b8 | 1043:1400 | Intel           | Atom/Celeron/Pentium ... | 41.2%  | 5.0.0    | 838DD8C3AC |
| 8086:22b8 | 1043:1c60 | Intel           | Atom/Celeron/Pentium ... | 20%    | 5.0.0    | 5FCF1662DB |
| 8086:22b8 | 1071:a126 | Intel           | Atom/Celeron/Pentium ... | 100%   |          | F2981C1775 |
| 8086:22b8 | 10cf:1925 | Intel           | Atom/Celeron/Pentium ... | 100%   |          | 6D19311F7E |
| 8086:22b8 | 1297:2063 | Intel           | Atom/Celeron/Pentium ... | 26.1%  | 5.0.0    | 18AE13312B |
| 8086:22b8 | 1414:0009 | Intel           | Atom/Celeron/Pentium ... | 33.3%  | 5.3.0    | 76A25407DE |
| 8086:22b8 | 17aa:222a | Intel           | Atom/Celeron/Pentium ... | 50%    | 5.0.0    | 5AF55E5191 |
| 8086:22b8 | 17aa:3809 | Intel           | Atom/Celeron/Pentium ... | 7.4%   | 5.0.0    | 85AC9B2B53 |
| 8086:22b8 | 17aa:38e3 | Intel           | Atom/Celeron/Pentium ... | 16.7%  | 4.19.110 | D738EDCC09 |
| 8086:22b8 | 8086:7270 | Intel           | Atom/Celeron/Pentium ... | 47.5%  | 4.19.0   | 126A1DE793 |
| 8086:5a88 |           | Intel           | Celeron N3350/Pentium... | 100%   |          | C242DEC3CC |
| 8086:8a19 | 1028:08b0 | Intel           | Image Signal Processor   | 100%   |          | CC9B7372FD |
| 8086:8a19 | 8086:7270 | Intel           | Image Signal Processor   | 100%   |          | 69744692B0 |
| 8086:9d32 |           | Intel           | CSI-2 Host Controller    | 18.2%  | 5.0.0    | C596B50DF9 |
| 8086:9d32 | 1028:07a4 | Intel           | CSI-2 Host Controller    | 15.4%  | 4.18.0   | AA661DFC05 |
| 8086:9d32 | 1028:07a5 | Intel           | CSI-2 Host Controller    | 100%   |          | 87A44EF029 |
| 8086:9d32 | 103c:8146 | Intel           | CSI-2 Host Controller    | 75%    | 5.4.0    | 70ACFD512F |
| 8086:9d32 | 1043:1410 | Intel           | CSI-2 Host Controller    | 100%   |          | 0B5AD4104E |
| 8086:9d32 | 17aa:380c | Intel           | CSI-2 Host Controller    | 33.3%  | 4.18.0   | 1D220D1155 |
| 8086:9d32 | 17aa:3812 | Intel           | CSI-2 Host Controller    | 16.7%  | 5.0.3    | 508333A652 |
| 8086:9d32 | 8086:7270 | Intel           | CSI-2 Host Controller    | 16.6%  | 4.18.0   | 124ECAD1CF |
| 8086:9d32 | 8086:9d32 | Intel           | CSI-2 Host Controller    | 23.1%  | 4.18.0   | 422797E8D2 |
| dd01:0006 | dd01:0022 | Digital Devices | Cine V7                  | 100%   |          | FCF4AFE5C6 |

### Net/ethernet (PCI)

102 out of 4813 (2.12%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 0000:0200 | 002c:0200 |                 | Ethernet controller      | 100%   |          | 32AE4212DF |
| 000c:0000 | 1043:83a3 |                 | Ethernet controller      | 100%   |          | B5189C3BF2 |
| 10ec:0139 | 10bd:0320 | Realtek Semi... | RTL-8139/8139C/8139C+... | 100%   |          | 305C35F50C |
| 10ec:3000 | 1025:132d | Realtek Semi... | Killer E3000 2.5GbE C... | 66.7%  | 5.4.7    | 17674B4CBD |
| 10ec:3000 | 1025:1375 | Realtek Semi... | Killer E3000 2.5GbE C... | 37.5%  | 5.4.5    | F6C3A576C2 |
| 10ec:3000 | 1028:08c4 | Realtek Semi... | Killer E3000 2.5GbE C... | 100%   |          | BA3ACE6663 |
| 10ec:3000 | 1028:093c | Realtek Semi... | Killer E3000 2.5GbE C... | 60%    | 5.4.25   | 5FCBF716A6 |
| 10ec:8125 | 1043:879b | Realtek Semi... | RTL8125 2.5GbE Contro... | 25.9%  | 5.4.0    | DA47170FAE |
| 10ec:8131 | 10ec:8131 | Realtek Semi... | RTL8131 PCIe Fast Eth... | 100%   |          | 4E43962152 |
| 10ec:8136 | 1025:061f | Realtek Semi... | RTL810xE PCI Express ... | 2.2%   | 3.14.44  | ADD6CC4F5F |
| 10ec:8136 | 1028:0555 | Realtek Semi... | RTL810xE PCI Express ... | 4%     | 4.1.15   | A7211B4E35 |
| 10ec:8136 | 1028:0597 | Realtek Semi... | RTL810xE PCI Express ... | 3.3%   | 3.14.25  | 0DD732A269 |
| 10ec:8136 | 1028:06b2 | Realtek Semi... | RTL810xE PCI Express ... | 2.1%   | 4.9.20   | A2E2A6CF66 |
| 10ec:8136 | 1028:0768 | Realtek Semi... | RTL810xE PCI Express ... | 4.8%   | 4.9.9    | 32E3129638 |
| 10ec:8136 | 1028:0810 | Realtek Semi... | RTL810xE PCI Express ... | 2.7%   | 4.4.0    | BE05348BE2 |
| 10ec:8136 | 103c:1484 | Realtek Semi... | RTL810xE PCI Express ... | 5%     | 4.9.60   | C7734FBAE0 |
| 10ec:8136 | 103c:148a | Realtek Semi... | RTL810xE PCI Express ... | 11.8%  | 4.1.38   | A8A7B70079 |
| 10ec:8136 | 103c:184a | Realtek Semi... | RTL810xE PCI Express ... | 1.5%   | 3.14.33  | 581C3578E1 |
| 10ec:8136 | 103c:2213 | Realtek Semi... | RTL810xE PCI Express ... | 3.6%   | 3.14.25  | F6CF1F21DF |
| 10ec:8136 | 103c:226a | Realtek Semi... | RTL810xE PCI Express ... | 6.7%   | 3.14.44  | A50758BDB0 |
| 10ec:8136 | 103c:306b | Realtek Semi... | RTL810xE PCI Express ... | 12.5%  | 3.14.44  | 93C0EF7223 |
| 10ec:8136 | 103c:81f5 | Realtek Semi... | RTL810xE PCI Express ... | 5%     | 4.1.34   | 045809FB67 |
| 10ec:8136 | 103c:81f6 | Realtek Semi... | RTL810xE PCI Express ... | 3.6%   | 4.1.25   | 142457C9EA |
| 10ec:8136 | 103c:820c | Realtek Semi... | RTL810xE PCI Express ... | 25%    | 4.1.25   | 21A7695D56 |
| 10ec:8136 | 1179:f920 | Realtek Semi... | RTL810xE PCI Express ... | 7.7%   | 4.9.9    | 0BC2465C23 |
| 10ec:8136 | 1462:7529 | Realtek Semi... | RTL810xE PCI Express ... | 3.7%   | 3.14.44  | 99777B72F9 |
| 10ec:8136 | 17aa:381f | Realtek Semi... | RTL810xE PCI Express ... | 5.7%   | 4.1.34   | 1952B1CCF3 |
| 10ec:8136 | 17aa:3861 | Realtek Semi... | RTL810xE PCI Express ... | 1.2%   | 4.9.60   | C2D5094A2D |
| 10ec:8168 | 1025:0866 | Realtek Semi... | RTL8111/8168/8411 PCI... | 2.4%   | 3.10.51  | 8B133744C1 |
| 10ec:8168 | 1025:0918 | Realtek Semi... | RTL8111/8168/8411 PCI... | 8.2%   | 4.1.19   | 68E659C87D |
| 10ec:8168 | 1025:0936 | Realtek Semi... | RTL8111/8168/8411 PCI... | 3.7%   | 3.8.0    | A2C7011157 |
| 10ec:8168 | 1025:1238 | Realtek Semi... | RTL8111/8168/8411 PCI... | 2.7%   | 4.15.0   | 3520CCDFCF |
| 10ec:8168 | 1025:125c | Realtek Semi... | RTL8111/8168/8411 PCI... | 1.6%   | 4.15.0   | 6AEFA7E06C |
| 10ec:8168 | 1028:04b8 | Realtek Semi... | RTL8111/8168/8411 PCI... | 12.5%  | 4.15.0   | A993CB7099 |
| 10ec:8168 | 1028:04d9 | Realtek Semi... | RTL8111/8168/8411 PCI... | 11.1%  | 4.15.0   | 6ECDF91891 |
| 10ec:8168 | 1028:0870 | Realtek Semi... | RTL8111/8168/8411 PCI... | 12.5%  | 4.15.0   | B0DF3027CF |
| 10ec:8168 | 103c:180d | Realtek Semi... | RTL8111/8168/8411 PCI... | 3%     | 3.10.42  | 41A6D6B87B |
| 10ec:8168 | 103c:2a94 | Realtek Semi... | RTL8111/8168/8411 PCI... | 5.3%   | 4.1.25   | 33AE5EBABC |
| 10ec:8168 | 103c:831c | Realtek Semi... | RTL8111/8168/8411 PCI... | 9.1%   | 4.9.60   | 854604BDAD |
| 10ec:8168 | 103c:84ac | Realtek Semi... | RTL8111/8168/8411 PCI... | 1.3%   | 4.15.0   | 6EC2D663E5 |
| 10ec:8168 | 1043:1447 | Realtek Semi... | RTL8111/8168/8411 PCI... | 6.7%   | 3.14.44  | F23B5BF0DA |
| 10ec:8168 | 1043:1477 | Realtek Semi... | RTL8111/8168/8411 PCI... | 6.2%   | 4.9.60   | BEE323A814 |
| 10ec:8168 | 1043:14f7 | Realtek Semi... | RTL8111/8168/8411 PCI... | 4.3%   | 3.14.44  | CE99670CEB |
| 10ec:8168 | 1043:200f | Realtek Semi... | RTL8111/8168/8411 PCI... | 0.3%   | 3.10.34  | 4D035C5605 |
| 10ec:8168 | 1043:8432 | Realtek Semi... | RTL8111/8168/8411 PCI... | 0.1%   | 3.0.38   | 58F57667EE |
| 10ec:8168 | 10ec:0123 | Realtek Semi... | RTL8111/8168/8411 PCI... | 0.1%   | 3.10.0   | AF51CAD146 |
| 10ec:8168 | 10ec:8168 | Realtek Semi... | RTL8111/8168/8411 PCI... | 0.3%   | 3.10.0   | 021596F9B3 |
| 10ec:8168 | 1297:2033 | Realtek Semi... | RTL8111/8168/8411 PCI... | 5%     | 4.9.20   | 51273F53DF |
| 10ec:8168 | 1458:e000 | Realtek Semi... | RTL8111/8168/8411 PCI... | 0.1%   | 3.10.0   | 621FF023C5 |
| 10ec:8168 | 1462:10b8 | Realtek Semi... | RTL8111/8168/8411 PCI... | 4%     | 4.1.25   | 1E515A2EC5 |
| 10ec:8168 | 14c0:0059 | Realtek Semi... | RTL8111/8168/8411 PCI... | 25%    | 4.19.0   | 42B3F11A1E |
| 10ec:8168 | 1558:1323 | Realtek Semi... | RTL8111/8168/8411 PCI... | 15.4%  | 4.15.0   | 75848692B4 |
| 10ec:8168 | 1558:1550 | Realtek Semi... | RTL8111/8168/8411 PCI... | 2.2%   | 3.14.33  | A0EB5DA51A |
| 10ec:8168 | 17aa:21fe | Realtek Semi... | RTL8111/8168/8411 PCI... | 9.1%   | 3.10.0   | E17730F707 |
| 10ec:8168 | 17aa:2224 | Realtek Semi... | RTL8111/8168/8411 PCI... | 5.9%   | 4.15.0   | C163822056 |
| 10ec:8168 | 17aa:38c7 | Realtek Semi... | RTL8111/8168/8411 PCI... | 2.2%   | 4.15.0   | E030A286C2 |
| 10ec:8168 | 17aa:5123 | Realtek Semi... | RTL8111/8168/8411 PCI... | 100%   |          | 4DABCB8D3F |
| 10ec:8168 | 17aa:5126 | Realtek Semi... | RTL8111/8168/8411 PCI... | 3.8%   | 4.15.0   | E720C77930 |
| 10ec:8168 | 1849:8168 | Realtek Semi... | RTL8111/8168/8411 PCI... | 0.1%   | 2.6.32   | B87BD193E6 |
| 10ec:8169 | 10ec:8169 | Realtek Semi... | RTL8169 PCI Gigabit E... | 0.6%   | 3.14.22  | 2DBD467937 |
| 1186:4200 | 1186:1103 | D-Link System   | DFE-520TX Fast Ethern... | 100%   |          | 790E740601 |
| 1186:4300 | 1186:4300 | D-Link System   | DGE-528T Gigabit Ethe... | 1.8%   | 3.10.0   | 6BA672F50B |
| 1186:4b01 | 1186:4b01 | D-Link System   | DGE-530T Gigabit Ethe... | 3.3%   | 3.14.44  | F195015CF8 |
| 11ab:4380 | 104d:907a | Marvell Tech... | 88E8057 PCI-E Gigabit... | 15.8%  | 4.9.155  | E6E4689D4B |
| 11ab:4381 | 104d:9071 | Marvell Tech... | Yukon Optima 88E8059 ... | 0.8%   | 3.14.44  | 908BC46E69 |
| 1374:0038 | 1374:0038 | Silicom         | Quad port Copper Ethe... | 100%   |          | 8BE6B42FC7 |
| 14e4:16a3 | 14e4:16a3 | Broadcom        | NetXtreme BCM57786 Gi... | 100%   |          | FE9743907C |
| 14e4:16a3 | 14e4:16b4 | Broadcom        | NetXtreme BCM57786 Gi... | 100%   |          | F0CC1D4EF7 |
| 14e4:16b5 | 1025:0504 | Broadcom        | NetLink BCM57785 Giga... | 0.7%   | 3.10.0   | B377A89C57 |
| 14e4:52a3 | d3a6:afcd | Broadcom Lim... | Ethernet controller      | 100%   |          | 191BA97155 |
| 168c:abcd |           | Qualcomm Ath... | Osprey Emulation Wire... | 100%   |          | 9DB07ADAF8 |
| 168c:ff1a |           | Qualcomm Ath... | Ethernet controller      | 100%   |          | 5ABFB915A2 |
| 1969:1083 | 1025:0686 | Qualcomm Ath... | AR8151 v2.0 Gigabit E... | 1.7%   | 3.14.44  | 910279B054 |
| 1969:e0b1 | 1462:11f2 | Qualcomm Ath... | Killer E2500 Gigabit ... | 20%    | 5.6.0    | 3DDF7394D8 |
| 197b:0250 | 1558:4120 | JMicron Tech... | JMC250 PCI Express Gi... | 12.5%  | 4.15.0   | DBA823C7CC |
| 1a47:0003 | 0000:0200 | 3DSP            | WLAN and Bluetooth Card  | 100%   |          | 3A17145633 |
| 1d6a:00b1 | 1043:874a | Aquantia        | AQC100 10G Ethernet M... | 100%   |          | F5152B2EC1 |
| 1d6a:07b1 | 1043:8757 | Aquantia        | AQC107 NBase-T/IEEE 8... | 11.1%  | 4.15.0   | F5152B2EC1 |
| 1d6a:07b1 | 1462:7c59 | Aquantia        | AQC107 NBase-T/IEEE 8... | 100%   |          | 7539DA519D |
| 1fc9:4027 | 1432:8104 | Tehuti Networks | TN9710P 10GBase-T/NBA... | 100%   |          | 4B605582DF |
| 1fc9:4027 | 1fc9:3015 | Tehuti Networks | TN9710P 10GBase-T/NBA... | 100%   |          | B7E4B34738 |
| 8086:0000 | 8086:0000 | Intel           | PROSet/Wireless WiFi ... | 100%   |          | 418C3E7B73 |
| 8086:0d4f | 17aa:2292 | Intel           | Ethernet Connection (... | 35.5%  | 5.0.0    | BCBC0E3494 |
| 8086:0d4f | 17aa:5078 | Intel           | Ethernet Connection (... | 33.3%  | 5.0.0    | 3BB77F19C3 |
| 8086:0d4f | 8086:2081 | Intel           | Ethernet Connection (... | 5.6%   | 4.15.0   | F2BFE6BFB3 |
| 8086:107c | 8086:1376 | Intel           | 82541PI Gigabit Ether... | 1.6%   | 2.6.32   | F801FAB1AD |
| 8086:109a | 8086:0000 | Intel           | 82573L Gigabit Ethern... | 40%    | 4.15.0   | ED27C7AA81 |
| 8086:10aa | 8086:0000 | Intel           | Ethernet controller      | 100%   |          | CBBE408AAC |
| 8086:10fb | 1028:1f72 | Intel           | 82599ES 10-Gigabit SF... | 100%   |          | 77A5A8BF12 |
| 8086:1229 | 1014:005c | Intel           | 82557/8/9/0/1 Etherne... | 50%    | 4.9.60   | 3BE565CCFD |
| 8086:1229 | 8086:0050 | Intel           | 82557/8/9/0/1 Etherne... | 10.5%  | 3.10.0   | E568C873E2 |
| 8086:15a0 | 103c:2129 | Intel           | Ethernet Connection (... | 9.1%   | 4.15.0   | 71CFEF0293 |
| 8086:15a1 | 1458:e000 | Intel           | Ethernet Connection (... | 3.6%   | 4.1.15   | F2EDD659F0 |
| 8086:15b8 | 1043:8672 | Intel           | Ethernet Connection (... | 0.2%   | 4.1.15   | 51B31F180E |
| 8086:15bc | 1028:0851 | Intel           | Ethernet Connection (... | 100%   |          | 05D6B79D2F |
| 8086:15bc | 1462:7b23 | Intel           | Ethernet Connection (... | 25%    | 4.18.0   | 37076CEBE8 |
| 8086:15bc | 1849:15bc | Intel           | Ethernet Connection (... | 3.4%   | 4.13.0   | BA39531B87 |
| 8086:15be | 17aa:2286 | Intel           | Ethernet Connection (... | 6.7%   | 4.18.0   | 12B5E06A49 |
| 8086:3100 | 8086:0000 | Intel           | Ethernet controller      | 60%    | 5.4.0    | CA5D80F8F9 |
| 8086:37cc | 103c:81c7 | Intel           | Ethernet Connection X722 | 100%   |          | 670706063D |
| 8086:37cc | 15d9:0000 | Intel           | Ethernet Connection X722 | 100%   |          | 2794B14FEE |
| 8086:37cc | 17aa:4020 | Intel           | Ethernet Connection X722 | 100%   |          | FE32C2BD18 |

### Net/wireless (PCI)

225 out of 1105 (20.36%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 104c:8400 | 1186:3b01 | Texas Instru... | ACX 100 22Mbps Wirele... | 100%   |          | E804B92A1F |
| 104c:9066 | 1086:3b04 | Texas Instru... | ACX 111 54Mbps Wirele... | 100%   |          | DBFFE622A8 |
| 104c:9066 | 1186:3b04 | Texas Instru... | ACX 111 54Mbps Wirele... | 80%    | 4.18.16  | 713C36EFA0 |
| 104c:9066 | 13d1:ab90 | Texas Instru... | ACX 111 54Mbps Wirele... | 100%   |          | 6FF7C7478E |
| 10ec:8176 | 1a3b:1139 | Realtek Semi... | RTL8188CE 802.11b/g/n... | 2%     | 3.14.33  | 51273F53DF |
| 10ec:8179 | 17aa:0179 | Realtek Semi... | RTL8188EE Wireless Ne... | 6.2%   | 3.14.44  | 08BB09B100 |
| 10ec:8179 | 1a3b:1f38 | Realtek Semi... | RTL8188EE Wireless Ne... | 2.6%   | 4.1.13   | 550953CFA8 |
| 10ec:8185 | 10ec:8225 | Realtek Semi... | RTL-8185 IEEE 802.11a... | 2.1%   | 3.14.44  | E44354FF81 |
| 10ec:818b | 10ec:818b | Realtek Semi... | RTL8192EE PCIe Wirele... | 50%    | 5.6.11   | 26018540A4 |
| 10ec:818b | 10ec:8196 | Realtek Semi... | RTL8192EE PCIe Wirele... | 7.1%   | 4.15.0   | 52D70A47DA |
| 10ec:8190 | 10ec:8190 | Realtek Semi... | RTL8190 802.11n PCI W... | 100%   |          | 7EA9D53F04 |
| 10ec:8723 | 10ec:0726 | Realtek Semi... | RTL8723AE PCIe Wirele... | 0.9%   | 3.18.10  | 598F621727 |
| 10ec:8723 | 10ec:0733 | Realtek Semi... | RTL8723AE PCIe Wirele... | 100%   |          | 2F246CACD8 |
| 10ec:8821 | 1a3b:2161 | Realtek Semi... | RTL8821AE 802.11ac PC... | 10%    | 3.14.44  | 5EEDC9CEE8 |
| 10ec:b723 | 1025:b734 | Realtek Semi... | RTL8723BE PCIe Wirele... | 11.8%  | 4.1.10   | DE10405623 |
| 10ec:b723 | 103c:2231 | Realtek Semi... | RTL8723BE PCIe Wirele... | 28.1%  | 3.18.11  | 8DCBD3C2B1 |
| 10ec:b723 | 103c:8167 | Realtek Semi... | RTL8723BE PCIe Wirele... | 50%    | 4.9.60   | A17480222D |
| 10ec:b723 | 10ec:b729 | Realtek Semi... | RTL8723BE PCIe Wirele... | 28.8%  | 3.17.4   | FD5BC52C49 |
| 10ec:b723 | 10ec:b733 | Realtek Semi... | RTL8723BE PCIe Wirele... | 11.1%  | 4.1.38   | BDAF59B6EB |
| 10ec:b723 | 11ad:1723 | Realtek Semi... | RTL8723BE PCIe Wirele... | 2.2%   | 4.9.9    | E6285FD8C3 |
| 10ec:b723 | 17aa:b728 | Realtek Semi... | RTL8723BE PCIe Wirele... | 27.3%  | 3.18.14  | 02D1977887 |
| 10ec:b723 | 17aa:b736 | Realtek Semi... | RTL8723BE PCIe Wirele... | 13%    | 3.18.16  | 39A9917502 |
| 10ec:b723 | 1a3b:2159 | Realtek Semi... | RTL8723BE PCIe Wirele... | 4.8%   | 4.1.15   | DDF48A7B95 |
| 10ec:b723 | 1b9a:2485 | Realtek Semi... | RTL8723BE PCIe Wirele... | 5.9%   | 4.3.3    | D57B5C86E0 |
| 10ec:b822 | 103c:831b | Realtek Semi... | RTL8822BE 802.11a/b/g... | 2.7%   | 4.12.14  | 9C6AD0A8DB |
| 10ec:b822 | 1043:8746 | Realtek Semi... | RTL8822BE 802.11a/b/g... | 1.1%   | 4.15.0   | 27EB064D7D |
| 10ec:b822 | 1a3b:2950 | Realtek Semi... | RTL8822BE 802.11a/b/g... | 2.2%   | 4.13.0   | 935C7208E3 |
| 10ec:c821 | 103c:831a | Realtek Semi... | RTL8821CE 802.11ac PC... | 93.8%  | 4.15.0   | 72D8C77A16 |
| 10ec:c821 | 1043:87b0 | Realtek Semi... | RTL8821CE 802.11ac PC... | 100%   |          | 138AF0B756 |
| 10ec:c821 | 10ec:c821 | Realtek Semi... | RTL8821CE 802.11ac PC... | 100%   |          | F71EFE50CF |
| 10ec:c821 | 10ec:c827 | Realtek Semi... | RTL8821CE 802.11ac PC... | 80%    | 4.15.0   | BAA8C5FD79 |
| 10ec:c821 | 17aa:c024 | Realtek Semi... | RTL8821CE 802.11ac PC... | 95.5%  | 4.9.124  | 05E6C3C6BC |
| 10ec:c821 | 1a3b:3040 | Realtek Semi... | RTL8821CE 802.11ac PC... | 95.8%  | 4.18.16  | 5835F9DE60 |
| 10ec:c821 | 1a3b:3041 | Realtek Semi... | RTL8821CE 802.11ac PC... | 55%    | 4.18.16  | 36F5E879AD |
| 10ec:c822 | 17aa:c123 | Realtek Semi... | RTL8822CE 802.11ac PC... | 50%    | 5.6.19   | E6E2F26ADE |
| 10ec:c822 | 1a3b:3750 | Realtek Semi... | RTL8822CE 802.11ac PC... | 66.7%  | 5.4.32   | 9C797156F9 |
| 10ec:c82f | 17aa:c02f | Realtek Semi... | RTL8822CE 802.11ac PC... | 100%   |          | C720614026 |
| 10ec:d723 | 103c:8319 | Realtek Semi... | RTL8723DE Wireless Ne... | 94.7%  | 4.9.41   | CC1E0B07DA |
| 11ab:1fa6 | 1043:138f | Marvell Tech... | Marvell W8300 802.11 ... | 100%   |          | E75F4538BC |
| 11ab:1fa6 | 1186:3b09 | Marvell Tech... | Marvell W8300 802.11 ... | 100%   |          | 4BDC000ABE |
| 11ab:1fa7 | 1043:138f | Marvell Tech... | 88W8310 and 88W8000G ... | 100%   |          | 436FC401D1 |
| 11ab:1faa | 11ab:1faa | Marvell Tech... | 88w8335 [Libertas] 80... | 100%   |          | 07DCDB2C01 |
| 11ab:1faa | 1385:6b00 | Marvell Tech... | 88w8335 [Libertas] 80... | 100%   |          | 59451C84FF |
| 11ab:2a02 | 1385:7e00 | Marvell Tech... | 88W8361 [TopDog] 802.... | 100%   |          | 51F69F1430 |
| 11ab:2a08 | 11ab:2a08 | Marvell Tech... | 88W8362e [TopDog] 802... | 100%   |          | 5B3E8B9EF1 |
| 14c3:7630 | 103c:197c | MEDIATEK        | MT7630e 802.11bgn Wir... | 100%   |          | 26940AEEC6 |
| 14c3:7630 | 105b:e074 | MEDIATEK        | MT7630e 802.11bgn Wir... | 100%   |          | D23CC368BB |
| 14c3:7630 | 105b:e084 | MEDIATEK        | MT7630e 802.11bgn Wir... | 100%   |          | DF4413AF58 |
| 14e4:4311 | 1028:0007 | Broadcom        | BCM4311 802.11b/g WLAN   | 1.1%   | 3.10.34  | 968EBC7FAC |
| 14e4:4311 | 103c:1363 | Broadcom        | BCM4311 802.11b/g WLAN   | 3.6%   | 3.10.34  | 6B4A8EAB4C |
| 14e4:4311 | 103c:1364 | Broadcom        | BCM4311 802.11b/g WLAN   | 3.1%   | 3.14.33  | F22AB20BAE |
| 14e4:4311 | 1468:0316 | Broadcom        | BCM4311 802.11b/g WLAN   | 100%   |          | 7F0BB0CC92 |
| 14e4:4311 | 1468:0422 | Broadcom        | BCM4311 802.11b/g WLAN   | 1.7%   | 3.10.34  | 918743233C |
| 14e4:4312 | 1028:0007 | Broadcom Lim... | BCM4311 802.11a/b/g      | 12.1%  | 3.14.44  | 8BBB9EE1AF |
| 14e4:4315 | 103c:1508 | Broadcom        | BCM4312 802.11b/g LP-PHY | 1.1%   | 3.14.44  | D0F06C8499 |
| 14e4:4318 | 103c:1356 | Broadcom        | BCM4318 [AirForce One... | 6.7%   | 4.1.19   | 306E665622 |
| 14e4:4318 | 1468:0312 | Broadcom Lim... | BCM4318 [AirForce One... | 12.5%  | 3.10.34  | A28F7B2623 |
| 14e4:4320 | 103c:12f8 | Broadcom        | BCM4306 802.11b/g Wir... | 40%    | 3.10.34  | FE61304CD4 |
| 14e4:4320 | 103c:12fa | Broadcom        | BCM4306 802.11b/g Wir... | 100%   |          | 0FE7032974 |
| 14e4:4324 | 1028:0003 | Broadcom        | BCM4309 802.11abg Wir... | 50%    | 4.15.0   | 0077E52877 |
| 14e4:4328 | 106b:0088 | Broadcom        | BCM4321 802.11a/b/g/n    | 4.7%   | 4.1.15   | 542EE658B9 |
| 14e4:4328 | 106b:008c | Broadcom        | BCM4321 802.11a/b/g/n    | 2.3%   | 4.1.38   | 48D30CB977 |
| 14e4:4328 | 106b:0090 | Broadcom Lim... | BCM4321 802.11a/b/g/n    | 4%     | 4.1.22   | 030A81E657 |
| 14e4:432b | 1028:000d | Broadcom        | BCM4322 802.11a/b/g/n... | 4.5%   | 3.10.0   | 103788F3AC |
| 14e4:432b | 103c:1510 | Broadcom        | BCM4322 802.11a/b/g/n... | 100%   |          | 23C8DE7582 |
| 14e4:4331 | 106b:00d6 | Broadcom        | BCM4331 802.11a/b/g/n    | 2.6%   | 4.1.25   | FAA3B94DC4 |
| 14e4:4331 | 106b:00f5 | Broadcom        | BCM4331 802.11a/b/g/n    | 3.7%   | 4.9.20   | 437B3EB74D |
| 14e4:4331 | 14e4:4331 | Broadcom        | BCM4331 802.11a/b/g/n    | 1.4%   | 4.1.25   | 1281C8C30D |
| 14e4:4353 | 1028:000e | Broadcom        | BCM43224 802.11a/b/g/n   | 3%     | 4.1.15   | E572489472 |
| 14e4:4353 | 106b:0093 | Broadcom        | BCM43224 802.11a/b/g/n   | 1.3%   | 4.1.15   | 4E11213A56 |
| 14e4:4357 | 105b:e021 | Broadcom        | BCM43225 802.11b/g/n     | 2.3%   | 3.14.25  | 68F61986F8 |
| 14e4:4358 | 105b:e040 | Broadcom        | BCM43227 802.11b/g/n     | 1%     | 3.14.33  | 9D65BC9B14 |
| 14e4:4359 | 1028:0011 | Broadcom        | BCM43228 802.11a/b/g/n   | 2.6%   | 3.14.44  | 49AC9F2B94 |
| 14e4:4359 | 1028:0014 | Broadcom        | BCM43228 802.11a/b/g/n   | 4%     | 3.14.44  | 71510169F8 |
| 14e4:4359 | 103c:182c | Broadcom        | BCM43228 802.11a/b/g/n   | 1.9%   | 4.1.25   | 10B4B2CF4D |
| 14e4:4359 | 103c:2135 | Broadcom        | BCM43228 802.11a/b/g/n   | 50%    | 4.1.25   | 3E13F8A157 |
| 14e4:4359 | 1043:850c | Broadcom        | BCM43228 802.11a/b/g/n   | 11.1%  | 3.14.44  | C22EF5B009 |
| 14e4:4359 | 105b:e04b | Broadcom        | BCM43228 802.11a/b/g/n   | 1.1%   | 3.14.44  | EAC775D35E |
| 14e4:4359 | 105b:e08b | Broadcom Lim... | BCM43228 802.11a/b/g/n   | 9.1%   | 4.1.34   | 0D43FC94FE |
| 14e4:4359 | 11ad:6603 | Broadcom        | BCM43228 802.11a/b/g/n   | 7.1%   | 4.1.15   | C6F99AC92E |
| 14e4:4359 | 14e4:05e2 | Broadcom        | BCM43228 802.11a/b/g/n   | 6.7%   | 3.10.42  | 312789572C |
| 14e4:4359 | 14e4:0607 | Broadcom Lim... | BCM43228 802.11a/b/g/n   | 2.7%   | 3.14.44  | A30712CD7D |
| 14e4:4365 | 1028:0016 | Broadcom        | BCM43142 802.11b/g/n     | 7.1%   | 3.14.33  | 080C4F6F04 |
| 14e4:4365 | 1028:0018 | Broadcom        | BCM43142 802.11b/g/n     | 33.3%  | 4.1.25   | 7617FC2496 |
| 14e4:4365 | 103c:2230 | Broadcom        | BCM43142 802.11b/g/n     | 36.2%  | 3.14.44  | 8FC95EBCD2 |
| 14e4:4365 | 103c:2232 | Broadcom        | BCM43142 802.11b/g/n     | 33.3%  | 4.19.0   | 36182F214B |
| 14e4:4365 | 103c:804a | Broadcom        | BCM43142 802.11b/g/n     | 24%    | 4.1.15   | F4B2E3494D |
| 14e4:4365 | 105b:e071 | Broadcom        | BCM43142 802.11b/g/n     | 37.2%  | 3.14.44  | 1C30FA8D64 |
| 14e4:4365 | 105b:e07e | Broadcom        | BCM43142 802.11b/g/n     | 53.6%  | 3.14.44  | 618A210720 |
| 14e4:4365 | 11ad:6605 | Broadcom        | BCM43142 802.11b/g/n     | 10.6%  | 3.14.33  | 4F1BBD40B7 |
| 14e4:4365 | 11ad:6645 | Broadcom        | BCM43142 802.11b/g/n     | 32.4%  | 3.14.33  | 2CC492CF55 |
| 14e4:4365 | 11ad:6655 | Broadcom        | BCM43142 802.11b/g/n     | 70%    | 4.9.9    | 7BA4E68002 |
| 14e4:4365 | 11ad:6675 | Broadcom Lim... | BCM43142 802.11b/g/n     | 40%    | 3.14.44  | 5FCB4E6866 |
| 14e4:4365 | 17aa:0611 | Broadcom        | BCM43142 802.11b/g/n     | 7.2%   | 3.14.25  | 4EBA6CB14F |
| 14e4:4365 | 17aa:0621 | Broadcom        | BCM43142 802.11b/g/n     | 18.3%  | 3.14.25  | 2E7C3657FB |
| 14e4:4365 | 1a3b:2155 | Broadcom        | BCM43142 802.11b/g/n     | 50%    | 4.15.0   | 3F8D8F2725 |
| 14e4:4365 | 1b9a:3002 | Broadcom        | BCM43142 802.11b/g/n     | 69.7%  | 4.1.25   | C8D6ED9E03 |
| 14e4:43a0 | 1043:85df | Broadcom        | BCM4360 802.11ac Wire... | 15.8%  | 4.15.0   | 19EB0446A2 |
| 14e4:43a0 | 1043:8659 | Broadcom        | BCM4360 802.11ac Wire... | 23.1%  | 3.10.0   | D7B6109B94 |
| 14e4:43a0 | 106b:0117 | Broadcom Lim... | BCM4360 802.11ac Wire... | 18.8%  | 4.18.0   | DA4BD8A9EF |
| 14e4:43a0 | 106b:0135 | Broadcom        | BCM4360 802.11ac Wire... | 60%    | 5.0.0    | 9F3D443A21 |
| 14e4:43a0 | 106b:013b | Broadcom Lim... | BCM4360 802.11ac Wire... | 33.3%  | 4.18.0   | BBE81BBD03 |
| 14e4:43a0 | 14e4:0619 | Broadcom        | BCM4360 802.11ac Wire... | 7.4%   | 4.15.0   | B60F9E1AE7 |
| 14e4:43ae | 17aa:0622 | Broadcom        | BCM43162 802.11ac Wir... | 73.9%  | 4.18.16  | 6D9836BB74 |
| 14e4:43b1 | 1028:0019 | Broadcom Lim... | BCM4352 802.11ac Wire... | 57.1%  | 5.0.9    | BC19C77210 |
| 14e4:43b1 | 103c:2154 | Broadcom Lim... | BCM4352 802.11ac Wire... | 86.4%  | 4.18.0   | 19571AD1C9 |
| 14e4:43b1 | 1043:855c | Broadcom        | BCM4352 802.11ac Wire... | 25%    | 4.15.0   | A16A7137A3 |
| 14e4:43b1 | 1043:85ba | Broadcom        | BCM4352 802.11ac Wire... | 50%    | 4.18.0   | 94146BB179 |
| 14e4:43b1 | 17aa:0623 | Broadcom Lim... | BCM4352 802.11ac Wire... | 11.1%  | 4.15.0   | FC0DC30BF0 |
| 14e4:43b1 | 1a3b:2b23 | Broadcom        | BCM4352 802.11ac Wire... | 33.3%  | 4.15.0   | 14ABE97F88 |
| 14e4:43ba | 106b:0133 | Broadcom        | BCM43602 802.11ac Wir... | 2.4%   | 4.9.9    | B0C6F48549 |
| 14e4:43ba | 106b:014a | Broadcom        | BCM43602 802.11ac Wir... | 16.7%  | 4.19.88  | 5984E1BBAC |
| 14e4:43ba | 106b:0173 | Broadcom        | BCM43602 802.11ac Wir... | 16.7%  | 5.3.0    | 6F3816ABBD |
| 14e4:43c3 | 1043:86fb | Broadcom        | Network controller       | 5.9%   | 4.15.0   | 530CC43BE2 |
| 14e4:4464 | 106b:07bf | Broadcom        | BCM4364 802.11ac Wire... | 94.3%  | 5.6.17   | D26B114C5C |
| 14e4:4488 | 106b:0870 | Broadcom        | BCM4377b Wireless Net... | 100%   |          | D3A040508D |
| 14e4:4727 | 1028:0010 | Broadcom        | BCM4313 802.11bgn Wir... | 3.7%   | 4.13.0   | 4F60CF51A6 |
| 14e4:4727 | 1028:0012 | Broadcom Lim... | BCM4313 802.11bgn Wir... | 21.4%  | 4.15.0   | 40D48C06A1 |
| 14e4:4727 | 1028:0015 | Broadcom        | BCM4313 802.11bgn Wir... | 14.8%  | 4.15.0   | C5B82BEB1E |
| 14e4:4727 | 103c:145c | Broadcom        | BCM4313 802.11bgn Wir... | 4.5%   | 3.10.42  | A32C0DB8BB |
| 14e4:4727 | 103c:1483 | Broadcom        | BCM4313 802.11bgn Wir... | 3.7%   | 4.1.34   | 04BAC3F07D |
| 14e4:4727 | 103c:1795 | Broadcom        | BCM4313 802.11bgn Wir... | 3.2%   | 3.10.42  | 06AA196398 |
| 14e4:4727 | 105b:e042 | Broadcom        | BCM4313 802.11bgn Wir... | 5%     | 4.15.0   | D148A20413 |
| 14e4:4727 | 144f:7175 | Broadcom        | BCM4313 802.11bgn Wir... | 9.1%   | 4.15.0   | 93629DD831 |
| 14e4:4727 | 144f:7179 | Broadcom        | BCM4313 802.11bgn Wir... | 11.1%  | 3.10.34  | 26ABB03AC7 |
| 14e4:4727 | 14e4:0510 | Broadcom        | BCM4313 802.11bgn Wir... | 17.2%  | 4.2.6    | A911172500 |
| 14e4:4727 | 14e4:051b | Broadcom        | BCM4313 802.11bgn Wir... | 4.5%   | 2.6.32   | 0DB2A8DFAD |
| 14e4:4727 | 14e4:0587 | Broadcom Lim... | BCM4313 802.11bgn Wir... | 8.7%   | 4.15.0   | 8D6C57DC63 |
| 14e4:4727 | 14e4:0608 | Broadcom        | BCM4313 802.11bgn Wir... | 14.3%  | 4.1.38   | 65C68A39C0 |
| 14e4:4727 | 185f:051a | Broadcom        | BCM4313 802.11bgn Wir... | 3.3%   | 4.9.0    | 86A1DD9578 |
| 14e4:4727 | 1a3b:2a47 | Broadcom Lim... | BCM4313 802.11bgn Wir... | 25%    | 3.10.34  | 79326DA8CA |
| 167b:2116 | 340f:187e | ZyDAS Techno... | ZD1212B Wireless Adapter | 100%   |          | C399CBB5F3 |
| 168c:001c | 103c:137b | Qualcomm Ath... | AR242x / AR542x Wirel... | 0.8%   | 3.14.33  | 93C0EF7223 |
| 168c:002b | 103c:1461 | Qualcomm Ath... | AR9285 Wireless Netwo... | 0.6%   | 3.14.33  | F4DE983D96 |
| 168c:002b | 144f:7173 | Qualcomm Ath... | AR9285 Wireless Netwo... | 1.9%   | 3.14.44  | 211A9802DB |
| 168c:002d | 168c:0300 | Qualcomm Ath... | AR9227 Wireless Netwo... | 2%     | 3.14.33  | AA24EEDD97 |
| 168c:002e | 105b:e034 | Qualcomm Ath... | AR9287 Wireless Netwo... | 0.3%   | 3.10.0   | 8FE3AF49FB |
| 168c:002e | 10cf:158f | Qualcomm Ath... | AR9287 Wireless Netwo... | 5%     | 4.1.25   | 958D094890 |
| 168c:0032 | 11ad:6608 | Qualcomm Ath... | AR9485 Wireless Netwo... | 2.3%   | 3.14.33  | 67009EFFAA |
| 168c:0032 | 11ad:6617 | Qualcomm Ath... | AR9485 Wireless Netwo... | 0.4%   | 3.14.25  | 86D2D3B0E1 |
| 168c:0032 | 11ad:6628 | Qualcomm Ath... | AR9485 Wireless Netwo... | 1.2%   | 3.14.44  | 469E04E0D5 |
| 168c:0036 | 11ad:0642 | Qualcomm Ath... | QCA9565 / AR9565 Wire... | 0.5%   | 3.10.51  | 2F2C11E46D |
| 168c:0036 | 11ad:0803 | Qualcomm Ath... | QCA9565 / AR9565 Wire... | 1.7%   | 3.14.44  | 401BBED185 |
| 168c:0037 | 1a3b:1195 | Qualcomm Ath... | AR9485 Wireless Netwo... | 11.1%  | 4.9.20   | CE8124E5F4 |
| 168c:0037 | 1a3b:2100 | Qualcomm Ath... | AR9485 Wireless Netwo... | 2.9%   | 3.14.25  | 0F8E9B7955 |
| 168c:003e | 1a56:1535 | Qualcomm Ath... | QCA6174 802.11ac Wire... | 0.4%   | 4.4.0    | 6695D2A05E |
| 168c:0042 | 1028:1810 | Qualcomm Ath... | QCA9377 802.11ac Wire... | 0.2%   | 4.4.0    | F591FD6F3D |
| 168c:0042 | 11ad:0806 | Qualcomm Ath... | QCA9377 802.11ac Wire... | 5.5%   | 4.4.0    | ECB6A89DFC |
| 168c:0042 | 11ad:08a6 | Qualcomm Ath... | QCA9377 802.11ac Wire... | 0.1%   | 3.10.0   | E7395D0EE2 |
| 168c:0042 | 17aa:0901 | Qualcomm Ath... | QCA9377 802.11ac Wire... | 0.2%   | 4.4.0    | C23D0EF968 |
| 168c:0042 | 17aa:4035 | Qualcomm Ath... | QCA9377 802.11ac Wire... | 0.7%   | 4.8.0    | C3352134E9 |
| 17cb:0001 | 1737:0045 | Qualcomm        | AGN100 802.11 a/b/g T... | 100%   |          | 7D17E6E1A3 |
| 17fe:2220 | 1468:0305 | InProComm       | IPN 2220 802.11g         | 100%   |          | 76920BC1B7 |
| 17fe:2220 | 1468:0310 | InProComm       | IPN 2220 802.11g         | 100%   |          | E9BD04F647 |
| 1814:0301 | 1814:2561 | Ralink          | RT2561/RT61 802.11g PCI  | 2.4%   | 3.14.33  | E40B76E473 |
| 1814:3062 | 1814:3062 | Ralink          | RT3062 Wireless 802.1... | 2.5%   | 3.14.44  | 9D9E2DB550 |
| 1814:3090 | 1462:6894 | Ralink          | RT3090 Wireless 802.1... | 14.3%  | 4.18.16  | E40B76E473 |
| 1814:3290 | 103c:18ec | Ralink          | RT3290 Wireless 802.1... | 1%     | 3.14.15  | 387BBD9C5B |
| 1814:5392 | 1814:5392 | Ralink          | RT5392 PCIe Wireless ... | 23.5%  | 4.18.0   | 57643353CE |
| 1814:539a | 103c:1839 | Ralink          | WLAN controller          | 12.5%  | 4.1.15   | 2E60620A98 |
| 1814:539f | 103c:1637 | Ralink          | RT5390 [802.11 b/g/n ... | 2.3%   | 3.14.44  | ED2FBC90A0 |
| 1814:5592 | 1043:851a | Ralink          | RT5592 PCIe Wireless ... | 100%   |          | BB6D6E1681 |
| 1814:5592 | 1814:5592 | Ralink          | RT5592 PCIe Wireless ... | 100%   |          | 760C31A638 |
| 8086:0082 | 8086:1321 | Intel           | Centrino Advanced-N 6... | 0.7%   | 3.14.33  | F33530C32A |
| 8086:0085 | 8086:1311 | Intel           | Centrino Advanced-N 6... | 0.2%   | 3.10.0   | 55427995B5 |
| 8086:0085 | 8086:c220 | Intel           | Centrino Advanced-N 6... | 8%     | 3.14.15  | 1CFB078C4E |
| 8086:008a | 8086:0000 | Intel           | Centrino Wireless-N 1... | 100%   |          | 28086B6CA8 |
| 8086:02f0 | 8086:0034 | Intel           | Comet Lake PCH-LP CNV... | 4.3%   | 5.0.0    | FCD9F8DF27 |
| 8086:02f0 | 8086:0074 | Intel           | Comet Lake PCH-LP CNV... | 7.1%   | 3.10.0   | 8D589B1A7E |
| 8086:088e | 8086:4060 | Intel           | Centrino Advanced-N 6235 | 0.3%   | 3.10.34  | AC608E1D37 |
| 8086:0893 | 8086:0262 | Intel           | Centrino Wireless-N 135  | 3.9%   | 3.14.25  | 2DD89E3983 |
| 8086:08ae | 8086:1005 | Intel           | Centrino Wireless-N 100  | 1.4%   | 3.10.42  | CF401BD3E4 |
| 8086:08b1 | 8086:4070 | Intel           | Wireless 7260            | 0.3%   | 3.10.0   | 550460AAAC |
| 8086:08b1 | 8086:4470 | Intel           | Wireless 7260            | 0.4%   | 3.14.44  | 8EA71BA2AE |
| 8086:08b1 | 8086:c070 | Intel           | Wireless 7260            | 3.4%   | 4.1.15   | 2B62BC6C8A |
| 8086:08b2 | 8086:c260 | Intel           | Wireless 7260            | 1.3%   | 4.1.16   | 819B048062 |
| 8086:08b3 | 8086:8470 | Intel           | Wireless 3160            | 0.5%   | 3.16.0   | 7E3EEBA3CA |
| 8086:08b4 | 8086:8270 | Intel           | Wireless 3160            | 1.2%   | 3.14.44  | AB6BD693BE |
| 8086:093c | 8086:0181 | Intel           | Wireless Gigabit 17265   | 100%   |          | D33E07EEAB |
| 8086:093c | 8086:2181 | Intel           | Wireless Gigabit 17265   | 100%   |          | 8CAA0AA306 |
| 8086:093c | 8086:2191 | Intel           | Wireless Gigabit 17265   | 100%   |          | 805B5CFC62 |
| 8086:093c | 8086:7001 | Intel           | Wireless Gigabit 17265   | 100%   |          | E9AD7E6B83 |
| 8086:095a | 8086:5010 | Intel           | Wireless 7265            | 0.1%   | 3.14.44  | 5DBE9649A7 |
| 8086:095a | 8086:5400 | Intel           | Wireless 7265            | 4.3%   | 4.1.25   | 0A99E4D896 |
| 8086:095a | 8086:5410 | Intel           | Wireless 7265            | 0.7%   | 4.1.18   | 62308C2EBC |
| 8086:095b | 8086:5210 | Intel           | Wireless 7265            | 2.2%   | 4.1.34   | 6BCE8819C3 |
| 8086:24f3 | 8086:0130 | Intel           | Wireless 8260            | 1.7%   | 4.4.0    | B612D89D47 |
| 8086:24f3 | 8086:1010 | Intel           | Wireless 8260            | 1.1%   | 4.1.15   | 107A11048C |
| 8086:24f3 | 8086:1130 | Intel           | Wireless 8260            | 1.3%   | 4.4.0    | 3A43711362 |
| 8086:24fb | 8086:2110 | Intel           | Dual Band Wireless-AC... | 0.3%   | 3.10.0   | 41F9DC6E07 |
| 8086:24fd | 8086:0010 | Intel           | Wireless 8265 / 8275     | 0.2%   | 3.10.0   | 7D7E6AD5D5 |
| 8086:24fd | 8086:0110 | Intel           | Wireless 8265 / 8275     | 0.5%   | 4.12.14  | F2102769EB |
| 8086:24fd | 8086:1010 | Intel           | Wireless 8265 / 8275     | 0.2%   | 4.8.15   | BF84028302 |
| 8086:24fd | 8086:9010 | Intel           | Wireless 8265 / 8275     | 1.3%   | 4.9.9    | E7A9120C09 |
| 8086:2526 | 1a56:1550 | Intel           | Wireless-AC 9260         | 2.3%   | 4.15.0   | EA77C657C0 |
| 8086:2526 | 8086:0014 | Intel           | Wireless-AC 9260         | 1.6%   | 4.15.0   | B739E651BA |
| 8086:2723 | 1a56:1654 | Intel           | Wi-Fi 6 AX200            | 4.3%   | 4.15.0   | 68365E0B80 |
| 8086:2723 | 8086:0080 | Intel           | Wi-Fi 6 AX200            | 9.2%   | 4.18.0   | F7DB97FB08 |
| 8086:2723 | 8086:0084 | Intel           | Wi-Fi 6 AX200            | 10.9%  | 4.15.0   | 3D49020A7B |
| 8086:2723 | 8086:008c | Intel           | Wi-Fi 6 AX200            | 27.3%  | 5.3.0    | A838427772 |
| 8086:2723 | 8086:4080 | Intel           | Wi-Fi 6 AX200            | 5.7%   | 4.15.0   | BE3EF4D26F |
| 8086:3165 | 8086:4010 | Intel           | Wireless 3165            | 0.4%   | 4.1.15   | 54574B77F2 |
| 8086:3165 | 8086:8110 | Intel           | Wireless 3165            | 1.1%   | 4.9.20   | 48E3CC8030 |
| 8086:3166 | 8086:4210 | Intel           | Dual Band Wireless-AC... | 0.6%   | 4.1.15   | FC2E5D7E80 |
| 8086:31dc | 8086:0034 | Intel           | Gemini Lake PCH CNVi ... | 4.3%   | 4.13.0   | 172A00D950 |
| 8086:34f0 | 8086:0074 | Intel           | Ice Lake-LP PCH CNVi ... | 2.9%   | 5.3.0    | 3F4D79EA3B |
| 8086:4222 | 103c:135c | Intel           | PRO/Wireless 3945ABG ... | 1.6%   | 3.14.25  | 9EDB73DD0E |
| 8086:4223 | 8086:1040 | Intel           | PRO/Wireless 2915ABG ... | 16.7%  | 4.15.0   | 8488B3D0B9 |
| 8086:4229 | 8086:1001 | Intel           | PRO/Wireless 4965 AG ... | 4.3%   | 3.14.44  | 13824A2872 |
| 8086:422c | 8086:1321 | Intel           | Centrino Advanced-N 6200 | 0.8%   | 4.1.15   | ACDA89894A |
| 8086:4232 | 8086:1201 | Intel           | WiFi Link 5100           | 0.3%   | 3.10.34  | 8596529915 |
| 8086:4232 | 8086:1301 | Intel           | WiFi Link 5100           | 0.9%   | 3.10.46  | 4ED6CCC4E4 |
| 8086:4237 | 8086:1311 | Intel           | PRO/Wireless 5100 AGN... | 5.9%   | 3.10.34  | 10708BAA81 |
| 8086:4239 | 8086:1311 | Intel           | Centrino Advanced-N 6200 | 0.6%   | 3.0.28   | 5DD7A5FCE1 |
| 8086:7360 |           | Intel           | XMM7360 LTE Advanced ... | 100%   |          | B65F3E7B62 |
| 8086:7360 | 1028:5820 | Intel           | XMM7360 LTE Advanced ... | 100%   |          | DAE8FD20B4 |
| 8086:7360 | 103c:8337 | Intel           | XMM7360 LTE Advanced ... | 96.3%  | 5.3.18   | B6BE78472B |
| 8086:7360 | 1cf8:8521 | Intel           | XMM7360 LTE Advanced ... | 100%   |          | 050C997025 |
| 8086:7360 | 8086:0020 | Intel           | XMM7360 LTE Advanced ... | 98%    | 5.7.0    | CCF327B2F0 |
| 8086:7560 | 1cf8:8601 | Intel           | Wireless controller      | 100%   |          | ACBDAC722C |
| 8086:9df0 | 8086:2034 | Intel           | Cannon Point-LP CNVi ... | 4.5%   | 4.18.0   | D60073EAD5 |
| 8086:9df0 | 8086:42a4 | Intel           | Cannon Point-LP CNVi ... | 2.9%   | 4.15.0   | DAF389F21B |
| 8086:a370 | 1a56:1552 | Intel           | Cannon Lake PCH CNVi ... | 3.6%   | 4.18.0   | EFAA58FCC8 |
| 8086:a370 | 8086:0034 | Intel           | Cannon Lake PCH CNVi ... | 0.9%   | 3.10.0   | 82470B81BA |
| 8086:a370 | 8086:02a4 | Intel           | Cannon Lake PCH CNVi ... | 1.1%   | 4.15.0   | 40ED220090 |

### Network (PCI)

38 out of 904 (4.20%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 0000:0002 | 002c:0000 |                 | Network controller       | 100%   |          | 3859A12973 |
| 0000:0210 | 002c:0000 |                 | Network controller       | 100%   |          | 3859A12973 |
| 0000:0210 | 1105:8300 |                 |                          | 100%   |          | 3859A12973 |
| 03d0:2103 | 03d0:2103 |                 | Network controller       | 100%   |          | AD6A707B6C |
| 1006:3106 | 1086:1405 | Reply Group     | Reply Ethernet contro... | 100%   |          | F597A38FF5 |
| 10ec:8125 | 1043:87d7 | Realtek Semi... | RTL8125 2.5GbE Contro... | 50%    | 5.4.0    | E122EE6E1D |
| 10ec:8125 | 10ec:0123 | Realtek Semi... | RTL8125 2.5GbE Contro... | 18.2%  | 4.14.24  | C8A9642B81 |
| 10ec:8125 | 1458:e000 | Realtek Semi... | RTL8125 2.5GbE Contro... | 40.9%  | 5.4.0    | DF8EE1AEB2 |
| 10ec:8125 | 1462:7c06 | Realtek Semi... | RTL8125 2.5GbE Contro... | 100%   |          | 8112942B50 |
| 10ec:8125 | 1462:7c35 | Realtek Semi... | RTL8125 2.5GbE Contro... | 20%    | 5.0.0    | DC7E369D45 |
| 10ec:8125 | 1462:7c84 | Realtek Semi... | RTL8125 2.5GbE Contro... | 100%   |          | A7879DFBC3 |
| 10ec:8125 | 1849:8125 | Realtek Semi... | RTL8125 2.5GbE Contro... | 42.9%  | 5.0.0    | A552E6AAA0 |
| 1106:1106 | 1186:1405 | VIA Technolo... | VT82C570MV               | 100%   |          | 1EF54091BE |
| 1106:3065 | 1849:3065 | VIA Technolo... | VT6102/VT6103 [Rhine-II] | 10%    | 3.10.0   | 6FAC734286 |
| 1106:3102 | 1186:1401 | VIA Technolo... | VT8662 Host Bridge       | 100%   |          | EAD04A61E4 |
| 1106:3106 | 1106:0105 | VIA Technolo... | VT6105/VT6106S [Rhine... | 50%    | 4.1.16   | A6659EE127 |
| 1106:a409 | 1106:a409 | VIA Technolo... | VX855/VX875/VX900 Ser... | 100%   |          | 528A1449B7 |
| 1260:3886 | 16be:2004 | Intersil        | ISL3886 [Prism Javeli... | 20%    | 5.0.0    | ACACF55F1F |
| 12d0:2103 | 12d0:2103 | GDE Systems     | GDE Network controller   | 100%   |          | 8C5E6472B2 |
| 148c:002d | 148c:0301 | Tul Corporat... | Network controller       | 100%   |          | 15959C0828 |
| 14e4:170c | 1028:01af | Broadcom        | BCM4401-B0 100Base-TX    | 2.7%   | 3.14.44  | A6BB0BFD0B |
| 14e4:170c | 1028:01f1 | Broadcom        | BCM4401-B0 100Base-TX    | 17.6%  | 3.14.53  | B5A30E2784 |
| 14e4:5fa0 | 106b:0870 | Broadcom        | Network controller       | 100%   |          | D3A040508D |
| 168c:004a | 15aa:4035 | Qualcomm Ath... | Network controller       | 100%   |          | 04F6BB6978 |
| 168c:0063 | 168c:3071 | Qualcomm Ath... | Network controller       | 100%   |          | 8F99628F42 |
| 1810:3060 | 8001:0000 | HCL Technolo... | Network controller       | 100%   |          | CFD57C3B89 |
| 8086:10d3 | 8086:0000 | Intel           | 82574L Gigabit Networ... | 11.5%  | 4.4.0    | ADB076ED03 |
| 8086:10d3 | 8086:a01f | Intel           | 82574L Gigabit Networ... | 0.9%   | 3.10.0   | 9B75A42A1E |
| 8086:10de | 103c:3034 | Intel           | 82567LM-3 Gigabit Net... | 3.7%   | 3.14.44  | 5DC57BDE0C |
| 8086:10eb | 8086:0000 | Intel           | 82577LC Gigabit Netwo... | 87.5%  | 5.3.0    | 26F28ABE7E |
| 8086:10f0 | 1019:1324 | Intel           | 82578DC Gigabit Netwo... | 50%    | 5.4.0    | 50B445BA68 |
| 8086:1502 | 1028:0493 | Intel           | 82579LM Gigabit Netwo... | 0.8%   | 3.14.33  | 3F252A50FB |
| 8086:1502 | 103c:179b | Intel           | 82579LM Gigabit Netwo... | 2.1%   | 3.14.44  | 18835A8B6C |
| 8086:1502 | 1043:849c | Intel           | 82579LM Gigabit Netwo... | 100%   |          | 44AA7CC920 |
| 8086:1531 | 8086:0000 | Intel           | I210 Gigabit Unprogra... | 100%   |          | 25D911A50B |
| 8086:1539 | 1043:85f0 | Intel           | I211 Gigabit Network ... | 0.3%   | 3.14.44  | ADAC2225D4 |
| 8086:1539 | 1458:e000 | Intel           | I211 Gigabit Network ... | 0.3%   | 4.9.0    | 6BEE5D9A22 |
| 8086:1539 | 1849:1539 | Intel           | I211 Gigabit Network ... | 0.3%   | 3.10.0   | AC6DF0A8C0 |

### Sd host controller (PCI)

79 out of 814 (9.71%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 104c:8034 | 103c:3085 | Texas Instru... | PCIxx21/PCIxx11 SD Ho... | 12.5%  | 4.19.66  | E643DE7D13 |
| 104c:803c | 17aa:207d | Texas Instru... | PCIxx12 SDA Standard ... | 12.5%  | 3.14.44  | E5C5CE1445 |
| 10ec:5209 | 103c:1659 | Realtek Semi... | RTS5209 PCI Express C... | 6.7%   | 4.1.15   | 119A35F980 |
| 1180:0822 | 103c:7008 | Ricoh           | R5C822 SD/SDIO/MMC/MS... | 2.2%   | 3.10.34  | 5DD7A5FCE1 |
| 1217:8221 | 1028:0493 | O2 Micro        | OZ600FJ0/OZ900FJ0/OZ6... | 0.8%   | 3.14.33  | F33530C32A |
| 1217:8520 | 1028:05cb | O2 Micro        | SD/MMC Card Reader Co... | 2%     | 4.9.60   | 037A28C347 |
| 1217:8520 | 1028:05e0 | O2 Micro        | SD/MMC Card Reader Co... | 3.3%   | 4.9.9    | 8EA71BA2AE |
| 1217:8621 | 17aa:3824 | O2 Micro        | SD/MMC Card Reader Co... | 3.1%   | 4.15.0   | 80F496EACD |
| 14e4:16bc | 1025:0647 | Broadcom        | BCM57765/57785 SDXC/M... | 0.2%   | 3.10.34  | 86D2D3B0E1 |
| 17a0:9750 | 17aa:2279 | Genesys Logic   | GL9750 SD Host Contro... | 6.1%   | 4.15.0   | 15419D9561 |
| 17a0:9750 | 17aa:2286 | Genesys Logic   | GL9750 SD Host Contro... | 7.7%   | 4.18.0   | D4FA985843 |
| 197b:2381 | 1025:013d | JMicron Tech... | Standard SD Host Cont... | 9.1%   | 4.15.0   | F922502A91 |
| 197b:2381 | 1025:0140 | JMicron Tech... | Standard SD Host Cont... | 20%    | 5.3.0    | C85107D1C1 |
| 197b:2381 | 1025:0145 | JMicron Tech... | Standard SD Host Cont... | 57.1%  | 4.1.15   | 3C60271275 |
| 197b:2381 | 1025:0260 | JMicron Tech... | Standard SD Host Cont... | 10%    | 4.15.0   | ABC5736623 |
| 197b:2381 | 1025:0275 | JMicron Tech... | Standard SD Host Cont... | 53.8%  | 4.15.0   | 09734ADC68 |
| 197b:2381 | 103c:2aa2 | JMicron Tech... | Standard SD Host Cont... | 33.3%  | 4.1.15   | 744EE1496B |
| 197b:2381 | 103c:30f4 | JMicron Tech... | Standard SD Host Cont... | 3.7%   | 3.14.53  | C727A0FA74 |
| 197b:2381 | 103c:30f7 | JMicron Tech... | Standard SD Host Cont... | 28.6%  | 4.1.25   | B25D0327CA |
| 197b:2381 | 103c:30fc | JMicron Tech... | Standard SD Host Cont... | 50%    | 4.18.0   | 039F952C77 |
| 197b:2381 | 103c:3603 | JMicron Tech... | Standard SD Host Cont... | 7.4%   | 3.14.44  | B69F9ABF10 |
| 197b:2381 | 103c:3610 | JMicron Tech... | Standard SD Host Cont... | 25%    | 5.0.0    | 058A1A1E85 |
| 197b:2381 | 103c:361b | JMicron Tech... | Standard SD Host Cont... | 42.9%  | 4.15.0   | 63C2E0460D |
| 197b:2381 | 103c:3624 | JMicron Tech... | Standard SD Host Cont... | 4.3%   | 4.1.16   | FF9CED6EF0 |
| 197b:2381 | 103c:3628 | JMicron Tech... | Standard SD Host Cont... | 7.8%   | 3.14.44  | 4833031B9B |
| 197b:2381 | 103c:363c | JMicron Tech... | Standard SD Host Cont... | 75%    | 5.6.7    | D9418273DF |
| 197b:2381 | 103c:7001 | JMicron Tech... | Standard SD Host Cont... | 15%    | 3.0.28   | 298015ECAC |
| 197b:2381 | 1043:1a07 | JMicron Tech... | Standard SD Host Cont... | 3.9%   | 3.10.34  | 3FCBF67BDC |
| 197b:2381 | 1043:84af | JMicron Tech... | Standard SD Host Cont... | 100%   |          | DF82BB0E17 |
| 197b:2381 | 1071:9525 | JMicron Tech... | Standard SD Host Cont... | 60%    | 5.3.0    | EC12AF8F5D |
| 197b:2381 | 1179:fd30 | JMicron Tech... | Standard SD Host Cont... | 22.2%  | 3.14.33  | 9F5CEF220A |
| 197b:2381 | 1297:2000 | JMicron Tech... | Standard SD Host Cont... | 35.7%  | 4.4.0    | C227E1334E |
| 197b:2381 | 1297:2008 | JMicron Tech... | Standard SD Host Cont... | 100%   |          | 8F6ED609DD |
| 197b:2381 | 1297:2020 | JMicron Tech... | Standard SD Host Cont... | 42.9%  | 5.0.0    | DFE23BF8AF |
| 197b:2381 | 1297:2023 | JMicron Tech... | Standard SD Host Cont... | 100%   |          | C9ACF37E3D |
| 197b:2381 | 1297:2027 | JMicron Tech... | Standard SD Host Cont... | 53.1%  | 4.15.0   | F7F3A52A77 |
| 197b:2381 | 1297:2028 | JMicron Tech... | Standard SD Host Cont... | 16.7%  | 4.9.0    | 54C077FDFC |
| 197b:2381 | 14c0:0031 | JMicron Tech... | Standard SD Host Cont... | 100%   |          | 56B05900A0 |
| 197b:2381 | 1558:0801 | JMicron Tech... | Standard SD Host Cont... | 10.3%  | 4.9.20   | 7F6BCA365F |
| 197b:2381 | 1558:0803 | JMicron Tech... | Standard SD Host Cont... | 18.8%  | 4.15.0   | 72186D36EB |
| 197b:2381 | 1558:4120 | JMicron Tech... | Standard SD Host Cont... | 75%    | 4.20.17  | 127BDEC728 |
| 197b:2381 | 1558:7465 | JMicron Tech... | Standard SD Host Cont... | 14.3%  | 4.9.20   | 9E8AE2F340 |
| 197b:2381 | 17aa:212d | JMicron Tech... | Standard SD Host Cont... | 7.3%   | 3.14.44  | 3C9B38C20A |
| 197b:2381 | 17aa:3d9a | JMicron Tech... | Standard SD Host Cont... | 20%    | 4.1.3    | B0D0A28CC2 |
| 197b:2391 | 103c:1618 | JMicron Tech... | Standard SD Host Cont... | 9.8%   | 4.1.15   | E370B463B1 |
| 197b:2391 | 103c:1619 | JMicron Tech... | Standard SD Host Cont... | 7.4%   | 4.1.34   | 72808D19A6 |
| 197b:2391 | 103c:161c | JMicron Tech... | Standard SD Host Cont... | 26.1%  | 4.1.15   | 4536F4B488 |
| 197b:2391 | 103c:161d | JMicron Tech... | Standard SD Host Cont... | 33.3%  | 4.15.0   | 9A8967631B |
| 197b:2391 | 103c:1621 | JMicron Tech... | Standard SD Host Cont... | 61.5%  | 4.18.16  | 877E10CCD2 |
| 197b:2391 | 103c:162a | JMicron Tech... | Standard SD Host Cont... | 23.5%  | 4.15.0   | 9B95813BBB |
| 197b:2391 | 103c:162b | JMicron Tech... | Standard SD Host Cont... | 2.2%   | 3.14.44  | F5AF8974CF |
| 197b:2391 | 103c:1631 | JMicron Tech... | Standard SD Host Cont... | 13.3%  | 4.1.19   | F1C7178572 |
| 197b:2391 | 103c:1635 | JMicron Tech... | Standard SD Host Cont... | 66.7%  | 5.3.0    | 19BAD7A13F |
| 197b:2391 | 103c:167c | JMicron Tech... | Standard SD Host Cont... | 7.7%   | 4.1.4    | EB33D77F93 |
| 197b:2391 | 103c:167e | JMicron Tech... | Standard SD Host Cont... | 8.3%   | 3.14.44  | 9731571EC7 |
| 197b:2391 | 103c:168b | JMicron Tech... | Standard SD Host Cont... | 16.7%  | 3.14.44  | A8ED76864C |
| 197b:2391 | 103c:176b | JMicron Tech... | Standard SD Host Cont... | 4.8%   | 4.9.76   | F2997E7CAB |
| 197b:2391 | 103c:176c | JMicron Tech... | Standard SD Host Cont... | 9.1%   | 4.15.0   | FDBA82A5B5 |
| 197b:2391 | 103c:179b | JMicron Tech... | Standard SD Host Cont... | 20.8%  | 3.14.44  | DF84BBBC37 |
| 197b:2391 | 103c:179c | JMicron Tech... | Standard SD Host Cont... | 6.9%   | 4.9.20   | BDCEC83002 |
| 197b:2391 | 103c:17a7 | JMicron Tech... | Standard SD Host Cont... | 34.4%  | 3.14.44  | 4EDE694438 |
| 197b:2391 | 103c:17ab | JMicron Tech... | Standard SD Host Cont... | 17%    | 4.1.25   | 4D28001A69 |
| 197b:2391 | 103c:17ed | JMicron Tech... | Standard SD Host Cont... | 35.3%  | 3.14.44  | 6AE3EB396F |
| 197b:2391 | 103c:17f3 | JMicron Tech... | Standard SD Host Cont... | 40%    | 4.9.193  | 730E093BC4 |
| 197b:2391 | 103c:17f6 | JMicron Tech... | Standard SD Host Cont... | 14.7%  | 3.14.39  | 9D5FFAEF1D |
| 197b:2391 | 103c:180f | JMicron Tech... | Standard SD Host Cont... | 22.2%  | 4.9.20   | 06DA2207CD |
| 197b:2391 | 103c:18df | JMicron Tech... | Standard SD Host Cont... | 15.4%  | 3.14.44  | 4F747E9C8A |
| 197b:2391 | 103c:18f8 | JMicron Tech... | Standard SD Host Cont... | 16.7%  | 4.18.0   | E5FEF38D4A |
| 197b:2391 | 103c:3596 | JMicron Tech... | Standard SD Host Cont... | 100%   |          | 265CDC3301 |
| 197b:2391 | 1179:fc30 | JMicron Tech... | Standard SD Host Cont... | 12%    | 4.15.0   | 9D89ACB875 |
| 197b:2391 | 14c0:006b | JMicron Tech... | Standard SD Host Cont... | 100%   |          | C97368216B |
| 197b:2391 | 1558:2431 | JMicron Tech... | Standard SD Host Cont... | 100%   |          | F395EB44CF |
| 197b:2391 | 1558:2432 | JMicron Tech... | Standard SD Host Cont... | 100%   |          | 16EFC2E75F |
| 197b:2391 | 1558:2450 | JMicron Tech... | Standard SD Host Cont... | 100%   |          | 450ED4C040 |
| 197b:2391 | 1558:2700 | JMicron Tech... | Standard SD Host Cont... | 100%   |          | FBD3F68C8C |
| 197b:2391 | 1558:3500 | JMicron Tech... | Standard SD Host Cont... | 25%    | 4.15.0   | 7434BE9250 |
| 197b:2391 | 1558:4510 | JMicron Tech... | Standard SD Host Cont... | 40%    | 4.15.0   | 7886F96B81 |
| 197b:2391 | 17aa:3976 | JMicron Tech... | Standard SD Host Cont... | 4.3%   | 3.14.44  | A85C0AB7E0 |
| 197b:2391 | 17aa:3977 | JMicron Tech... | Standard SD Host Cont... | 28.6%  | 4.1.34   | 1EAEC7E819 |

### Sound (PCI)

224 out of 11675 (1.92%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 0045:c061 | 0045:c061 |                 | Audio device             | 100%   |          | 8D884B92FA |
| 1002:1308 | 1025:0864 | AMD             | Kaveri HDMI/DP Audio ... | 4%     | 3.14.44  | 8D6D195DA2 |
| 1002:1314 | 1025:0520 | AMD             | Wrestler HDMI Audio      | 2.8%   | 3.14.44  | BF118AA31C |
| 1002:1314 | 1043:84e7 | AMD             | Wrestler HDMI Audio      | 33.3%  | 4.15.0   | 58F57667EE |
| 1002:15b3 | 103c:84ac | AMD             | High Definition Audio... | 1.4%   | 4.15.0   | 4F1105BCA0 |
| 1002:15b3 | 103c:84e5 | AMD             | High Definition Audio... | 33.3%  | 4.15.0   | 9087960124 |
| 1002:4383 | 1025:0520 | AMD             | SBx00 Azalia (Intel HDA) | 2.8%   | 3.14.44  | BF118AA31C |
| 1002:4383 | 1043:836c | AMD             | SBx00 Azalia (Intel HDA) | 1%     | 3.10.0   | 04BFACB4A7 |
| 1002:4383 | 1043:8444 | AMD             | SBx00 Azalia (Intel HDA) | 1.6%   | 3.14.33  | 9FE1C71EC5 |
| 1002:4383 | 1043:8445 | AMD             | SBx00 Azalia (Intel HDA) | 0.2%   | 3.10.0   | 8A4E34A210 |
| 1002:4383 | 1043:84fb | AMD             | SBx00 Azalia (Intel HDA) | 0.6%   | 3.14.44  | D3AEFE0601 |
| 1002:4383 | 1043:8576 | AMD             | SBx00 Azalia (Intel HDA) | 0.6%   | 3.14.44  | 35D0F345A4 |
| 1002:4383 | 1458:a182 | AMD             | SBx00 Azalia (Intel HDA) | 0.3%   | 3.10.0   | C3443E0857 |
| 1002:960f | 1002:960f | AMD             | RS780 HDMI Audio [Rad... | 0.8%   | 3.10.0   | C3443E0857 |
| 1002:970f | 1458:960f | AMD             | RS880 HDMI Audio [Rad... | 1.9%   | 3.14.44  | 911703286C |
| 1002:9840 | 103c:8245 | AMD             | Kabini HDMI/DP Audio     | 10%    | 4.9.20   | B348BC9186 |
| 1002:9840 | 17aa:2219 | AMD             | Kabini HDMI/DP Audio     | 25%    | 4.9.60   | 94058A82CA |
| 1002:9902 | 1462:7721 | AMD             | Trinity HDMI Audio Co... | 2.3%   | 3.14.44  | 4587AB8EDD |
| 1002:aa38 | 1002:aa38 | AMD             | RV710/730 HDMI Audio ... | 1.1%   | 3.14.25  | 8596529915 |
| 1002:aa38 | 1462:aa38 | AMD             | RV710/730 HDMI Audio ... | 2.3%   | 3.14.44  | 51837DE98F |
| 1002:aa38 | 174b:aa38 | AMD             | RV710/730 HDMI Audio ... | 2.9%   | 3.14.25  | B701C37D96 |
| 1002:aa68 | 1025:0487 | AMD             | Cedar HDMI Audio [Rad... | 2.9%   | 3.14.44  | 68F61986F8 |
| 1002:aa68 | 1545:aa68 | AMD             | Cedar HDMI Audio [Rad... | 33.3%  | 4.19.0   | 51D516FF60 |
| 1002:aa90 | 1179:fb41 | AMD             | Turks HDMI Audio [Rad... | 5.9%   | 3.14.44  | 67009EFFAA |
| 1002:aa98 | 1043:aa98 | AMD             | Caicos HDMI Audio [Ra... | 1.1%   | 3.0.38   | 2A34C16AB3 |
| 1002:aa98 | 174b:aa98 | AMD             | Caicos HDMI Audio [Ra... | 0.8%   | 3.14.22  | 24BF705591 |
| 1002:aab0 | 103c:1990 | AMD             | Oland/Hainan/Cape Ver... | 10%    | 4.18.0   | DCE9CDAF8E |
| 1002:aab0 | 1043:aab0 | AMD             | Oland/Hainan/Cape Ver... | 0.7%   | 3.14.22  | 66219C1D36 |
| 1002:aab0 | 1682:aab0 | AMD             | Oland/Hainan/Cape Ver... | 0.8%   | 3.14.22  | D3AEFE0601 |
| 1002:aab0 | 174b:aab0 | AMD             | Oland/Hainan/Cape Ver... | 0.2%   | 3.13.0   | 9B9C670167 |
| 1002:aac0 | 103c:aac0 | AMD             | Tobago HDMI Audio [Ra... | 50%    | 5.4.0    | B9EB4A5652 |
| 1002:aac0 | 1458:aac0 | AMD             | Tobago HDMI Audio [Ra... | 3.1%   | 3.14.44  | 62E0E97099 |
| 1002:aae0 | 1043:aae0 | AMD             | Baffin HDMI/DP Audio ... | 0.7%   | 4.1.25   | 9D3FE31D76 |
| 1002:aae0 | 1682:aae0 | AMD             | Baffin HDMI/DP Audio ... | 1.6%   | 4.9.60   | 8212CC8601 |
| 1002:aaf0 | 148c:aaf0 | AMD             | Ellesmere HDMI Audio ... | 0.9%   | 4.10.16  | F61EE20F03 |
| 1002:aaf0 | 1da2:aaf0 | AMD             | Ellesmere HDMI Audio ... | 0.8%   | 4.9.20   | 94B280C39D |
| 1022:1457 | 1462:cb09 | AMD             | Family 17h (Models 00... | 25%    | 4.15.0   | F7A48733A6 |
| 1022:1457 | 1462:cb79 | AMD             | Family 17h (Models 00... | 1.9%   | 4.9.60   | C818EB5CB4 |
| 1022:1457 | 1462:fa39 | AMD             | Family 17h (Models 00... | 6.2%   | 4.9.60   | 84ED791AF7 |
| 1022:1457 | 1849:2220 | AMD             | Family 17h (Models 00... | 5.6%   | 4.18.0   | 707960B3EC |
| 1022:1487 | 1022:c950 | AMD             | Starship/Matisse HD A... | 33.3%  | 5.6.4    | 09640A1376 |
| 1022:1487 | 1849:d887 | AMD             | Starship/Matisse HD A... | 25%    | 4.15.0   | F61EE20F03 |
| 1022:157a | 103c:84ac | AMD             | Family 15h (Models 60... | 1.5%   | 4.15.0   | 4F1105BCA0 |
| 1022:157a | 103c:84e5 | AMD             | Family 15h (Models 60... | 33.3%  | 4.15.0   | 9087960124 |
| 1022:2093 | 1022:2093 | AMD             | CS5536 [Geode compani... | 100%   |          | 6D9551F87E |
| 1022:780d | 1025:0864 | AMD             | FCH Azalia Controller    | 4%     | 3.14.44  | 8D6D195DA2 |
| 1022:780d | 103c:8245 | AMD             | FCH Azalia Controller    | 10%    | 4.9.20   | B348BC9186 |
| 1022:780d | 1043:8576 | AMD             | FCH Azalia Controller    | 0.3%   | 3.14.25  | 7E0AF76200 |
| 1022:780d | 1043:85cd | AMD             | FCH Azalia Controller    | 4%     | 3.14.44  | CDC3F83CDB |
| 1022:780d | 1043:86c7 | AMD             | FCH Azalia Controller    | 20%    | 4.9.14   | 71ABA86389 |
| 1022:780d | 1462:d721 | AMD             | FCH Azalia Controller    | 0.7%   | 3.14.33  | 4587AB8EDD |
| 106b:1803 | 106b:1803 | Apple           | Audio Device             | 100%   |          | B88416C7C1 |
| 106b:1803 | 106b:1880 | Apple           | Audio Device             | 83.3%  | 5.6.19   | 935B673683 |
| 106b:1803 | 106b:1881 | Apple           | Audio Device             | 100%   |          | E4D129C0D2 |
| 106b:1803 | 106b:1885 | Apple           | Audio Device             | 100%   |          | D3A040508D |
| 1073:1000 | 1073:1000 | Yamaha          | SW1000XG [XG Factory]    | 100%   |          | 4DCC71B299 |
| 10de:0059 | 1043:81ae | Nvidia          | CK804 AC'97 Audio Con... | 50%    | 3.14.25  | A6659EE127 |
| 10de:006b | 1043:0c11 | Nvidia          | nForce Audio Processi... | 100%   |          | 543960170E |
| 10de:006b | 147b:1c00 | Nvidia          | nForce Audio Processi... | 100%   |          | CB892B4614 |
| 10de:03f0 | 103c:2a6c | Nvidia          | MCP61 High Definition... | 2%     | 4.1.15   | 52991F9A5A |
| 10de:03f0 | 1458:a002 | Nvidia          | MCP61 High Definition... | 0.4%   | 3.14.15  | 9D9E2DB550 |
| 10de:03f0 | 1849:0888 | Nvidia          | MCP61 High Definition... | 19%    | 3.14.53  | B701C37D96 |
| 10de:0774 | 1043:836c | Nvidia          | MCP72XE/MCP72P/MCP78U... | 5.6%   | 3.10.19  | E1B7D175A1 |
| 10de:0774 | 1462:7578 | Nvidia          | MCP72XE/MCP72P/MCP78U... | 16.7%  | 4.9.20   | 8F804041A2 |
| 10de:0ac0 | 103c:2aa1 | Nvidia          | MCP79 High Definition... | 50%    | 4.18.0   | C2FD4F3C01 |
| 10de:0be3 | 1043:8354 | Nvidia          | High Definition Audio... | 1.9%   | 3.14.44  | 67BFE1B221 |
| 10de:0be3 | 1043:8490 | Nvidia          | High Definition Audio... | 21.7%  | 4.1.38   | A6659EE127 |
| 10de:0be3 | 1462:8094 | Nvidia          | High Definition Audio... | 1.1%   | 3.14.44  | 895D8612B4 |
| 10de:0be3 | 3842:1310 | Nvidia          | High Definition Audio... | 57.1%  | 4.9.124  | 9FE1C71EC5 |
| 10de:0bea | 1462:2304 | Nvidia          | GF108 High Definition... | 9.1%   | 3.14.44  | ED9D8A148D |
| 10de:0bea | 1991:5584 | Nvidia          | GF108 High Definition... | 50%    | 4.1.34   | CE8124E5F4 |
| 10de:0bee |           | Nvidia          | GF116 High Definition... | 1.1%   | 3.14.39  | 77909796EC |
| 10de:0e08 |           | Nvidia          | GF119 HDMI Audio Cont... | 2.8%   | 3.14.33  | 8F9504F263 |
| 10de:0e08 | 174b:0620 | Nvidia          | GF119 HDMI Audio Cont... | 50%    | 4.9.60   | 6566319F04 |
| 10de:0e0f | 1043:84f5 | Nvidia          | GK208 HDMI/DP Audio C... | 2.9%   | 3.14.44  | 35D0F345A4 |
| 10de:0e0f | 19da:7326 | Nvidia          | GK208 HDMI/DP Audio C... | 2.4%   | 4.9.60   | 84ED791AF7 |
| 10de:0e0f | 3842:1731 | Nvidia          | GK208 HDMI/DP Audio C... | 100%   |          | 04BFACB4A7 |
| 10de:0e1b | 10de:094b | Nvidia          | GK107 HDMI Audio Cont... | 5.3%   | 4.1.15   | 949DD823D7 |
| 10de:0e1b | 1462:8a9e | Nvidia          | GK107 HDMI Audio Cont... | 4.2%   | 3.14.44  | 05258AEA35 |
| 10de:0e1b | 1569:0fc6 | Nvidia          | GK107 HDMI Audio Cont... | 1%     | 3.14.33  | 8F804041A2 |
| 10de:0fb0 | 1462:3232 | Nvidia          | GM200 High Definition... | 12.5%  | 5.0.0    | AF58D23265 |
| 10de:0fb9 | 1025:1265 | Nvidia          | GP107GL High Definiti... | 2.1%   | 4.15.0   | 077D639C2D |
| 10de:0fb9 | 1043:85d3 | Nvidia          | GP107GL High Definiti... | 16.7%  | 4.1.25   | E1E2F84AB5 |
| 10de:0fb9 | 10de:12af | Nvidia          | GP107GL High Definiti... | 100%   |          | C11BA25134 |
| 10de:0fb9 | 1462:8c96 | Nvidia          | GP107GL High Definiti... | 1.9%   | 4.1.38   | 15193EDA95 |
| 10de:0fba | 1043:8520 | Nvidia          | GM206 High Definition... | 2.6%   | 3.14.53  | 8D2A73DD23 |
| 10de:0fba | 3842:2962 | Nvidia          | GM206 High Definition... | 100%   |          | 707960B3EC |
| 10de:0fbb | 1458:3672 | Nvidia          | GM204 High Definition... | 66.7%  | 4.15.0   | 57643353CE |
| 10de:0fbb | 1458:367c | Nvidia          | GM204 High Definition... | 100%   |          | 57643353CE |
| 10de:0fbc | 1462:3102 | Nvidia          | GM107 High Definition... | 4.5%   | 3.14.44  | 071F922873 |
| 10de:0fbc | 3842:3753 | Nvidia          | GM107 High Definition... | 7.1%   | 4.9.60   | 541846E7D7 |
| 10de:10ef | 1462:3602 | Nvidia          | GP102 HDMI Audio Cont... | 10%    | 4.15.0   | 6AFD8A5657 |
| 10de:10ef | 1462:360c | Nvidia          | GP102 HDMI Audio Cont... | 75%    | 5.7.6    | F7A48733A6 |
| 10de:10f0 | 1043:8597 | Nvidia          | GP104 High Definition... | 16.7%  | 4.15.0   | 32166A5865 |
| 10de:10f0 | 1558:0879 | Nvidia          | GP104 High Definition... | 50%    | 4.19.0   | A7DB7C544F |
| 10de:10f0 | 19da:2435 | Nvidia          | GP104 High Definition... | 3.3%   | 5.1.6    | C818EB5CB4 |
| 10de:10f1 | 103c:8581 | Nvidia          | GP106 High Definition... | 25%    | 4.15.0   | 85885ECEF9 |
| 10de:10f1 | 10de:1c03 | Nvidia          | GP106 High Definition... | 1.6%   | 4.9.20   | E996F15E3E |
| 10de:10f1 | 1458:3724 | Nvidia          | GP106 High Definition... | 1.6%   | 4.1.34   | E40B76E473 |
| 10de:10f1 | 1462:3490 | Nvidia          | GP106 High Definition... | 20%    | 4.15.0   | 1B722DF896 |
| 10de:10f9 | 10de:12fe | Nvidia          | TU106 High Definition... | 33.3%  | 5.4.0    | 0FA979BBFB |
| 10de:10fa | 103c:8611 | Nvidia          | TU107 GeForce GTX 165... | 100%   |          | BDD15B19B1 |
| 10de:1aeb | 1028:0949 | Nvidia          | TU116 High Definition... | 3.4%   | 5.0.0    | E0FB0728BB |
| 10de:1aeb | 1458:4014 | Nvidia          | TU116 High Definition... | 14.3%  | 5.3.0    | 03EEF2B7D3 |
| 1102:0004 | 1102:1003 | Creative Labs   | EMU10k2/CA0100/CA0102... | 6.7%   | 4.1.15   | D74C162548 |
| 1102:0004 | 1102:2002 | Creative Labs   | EMU10k2/CA0100/CA0102... | 1.6%   | 3.14.44  | 2B0A36F85F |
| 1102:0007 | 1102:100a | Creative Labs   | CA0106/CA0111 [SB Liv... | 1.7%   | 3.14.25  | BCEA5A9B37 |
| 1102:000b | 1102:0041 | Creative Labs   | EMU20k2 [Sound Blaste... | 4.5%   | 4.1.16   | 947267E711 |
| 1102:0012 | 1102:0010 | Creative Labs   | Sound Core3D [Sound B... | 1.2%   | 3.14.44  | 57643353CE |
| 1274:1371 | 1274:1371 | Ensoniq         | ES1371/ES1373 / Creat... | 8.1%   | 3.14.44  | CB5FCEB934 |
| 13f2:0111 |           | Ford Microel... |                          | 100%   |          | 95162A226D |
| 13f2:0111 | ffff:ffff | Ford Microel... | Multimedia audio cont... | 100%   |          | 95162A226D |
| 13f6:0111 | 153b:1144 | C-Media Elec... | CMI8738/CMI8768 PCI A... | 5.6%   | 4.1.25   | 86F297ED58 |
| 13f6:8788 | 1043:8427 | C-Media Elec... | CMI8788 [Oxygen HD Au... | 100%   |          | BFB822D98C |
| 13f6:8788 | 1043:8463 | C-Media Elec... | CMI8788 [Oxygen HD Au... | 100%   |          | 9E13784BB3 |
| 13f6:8788 | 1043:8521 | C-Media Elec... | CMI8788 [Oxygen HD Au... | 1.6%   | 3.14.44  | 45FCBC8B9A |
| 13f6:8788 | 1043:855e | C-Media Elec... | CMI8788 [Oxygen HD Au... | 100%   |          | A610823FCB |
| 13f6:8788 | 7284:9783 | C-Media Elec... | CMI8788 [Oxygen HD Au... | 100%   |          | 40EA4505B9 |
| 1412:1624 | 1412:2403 | VIA Technolo... | Multimedia audio cont... | 100%   |          | 2AF6424751 |
| 19fe:7000 | 0e51:0002 | ESI             | MAYA44e Controller       | 100%   |          | D91E94A951 |
| 8086:02c8 | 1028:0954 | Intel           | Comet Lake PCH-LP cAVS   | 100%   |          | 8740133E10 |
| 8086:02c8 | 1043:1a61 | Intel           | Comet Lake PCH-LP cAVS   | 50%    | 5.3.0    | 4EA8D503AE |
| 8086:0a0c | 103c:2249 | Intel           | Haswell-ULT HD Audio ... | 12.5%  | 4.1.25   | 8DCBD3C2B1 |
| 8086:0c0c | 8086:0c0c | Intel           | Xeon E3-1200 v3/4th G... | 5.3%   | 4.9.60   | 77909796EC |
| 8086:0c0c | 8086:2010 | Intel           | Xeon E3-1200 v3/4th G... | 0.5%   | 2.6.32   | DFDA14135D |
| 8086:0f04 | 1043:14dd | Intel           | Atom Processor Z36xxx... | 1.6%   | 3.14.33  | 106830C1CC |
| 8086:0f04 | 17aa:3695 | Intel           | Atom Processor Z36xxx... | 50%    | 4.15.0   | 08BB09B100 |
| 8086:0f28 | 17aa:3907 | Intel           | Atom Processor Z36xxx... | 100%   |          | 6D960BD235 |
| 8086:0f28 | 8086:0f28 | Intel           | Atom Processor Z36xxx... | 100%   |          | 87E6D2F056 |
| 8086:0f28 | 8086:7270 | Intel           | Atom Processor Z36xxx... | 100%   |          | 44359D461E |
| 8086:160c | 1025:098a | Intel           | Broadwell-U Audio Con... | 1%     | 3.14.44  | 4F849E1E80 |
| 8086:160c | 1025:1019 | Intel           | Broadwell-U Audio Con... | 100%   |          | 5DBE9649A7 |
| 8086:160c | 17aa:390b | Intel           | Broadwell-U Audio Con... | 4.5%   | 4.9.60   | AB6BD693BE |
| 8086:1c20 | 1025:0504 | Intel           | 6 Series/C200 Series ... | 0.5%   | 3.10.0   | 8FE3AF49FB |
| 8086:1c20 | 1028:0492 | Intel           | 6 Series/C200 Series ... | 5%     | 4.9.60   | EAFEF7DB79 |
| 8086:1c20 | 1028:0493 | Intel           | 6 Series/C200 Series ... | 3.9%   | 3.14.33  | EFD71FBD61 |
| 8086:1c20 | 1043:841b | Intel           | 6 Series/C200 Series ... | 2.4%   | 3.10.34  | 07EF877C6B |
| 8086:1c20 | 1043:8445 | Intel           | 6 Series/C200 Series ... | 0.3%   | 3.10.0   | 1678EE56C3 |
| 8086:1c20 | 10cf:15dc | Intel           | 6 Series/C200 Series ... | 1.9%   | 4.1.34   | 958D094890 |
| 8086:1c20 | 1462:7673 | Intel           | 6 Series/C200 Series ... | 6.7%   | 3.14.33  | 15193EDA95 |
| 8086:1c20 | 1849:1892 | Intel           | 6 Series/C200 Series ... | 2.2%   | 3.10.0   | 895D8612B4 |
| 8086:1c20 | 1849:3662 | Intel           | 6 Series/C200 Series ... | 2.9%   | 3.14.25  | 0139CCFE4A |
| 8086:1d20 | 1028:05d2 | Intel           | C600/X79 series chips... | 4.2%   | 4.12.14  | 949DD823D7 |
| 8086:1d20 | 8086:1d20 | Intel           | C600/X79 series chips... | 4.8%   | 4.4.0    | BBFC99D048 |
| 8086:1e20 | 1025:074f | Intel           | 7 Series/C216 Chipset... | 66.7%  | 5.4.0    | 6566319F04 |
| 8086:1e20 | 1028:052c | Intel           | 7 Series/C216 Chipset... | 3.7%   | 4.15.0   | 29A0FC6CE0 |
| 8086:1e20 | 103c:1845 | Intel           | 7 Series/C216 Chipset... | 16.7%  | 3.14.44  | 2E60620A98 |
| 8086:1e20 | 1179:fb40 | Intel           | 7 Series/C216 Chipset... | 12.5%  | 4.1.15   | 67009EFFAA |
| 8086:1e20 | 1297:2033 | Intel           | 7 Series/C216 Chipset... | 11.1%  | 4.9.20   | 9137B29AFE |
| 8086:1e20 | 1458:a002 | Intel           | 7 Series/C216 Chipset... | 0.5%   | 4.15.0   | 740BF21A40 |
| 8086:1e20 | 17aa:21fb | Intel           | 7 Series/C216 Chipset... | 8%     | 4.9.20   | 55427995B5 |
| 8086:1e20 | 17aa:3083 | Intel           | 7 Series/C216 Chipset... | 10%    | 4.9.111  | E3BF127788 |
| 8086:1e20 | 17aa:3977 | Intel           | 7 Series/C216 Chipset... | 0.3%   | 3.10.42  | 2DD89E3983 |
| 8086:1e20 | 8086:1e20 | Intel           | 7 Series/C216 Chipset... | 2.8%   | 4.1.34   | CE8124E5F4 |
| 8086:2284 | 1025:1009 | Intel           | Atom/Celeron/Pentium ... | 16.7%  | 4.9.20   | 401BBED185 |
| 8086:2284 | 1028:06ac | Intel           | Atom/Celeron/Pentium ... | 1.7%   | 4.4.18   | B5721FA9D5 |
| 8086:2284 | 1043:1cbd | Intel           | Atom/Celeron/Pentium ... | 14.3%  | 4.9.9    | 71CCEBC0C1 |
| 8086:22a8 | 8086:7270 | Intel           | Atom/Celeron/Pentium ... | 100%   |          | 29FF18D6F2 |
| 8086:266e | 103c:3006 | Intel           | 82801FB/FBM/FR/FW/FRW... | 25%    | 4.9.20   | 51837DE98F |
| 8086:266e | 1179:ff00 | Intel           | 82801FB/FBM/FR/FW/FRW... | 3.7%   | 4.15.0   | 8488B3D0B9 |
| 8086:266e | 1458:ae01 | Intel           | 82801FB/FBM/FR/FW/FRW... | 8%     | 3.14.44  | FD291EB728 |
| 8086:269a | 103c:1307 | Intel           | 631xESB/632xESB High ... | 42.9%  | 4.1.15   | 51D516FF60 |
| 8086:27d8 | 1019:2683 | Intel           | NM10/ICH7 Family High... | 1.9%   | 3.14.44  | EAA25586D2 |
| 8086:27d8 | 1025:0349 | Intel           | NM10/ICH7 Family High... | 1%     | 3.14.44  | F556D9CE96 |
| 8086:27d8 | 1028:0220 | Intel           | NM10/ICH7 Family High... | 4.3%   | 3.14.44  | BBA0FE2672 |
| 8086:27d8 | 1043:8290 | Intel           | NM10/ICH7 Family High... | 0.4%   | 3.14.25  | 45FCBC8B9A |
| 8086:27d8 | 1043:83d4 | Intel           | NM10/ICH7 Family High... | 1.1%   | 3.14.44  | 8807184E95 |
| 8086:27d8 | 104d:81fc | Intel           | NM10/ICH7 Family High... | 100%   |          | 7F0BB0CC92 |
| 8086:27d8 | 1458:a002 | Intel           | NM10/ICH7 Family High... | 0.1%   | 3.13.0   | D6C3BCD69B |
| 8086:27d8 | 1462:104e | Intel           | NM10/ICH7 Family High... | 20%    | 4.1.15   | 5F15F028A8 |
| 8086:27d8 | 1854:005f | Intel           | NM10/ICH7 Family High... | 20%    | 4.15.0   | F60C56AC42 |
| 8086:27d8 | 1b0a:0001 | Intel           | NM10/ICH7 Family High... | 3.7%   | 3.14.44  | 396BE2A324 |
| 8086:284b | 103c:3618 | Intel           | 82801H (ICH8 Family) ... | 10.5%  | 3.14.44  | 13824A2872 |
| 8086:284b | 1734:1083 | Intel           | 82801H (ICH8 Family) ... | 17.6%  | 3.14.44  | F626D15B06 |
| 8086:293e | 1025:017e | Intel           | 82801I (ICH9 Family) ... | 20%    | 4.1.25   | 8596529915 |
| 8086:293e | 103c:281e | Intel           | 82801I (ICH9 Family) ... | 1.7%   | 3.14.44  | 61D1ED752A |
| 8086:293e | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 12.5%  | 3.14.44  | 93C0EF7223 |
| 8086:293e | 1458:a022 | Intel           | 82801I (ICH9 Family) ... | 6.7%   | 3.14.44  | 071F922873 |
| 8086:34c8 | 1028:0979 | Intel           | Ice Lake-LP Smart Sou... | 10.5%  | 5.0.0    | 7F4CE08DF9 |
| 8086:34c8 | 1028:097a | Intel           | Ice Lake-LP Smart Sou... | 16.7%  | 5.4.0    | 187E195C78 |
| 8086:3a3e | 1028:0293 | Intel           | 82801JI (ICH10 Family... | 4.2%   | 3.10.0   | 9434F7214C |
| 8086:3a6e | 1028:0420 | Intel           | 82801JD/DO (ICH10 Fam... | 0.9%   | 3.10.0   | 2B2AA48899 |
| 8086:3b56 | 1025:0487 | Intel           | 5 Series/3400 Series ... | 0.5%   | 3.14.25  | 68F61986F8 |
| 8086:3b56 | 103c:3674 | Intel           | 5 Series/3400 Series ... | 9.1%   | 4.15.0   | F4DE983D96 |
| 8086:3b56 | 103c:7008 | Intel           | 5 Series/3400 Series ... | 2.2%   | 3.10.34  | 5DD7A5FCE1 |
| 8086:3b56 | 1043:8375 | Intel           | 5 Series/3400 Series ... | 1%     | 3.14.44  | E40B76E473 |
| 8086:3b56 | 1458:a002 | Intel           | 5 Series/3400 Series ... | 0.5%   | 3.10.42  | 66219C1D36 |
| 8086:3b56 | 1849:6718 | Intel           | 5 Series/3400 Series ... | 10%    | 3.14.25  | 1D9934126C |
| 8086:5a98 | 8086:7270 | Intel           | Celeron N3350/Pentium... | 12%    | 4.4.0    | 622CED4019 |
| 8086:8c20 | 1028:05a4 | Intel           | 8 Series/C220 Series ... | 1.3%   | 3.10.0   | 541846E7D7 |
| 8086:8c20 | 1043:143f | Intel           | 8 Series/C220 Series ... | 9.1%   | 4.9.41   | A268D267B1 |
| 8086:8c20 | 1458:a002 | Intel           | 8 Series/C220 Series ... | 0.9%   | 3.10.0   | E996F15E3E |
| 8086:8c20 | 8086:8c20 | Intel           | 8 Series/C220 Series ... | 7.1%   | 4.9.124  | 77909796EC |
| 8086:8ca0 | 1462:d917 | Intel           | 9 Series Chipset Fami... | 3.8%   | 4.1.15   | 8D2A73DD23 |
| 8086:8d20 | 1043:8699 | Intel           | C610/X99 series chips... | 25%    | 4.1.25   | 8212CC8601 |
| 8086:8d20 | 1458:a182 | Intel           | C610/X99 series chips... | 7.1%   | 4.1.15   | 6AFD8A5657 |
| 8086:9c20 | 103c:2249 | Intel           | 8 Series HD Audio Con... | 12.5%  | 4.1.25   | 8DCBD3C2B1 |
| 8086:9ca0 | 1025:098a | Intel           | Wildcat Point-LP High... | 1%     | 3.14.44  | 4F849E1E80 |
| 8086:9ca0 | 1025:1019 | Intel           | Wildcat Point-LP High... | 100%   |          | 5DBE9649A7 |
| 8086:9ca0 | 17aa:390b | Intel           | Wildcat Point-LP High... | 4.5%   | 4.9.60   | AB6BD693BE |
| 8086:9d71 | 1028:075b | Intel           | Sunrise Point-LP HD A... | 2.1%   | 4.4.0    | 6695D2A05E |
| 8086:9d71 | 17aa:225d | Intel           | Sunrise Point-LP HD A... | 2.2%   | 4.14.35  | 7D7E6AD5D5 |
| 8086:9d71 | 1ae0:006b | Intel           | Sunrise Point-LP HD A... | 33.3%  | 5.1.15   | 5F781E103C |
| 8086:9d71 | 1ae0:006c | Intel           | Sunrise Point-LP HD A... | 100%   |          | 937EA6678F |
| 8086:9d72 | 1028:06e6 | Intel           | 300 Series Chipset Sm... | 100%   |          | B7465A5AE4 |
| 8086:9dc8 | 1025:129a | Intel           | Cannon Point-LP High ... | 14.3%  | 5.0.0    | 6E9BFB3B01 |
| 8086:9dc8 | 1028:089d | Intel           | Cannon Point-LP High ... | 11.1%  | 4.15.0   | DAF389F21B |
| 8086:9dc8 | 1028:08a8 | Intel           | Cannon Point-LP High ... | 11.1%  | 4.15.0   | B6DF9FEC5F |
| 8086:9dc8 | 103c:857f | Intel           | Cannon Point-LP High ... | 25%    | 5.3.0    | A838427772 |
| 8086:a170 | 103c:8257 | Intel           | 100 Series/C230 Serie... | 14.3%  | 4.15.0   | D079BA6F90 |
| 8086:a170 | 1043:86ae | Intel           | 100 Series/C230 Serie... | 4%     | 4.1.38   | 57643353CE |
| 8086:a170 | 1462:d970 | Intel           | 100 Series/C230 Serie... | 16.7%  | 4.1.25   | 0FA979BBFB |
| 8086:a170 | 1462:f996 | Intel           | 100 Series/C230 Serie... | 1.4%   | 4.1.15   | 9B9C670167 |
| 8086:a171 | 144d:c790 | Intel           | CM238 HD Audio Contro... | 25%    | 4.15.0   | F8A5C21D24 |
| 8086:a2f0 | 103c:82f2 | Intel           | 200 Series PCH HD Audio  | 8.3%   | 4.9.60   | 49D42CD641 |
| 8086:a2f0 | 1043:8735 | Intel           | 200 Series PCH HD Audio  | 8%     | 4.9.95   | 816A1797C5 |
| 8086:a2f0 | 1458:a182 | Intel           | 200 Series PCH HD Audio  | 1.2%   | 3.10.0   | 1A67024C19 |
| 8086:a2f0 | 1558:0879 | Intel           | 200 Series PCH HD Audio  | 25%    | 4.18.0   | A7DB7C544F |
| 8086:a348 | 1025:126c | Intel           | Cannon Lake PCH cAVS     | 100%   |          | C1339E884A |
| 8086:a348 | 1028:0851 | Intel           | Cannon Lake PCH cAVS     | 100%   |          | 05D6B79D2F |
| 8086:a348 | 1028:0949 | Intel           | Cannon Lake PCH cAVS     | 2.1%   | 4.19.0   | E0FB0728BB |
| 8086:a348 | 103c:8581 | Intel           | Cannon Lake PCH cAVS     | 25%    | 4.15.0   | 85885ECEF9 |
| 8086:a348 | 103c:860f | Intel           | Cannon Lake PCH cAVS     | 50%    | 5.3.0    | BDD15B19B1 |
| 8086:a348 | 17aa:36e7 | Intel           | Cannon Lake PCH cAVS     | 25%    | 4.15.0   | 1B722DF896 |

### Storage (PCI)

67 out of 182 (36.81%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 104c:8033 | 1179:ff05 | Texas Instru... | PCIxx21/PCIxx11 Flash... | 5.9%   | 4.15.0   | 8488B3D0B9 |
| 104c:803b | 1025:011f | Texas Instru... | PCIxx12 Flash Media C... | 0.7%   | 3.14.33  | 2EE51E8201 |
| 104c:803b | 104d:81fc | Texas Instru... | PCIxx12 Flash Media C... | 100%   |          | 7F0BB0CC92 |
| 104c:803b | 17aa:207c | Texas Instru... | PCIxx12 Flash Media C... | 12.5%  | 3.14.44  | E5C5CE1445 |
| 1106:401a | 1028:02f5 | VIA Technolo... | VIA Card Reader Host ... | 100%   |          | 7AE0ACB2B9 |
| 1106:401a | 1028:0408 | VIA Technolo... | VIA Card Reader Host ... | 100%   |          | 3125B9C83A |
| 1106:401a | 1071:9515 | VIA Technolo... | VIA Card Reader Host ... | 100%   |          | E028F277D4 |
| 1106:401a | 1106:401a | VIA Technolo... | VIA Card Reader Host ... | 100%   |          | AAF6FAFAD6 |
| 1106:401a | 17aa:3608 | VIA Technolo... | VIA Card Reader Host ... | 100%   |          | 72EB4FFFCD |
| 117c:0064 | 117c:0064 | ATTO Technology | Celerity FC 16Gb/s Ge... | 100%   |          | 43EE2001E1 |
| 11f8:8032 | 117c:003b | PMC-Sierra      | PM8032 Tachyon QE8       | 66.7%  | 4.15.0   | 48E71CC737 |
| 1217:7130 | 1019:300e | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 3C221F81A4 |
| 1217:7130 | 1025:010d | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | BA71663ED2 |
| 1217:7130 | 1025:011a | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 9BB4619272 |
| 1217:7130 | 1025:0123 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | B127BEAD10 |
| 1217:7130 | 1025:0124 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 5AAFE28787 |
| 1217:7130 | 1025:012b | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 21509117BA |
| 1217:7130 | 1025:013c | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | CBD537F7C5 |
| 1217:7130 | 1028:026f | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 92D79B3562 |
| 1217:7130 | 1028:0273 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 18A84B723B |
| 1217:7130 | 1028:0275 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | B0314C0713 |
| 1217:7130 | 1071:8258 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 98006DB3BD |
| 1217:7130 | 107b:0390 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 2654A3A599 |
| 1217:7130 | 107b:0696 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | E9F51C8451 |
| 1217:7130 | 107b:0704 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 713D68894F |
| 1217:7130 | 10cf:13c6 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 7B7919A092 |
| 1217:7130 | 10cf:143d | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | AA22FCA8FD |
| 1217:7130 | 10cf:14d6 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 26C7C388C2 |
| 1217:7130 | 1179:ff50 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 872199F2C5 |
| 1217:7130 | 1462:3fbb | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | FDCEAF9E02 |
| 1217:7130 | 1462:3fc1 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | BB5381D738 |
| 1217:7130 | 1462:3fe9 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | DA33747D00 |
| 1217:7130 | 1462:3ff3 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 151BD38176 |
| 1217:7130 | 1462:4327 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 3F04DA7D3F |
| 1217:7130 | 1462:63f6 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | BA35BAD99E |
| 1217:7130 | 1462:6440 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 43D96E36AB |
| 1217:7130 | 1462:7220 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | F3055F11EE |
| 1217:7130 | 14ff:a003 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 7EE061C41D |
| 1217:7130 | 1631:0188 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 856B9A1A68 |
| 1217:7130 | 1631:c218 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | D49593181C |
| 1217:7130 | 1734:10b8 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | F374910DD4 |
| 1217:7130 | 1734:10c7 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | F231CEAF4A |
| 1217:7130 | 17aa:3a21 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | BF3EE678DA |
| 1217:8130 | 1025:019f | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | 806ABC807D |
| 1217:8130 | 1025:038b | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | 1B520F3904 |
| 1217:8130 | 1028:02bb | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | 82F898B8B3 |
| 1217:8130 | 1028:02bc | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | E66BD45962 |
| 1217:8130 | 1028:02c0 | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | 9A7F9AAED3 |
| 1217:8130 | 1028:02ea | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | EFA8CE8686 |
| 1217:8130 | 1028:02eb | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | 7AB545CC97 |
| 1217:8130 | 1028:041b | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | EF8551E796 |
| 1217:8130 | 10cf:1568 | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | 58DBBB5F10 |
| 1217:8130 | 1179:ff50 | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | CECAD53985 |
| 1217:8231 | 1028:0493 | O2 Micro        | O2Micro Integrated MS... | 100%   |          | 31856A4442 |
| 1217:8231 | 1028:04a9 | O2 Micro        | O2Micro Integrated MS... | 100%   |          | 2177469041 |
| 1217:8330 | 1028:04a3 | O2 Micro        | OZ600 MS/xD Controller   | 100%   |          | 2FB606DA9C |
| 1217:8330 | 1028:04a4 | O2 Micro        | OZ600 MS/xD Controller   | 100%   |          | 6D3F2A9279 |
| 1217:8330 | 10cf:16ae | O2 Micro        | OZ600 MS/xD Controller   | 100%   |          | 1D864A6855 |
| 1217:8331 | 1028:0494 | O2 Micro        | O2 Flash Memory Card     | 100%   |          | F0B7BBB9AE |
| 1217:8331 | 1028:049a | O2 Micro        | O2 Flash Memory Card     | 100%   |          | 3597218890 |
| 1217:8331 | 1028:049b | O2 Micro        | O2 Flash Memory Card     | 100%   |          | FCE7DD38A2 |
| 1217:8331 | 1bcf:a013 | O2 Micro        | O2 Flash Memory Card     | 100%   |          | 5C63F6A905 |
| 1261:3001 | 1261:3001 | Matsushita-K... | Storage controller       | 100%   |          | BC1A12A76F |
| 1aed:2001 | 1590:006d | SanDisk         | ioDrive2                 | 100%   |          | 4A5147AC07 |
| 1aed:3002 | 1014:04d3 | SanDisk         | ioMemory HHHL            | 100%   |          | FB0D0A1860 |
| ace1:0005 | ace1:0005 |                 | Storage controller       | 100%   |          | 22F215C605 |
| ace1:0006 | ace1:0006 |                 | Storage controller       | 100%   |          | EF20304D33 |

### Storage/ata (PCI)

11 out of 5187 (0.21%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1022:43b6 | 1b21:1062 | AMD             | X399 Series Chipset S... | 1%     | 3.10.0   | F29791E5C7 |
| 1022:43c8 | 1b21:1062 | AMD             | 400 Series Chipset SA... | 0.1%   | 3.10.0   | 21D76CDE28 |
| 1022:7901 | 1043:87c0 | AMD             | FCH SATA Controller [... | 0.6%   | 4.15.0   | 21D76CDE28 |
| 1022:7901 | 1462:7b92 | AMD             | FCH SATA Controller [... | 50%    | 5.4.0    | F29791E5C7 |
| 11ab:6141 | 1043:81d6 | Marvell Tech... | 88SE614x SATA II PCI-... | 100%   |          | 9EA64D6592 |
| 1b4b:9130 | 1043:8438 | Marvell Tech... | 88SE9128 PCIe SATA 6 ... | 0.9%   | 3.14.22  | 513772FEBC |
| 8086:02d3 | 17aa:3802 | Intel           | Comet Lake SATA AHCI ... | 4%     | 5.3.0    | 78ECA17C40 |
| 8086:2929 | 103c:306b | Intel           | 82801IBM/IEM (ICH9M/I... | 12.5%  | 3.14.44  | 93C0EF7223 |
| 8086:a103 | 103c:83bb | Intel           | HM170/QM170 Chipset S... | 11.1%  | 5.0.0    | 20EA46B0CE |
| 8086:a353 | 1028:087c | Intel           | Cannon Lake Mobile PC... | 1.6%   | 4.15.0   | C917477768 |
| 8086:a353 | 1028:0905 | Intel           | Cannon Lake Mobile PC... | 3.8%   | 4.15.0   | 293A792A22 |

### Storage/ide (PCI)

18 out of 3858 (0.47%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1002:439c | 1043:82ef | AMD             | SB7x0/SB8x0/SB9x0 IDE... | 0.8%   | 3.14.15  | 32AD3B2344 |
| 1002:439c | 1458:5002 | AMD             | SB7x0/SB8x0/SB9x0 IDE... | 0.2%   | 3.10.0   | 9FF481D661 |
| 1022:780c | 1458:5002 | AMD             | FCH IDE Controller       | 0.7%   | 3.14.25  | 1013DC1D5F |
| 1022:780c | 1458:b002 | AMD             | FCH IDE Controller       | 12.5%  | 4.1.38   | FA543553EC |
| 10de:0053 | 1043:815a | Nvidia          | CK804 IDE                | 3.4%   | 3.10.19  | A6659EE127 |
| 10de:056c | 1631:e038 | Nvidia          | MCP73 IDE Controller     | 25%    | 4.15.0   | 8CBA2E7FA8 |
| 11ab:6101 | 11ab:6101 | Marvell Tech... | 88SE6101/6102 single-... | 0.6%   | 3.14.22  | CCA71067AA |
| 1283:8213 | 1458:b000 | Integrated T... | IT8213 IDE Controller    | 1.6%   | 3.10.42  | 13ACEC4985 |
| 197b:2363 | 1458:b000 | JMicron Tech... | JMB363 SATA/IDE Contr... | 0.2%   | 3.10.0   | C1CD5017A5 |
| 197b:2368 | 1462:7636 | JMicron Tech... | JMB368 IDE controller    | 14.3%  | 4.1.19   | 48D4121155 |
| 1b21:0611 | 1b21:1060 | ASMedia Tech... | ASM1061 SATA IDE Cont... | 9.1%   | 3.14.25  | 98BA9E428E |
| 8086:1d3c | 1028:05d4 | Intel           | C600/X79 series chips... | 50%    | 5.4.0    | 19FB02CA4E |
| 8086:27df | 17aa:200c | Intel           | 82801G (ICH7 Family) ... | 3%     | 3.14.44  | E5C5CE1445 |
| 8086:29b6 | 17aa:3038 | Intel           | 82Q35 Express PT IDER... | 6.7%   | 4.1.15   | BDBE169E81 |
| 8086:2a06 | 17aa:20d3 | Intel           | Mobile PM965/GM965 PT... | 19.2%  | 3.14.53  | B0F13713A3 |
| 8086:2a46 | 10cf:1466 | Intel           | Mobile 4 Series Chips... | 100%   |          | CD2222973B |
| 8086:2e16 | 17aa:3048 | Intel           | 4 Series Chipset PT I... | 9.3%   | 4.1.15   | 18277A92CE |
| 8086:2e16 | 17aa:3049 | Intel           | 4 Series Chipset PT I... | 20%    | 4.4.0    | 1B004D7746 |

### Storage/nvme (PCI)

5 out of 102 (4.90%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 106b:2005 | 106b:1800 | Apple           | ANS2 NVMe Controller     | 29%    | 5.4.0    | 935B673683 |
| 10ec:5760 | 5760:10ec | Realtek Semi... | Realtek Non-Volatile ... | 6.2%   | 4.12.14  | 53EA23119E |
| 10ec:5762 | 10ec:5762 | Realtek Semi... | RTS5763DL NVMe SSD Co... | 1.6%   | 4.15.0   | E46B59C4D2 |
| 1987:5012 | 1987:5012 | Phison Elect... | E12 NVMe Controller      | 0.6%   | 4.9.0    | EA6F3DC938 |
| 8086:f1a6 | 8086:390b | Intel           | SSD Pro 7600p/760p/E ... | 0.8%   | 3.10.0   | 1E7ADBE67A |

### Storage/raid (PCI)

18 out of 864 (2.08%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1000:0010 | 0e11:4040 | Broadcom / LSI  | 53C1510                  | 100%   |          | 0B5D843F10 |
| 1000:0073 | 1000:9240 | Broadcom / LSI  | MegaRAID SAS 2008 [Fa... | 20%    | 5.3.0    | 38E4B2547A |
| 1000:0411 | 8086:1003 | Broadcom / LSI  | MegaRAID SAS 1068        | 100%   |          | 0E19261B88 |
| 1022:43bd | 1b21:1062 | AMD             | FCH RAID Controller      | 76.5%  | 5.3.0    | 31BF3FAE67 |
| 1028:0016 | 1028:1f24 | Dell            | PowerEdge Expandable ... | 100%   |          | 389DD308F7 |
| 103c:193f | 103c:3381 | Hewlett-Packard | Dynamic Smart Array B... | 100%   |          | 4825C12F7D |
| 1095:1114 | 1095:5114 | Silicon Image   | RAID bus controller      | 100%   |          | 126A2B0E4F |
| 1103:0611 | 1103:0611 | HighPoint Te... | RAID bus controller      | 100%   |          | E8AECFE123 |
| 1103:0622 | 1103:0001 | HighPoint Te... | RocketRAID 622 2 Port... | 100%   |          | 64A313C9E3 |
| 1103:0622 | 1103:0100 | HighPoint Te... | RocketRAID 622 2 Port... | 100%   |          | 24D6E7E1CE |
| 1103:0640 | 1103:0001 | HighPoint Te... | RocketRAID 640 4 Port... | 100%   |          | C1648A7961 |
| 1103:2840 | 1103:0000 | HighPoint Te... | RAID bus controller      | 100%   |          | 7653740066 |
| 1103:7103 | 1103:0001 | HighPoint Te... | RAID bus controller      | 100%   |          | DF1A8A847C |
| 1103:7110 | 1103:0000 | HighPoint Te... | RAID bus controller      | 100%   |          | EA6F3DC938 |
| 117c:002c | 117c:002c | ATTO Technology | ExpressSAS R380          | 100%   |          | F233ABA040 |
| 1590:0045 | 1590:0045 | Hewlett-Packard | RAID bus controller      | 100%   |          | 3FAC52AF81 |
| 6883:0dd4 | 6883:0dd4 |                 | RAID bus controller      | 100%   |          | 7211932892 |
| 8086:02d7 | 1043:1c51 | Intel           | Comet Lake PCH-LP SAT... | 100%   |          | C5079022A9 |

### System peripheral (PCI)

144 out of 776 (18.56%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 0014:7a0b |           | Loongson Tec... | SPI Controller           | 100%   |          | DD319B8387 |
| 0e11:a0f0 | 0e11:b0f3 | Compaq Computer | Advanced System Manag... | 100%   |          | 0B5D843F10 |
| 0e11:b203 | 103c:3305 | Compaq Computer | Integrated Lights Out... | 91.7%  | 4.9.60   | 2AF0FAD914 |
| 103c:3306 | 103c:3309 | Hewlett-Packard | Integrated Lights-Out... | 81.2%  | 2.6.32   | 2A20A0C0BA |
| 103c:3306 | 103c:330e | Hewlett-Packard | Integrated Lights-Out... | 100%   |          | 0EEE02F427 |
| 103c:3306 | 103c:3381 | Hewlett-Packard | Integrated Lights-Out... | 60.3%  | 2.6.32   | AFD4A44315 |
| 104c:8201 | 103c:006d | Texas Instru... | PCI1620 Firmware Load... | 100%   |          | 10266A11DF |
| 104c:8201 | 103c:08b0 | Texas Instru... | PCI1620 Firmware Load... | 100%   |          | 316E375A5C |
| 104c:8204 | 1028:0139 | Texas Instru... | PCI7410/7510/7610 PCI... | 100%   |          | 1629FF31A1 |
| 104c:8204 | 1028:014e | Texas Instru... | PCI7410/7510/7610 PCI... | 100%   |          | 0493B906A1 |
| 10b5:2065 | 10b5:9030 | PLX Technology  | System peripheral        | 100%   |          | BF5B58520E |
| 10b5:8609 | 10b5:8609 | PLX Technology  | PEX 8609 8-lane, 8-Po... | 50%    | 5.3.0    | E8AECFE123 |
| 1179:0805 | 1179:0001 | Toshiba Amer... | SD TypA Controller       | 40%    | 4.1.34   | 6ED70A9B46 |
| 1180:0576 | 10cf:1256 | Ricoh           | R5C576 SD Bus Host Ad... | 100%   |          | 4DCFB332DF |
| 1180:0576 | ffff:ffff | Ricoh           | R5C576 SD Bus Host Ad... | 100%   |          | 116C24A4D7 |
| 1180:0592 | 17aa:20ca | Ricoh           | R5C592 Memory Stick B... | 1.2%   | 3.14.25  | 81A4DA9481 |
| 1180:0852 | 1028:029f | Ricoh           | xD-Picture Card Contr... | 20%    | 4.1.15   | 44C743E996 |
| 1180:0852 | 1043:1877 | Ricoh           | xD-Picture Card Contr... | 3.2%   | 3.0.28   | 70CC866946 |
| 1180:0852 | 1734:10ad | Ricoh           | xD-Picture Card Contr... | 10%    | 4.1.33   | D6BC4ADE36 |
| 1180:0852 | 17aa:20cb | Ricoh           | xD-Picture Card Contr... | 3.7%   | 3.14.25  | 8D383C8BA6 |
| 1180:e230 | 1028:02bd | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | B28C0565FF |
| 1180:e230 | 1028:02fe | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 23814BCC77 |
| 1180:e230 | 1028:0401 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | B524E2847B |
| 1180:e230 | 1028:0402 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | DDD1946BD2 |
| 1180:e230 | 1028:0413 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 45F9C0B075 |
| 1180:e230 | 1028:0442 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | F5AB56B086 |
| 1180:e230 | 103c:1455 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 786DF34E10 |
| 1180:e230 | 103c:146d | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 68F6F32B71 |
| 1180:e230 | 103c:1471 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | BE0095E38A |
| 1180:e230 | 103c:1722 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 638A36ACC8 |
| 1180:e230 | 103c:1726 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 759D141031 |
| 1180:e230 | 103c:307e | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 7AB10A9CE6 |
| 1180:e230 | 1043:1b97 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 5977217568 |
| 1180:e230 | 1043:1f47 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 16105C86DB |
| 1180:e230 | 104d:905a | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | AE45786FEC |
| 1180:e230 | 104d:905e | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 353068F323 |
| 1180:e230 | 104d:9060 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 90A75A8826 |
| 1180:e230 | 104d:9066 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 1DE544887B |
| 1180:e230 | 104d:9067 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 55652DADF6 |
| 1180:e230 | 104d:9069 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | E297B43775 |
| 1180:e230 | 104d:9071 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | E99C8BC910 |
| 1180:e230 | 104d:9072 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 2E9D3ED45B |
| 1180:e230 | 104d:9074 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | E9B4918D6C |
| 1180:e230 | 104d:907a | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 7BA88076ED |
| 1180:e230 | 1179:0001 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 4128B3CD2D |
| 1180:e230 | 1179:ff1e | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | F7F3C03AD9 |
| 1180:e230 | 1179:ff40 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | CBB92D0BB3 |
| 1180:e230 | 1179:ffc0 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 96D989965C |
| 1180:e230 | 17aa:2134 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 229E816FB4 |
| 1180:e232 | 104d:907e | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 02FDC03CEB |
| 1180:e232 | 104d:9081 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | DAEDAF5374 |
| 1180:e232 | 104d:9083 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 2B4EF9468E |
| 1180:e232 | 104d:9086 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | C1F9CF2BE3 |
| 1180:e232 | 104d:9089 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 2E0915F8A9 |
| 1180:e232 | 104d:908e | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 59BB8EC907 |
| 1180:e232 | 104d:9095 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 9106956197 |
| 1180:e232 | 104d:9097 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 7685534B8E |
| 1180:e232 | 1179:0001 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 54A1281AE2 |
| 1180:e822 | 17aa:21fb | Ricoh           | MMC/SD Host Controller   | 20%    | 4.9.20   | 657F2A7F37 |
| 1180:e823 | 17aa:21fb | Ricoh           | PCIe SDXC/MMC Host Co... | 5.9%   | 4.15.0   | 55427995B5 |
| 1217:7110 | 10cf:11c4 | O2 Micro        | OZ711Mx 4-in-1 Memory... | 100%   |          | EA732BEA27 |
| 1217:7110 | 1734:106c | O2 Micro        | OZ711Mx 4-in-1 Memory... | 100%   |          | B66AF54651 |
| 14e4:16be | 1025:0500 | Broadcom        | BCM57765/57785 MS Car... | 100%   |          | 0275565E2B |
| 14e4:16be | 1025:0504 | Broadcom        | BCM57765/57785 MS Car... | 100%   |          | F70E4485BC |
| 14e4:16be | 1025:0599 | Broadcom Lim... | BCM57765/57785 MS Car... | 100%   |          | 7015489AD7 |
| 14e4:16be | 1025:0605 | Broadcom Lim... | BCM57765/57785 MS Car... | 100%   |          | 543A3B5FEF |
| 14e4:16be | 1025:0647 | Broadcom        | BCM57765/57785 MS Car... | 100%   |          | 61D106EA18 |
| 14e4:16bf | 1025:0500 | Broadcom        | BCM57765/57785 xD-Pic... | 100%   |          | 0275565E2B |
| 14e4:16bf | 1025:0504 | Broadcom        | BCM57765/57785 xD-Pic... | 100%   |          | F70E4485BC |
| 14e4:16bf | 1025:0599 | Broadcom Lim... | BCM57765/57785 xD-Pic... | 100%   |          | 7015489AD7 |
| 14e4:16bf | 1025:0605 | Broadcom Lim... | BCM57765/57785 xD-Pic... | 100%   |          | 543A3B5FEF |
| 14e4:16bf | 1025:0647 | Broadcom        | BCM57765/57785 xD-Pic... | 100%   |          | 61D106EA18 |
| 197b:2382 | 1297:2020 | JMicron Tech... | SD/MMC Host Controller   | 7.1%   | 4.15.0   | D826611187 |
| 197b:2384 | 1019:2238 | JMicron Tech... | xD Host Controller       | 100%   |          | 7E782321C8 |
| 197b:2384 | 1025:0128 | JMicron Tech... | xD Host Controller       | 100%   |          | EA94093CD5 |
| 197b:2384 | 1025:013b | JMicron Tech... | xD Host Controller       | 100%   |          | 0C78055950 |
| 197b:2384 | 1025:013d | JMicron Tech... | xD Host Controller       | 100%   |          | F922502A91 |
| 197b:2384 | 1025:013e | JMicron Tech... | xD Host Controller       | 100%   |          | B563FF6430 |
| 197b:2384 | 1025:0140 | JMicron Tech... | xD Host Controller       | 100%   |          | 0CD3F983C9 |
| 197b:2384 | 1025:0142 | JMicron Tech... | xD Host Controller       | 100%   |          | F00CF2C184 |
| 197b:2384 | 1025:0143 | JMicron Tech... | xD Host Controller       | 100%   |          | 310A169187 |
| 197b:2384 | 1025:0145 | JMicron Tech... | xD Host Controller       | 100%   |          | 3C60271275 |
| 197b:2384 | 1025:0146 | JMicron Tech... | xD Host Controller       | 100%   |          | 649CB24583 |
| 197b:2384 | 1025:014b | JMicron Tech... | xD Host Controller       | 100%   |          | EBB35F1079 |
| 197b:2384 | 1025:015b | JMicron Tech... | xD Host Controller       | 100%   |          | D77EF53611 |
| 197b:2384 | 1025:0160 | JMicron Tech... | xD Host Controller       | 100%   |          | BBCDDB4D27 |
| 197b:2384 | 1025:0200 | JMicron Tech... | xD Host Controller       | 100%   |          | 454098B840 |
| 197b:2384 | 1025:0259 | JMicron Tech... | xD Host Controller       | 100%   |          | 432C7B7B63 |
| 197b:2384 | 1025:0260 | JMicron Tech... | xD Host Controller       | 100%   |          | AFEFC6A739 |
| 197b:2384 | 1025:0311 | JMicron Tech... | xD Host Controller       | 100%   |          | 57FFADB7C2 |
| 197b:2384 | 1025:042f | JMicron Tech... | xD Host Controller       | 100%   |          | 1395FA2E0F |
| 197b:2384 | 103c:1489 | JMicron Tech... | xD Host Controller       | 100%   |          | A6305AD3A0 |
| 197b:2384 | 103c:2aa2 | JMicron Tech... | xD Host Controller       | 100%   |          | 24C07D9D0D |
| 197b:2384 | 103c:2aa6 | JMicron Tech... | xD Host Controller       | 100%   |          | 45542209AF |
| 197b:2384 | 103c:30f4 | JMicron Tech... | xD Host Controller       | 100%   |          | 029DDA08DF |
| 197b:2384 | 103c:30f7 | JMicron Tech... | xD Host Controller       | 100%   |          | 75277DFAA2 |
| 197b:2384 | 103c:30fb | JMicron Tech... | xD Host Controller       | 100%   |          | 017DE403F3 |
| 197b:2384 | 103c:30fc | JMicron Tech... | xD Host Controller       | 100%   |          | AA72037904 |
| 197b:2384 | 103c:30fe | JMicron Tech... | xD Host Controller       | 100%   |          | A8C476CD53 |
| 197b:2384 | 103c:3600 | JMicron Tech... | xD Host Controller       | 100%   |          | 41390482F3 |
| 197b:2384 | 103c:3603 | JMicron Tech... | xD Host Controller       | 100%   |          | 5DE992A496 |
| 197b:2384 | 103c:3610 | JMicron Tech... | xD Host Controller       | 100%   |          | A4A71A5F55 |
| 197b:2384 | 103c:361b | JMicron Tech... | xD Host Controller       | 100%   |          | 63C2E0460D |
| 197b:2384 | 103c:3624 | JMicron Tech... | xD Host Controller       | 100%   |          | 81B53C7180 |
| 197b:2384 | 103c:3628 | JMicron Tech... | xD Host Controller       | 100%   |          | 4833031B9B |
| 197b:2384 | 103c:3629 | JMicron Tech... | xD Host Controller       | 100%   |          | F1CC639EDF |
| 197b:2384 | 103c:3636 | JMicron Tech... | xD Host Controller       | 100%   |          | FF31E18FB9 |
| 197b:2384 | 103c:363c | JMicron Tech... | xD Host Controller       | 100%   |          | D9418273DF |
| 197b:2384 | 103c:363e | JMicron Tech... | xD Host Controller       | 100%   |          | A9E05596D5 |
| 197b:2384 | 103c:3659 | JMicron Tech... | xD Host Controller       | 100%   |          | 74FC66B923 |
| 197b:2384 | 103c:365c | JMicron Tech... | xD Host Controller       | 100%   |          | 45F200C40A |
| 197b:2384 | 103c:7001 | JMicron Tech... | xD Host Controller       | 100%   |          | 298015ECAC |
| 197b:2384 | 103c:7010 | JMicron Tech... | xD Host Controller       | 100%   |          | 6E70B36184 |
| 197b:2384 | 1043:1a07 | JMicron Tech... | xD Host Controller       | 100%   |          | E409C4193A |
| 197b:2384 | 1071:9525 | JMicron Tech... | xD Host Controller       | 100%   |          | 4B29F60F4E |
| 197b:2384 | 1179:fd30 | JMicron Tech... | xD Host Controller       | 100%   |          | 07BD67039C |
| 197b:2384 | 1179:fdb0 | JMicron Tech... | xD Host Controller       | 100%   |          | 3BF39D603E |
| 197b:2384 | 1179:ff02 | JMicron Tech... | xD Host Controller       | 100%   |          | 9D940F2CB6 |
| 197b:2384 | 1179:ff08 | JMicron Tech... | xD Host Controller       | 100%   |          | CFEF2899A5 |
| 197b:2384 | 1462:100f | JMicron Tech... | xD Host Controller       | 100%   |          | 9FEC6C5DE7 |
| 197b:2384 | 1462:6520 | JMicron Tech... | xD Host Controller       | 100%   |          | 12132D4EBD |
| 197b:2384 | 14c0:0031 | JMicron Tech... | xD Host Controller       | 100%   |          | 56B05900A0 |
| 197b:2384 | 152d:0834 | JMicron Tech... | xD Host Controller       | 100%   |          | C6D0242C42 |
| 197b:2384 | 1558:0803 | JMicron Tech... | xD Host Controller       | 100%   |          | 72186D36EB |
| 197b:2384 | 1558:0806 | JMicron Tech... | xD Host Controller       | 100%   |          | F3BF4D62C0 |
| 197b:2384 | 1734:113d | JMicron Tech... | xD Host Controller       | 100%   |          | BD5D293529 |
| 197b:2384 | 1734:113f | JMicron Tech... | xD Host Controller       | 100%   |          | C948F4D81B |
| 197b:2384 | 17aa:2130 | JMicron Tech... | xD Host Controller       | 100%   |          | BFDA7D01D5 |
| 197b:2384 | 17aa:3602 | JMicron Tech... | xD Host Controller       | 100%   |          | 55C2F8E26B |
| 197b:2384 | 17aa:3881 | JMicron Tech... | xD Host Controller       | 100%   |          | 7F669E0390 |
| 197b:2384 | 17c0:10da | JMicron Tech... | xD Host Controller       | 100%   |          | 74D6F0A5E2 |
| 197b:2387 | 17aa:3921 | JMicron Tech... | SD/MMC Host Controller   | 100%   |          | D2519403DD |
| 197b:2389 | 17aa:3924 | JMicron Tech... | xD Host Controller       | 100%   |          | D2519403DD |
| 197b:2394 | 1025:050a | JMicron Tech... | xD Host Controller       | 100%   |          | 63D11EBB5A |
| 197b:2394 | 1028:0446 | JMicron Tech... | xD Host Controller       | 100%   |          | 6B02B77843 |
| 197b:2394 | 1028:0468 | JMicron Tech... | xD Host Controller       | 100%   |          | F8F65007E0 |
| 197b:2394 | 103c:2ac6 | JMicron Tech... | xD Host Controller       | 100%   |          | 90725B3C8A |
| 197b:2394 | 103c:2ae5 | JMicron Tech... | xD Host Controller       | 100%   |          | DE0EC859C8 |
| 197b:2394 | 1179:fc30 | JMicron Tech... | xD Host Controller       | 100%   |          | A04002572A |
| 197b:2394 | 1462:107f | JMicron Tech... | xD Host Controller       | 100%   |          | 4D22D14A1D |
| 197b:2394 | 14c0:006b | JMicron Tech... | xD Host Controller       | 100%   |          | C97368216B |
| 197b:2394 | 17aa:3976 | JMicron Tech... | xD Host Controller       | 100%   |          | BA61D3B772 |
| 197b:2394 | 17aa:3977 | JMicron Tech... | xD Host Controller       | 100%   |          | 2D28ED1624 |
| 197b:2394 | ffff:ffff | JMicron Tech... | xD Host Controller       | 100%   |          | 6F346C88EC |

### Tv card (PCI)

8 out of 308 (2.60%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1131:7130 | 5ace:5050 | Philips Semi... | SAA7130 Video Broadca... | 3.1%   | 3.14.44  | D82F0A25EA |
| 1131:7133 | 16be:0007 | Philips Semi... | SAA7131/SAA7133/SAA71... | 100%   |          | 24A0914BA3 |
| 1131:7133 | 16be:0008 | Philips Semi... | SAA7131/SAA7133/SAA71... | 100%   |          | 24A0914BA3 |
| 11de:6057 | 1031:7efe | Zoran           | ZR36057PQC Video cutt... | 11.8%  | 3.14.44  | 9C4096F26A |
| 11de:6057 | 1031:d801 | Zoran           | ZR36057PQC Video cutt... | 100%   |          | F700FF20C6 |
| 14f1:8800 | 8922:8888 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 71.4%  | 4.1.25   | BDE6F8112F |
| 14f1:8802 | 8922:8888 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 71.4%  | 4.1.25   | BDE6F8112F |
| 4444:0016 | 0070:8801 | Internext Co... | iTVC16 (CX23416) Vide... | 5.9%   | 4.1.15   | 8854FD6644 |

### Usb controller (PCI)

80 out of 18900 (0.42%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1002:4396 | 1002:4396 | AMD             | SB7x0/SB8x0/SB9x0 USB... | 0.1%   | 3.10.0   | 012357C526 |
| 1002:4397 | 1002:4397 | AMD             | SB7x0/SB8x0/SB9x0 USB... | 0.1%   | 3.10.0   | 012357C526 |
| 1002:4397 | 1458:5004 | AMD             | SB7x0/SB8x0/SB9x0 USB... | 0.1%   | 3.10.0   | 0533339E4E |
| 1002:4399 | 1002:4399 | AMD             | SB7x0/SB8x0/SB9x0 USB... | 0.1%   | 3.10.0   | 012357C526 |
| 1002:4399 | 1458:5004 | AMD             | SB7x0/SB8x0/SB9x0 USB... | 0.1%   | 3.10.0   | 0533339E4E |
| 1022:7807 | 103c:216f | AMD             | FCH USB OHCI Controller  | 14.3%  | 4.9.20   | E190391A64 |
| 1022:7807 | 1458:5004 | AMD             | FCH USB OHCI Controller  | 0.2%   | 3.14.25  | FA543553EC |
| 1022:7808 | 103c:216f | AMD             | FCH USB EHCI Controller  | 14.3%  | 4.9.20   | E190391A64 |
| 1022:7809 | 1458:5004 | AMD             | FCH USB OHCI Controller  | 0.2%   | 3.14.25  | FA543553EC |
| 1022:7814 | 103c:216f | AMD             | FCH USB XHCI Controller  | 14.3%  | 4.9.20   | E190391A64 |
| 1033:00e0 | 1799:0002 | NEC Computers   | uPD72010x USB 2.0 Con... | 11.1%  | 4.15.0   | A715A916F9 |
| 1033:0194 | ffff:ffff | NEC Computers   | uPD720200 USB 3.0 Hos... | 1.6%   | 3.14.25  | C4006430A8 |
| 104c:8241 | 103c:17e2 | Texas Instru... | TUSB73x0 SuperSpeed U... | 20%    | 4.15.0   | B62CA0352C |
| 104c:8241 | 103c:2ada | Texas Instru... | TUSB73x0 SuperSpeed U... | 12.5%  | 4.15.0   | 3BB5A2AB3E |
| 106b:003f |           | Apple           | KeyLargo/Intrepid USB    | 100%   |          | 7740C04B4B |
| 10de:005a | 1043:815a | Nvidia          | CK804 USB Controller     | 3.4%   | 3.10.19  | A6659EE127 |
| 10de:005b | 1043:815a | Nvidia          | CK804 USB Controller     | 3.4%   | 3.10.19  | A6659EE127 |
| 1106:3038 | 1106:3038 | VIA Technolo... | VT82xx/62xx/VX700/8x0... | 0.2%   | 4.1.38   | 705CB8BD10 |
| 1106:3104 | 1106:3104 | VIA Technolo... | USB 2.0 EHCI-Complian... | 1.7%   | 4.1.38   | C9A1706533 |
| 1106:3104 | 1106:318a | VIA Technolo... | USB 2.0 EHCI-Complian... | 12.5%  | 4.1.25   | E56DD30CA2 |
| 1106:3432 | 1458:5007 | VIA Technolo... | VL800/801 xHCI USB 3.... | 2.4%   | 4.1.15   | 30536633CF |
| 1106:3483 | 1106:3483 | VIA Technolo... | VL805/806 xHCI USB 3.... | 0.9%   | 3.14.44  | 275AA1BAFE |
| 1106:3483 | 1458:5007 | VIA Technolo... | VL805/806 xHCI USB 3.... | 13%    | 3.10.0   | 7D3AB72CF8 |
| 1912:0014 | 103c:1996 | Renesas Tech... | uPD720201 USB 3.0 Hos... | 3.7%   | 4.4.4    | 7CF6D970EC |
| 1912:0014 | 1912:0014 | Renesas Tech... | uPD720201 USB 3.0 Hos... | 2.2%   | 4.1.15   | E3CF1A821F |
| 1912:0014 | ffff:ffff | Renesas Tech... | uPD720201 USB 3.0 Hos... | 0.4%   | 3.14.44  | 0C3CB9E44D |
| 1912:0015 |           | Renesas Tech... | uPD720202 USB 3.0 Hos... | 3.3%   | 3.14.25  | 740FC92339 |
| 1912:0015 | ffff:ffff | Renesas Tech... | uPD720202 USB 3.0 Hos... | 0.9%   | 3.14.44  | B621BEAB40 |
| 1b21:1042 | 1043:1059 | ASMedia Tech... | ASM1042 SuperSpeed US... | 0.2%   | 3.10.34  | 6C9107BCAD |
| 1b21:1042 | 1043:8488 | ASMedia Tech... | ASM1042 SuperSpeed US... | 0.1%   | 3.10.34  | CDF1DFEF46 |
| 1b21:1042 | 1462:7693 | ASMedia Tech... | ASM1042 SuperSpeed US... | 4.4%   | 3.14.15  | FC5F1E6327 |
| 1b21:1042 | 1849:1042 | ASMedia Tech... | ASM1042 SuperSpeed US... | 2.1%   | 3.10.0   | 101E707D3C |
| 1b6f:7023 | 1458:5007 | Etron Techno... | EJ168 USB 3.0 Host Co... | 0.1%   | 3.10.0   | 746ED0F095 |
| 1b73:1000 | 1043:1039 | Fresco Logic    | FL1000G USB 3.0 Host ... | 0.7%   | 3.0.28   | 0EAEBD5FCA |
| 8086:0f34 | 17aa:3986 | Intel           | Atom Processor Z36xxx... | 12.5%  | 3.14.44  | EC4481EC60 |
| 8086:0f37 | 8086:0f37 | Intel           | Atom Processor Z36xxx... | 3.6%   | 3.14.44  | 4668851708 |
| 8086:0f37 | 8086:7270 | Intel           | Atom Processor Z36xxx... | 8.3%   | 4.1.16   | C3623326F4 |
| 8086:1d26 | 8086:3582 | Intel           | C600/X79 series chips... | 100%   |          | 9F6D925B73 |
| 8086:1d2d | 8086:3582 | Intel           | C600/X79 series chips... | 100%   |          | 9F6D925B73 |
| 8086:1e26 | 1043:201f | Intel           | 7 Series/C216 Chipset... | 1.1%   | 3.10.34  | 3C52D09634 |
| 8086:1e26 | 1043:84ca | Intel           | 7 Series/C216 Chipset... | 0.1%   | 3.10.34  | 44E0CE8FC8 |
| 8086:1e2d | 1043:201f | Intel           | 7 Series/C216 Chipset... | 1.1%   | 3.10.34  | 3C52D09634 |
| 8086:1e2d | 1043:84ca | Intel           | 7 Series/C216 Chipset... | 0.1%   | 3.10.34  | 44E0CE8FC8 |
| 8086:1e31 | 1028:0533 | Intel           | 7 Series/C210 Series ... | 5.3%   | 4.9.20   | 8255A6BF31 |
| 8086:1e31 | 1028:0534 | Intel           | 7 Series/C210 Series ... | 4%     | 4.1.19   | 4FBBA78CD4 |
| 8086:1e31 | 103c:1970 | Intel           | 7 Series/C210 Series ... | 5.3%   | 3.14.44  | E2F0FC675A |
| 8086:1e31 | 1043:1447 | Intel           | 7 Series/C210 Series ... | 6.7%   | 3.14.44  | F23B5BF0DA |
| 8086:1e31 | 1043:84ca | Intel           | 7 Series/C210 Series ... | 0.1%   | 3.10.34  | 44E0CE8FC8 |
| 8086:1e31 | 104d:9095 | Intel           | 7 Series/C210 Series ... | 3.4%   | 3.14.25  | 2A2BD0A648 |
| 8086:1e31 | 1458:5007 | Intel           | 7 Series/C210 Series ... | 0.4%   | 3.10.0   | 837D994165 |
| 8086:1e31 | 17aa:21f3 | Intel           | 7 Series/C210 Series ... | 0.7%   | 3.14.44  | 3085B68179 |
| 8086:1e31 | 17aa:21fa | Intel           | 7 Series/C210 Series ... | 0.6%   | 3.10.42  | 689257C05A |
| 8086:22b7 | 17aa:380a | Intel           | USB Synopsys Controller  | 45.5%  | 5.3.11   | DE0F29B8A1 |
| 8086:22b7 | 8086:7270 | Intel           | USB Synopsys Controller  | 7.6%   | 4.9.9    | 4AC6DD88AA |
| 8086:2934 | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 12.5%  | 3.14.44  | 93C0EF7223 |
| 8086:2935 | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 12.5%  | 3.14.44  | 93C0EF7223 |
| 8086:2936 | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 12.5%  | 3.14.44  | 93C0EF7223 |
| 8086:2937 | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 12.5%  | 3.14.44  | 93C0EF7223 |
| 8086:2938 | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 12.5%  | 3.14.44  | 93C0EF7223 |
| 8086:2939 | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 12.5%  | 3.14.44  | 93C0EF7223 |
| 8086:293a | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 12.5%  | 3.14.44  | 93C0EF7223 |
| 8086:293c | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 12.5%  | 3.14.44  | 93C0EF7223 |
| 8086:3b36 | 8086:7270 | Intel           | 5 Series/3400 Series ... | 78%    | 3.14.44  | 7E0933DF40 |
| 8086:3b3b | 8086:7270 | Intel           | 5 Series/3400 Series ... | 78%    | 3.14.44  | 7E0933DF40 |
| 8086:5aaa | 8086:7270 | Intel           | USB Controller           | 55.6%  | 4.10.0   | 6166C5D0EE |
| 8086:8c26 | 103c:1909 | Intel           | 8 Series/C220 Series ... | 5.3%   | 4.9.0    | 196DFE92A3 |
| 8086:8c2d | 103c:1909 | Intel           | 8 Series/C220 Series ... | 5.3%   | 4.9.0    | 196DFE92A3 |
| 8086:8c31 | 8086:204a | Intel           | 8 Series/C220 Series ... | 7.1%   | 4.1.25   | 8C48173C7B |
| 8086:8d26 | 1043:8600 | Intel           | C610/X99 series chips... | 3.8%   | 3.10.0   | 89ABF0DB25 |
| 8086:8d2d | 1043:8600 | Intel           | C610/X99 series chips... | 3.8%   | 3.10.0   | 89ABF0DB25 |
| 8086:9c26 | 1025:0a11 | Intel           | 8 Series USB EHCI #1     | 33.3%  | 4.9.60   | C858E37129 |
| 8086:9c31 | 1028:05e0 | Intel           | 8 Series USB xHCI HC     | 3.3%   | 4.9.9    | 8EA71BA2AE |
| 8086:9ca6 | 1025:098a | Intel           | Wildcat Point-LP USB ... | 1%     | 3.14.44  | DE4737FCF1 |
| 8086:9ca6 | 1028:06be | Intel           | Wildcat Point-LP USB ... | 16.7%  | 4.15.0   | 1FBEE12FFE |
| 8086:9cb1 | 103c:806c | Intel           | Wildcat Point-LP USB ... | 100%   |          | 462F2D5347 |
| 8086:9d2f | 103c:807c | Intel           | Sunrise Point-LP USB ... | 4.8%   | 4.9.0    | 791A2EA6F5 |
| 8086:9d30 | 8086:7270 | Intel           | Skylake-U/Y USB Devic... | 100%   |          | D9F38D66C3 |
| 8086:9d30 | 8086:9d30 | Intel           | Skylake-U/Y USB Devic... | 20%    | 4.15.0   | 3E70A8DFF1 |
| 8086:a12f | 1734:121d | Intel           | 100 Series/C230 Serie... | 2.9%   | 3.16.0   | 19202ED9BC |
| 8086:a2af | 1043:872f | Intel           | 200 Series/Z370 Chips... | 2.2%   | 4.9.9    | 4027AAA720 |

USB Devices
-----------

Non-100% value in the 'Missed' column indicates that the driver for a device is available
in the latest kernel versions. You can find corresponding hwinfo reports for listed devices
by a probe ID.

Missed — percentage of probes with missed driver for the device,
Linux  — the minimum Linux kernel version in which the driver was found,
Probe  — latest probe ID with missed driver for the device.

### Audio (USB)

8 out of 125 (6.40%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 046d:0a0b | Logitech        | ClearChat Pro USB        | 14.3%  | 4.15.0   | 56D5984A14 |
| 046d:0a87 | Logitech        | G935 Gaming Headset      | 25%    | 5.0.0    | 58C9748044 |
| 04d2:ff05 | Altec Lansin... | ADA-305 Speakers         | 100%   |          | BBD2341205 |
| 0644:8030 | TEAC            | US-1800                  | 100%   |          | 75C7FE6B69 |
| 0763:201a | M-Audio         | M-Audio Micro            | 100%   |          | 4AFB8F7991 |
| 0955:7002 | Nvidia          | stereo controller        | 100%   |          | EFAB764BE0 |
| 1235:8016 | Focusrite-No... | Focusrite Scarlett 2i2   | 9.1%   | 4.9.20   | F16ADBF7F3 |
| b58e:0005 | Blue Microph... | Yeti Nano                | 9.1%   | 5.0.0    | A588768A6C |

### Bluetooth (USB)

51 out of 385 (13.25%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 03f0:171d | Hewlett-Packard | Bluetooth 2.0 Interfa... | 0.5%   | 3.2.0    | 13824A2872 |
| 044e:300c | Alps Electric   | Bluetooth Controller ... | 6.7%   | 4.1.15   | 7F0BB0CC92 |
| 0489:e031 | Foxconn / Ho... | BCM20702A0               | 6.2%   | 4.15.0   | 958D094890 |
| 0489:e036 | Foxconn / Ho... | Bluetooth USB Host Co... | 0.7%   | 3.0.28   | 69F933DD8C |
| 0489:e069 | Foxconn / Ho... | BT                       | 98.2%  | 4.9.41   | A24E3E59E4 |
| 0489:e080 | Foxconn / Ho... | BT                       | 100%   |          | DF4413AF58 |
| 04ca:2006 | Lite-On Tech... | Broadcom BCM43142A0 B... | 5.1%   | 4.0.8    | 805C7CD772 |
| 04ca:2007 | Lite-On Tech... | Broadcom BCM43142A0 B... | 8.6%   | 4.1.7    | BAA62D56E7 |
| 04ca:2009 | Lite-On Tech... | BCM43142A0               | 6.3%   | 4.0.2    | 14539CFCC1 |
| 04ca:300b | Lite-On Tech... | Atheros AR3012 Bluetooth | 0.6%   | 3.10.51  | F74452F6C3 |
| 04ca:300d | Lite-On Tech... | Atheros AR3012 Bluetooth | 6.1%   | 4.1.19   | D9F38D66C3 |
| 04ca:3014 | Lite-On Tech... | Qualcomm Atheros Blue... | 6%     | 4.1.25   | 401BBED185 |
| 05ac:8215 | Apple           | Built-in Bluetooth 2.... | 0.7%   | 3.14.44  | D5C9D589F2 |
| 05ac:8289 | Apple           | Bluetooth Host Contro... | 3.5%   | 4.1.15   | 109E02E0F2 |
| 05ac:8290 | Apple           | Bluetooth Host Contro... | 1.8%   | 4.9.9    | 91ED990D94 |
| 05e1:0100 | Syntek          | 802.11g + Bluetooth W... | 100%   |          | 67B7EC6A84 |
| 0930:0200 | Toshiba         | Integrated Bluetooth ... | 5%     | 4.1.16   | 3459EB4984 |
| 0930:0215 | Toshiba         | Bluetooth Device         | 9.1%   | 3.14.44  | 884E374E31 |
| 0930:0219 | Toshiba         | Bluetooth USB Host Co... | 1.7%   | 3.14.33  | 67009EFFAA |
| 0a12:0001 | Cambridge Si... | Bluetooth Dongle (HCI... | 0.1%   | 2.6.32   | B5737B7866 |
| 0a5c:216c | Broadcom        | BCM43142A0 Bluetooth ... | 1.2%   | 3.14.44  | 2F3CB20593 |
| 0a5c:21d7 | Broadcom        | BCM43142 Bluetooth 4.0   | 0.6%   | 3.14.33  | 854DAA05D0 |
| 0a5c:21e6 | Broadcom        | BCM20702 Bluetooth 4.... | 0.8%   | 3.14.15  | 867C47D444 |
| 0a5c:21e8 | Broadcom        | BCM20702A0 Bluetooth 4.0 | 0.3%   | 4.1.15   | E0CDE3F93B |
| 0bda:b001 | Realtek Semi... | Bluetooth Radio          | 0.5%   | 3.14.15  | 8DCBD3C2B1 |
| 0bda:b006 | Realtek Semi... | Bluetooth Radio          | 5%     | 4.1.15   | 9179EF8E4A |
| 0bda:b009 | Realtek Semi... | Realtek Bluetooth 4.2... | 0.1%   | 3.10.0   | 4F1105BCA0 |
| 0bda:b023 | Realtek Semi... | RTL8822BE Bluetooth 4... | 0.8%   | 4.15.0   | 80F496EACD |
| 0bda:b728 | Realtek Semi... | RTL8723B Bluetooth       | 0.5%   | 3.14.25  | 39A9917502 |
| 0cf3:3002 | Qualcomm Ath... | AR3011 Bluetooth         | 8.2%   | 3.14.44  | AD22DC7B9B |
| 0cf3:3004 | Qualcomm Ath... | AR3012 Bluetooth 4.0     | 0.5%   | 3.10.51  | 730C65E65D |
| 0cf3:3005 | Qualcomm Ath... | AR3011 Bluetooth         | 0.1%   | 3.10.0   | F4DE983D96 |
| 0cf3:3008 | Qualcomm Ath... | Bluetooth (AR3011)       | 1.7%   | 3.14.25  | F430167968 |
| 0cf3:e005 | Qualcomm Ath... | Qualcomm Atheros Blue... | 2.1%   | 3.13.0   | 689DFEA547 |
| 0e8d:763e | MediaTek        | MT7630e Bluetooth Ada... | 100%   |          | 28B795ED06 |
| 105b:e065 | Foxconn Inte... | BCM43142A0 Bluetooth ... | 10.7%  | 4.0.1    | F39685A972 |
| 1358:c123 | Realtek         | Bluetooth Radio          | 5.7%   | 4.15.0   | 763C1A213C |
| 13d3:3304 | IMC Networks    | Asus Integrated Bluet... | 2.6%   | 3.10.34  | 1787C065C7 |
| 13d3:3392 | IMC Networks    | Azurewave 43228+20702    | 50%    | 4.18.0   | 337156D639 |
| 13d3:3491 | IMC Networks    | Bluetooth Device         | 1.1%   | 4.4.0    | 94D2C67B3F |
| 413c:8143 | Dell            | Broadcom BCM20702A0 B... | 70.6%  | 4.15.0   | AE4C0F8B6B |
| 413c:8187 | Dell            | DW375 Bluetooth Module   | 0.4%   | 3.10.0   | F33530C32A |
| 413c:8197 | Dell            | BCM20702A0 Bluetooth ... | 1.5%   | 3.14.25  | 4E38982788 |
| 8087:0025 | Intel           | Wireless-AC 9260 Blue... | 0.2%   | 4.9.60   | 22662AAD4D |
| 8087:0026 | Intel           | Bluetooth Device         | 1%     | 3.10.0   | CA529580D5 |
| 8087:0029 | Intel           | AX200 Bluetooth          | 1.3%   | 3.10.0   | D7DFD2A0D2 |
| 8087:07da | Intel           | Centrino Bluetooth Wi... | 0.3%   | 4.4.0    | DC66CB5CAF |
| 8087:07dc | Intel           | Bluetooth wireless in... | 0.2%   | 3.10.0   | 8EA71BA2AE |
| 8087:0a2a | Intel           | Bluetooth wireless in... | 0.2%   | 3.10.0   | 12D0EDEC81 |
| 8087:0a2b | Intel           | Bluetooth wireless in... | 0.6%   | 3.10.0   | 84538E3769 |
| 8087:0aaa | Intel           | Bluetooth 9460/9560 J... | 0.6%   | 3.10.0   | 64802F828B |

### Camera (USB)

174 out of 2468 (7.05%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0402:5603 | ALi             | M5603 Video Camera Co... | 100%   |          | 775945A948 |
| 0402:9665 | ALi             | Gateway Webcam           | 0.4%   | 3.14.25  | 68F61986F8 |
| 0408:2fb1 | Quanta          | Laptop_Integrated_Web... | 1.5%   | 3.10.0   | A993CB7099 |
| 0408:5300 | Quanta          | HP Wide Vision HD Camera | 1.8%   | 4.15.0   | A42A77029D |
| 0408:a031 | Quanta          | VGA WebCam               | 0.5%   | 4.9.60   | F82BD4CF20 |
| 041e:400d | Creative Tec... | Webcam PD1001            | 100%   |          | 1892C5C88C |
| 041e:4039 | Creative Tec... | Webcam Live! Effects     | 100%   |          | D42D07BEBB |
| 0458:702a | KYE Systems ... | WebCAM USB2.0            | 100%   |          | 3D86369A82 |
| 045e:0779 | Microsoft       | LifeCam HD-3000          | 0.7%   | 3.14.33  | E0968088B3 |
| 045e:0a00 | Microsoft       | Lumia 950 Dual SIM (R... | 50%    | 5.0.0    | 490B159371 |
| 046d:081b | Logitech        | Webcam C310              | 0.4%   | 3.14.22  | 66219C1D36 |
| 046d:0825 | Logitech        | Webcam C270              | 0.2%   | 3.10.34  | 541846E7D7 |
| 046d:082c | Logitech        | HD Webcam C615           | 0.9%   | 3.14.44  | F61EE20F03 |
| 046d:085c | Logitech        | C922 Pro Stream Webcam   | 4.7%   | 4.9.0    | 781F2CDA04 |
| 046d:09a4 | Logitech        | QuickCam E 3500          | 3.6%   | 3.14.39  | 74709A1A7B |
| 04ca:7070 | Lite-On Tech... | Integrated Camera        | 1%     | 4.15.0   | D082B8D834 |
| 04ca:707f | Lite-On Tech... | HP Wide Vision HD Camera | 1.7%   | 4.4.0    | 06EE78EE4D |
| 04ca:7086 | Lite-On Tech... | HP Wide Vision FHD Ca... | 17.2%  | 4.15.0   | 04D98C9A75 |
| 04ca:709d | Lite-On Tech... | HP Wide Vision HD Camera | 9.1%   | 4.15.0   | ACFBF614C0 |
| 04f2:b163 | Chicony Elec... | HP Webcam [2 MP Macro]   | 3.2%   | 4.1.22   | 5DD7A5FCE1 |
| 04f2:b240 | Chicony Elec... | FJ Camera                | 6.7%   | 4.15.0   | 958D094890 |
| 04f2:b270 | Chicony Elec... | HP HD Webcam [Fixed]     | 2.7%   | 3.14.44  | C6E683B39B |
| 04f2:b272 | Chicony Elec... | Lenovo EasyCamera        | 0.3%   | 2.6.32   | AF1E15F9D1 |
| 04f2:b293 | Chicony Elec... | HP Webcam-101            | 4.5%   | 3.14.44  | 30478F743C |
| 04f2:b307 | Chicony Elec... | TOSHIBA Web Camera - HD  | 1.4%   | 3.14.44  | 67009EFFAA |
| 04f2:b315 | Chicony Elec... | Integrated Camera        | 5.3%   | 3.14.53  | B7014678B5 |
| 04f2:b335 | Chicony Elec... | HD WebCam                | 1.7%   | 3.14.44  | 6A087DD575 |
| 04f2:b374 | Chicony Elec... | HD WebCam                | 1.2%   | 3.14.44  | EB418048B3 |
| 04f2:b3b2 | Chicony Elec... | TOSHIBA Web Camera - FHD | 7.1%   | 4.15.0   | 550460AAAC |
| 04f2:b40e | Chicony Elec... | HP Truevision HD camera  | 1.4%   | 3.14.25  | 9596ECB170 |
| 04f2:b452 | Chicony Elec... | HD WebCam                | 1%     | 3.14.25  | AF59A812BC |
| 04f2:b45a | Chicony Elec... | USB2.0 FHD Camera        | 9.1%   | 3.14.44  | 78D39E18EF |
| 04f2:b469 | Chicony Elec... | HD WebCam                | 0.7%   | 3.10.51  | C525BE0C9B |
| 04f2:b47f | Chicony Elec... | VGA Webcam               | 0.5%   | 3.14.44  | 401BBED185 |
| 04f2:b51c | Chicony Elec... | HP HD Camera             | 2.1%   | 4.1.15   | 254C1F48DA |
| 04f2:b52b | Chicony Elec... | USB2.0 VGA UVC WebCam    | 1%     | 3.14.44  | 94D2C67B3F |
| 04f2:b52c | Chicony Elec... | Integrated Camera        | 13.3%  | 4.9.9    | B2649601D3 |
| 04f2:b59a | Chicony Elec... | XiaoMi USB 2.0 Webcam    | 10%    | 4.9.60   | B1B825395C |
| 04f2:b59e | Chicony Elec... | USB2.0 Camera            | 1.8%   | 4.9.124  | 1E90C18C1F |
| 04f2:b5a3 | Chicony Elec... | XiaoMi USB 2.0 Webcam    | 8.3%   | 4.8.14   | 1F8DE2B55C |
| 04f2:b5bb | Chicony Elec... | Integrated Camera        | 25%    | 5.2.18   | 7408A95129 |
| 04f2:b5f7 | Chicony Elec... | HD WebCam                | 1.6%   | 4.9.20   | E703CB72E3 |
| 04f2:b614 | Chicony Elec... | Integrated Camera        | 5.3%   | 3.10.0   | 4438A85B31 |
| 04f2:b615 | Chicony Elec... | Integrated IR Camera     | 12.5%  | 5.0.0    | 4547E0D6FE |
| 04f2:b61e | Chicony Elec... | Integrated Camera        | 1%     | 4.15.0   | 8E74730A87 |
| 04f2:b64f | Chicony Elec... | HD User Facing           | 4.6%   | 4.15.0   | 64802F828B |
| 04f2:b664 | Chicony Elec... | USB 2.0 Webcam Device    | 100%   |          | C521DF4D98 |
| 04f2:b669 | Chicony Elec... | HP HD Camera             | 5.3%   | 4.15.0   | BDD15B19B1 |
| 04f2:b671 | Chicony Elec... | HP Full-HD Camera        | 25%    | 5.5.7    | A838427772 |
| 04f2:b678 | Chicony Elec... | LG Camera                | 8.3%   | 4.15.0   | BF08AA9738 |
| 04f2:b67c | Chicony Elec... | Integrated Camera        | 1%     | 4.15.0   | CA529580D5 |
| 04f2:b67f | Chicony Elec... | HP TrueVision HD Camera  | 5.6%   | 4.15.0   | 4F1105BCA0 |
| 04f2:b684 | Chicony Elec... | USB2.0 Camera            | 9.1%   | 4.18.0   | 5CD28E369C |
| 04f2:b6c2 | Chicony Elec... | Integrated Camera        | 14.3%  | 5.4.0    | CA7CA5B14E |
| 0547:6512 | Anchor Chips    | UCMOS05100KPA            | 100%   |          | 93BF2F1F49 |
| 054c:0954 | Sony            | ILCE-7S                  | 100%   |          | 68979EBA8F |
| 0572:0040 | Conexant Sys... | Wondereye CP-115 Webcam  | 100%   |          | 6B3D175AF8 |
| 058f:5608 | Alcor Micro     | USB 2.0 Camera           | 0.4%   | 3.14.44  | E1C0563D70 |
| 058f:a001 | Alcor Micro     | HP Webcam-101            | 2.8%   | 3.14.44  | FD16921273 |
| 05ac:12a8 | Apple           | iPhone 5/5C/5S/6/SE      | 2.3%   | 3.10.0   | F558E48348 |
| 05ac:12aa | Apple           | iPod Touch 5.Gen [A1421] | 100%   |          | 409A76B0F1 |
| 05ac:8501 | Apple           | Built-in iSight [Micron] | 20%    | 4.15.0   | 6A774ADE41 |
| 05ac:8509 | Apple           | FaceTime HD Camera       | 1.2%   | 4.1.25   | 65031A9A6D |
| 05c8:0223 | Cheng Uei Pr... | HP Webcam-50             | 5.9%   | 3.14.44  | 2E60620A98 |
| 05c8:0359 | Cheng Uei Pr... | HP HD Webcam             | 2.4%   | 3.14.15  | 8DCBD3C2B1 |
| 05c8:0369 | Cheng Uei Pr... | HP HD Webcam             | 1.4%   | 4.1.25   | B0C4FE1761 |
| 05c8:0374 | Cheng Uei Pr... | HP EliteBook integrat... | 2.1%   | 4.9.0    | 82579034FE |
| 05c8:038f | Cheng Uei Pr... | HP TrueVision HD         | 0.9%   | 4.9.41   | 5F80EB8AB2 |
| 05c8:03ab | Cheng Uei Pr... | HP Wide Vision HD Camera | 11.1%  | 4.9.60   | 142D7492C2 |
| 05c8:0815 | Cheng Uei Pr... | HP Wide Vision FHD Ca... | 20%    | 4.19.10  | 8AAAF9416E |
| 05ca:1810 | Ricoh           | Pavilion Webcam [R5U870] | 22.2%  | 4.1.15   | AA60C58ED4 |
| 05ca:181a | Ricoh           | Laptop_Integrated_Web... | 25%    | 4.9.0    | 898AE3EA34 |
| 05ca:1830 | Ricoh           | Visual Communication ... | 100%   |          | 047C3A9402 |
| 05ca:1834 | Ricoh           | Visual Communication ... | 100%   |          | 7DFBCB9E53 |
| 05ca:1836 | Ricoh           | Visual Communication ... | 100%   |          | 94AD68CB82 |
| 05ca:1839 | Ricoh           | Visual Communication ... | 5.4%   | 3.14.44  | 3214D06F2C |
| 05ca:183a | Ricoh           | Visual Communication ... | 18.2%  | 3.14.44  | D9A021B2CC |
| 05ca:183f | Ricoh           | Sony Visual Communica... | 12.5%  | 4.9.76   | F9D3268ABE |
| 05ca:1870 | Ricoh           | Webcam 1000              | 100%   |          | FB7F51216E |
| 05ca:18ba | Ricoh           | Sony Visual Communica... | 3.3%   | 4.9.155  | 55652DADF6 |
| 05ca:18c0 | Ricoh           | USB2.0 Camera            | 1.5%   | 3.14.22  | EC69106A89 |
| 05ca:18ff | Ricoh           | NoData                   | 100%   |          | 67B4F58033 |
| 064e:8110 | Suyin           | Laptop_Integrated_Web... | 100%   |          | 4E9804E6ED |
| 064e:a103 | Suyin           | Acer/HP Integrated We... | 1.4%   | 3.14.33  | 8596529915 |
| 064e:a117 | Suyin           | HD Video WebCam          | 1.3%   | 3.14.44  | E0BCC4DF92 |
| 064e:d213 | Suyin           | UVC HD Webcam            | 2.2%   | 3.14.15  | DF8F241425 |
| 064e:d281 | Suyin           | HP TrueVision HD         | 3.3%   | 3.14.44  | 119A35F980 |
| 093a:7011 | Pixart Imaging  | Digital Wireless Camera  | 100%   |          | F8FD891B32 |
| 0ac8:3420 | Z-Star Micro... | Venus USB2.0 Camera      | 0.2%   | 3.14.15  | CDC3F83CDB |
| 0ac8:3450 | Z-Star Micro... | UVC USB2.0 Camera        | 0.4%   | 3.14.22  | 3C44204AA0 |
| 0ac8:c326 | Z-Star Micro... | Namuga 1.3M Webcam       | 6.7%   | 4.1.15   | 3AD0FF0E13 |
| 0ac8:c40a | Z-Star Micro... | A4 TECH USB2.0 PC Cam... | 0.3%   | 3.10.34  | B2C845B843 |
| 0b05:200b | ASUSTek Comp... | ASUS_Z00VD               | 100%   |          | EDFAB941DF |
| 0b97:8381 | O2 Micro        | Mini S USB2.0 Camera     | 100%   |          | F1A2C19FEB |
| 0bda:5520 | Realtek Semi... | Integrated_Webcam_HD     | 2.6%   | 4.9.60   | 90B19AF55F |
| 0bda:564b | Realtek Semi... | WebCamera                | 25%    | 5.0.0    | 5EA0111CED |
| 0bda:5650 | Realtek Semi... | Integrated Webcam_HD     | 2.4%   | 4.4.0    | 53190BC040 |
| 0bda:5659 | Realtek Semi... | Integrated_Webcam_HD     | 12.5%  | 4.15.0   | DAF389F21B |
| 0bda:568c | Realtek Semi... | Integrated_Webcam_HD     | 1.2%   | 4.9.76   | B8337B4780 |
| 0bda:56c1 | Realtek Semi... | USB Camera               | 14.3%  | 4.15.0   | 1A171E7553 |
| 0bda:57cc | Realtek Semi... | HD Webcam - Realtek S... | 1%     | 4.1.25   | 5DBE9649A7 |
| 0bda:57ed | Realtek Semi... | USB2.0 VGA UVC WebCam    | 6.9%   | 4.9.9    | 551FF040B5 |
| 0bda:58bd | Realtek Semi... | USB2.0 HD UVC WebCam     | 20%    | 3.14.44  | B857F2B82D |
| 0bda:58be | Realtek Semi... | Laptop_Integrated_Web... | 3.8%   | 4.1.15   | A7211B4E35 |
| 0c45:62c0 | Microdia        | Sonix USB 2.0 Camera     | 0.9%   | 2.6.32   | C1A1180C7A |
| 0c45:6310 | Microdia        | Sonix USB 2.0 Camera     | 1.8%   | 3.14.44  | E6398EEC82 |
| 0c45:6350 | Microdia        | USB 2.0 Camera           | 100%   |          | 34DDCDDC0E |
| 0c45:6362 | Microdia        | JOYACCESS JA-Webcam      | 100%   |          | CBDE0F0553 |
| 0c45:6369 | Microdia        | USB 2.0 Camera           | 67.9%  | 5.3.0    | C144D3A1BC |
| 0c45:63ee | Microdia        | Integrated_Webcam_1.3M   | 5.9%   | 4.4.16   | 536E9A34A7 |
| 0c45:6433 | Microdia        | Laptop Integrated Web... | 10%    | 4.9.60   | EAFEF7DB79 |
| 0c45:643f | Microdia        | Dell Integrated HD We... | 3%     | 4.1.15   | 4E38982788 |
| 0c45:649d | Microdia        | Laptop_Integrated_Web... | 1.9%   | 4.9.20   | 8EA71BA2AE |
| 0c45:64cb | Microdia        | Integrated_Webcam_HD     | 8%     | 3.14.44  | BFA1F898FB |
| 0c45:64d2 | Microdia        | Integrated Webcam        | 2.7%   | 4.9.60   | 037A28C347 |
| 0c45:6709 | Microdia        | Integrated_Webcam_HD     | 5.6%   | 4.1.18   | 173ECC36BA |
| 0c45:670c | Microdia        | Integrated Webcam HD     | 2.8%   | 4.1.25   | 6695D2A05E |
| 0c45:6718 | Microdia        | Integrated_Webcam_HD     | 5.9%   | 4.15.0   | DD4521B554 |
| 0c45:671d | Microdia        | Integrated_Webcam_HD     | 5.3%   | 4.15.0   | E31ABB4A0C |
| 0c45:6a08 | Microdia        | Integrated_Webcam_HD     | 7.1%   | 4.15.0   | 6548681F70 |
| 0e8d:200b | MediaTek        | RAPID_10_LTE             | 100%   |          | F2CD8A3FFB |
| 0f00:0050 | ndd Medizint... | EasyOne PictBridge Cr... | 100%   |          | 6C32F3272C |
| 0fce:0a07 | Sony Ericsso... | Xperia XA2               | 100%   |          | 20DB446598 |
| 13d3:56a6 | IMC Networks    | Integrated Camera        | 2.5%   | 4.15.0   | CD929CAF4F |
| 13d3:56b2 | IMC Networks    | Integrated Camera        | 0.7%   | 3.10.0   | BCCEC7C3D1 |
| 13d3:56dd | IMC Networks    | USB2.0 HD UVC WebCam     | 1.4%   | 4.15.0   | F856F4367C |
| 13d3:56e4 | IMC Networks    | USB2.0 HD IR UVC WebCam  | 40%    | 5.0.0    | 65529AFB99 |
| 13d3:56e5 | IMC Networks    | USB2.0 HD UVC WebCam     | 100%   |          | 9C797156F9 |
| 13d3:5727 | IMC Networks    | Lenovo EasyCamera        | 4.1%   | 4.1.15   | AB6BD693BE |
| 13d3:5a01 | IMC Networks    | USB2.0 VGA UVC WebCam    | 0.6%   | 4.9.0    | E2ABCBDE3E |
| 13d3:5a07 | IMC Networks    | VGA UVC WebCam           | 2.8%   | 4.9.0    | 9F07F64EBF |
| 152d:0770 | JMicron Tech... | Alienware Integrated ... | 33.3%  | 5.0.0    | 7E166AFA9D |
| 174f:1122 | Syntek          | HP Webcam                | 25%    | 4.9.0    | 0230A47B05 |
| 174f:114f | Syntek          | Lenovo EasyCamera        | 11.8%  | 3.14.44  | 2DD89E3983 |
| 174f:14af | Syntek          | Lenovo EasyCamera        | 50%    | 4.15.0   | 08BB09B100 |
| 174f:14b8 | Syntek          | Lenovo EasyCamera        | 20%    | 4.1.15   | 39A9917502 |
| 174f:2408 | Syntek          | EasyCamera               | 8.6%   | 4.5.2    | C3D3D42413 |
| 174f:2426 | Syntek          | Integrated Camera        | 1.6%   | 4.18.0   | 80F496EACD |
| 174f:5a35 | Syntek          | Sonix 1.3MPixel USB 2... | 1.7%   | 3.14.33  | 0A87DE5887 |
| 174f:6a33 | Syntek          | Web Cam - Asus F3SA, ... | 100%   |          | 02A14B04F7 |
| 174f:6a51 | Syntek          | 2.0MPixel Web Cam - A... | 100%   |          | 224062149F |
| 174f:a821 | Syntek          | Web Cam - Packard Bel... | 100%   |          | 565D130BB6 |
| 1782:4011 | Spreadtrum C... | Spreadtrum Phone         | 100%   |          | DA34ABBC7C |
| 17ef:4816 | Lenovo          | Integrated Webcam        | 1.9%   | 3.14.44  | 85AC90E935 |
| 1871:01b0 | Aveo Technology | Cheetah3 USB2.0 Device   | 100%   |          | 0DB51928B9 |
| 18d1:4ee2 | Google          | Nexus/Pixel Device (M... | 53.8%  | 4.15.0   | A1E4EE1CB6 |
| 18d1:4ee5 | Google          | Nexus 4 (PTP)            | 50%    | 5.4.28   | 383D5B106E |
| 18ec:3399 | Arkmicro Tec... | USB2.0 PC CAMERA         | 0.7%   | 3.14.25  | 9D9E2DB550 |
| 1908:2310 | GEMBIRD         | USB2.0 PC CAMERA         | 1.2%   | 4.1.15   | C1582B3202 |
| 1b17:6111 | DarkHorse .     | USB2.0 Web Camera        | 100%   |          | 6E9BA31D2B |
| 1b3b:2938 | iPassion Tec... | PC Camera/Webcam cont... | 100%   |          | 87142BF4F1 |
| 1b3f:2002 | Generalplus ... | 808 Camera #9 (web-ca... | 7.7%   | 3.19.0   | 8F5CBE37DA |
| 1bbb:0170 | T & A Mobile... | VFD 529                  | 100%   |          | 875A197A28 |
| 1bcf:2802 | Sunplus Inno... | Laptop_Integrated_Web... | 2.3%   | 3.14.44  | F33530C32A |
| 1bcf:288a | Sunplus Inno... | 1.3M HD WebCam           | 1.8%   | 3.14.44  | 8FE3AF49FB |
| 1bcf:2b95 | Sunplus Inno... | Integrated_Webcam_HD     | 4%     | 4.9.0    | 26DBEC9F3A |
| 1bcf:2c6e | Sunplus Inno... | Laptop Integrated Web... | 1.7%   | 3.14.25  | 8D6D195DA2 |
| 1bcf:2c81 | Sunplus Inno... | HD WebCam                | 1.6%   | 4.1.15   | AA51C338B2 |
| 1bcf:2c87 | Sunplus Inno... | HP Wide Vision HD        | 4%     | 4.9.20   | 7BD53B3FFB |
| 1bcf:2c9b | Sunplus Inno... | HP TrueVision HD Camera  | 2.1%   | 4.9.60   | FB1A60597A |
| 2104:0124 | Tobii Techno... | EyeChip                  | 7.1%   | 4.9.60   | ACA7993158 |
| 22b8:2e83 | Motorola PCS    | Moto E (4) Plus          | 100%   |          | BC5ED8DEA4 |
| 22d9:2771 | MediaTek        | CPH1725                  | 100%   |          | 546A8D0043 |
| 2717:ff10 | Xiaomi          | Mi/Redmi series (PTP)    | 66.7%  | 4.15.0   | D633DC9722 |
| 2970:4011 | Fly             | Life Jet                 | 100%   |          | 0C91AAB0FF |
| 5986:0143 | Acer            | HP Webcam                | 4%     | 4.1.16   | 0C8D7641B2 |
| 5986:024b | Acer            | BisonCam, NB Pro         | 4%     | 3.14.44  | CD89DD62C8 |
| 5986:02d5 | Acer            | Integrated Camera        | 4.7%   | 3.14.44  | 55427995B5 |
| 5986:0683 | Acer            | BisonCam, NB Pro         | 3.7%   | 4.9.20   | 54574B77F2 |
| 5986:06b3 | Acer            | EasyCamera               | 4.2%   | 4.1.25   | D64B4A56E0 |
| 5986:1141 | Acer            | Integrated IR Camera     | 7.1%   | 4.15.0   | 6A667C9BA7 |
| 5986:2113 | Acer            | Integrated Camera        | 0.6%   | 4.13.0   | 6A667C9BA7 |
| 5986:9102 | Acer            | BisonCam,NB Pro          | 2.4%   | 4.15.0   | 320DADA481 |
| 6993:b019 | Yealink Netw... |                          | 100%   |          | 26DBEC9F3A |

### Card reader (USB)

16 out of 23 (69.57%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 04e6:512b | SCM Microsys... | SDI011 Contactless Re... | 100%   |          | 3810E77092 |
| 062d:0001 | Taiwan Tai-H... | Smart Card Reader        | 100%   |          | 52D70A47DA |
| 072f:9000 | Advanced Car... | ACR38 AC1038-based Sm... | 10.5%  | 4.15.0   | 870D0FE48E |
| 0b0c:003f | Todos AB        | Todos C400 smartcard ... | 100%   |          | 761778D6DF |
| 0bda:0129 | Realtek Semi... | RTS5129 Card Reader C... | 0.2%   | 3.8.0    | E703CB72E3 |
| 0bda:0139 | Realtek Semi... | RTS5139 Card Reader C... | 0.4%   | 3.10.34  | 81A1579081 |
| 0bda:0150 | Realtek Semi... | Realtek USB 2.0 Card ... | 100%   |          | 3C44204AA0 |
| 0c45:1018 | Microdia        | Compact Flash storage... | 100%   |          | 696C2127B6 |
| 0c4b:0500 | Reiner SCT K... | cyberJack RFID standa... | 80%    | 4.4.4    | 185846031E |
| 0c4b:0501 | Reiner SCT K... | cyberJack RFID comfor... | 76.2%  | 4.19.0   | 6166C5D0EE |
| 0ca6:0010 | Castles Tech... | EZUSB PC/SC Smart Car... | 100%   |          | E783786489 |
| 0d8c:5200 | C-Media Elec... | Mass Storage Controll... | 100%   |          | 90202855A8 |
| 11c5:0521 | Inmax           | IMT-0521 Smartcard Re... | 100%   |          | A8BFE861D7 |
| 17ef:3075 | Lenovo          | USB Billboard Device     | 100%   |          | 52144EB02A |
| 17ef:3078 | Lenovo          | USB Billboard            | 100%   |          | 5C664D23D8 |
| 2ce3:9563 |                 | EMV Smartcard Reader     | 100%   |          | 6B0ED71AF5 |

### Chipcard (USB)

55 out of 69 (79.71%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0403:e3b4 | Future Techn... | Parsec Desktop Reader... | 100%   |          | 775160993D |
| 046a:0070 | Cherry          | SmartTerminal XX1X       | 100%   |          | 181CA18DFB |
| 048d:1365 | Integrated T... | SmartCard Reader         | 100%   |          | DB4B891E15 |
| 04cc:5072 | ST-Ericsson     | Chipcard Reader          | 100%   |          | 65FD9B5315 |
| 04e6:5116 | SCM Microsys... | SCR331-LC1 / SCR3310 ... | 100%   |          | 9EC8A8D087 |
| 04e6:5119 | SCM Microsys... | SCR3340 - ExpressCard... | 66.7%  | 3.10.0   | 786DF34E10 |
| 04e6:5410 | SCM Microsys... | SCR35xx Smart Card Re... | 100%   |          | 219BC0E959 |
| 04e6:e001 | SCM Microsys... | SCR331 SmartCard Reader  | 50%    | 3.10.0   | D3D8B39015 |
| 0529:0620 | Aladdin Know... | Token JC                 | 88.9%  | 2.6.32   | 349BCE1A50 |
| 058f:9520 | Alcor Micro     | Watchdata W 1981         | 85.7%  | 4.15.0   | 512E21A61B |
| 058f:9540 | Alcor Micro     | AU9540 Smartcard Reader  | 93.1%  | 4.13.0   | 9A514460F0 |
| 072f:2200 | Advanced Car... | ACR122U                  | 40%    | 4.15.0   | B6F4A8F034 |
| 072f:2224 | Advanced Car... | ACR1281 1S Dual Reader   | 100%   |          | 04E5B85D84 |
| 072f:90cc | Advanced Car... | ACR38 SmartCard Reader   | 37.5%  | 4.8.13   | 66DFF7439E |
| 072f:90de | Advanced Car... | Token USB 64K            | 50%    | 4.1.25   | 02F1FBC843 |
| 072f:b000 | Advanced Car... | ACR3901U                 | 100%   |          | A44B651190 |
| 076b:1021 | OmniKey         | CardMan 1021             | 62.5%  | 4.15.0   | 3D9E77AE8A |
| 076b:3021 | OmniKey         | CardMan 3121             | 63.6%  | 3.14.33  | D9620F619F |
| 076b:3031 | OmniKey         | 3x21 Smart Card Reader   | 100%   |          | 11EBF93798 |
| 076b:4321 | OmniKey         | CardMan 4321             | 100%   |          | B7B58BA2D6 |
| 076b:5421 | OmniKey         | Smart Card Reader USB    | 100%   |          | EE4E49C4A1 |
| 076b:a022 | OmniKey         | CardMan Smart@Link       | 100%   |          | 0138C33179 |
| 08e6:3437 | Gemalto (was... | GemPC Twin SmartCard ... | 68%    | 4.15.0   | 1A72632C64 |
| 08e6:3438 | Gemalto (was... | GemPC Key SmartCard R... | 100%   |          | 4CCFEAF9AE |
| 08e6:34ec | Gemalto (was... | Compact Smart Card Re... | 95%    | 4.15.0   | EBBD146327 |
| 0a5c:5800 | Broadcom        | BCM5880 Secure Applic... | 98.9%  | 3.10.36  | 44A14CCEA9 |
| 0a5c:5801 | Broadcom        | BCM5880 Secure Applic... | 97.6%  | 3.16.7   | B3BB493388 |
| 0a5c:5802 | Broadcom        | BCM5880 Secure Applic... | 100%   |          | 6AEC870554 |
| 0a5c:5804 | Broadcom        | BCM5880 Secure Applic... | 98.1%  | 5.5.9    | 6E9A34515B |
| 0a5c:5805 | Broadcom        | 5880                     | 100%   |          | 4C46B3C18D |
| 0a5c:5832 | Broadcom        | 5880                     | 96.1%  | 3.10.0   | F6D2736398 |
| 0a5c:5833 | Broadcom        | 5880                     | 100%   |          | 1E8DF38010 |
| 0a5c:5834 | Broadcom        | 5880                     | 89.5%  | 3.10.0   | F861E71F84 |
| 0a5c:5842 | Broadcom        | 58200                    | 95.5%  | 4.15.0   | 910252FDF1 |
| 0a5c:5843 | Broadcom        | 58200                    | 91.3%  | 5.3.16   | 94EC8D2A1D |
| 0a89:0025 | Aktiv           | Rutoken lite             | 50%    | 4.1.25   | 8FA80B8A39 |
| 0b97:7762 | O2 Micro        | Oz776 SmartCard Reader   | 100%   |          | 8A3157EA9C |
| 0b97:7772 | O2 Micro        | OZ776 CCID Smartcard ... | 98.6%  | 4.15.0   | 8BBB9EE1AF |
| 0bda:0165 | Realtek Semi... | Smart Card Reader Int... | 83.3%  | 4.4.0    | 4D466ADC68 |
| 0bf8:1006 | Fujitsu Siem... | SmartCard Reader 2A      | 100%   |          | 4CDB503B48 |
| 0c4b:0551 | Reiner SCT K... | tanJack USB              | 100%   |          | 22858CD970 |
| 0c4b:0580 | Reiner SCT K... | cyberJack one            | 100%   |          | 641E5EEB2A |
| 0c4b:9102 | Reiner SCT K... | cyberJack RFID basis ... | 100%   |          | D084073730 |
| 0ca6:00a0 | Castles Tech... | EZCCID Smart Card Reader | 100%   |          | 3DC7A36CB3 |
| 0d46:3010 | Kobil Systems   | KOBIL Class 3 Reader     | 100%   |          | CE2E3AD9AE |
| 0dc3:1004 | Athena Smart... | ASEDrive V2C             | 100%   |          | 8FC4603F6C |
| 147e:2020 | Upek            | TouchChip Fingerprint... | 100%   |          | 61709B5FFC |
| 17ef:1003 | Lenovo          | Integrated Smart Card... | 96.2%  | 3.10.0   | 2D15D63764 |
| 1a44:0001 | VASCO Data S... | Digipass 905 SmartCar... | 50%    | 4.15.0   | 171DAE0500 |
| 1a44:0870 | VASCO Data S... | DIGIPASS 870             | 75%    | 5.4.0    | CF5FE3DBCE |
| 20a0:4108 | Clay Logic      | Nitrokey Pro             | 11.1%  | 4.19.0   | 9C7B7CDE1E |
| 20a0:4230 | Clay Logic      | Nitrokey HSM             | 100%   |          | DEDECE32F6 |
| 23a0:0004 | BIFIT           | iBank2Key                | 100%   |          | A8A89AC09A |
| 24dc:0101 | ARDS            | JaCarta                  | 66.7%  | 4.15.0   | DA308A78C4 |
| 25dd:3111 | BIT4ID          | miniLector EVO           | 100%   |          | D0FE69A9DA |

### Converter (USB)

4 out of 6 (66.67%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0403:1237 | Future Techn... | Z397 GUARD Converter     | 100%   |          | 5F015278B6 |
| 0403:7a58 | Future Techn... | USB <-> Serial Cable     | 100%   |          | 1E0980990D |
| 0a12:0042 | Cambridge Si... | SPI Converter            | 100%   |          | E1C0C74CA6 |
| 110a:1110 | Moxa Technol... | UPort 1110               | 66.7%  | 4.9.124  | 3864E6C70F |

### Disk (USB)

33 out of 1971 (1.67%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0000:0000 |                 | UHCI Host Controller     | 6.2%   | 3.14.44  | 2AF0FAD914 |
| 048d:1336 | Integrated T... | SD/MMC Cardreader        | 0.4%   | 3.14.22  | 2CA048A380 |
| 054c:05ba | Sony            | Storage Media            | 2.6%   | 3.14.44  | 23BBED2E16 |
| 058f:6362 | Alcor Micro     | Flash Card Reader/Writer | 0.1%   | 3.8.12   | 0D4B7AD71C |
| 05c6:f000 | Qualcomm        | MMC Storage              | 50%    | 4.15.0   | 5DB09AE3F4 |
| 05dc:a01a | Lexar Media     | Echo                     | 100%   |          | 15870EE6D4 |
| 05e3:0716 | Genesys Logic   | USB 2.0 Multislot Car... | 0.5%   | 3.14.25  | C2EDD5FBAF |
| 05e3:0723 | Genesys Logic   | GL827L SD/MMC/MS Flas... | 3.3%   | 3.14.33  | B09664C500 |
| 0718:069c | Imation         | TF35 USB 3.0             | 100%   |          | 92BF714334 |
| 0781:5567 | SanDisk         | Cruzer Blade             | 0.1%   | 3.14.33  | 1A7FD48C0D |
| 0781:5581 | SanDisk         | Ultra                    | 0.2%   | 3.10.0   | 2B1062016D |
| 0781:55a5 | SanDisk         | Cruzer U                 | 3.4%   | 3.14.44  | 49EFA544EE |
| 090c:1000 | Silicon Motion  | Silicon-Power8G          | 0.1%   | 2.6.32   | 0C8D7641B2 |
| 0951:1603 | Kingston Tec... | DataTraveler 1GB/2GB ... | 2.1%   | 3.14.25  | FCD84BA9A1 |
| 0951:1666 | Kingston Tec... | DataTraveler 100 G3/G... | 0.2%   | 3.10.0   | AF97E15AFB |
| 0984:0301 | Apricorn        | SATAWire 6G              | 14.3%  | 4.4.0    | D20CC6E64D |
| 0a89:0030 | Aktiv           | Rutoken ECP              | 42.9%  | 4.1.25   | 1BB59DF9A7 |
| 0bda:0184 | Realtek Semi... | RTS5182 Card Reader      | 1.9%   | 3.14.44  | 6566319F04 |
| 0bda:0316 | Realtek Semi... | SD/MMC                   | 1.1%   | 3.14.44  | CB716FCDD9 |
| 0bda:0328 | Realtek Semi... | SD/MMC CRW               | 0.9%   | 3.10.0   | 4B9BEB25C2 |
| 0e8d:0002 | MediaTek        | 1030D                    | 25%    | 4.9.60   | E4B342382F |
| 1005:b113 | Apacer Techn... | Handy Steno 2.0/HT203    | 0.3%   | 3.0.28   | 8652B8318D |
| 12d1:2590 | Huawei Techn... | ORINOQUIA Auyantepui+... | 100%   |          | BEBC187DBD |
| 1307:1171 | Transcend       | Fingerprint Reader       | 88.9%  | 4.12.14  | F38B4218AA |
| 13fd:1617 | Initio          | Flash Padlock            | 100%   |          | 95CE4B3495 |
| 13fe:4300 | Kingston Tec... | USB DISK                 | 0.7%   | 4.1.38   | 704DE6C8EA |
| 13fe:5500 | Kingston Tec... | Patriot Memory           | 1.2%   | 3.14.44  | CE392DF9C0 |
| 152d:0578 | JMicron Tech... | JMS578 SATA 6Gb/s        | 0.4%   | 4.1.25   | F962D4BBF9 |
| 1d5c:2000 | Fresco Logic    | FL2000/FL2000DX VGA/D... | 66.7%  | 5.4.0    | 94839129C9 |
| 1f75:0817 | Innostor Tec... | innostor                 | 5.6%   | 4.1.25   | 06E385B318 |
| 5136:4678 | USB2.0          | Flash Disk 2.0           | 20%    | 4.1.38   | C1841B0A29 |
| 8644:8303 | Intenso GmbG    | USB Flash Disk           | 16.7%  | 4.9.20   | CE376CD0F4 |
| ffff:5678 | VendorCo        | Disk 2.0                 | 3.2%   | 4.4.0    | C7F73C8073 |

### Dvb card (USB)

18 out of 70 (25.71%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 04ca:f01c | Lite-On Tech... | TT1280DA DVB-T TV Tuner  | 100%   |          | 646D7B3BFD |
| 07ca:0810 | AVerMedia Te... | H810 USB Hybrid DVB-T    | 100%   |          | B46F2FEE35 |
| 07ca:0830 | AVerMedia Te... | H830 USB Hybrid DVB-T    | 100%   |          | 79A097BF6F |
| 07ca:0831 | AVerMedia Te... | H831 USB Hybrid DVB-T/T2 | 100%   |          | D5A4F195AE |
| 07ca:1334 | AVerMedia Te... | H334 MiniCard Hybrid ... | 100%   |          | 66815F42A2 |
| 07ca:1335 | AVerMedia Te... | H335C                    | 100%   |          | 432498EF4E |
| 07ca:1336 | AVerMedia Te... | A336 MiniCard Hybrid ... | 100%   |          | 21897DE2FC |
| 07ca:1831 | AVerMedia Te... | H831 USB Hybrid DVB-T/T2 | 100%   |          | 7DAAC9434C |
| 07ca:3867 | AVerMedia Te... | A867                     | 100%   |          | 159AB17857 |
| 07ca:4336 | AVerMedia Te... | A336 MiniCard Hybrid ... | 100%   |          | 0C3E26BCE7 |
| 07ca:a373 | AVerMedia Te... | A373                     | 100%   |          | 22317B4B49 |
| 0bda:2832 | Realtek Semi... | RTL2832U DVB-T           | 25%    | 4.1.19   | B6F4A8F034 |
| 0bda:2838 | Realtek Semi... | RTL2838 DVB-T            | 9.3%   | 3.14.25  | 2FF14127D7 |
| 1164:3edc | YUAN High-Te... | STK7700D                 | 100%   |          | DF82BB0E17 |
| 13d3:3282 | IMC Networks    | DVB-T + GPS Minicard ... | 100%   |          | 7F0F347502 |
| 1b80:c161 | Afatech         | DVB-T 2                  | 100%   |          | 2A8FB37B8C |
| 1b80:e39a | Afatech         | DVB-T395U [af9015]       | 100%   |          | 2A8FB37B8C |
| eb1a:5013 | eMPIA Techno... | USB 2883 Device          | 100%   |          | 5DD14F9164 |

### Fingerprint reader (USB)

81 out of 84 (96.43%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0483:2016 | STMicroelect... | Fingerprint Reader       | 100%   |          | EB1AFC0466 |
| 04e8:7301 | Samsung Elec... | Fingerprint Device       | 100%   |          | 8A2B72A9A1 |
| 04e8:7309 | Samsung Elec... | Fingerprint Device       | 100%   |          | 739EE63E1D |
| 04e8:730a | Samsung Elec... | Fingerprint Device       | 100%   |          | 7A33F1CF7E |
| 04f3:0903 | Elan Microel... | ELAN:Fingerprint         | 100%   |          | 66535AF0EC |
| 04f3:0c01 | Elan Microel... | ELAN:Fingerprint         | 100%   |          | CC938243FC |
| 04f3:0c03 | Elan Microel... | ELAN:Fingerprint         | 100%   |          | E6D69FEED2 |
| 04f3:0c10 | Elan Microel... | ELAN:Fingerprint         | 100%   |          | 74C0BDD4EB |
| 04f3:0c1a | Elan Microel... | ELAN:Fingerprint         | 100%   |          | 1C736E7FE5 |
| 04f3:0c28 | Elan Microel... | fingerprint sensor [F... | 100%   |          | C75DC69233 |
| 04f3:0c3a | Elan Microel... | Elan Security-WBF Fin... | 100%   |          | F3F60A5C06 |
| 05ba:0002 | DigitalPersona  | Fingerprint Scanner, ... | 100%   |          | AE361E5F23 |
| 05ba:000a | DigitalPersona  | Fingerprint Reader       | 66.7%  | 5.4.13   | 147176E686 |
| 06cb:0078 | Synaptics       | WBDI Device              | 100%   |          | 5D3ACC6984 |
| 06cb:0081 | Synaptics       | Synaptics WBDI           | 100%   |          | F59C4C5727 |
| 06cb:0082 | Synaptics       | Synaptics WBDI Finger... | 100%   |          | C0AED5851E |
| 06cb:009a | Synaptics       | Metallica MIS Touch F... | 99.5%  | 4.15.0   | 758A8710D7 |
| 06cb:009b | Synaptics       |                          | 100%   |          | 26CE84E83B |
| 06cb:00a2 | Synaptics       | Metallica MOH Touch F... | 100%   |          | D3C0F51CF4 |
| 06cb:00a8 | Synaptics       |                          | 100%   |          | DD10CAA4C9 |
| 06cb:00b7 | Synaptics       | Synaptics VFS7552 Tou... | 100%   |          | F3F9F777FA |
| 06cb:00bb | Synaptics       |                          | 100%   |          | EBF056CC0B |
| 06cb:00bd | Synaptics       | Prometheus MIS Touch ... | 99.7%  | 5.4.0    | F1E82D3EEC |
| 06cb:00be | Synaptics       |                          | 100%   |          | FCD42BE9CB |
| 06cb:00c7 | Synaptics       |                          | 100%   |          | 3FBD330995 |
| 06cb:00c9 | Synaptics       |                          | 100%   |          | 1169B084AC |
| 06cb:00df | Synaptics       | Synaptics FS7604 Touc... | 100%   |          | 3638848F89 |
| 06cb:00e7 | Synaptics       |                          | 100%   |          | 1708B21DAB |
| 08ff:1600 | AuthenTec       | AES1600                  | 100%   |          | DAD5C8901D |
| 08ff:1660 | AuthenTec       | AES1660 Fingerprint S... | 100%   |          | F721B40A9C |
| 08ff:1686 | AuthenTec       | Fingerprint Sensor       | 100%   |          | 32C7E07A9A |
| 08ff:168a | AuthenTec       | Fingerprint Sensor       | 100%   |          | DC79EFB422 |
| 08ff:168b | AuthenTec       | Fingerprint Sensor       | 100%   |          | 54A1281AE2 |
| 08ff:168c | AuthenTec       | Fingerprint Sensor       | 100%   |          | DEFBCB9F08 |
| 08ff:168f | AuthenTec       | AES1660 Fingerprint S... | 100%   |          | C30562509E |
| 08ff:2500 | AuthenTec       | AES2501                  | 100%   |          | 4DCFB332DF |
| 08ff:2550 | AuthenTec       | AES2550 Fingerprint S... | 100%   |          | CECAD53985 |
| 08ff:2580 | AuthenTec       | AES2501 Fingerprint S... | 100%   |          | 9F80EA24A6 |
| 08ff:2665 | AuthenTec       | Fingerprint Sensor       | 100%   |          | DE2871CB64 |
| 08ff:2683 | AuthenTec       | Fingerprint Sensor       | 100%   |          | 7D4E0682DE |
| 08ff:2691 | AuthenTec       | Fingerprint Sensor       | 100%   |          | DE6B18FB9E |
| 08ff:2810 | AuthenTec       | AES2810                  | 100%   |          | BA90ADF2A9 |
| 138a:0001 | Validity Sen... | VFS101 Fingerprint Re... | 100%   |          | F56CA79C1E |
| 138a:0005 | Validity Sen... | VFS301 Fingerprint Re... | 100%   |          | 98D6C0C7B6 |
| 138a:0007 | Validity Sen... | VFS451 Fingerprint Re... | 99%    | 4.15.0   | 68F6F32B71 |
| 138a:0008 | Validity Sen... | VFS300 Fingerprint Re... | 100%   |          | 2E787CBAD7 |
| 138a:0010 | Validity Sen... | VFS Fingerprint sensor   | 100%   |          | 2C94B496CE |
| 138a:0011 | Validity Sen... | VFS5011 Fingerprint R... | 100%   |          | 41DA4C05AB |
| 138a:0017 | Validity Sen... | VFS 5011 fingerprint ... | 99.6%  | 4.18.0   | 5C49970B6B |
| 138a:0018 | Validity Sen... | Fingerprint scanner      | 100%   |          | 42B3B41FC9 |
| 138a:003c | Validity Sen... | VFS471 Fingerprint Re... | 99.2%  | 5.2.5    | 19BAD7A13F |
| 138a:003d | Validity Sen... | VFS491                   | 99.6%  | 5.6.12   | A960A3762F |
| 138a:003f | Validity Sen... | VFS495 Fingerprint Re... | 95.9%  | 4.9.0    | 0957532611 |
| 138a:0050 | Validity Sen... | Swipe Fingerprint Sensor | 100%   |          | 445CFE436D |
| 138a:0090 | Validity Sen... | VFS7500 Touch Fingerp... | 98.8%  | 4.15.0   | 75C64E9F90 |
| 138a:0091 | Validity Sen... | VFS7552 Touch Fingerp... | 100%   |          | DC3F9862DE |
| 138a:0092 | Validity Sen... | Synaptics VFS7552 Tou... | 100%   |          | 5FF09A0DFC |
| 138a:0094 | Validity Sen... | Synaptics WBDI           | 100%   |          | D0F33583B0 |
| 138a:0097 | Validity Sen... | Synaptics WBDI           | 100%   |          | DBAD89F493 |
| 138a:009d | Validity Sen... | Synaptics WBDI           | 100%   |          | 719A914957 |
| 138a:00a6 | Validity Sen... | Synaptics VFS7552 Tou... | 100%   |          | AC4B56556E |
| 138a:00ab | Validity Sen... | Synaptics VFS7552 Tou... | 100%   |          | E957F17330 |
| 147e:1000 | Upek            | Biometric Touchchip/T... | 100%   |          | 93AC7DDF97 |
| 147e:1001 | Upek            | TCS5B Fingerprint sensor | 100%   |          | BFDA7D01D5 |
| 147e:1002 | Upek            | Biometric Touchchip/T... | 100%   |          | 8DC078EA24 |
| 147e:2016 | Upek            | Biometric Touchchip/T... | 100%   |          | 97EB449D0D |
| 147e:5002 | Upek            | TouchStrip Fingerprin... | 100%   |          | 335EF1CCCD |
| 1c7a:0570 | LighTuning T... | EgisTec Touch Fingerp... | 100%   |          | 6F94930E8E |
| 1c7a:0577 | LighTuning T... | Fingerprint Sensor       | 100%   |          | 225373558D |
| 1c7a:0603 | LighTuning T... | ES603 Swipe Fingerpri... | 100%   |          | E70C8CB7E8 |
| 1c7a:0801 | LighTuning T... | Fingerprint Reader       | 100%   |          | A24F318D52 |
| 27c6:5110 | Shenzhen Goo... | Goodix Fingerprint De... | 100%   |          | 2C5F8C0B72 |
| 27c6:5117 | Shenzhen Goo... | Fingerprint Reader       | 100%   |          | 383EDE6256 |
| 27c6:530c | Shenzhen Goo... | Fingerprint Reader       | 100%   |          | 34A262F0C9 |
| 27c6:533c | Shenzhen Goo... | FingerPrint              | 100%   |          | B0029DA795 |
| 27c6:538c | Shenzhen Goo... | Fingerprint Reader       | 100%   |          | 353479C671 |
| 27c6:5584 | Shenzhen Goo... | Fingerprint Reader       | 100%   |          | 4495AD8461 |
| 27c6:55a2 | Shenzhen Goo... | Goodix FingerPrint De... | 100%   |          | C2C3727C6A |
| 27c6:55a4 | Shenzhen Goo... | Goodix FingerPrint De... | 100%   |          | CECB990CFA |
| 27c6:55b4 | Shenzhen Goo... | Fingerprint Reader       | 98.9%  | 5.3.0    | A4FE72C063 |
| 2808:9338 | Focal-system... | FT9201Fingerprint.       | 100%   |          | 4C94E488C0 |

### Hardware key (USB)

4 out of 4 (100%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0471:485d | Philips (or ... | Senselock SenseIV v2.x   | 100%   |          | E4A6E39276 |
| 0a89:0003 | Aktiv           | Guardant Stealth 2       | 100%   |          | 5149320E81 |
| 0a89:0020 | Aktiv           | Rutoken S                | 72.7%  | 3.14.15  | 35FB98B552 |
| 14a8:0001 | Soft protect... | Soft protection devic... | 100%   |          | 2CF2098617 |

### Hasp (USB)

1 out of 1 (100%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0529:0001 | Aladdin Know... | HASP copy protection ... | 98.9%  | 4.15.18  | EB2E75E011 |

### Hub (USB)

17 out of 490 (3.47%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 03eb:3301 | Atmel           | at43301 4-Port Hub       | 2.7%   | 3.14.44  | 8CF625BE49 |
| 03eb:3325 | Atmel           | RDU_84_T7                | 100%   |          | 10DB69DD6C |
| 0451:1446 | Texas Instru... | TUSB2040/2070 Hub        | 5.6%   | 4.15.0   | 593A72A02B |
| 05e3:0606 | Genesys Logic   | USB 2.0 Hub / D-Link ... | 0.2%   | 3.14.39  | 9AB71624F9 |
| 05e3:0608 | Genesys Logic   | Hub                      | 0%     | 2.6.32   | 704DE6C8EA |
| 0a05:7211 | Unknown Manu... | hub                      | 3.7%   | 3.14.44  | C389CF184F |
| 0a5c:4500 | Broadcom        | BCM2046B1 USB 2.0 Hub... | 0.1%   | 3.0.28   | C64FCF2A5D |
| 1a40:0101 | Terminus Tec... | Hub                      | 0.1%   | 3.2.0    | 9596ECB170 |
| 2109:0810 | VIA Labs        | VL81x Hub                | 1.2%   | 3.14.33  | B1EFC2E064 |
| 2109:0813 | VIA Labs        | VL813 Hub                | 0.5%   | 4.1.33   | 1EC556E585 |
| 2109:2813 | VIA Labs        | VL813 Hub                | 0.4%   | 3.10.0   | 1EC556E585 |
| 2109:8817 | VIA Labs        | USB Billboard Device     | 100%   |          | E20EBFF9C9 |
| 8087:0020 | Intel           | Integrated Rate Match... | 0%     | 3.0.28   | 57943279FE |
| 8087:0024 | Intel           | Integrated Rate Match... | 0.1%   | 3.10.0   | 269CE86EE6 |
| 8087:8000 | Intel           | Integrated Rate Match... | 0%     | 2.6.32   | B0C4FE1761 |
| 8087:8001 | Intel           | Integrated Hub           | 0.1%   | 2.6.32   | BD6F7205F3 |
| 8087:8008 | Intel           | Integrated Rate Match... | 0%     | 2.6.32   | B0C4FE1761 |

### Human interface (USB)

14 out of 607 (2.31%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 043e:9a39 | LG Electronics  | USB Controls             | 25%    | 4.15.0   | 98CE925293 |
| 044f:b10a | ThrustMaster    | T.16000M Joystick        | 5.6%   | 4.1.25   | 417453E269 |
| 045e:0659 | Microsoft       | HoloLens Sensors         | 25%    | 5.0.0    | A0BFCEB399 |
| 046d:c122 | Logitech        | Harmony 650/700 Remote   | 100%   |          | D7BCE39C2A |
| 0483:91d1 | STMicroelect... | Sensor Hub               | 1%     | 3.10.34  | BFA1F898FB |
| 04b4:fd13 | Cypress Semi... | Programmable power so... | 50%    | 4.18.0   | 7C4C7CAF9A |
| 056d:4044 | EIZO            | EIZO USB HID Monitor     | 100%   |          | 5391547134 |
| 05ac:1393 | Apple           | AirPods case             | 33.3%  | 5.0.0    | 613B95C545 |
| 096e:0201 | Feitian Tech... | USB DONGLE               | 57.1%  | 5.3.0    | 670706063D |
| 11ff:3341 |                 | USB Joystick             | 20%    | 4.1.7    | CD7FA9B160 |
| 1462:7b93 | Micro Star I... | MYSTIC LIGHT             | 25%    | 4.15.0   | 5D99916419 |
| 1770:ff00 | MSI             | steel series rgb keyb... | 0.3%   | 3.10.0   | 1C47BC90E4 |
| 1e71:170e | NZXT            | Kraken X                 | 3.3%   | 4.15.0   | 60038B2000 |
| 2386:350e | Raydium         | Touch System             | 100%   |          | 0636C222DC |

### Imaging (USB)

1 out of 2 (50%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 04a7:04d0 | Visioneer       | Xerox DocuMate 5460      | 100%   |          | 4ABAC242CC |

### Input/keyboard (USB)

11 out of 1849 (0.59%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 046d:c52b | Logitech        | Unifying Receiver        | 0%     | 3.10.0   | 8FC2C0633B |
| 046d:c534 | Logitech        | Unifying Receiver        | 0.1%   | 3.10.0   | AB3C4986E4 |
| 048d:8297 | Integrated T... | IT8297 RGB LED Contro... | 1.1%   | 4.12.14  | EFA77A90CB |
| 048d:ce00 | Integrated T... | ITE Device(8291)         | 2.6%   | 4.15.0   | AEFADA807A |
| 05ac:0236 | Apple           | Internal Keyboard/Tra... | 1.1%   | 4.1.16   | C6A5BE7D44 |
| 0624:0294 | Avocent         | Dell 03R874 KVM dongle   | 9.1%   | 3.10.0   | 97313ACF09 |
| 0a5c:4502 | Broadcom        | Keyboard (Boot Interf... | 0.4%   | 3.0.28   | 0C3E26BCE7 |
| 0b05:17fd | ASUSTek Comp... | ASUS ROG Macrokey        | 9.1%   | 3.14.44  | C5777BA928 |
| 0c45:7401 | Microdia        | TEMPer Temperature Se... | 75.8%  | 4.15.0   | 8115314F39 |
| 1050:0405 | Yubico.com      | Yubikey 4 OTP+CCID       | 33.3%  | 5.2.9    | B0543D9256 |
| 2717:ff40 | Xiaomi          | Mi/Redmi series (MTP)    | 35.7%  | 4.4.0    | 9412BBF453 |

### Input/mouse (USB)

18 out of 2014 (0.89%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 03eb:8a0c | Atmel           | maXTouch Digitizer       | 50%    | 4.15.0   | E994E96768 |
| 0458:003a | KYE Systems ... | NetScroll+ Mini Trave... | 0.1%   | 3.10.0   | 5599435B69 |
| 045e:0040 | Microsoft       | Wheel Mouse Optical      | 0.4%   | 3.10.0   | BFCD766C51 |
| 046d:c06c | Logitech        | Optical Mouse            | 0.4%   | 2.6.32   | C6690BB6D9 |
| 048d:8910 | Integrated T... | ITE Device(8910)         | 2.5%   | 4.13.0   | 2D91F64A77 |
| 04b4:0033 | Cypress Semi... | Mouse                    | 0.8%   | 3.14.25  | 4BCDE0B215 |
| 08ca:0010 | Aiptek Inter... | Tablet                   | 12.5%  | 3.14.44  | D295EC1834 |
| 0a5c:4503 | Broadcom        | Mouse (Boot Interface... | 0.4%   | 3.0.28   | A175422412 |
| 0b57:80b3 | Beijing Hanw... | Tablet                   | 100%   |          | 4B67EBD0C6 |
| 0bc7:0006 | X10 Wireless... | Wireless Transceiver ... | 15.3%  | 3.14.25  | BDE6F8112F |
| 1532:0037 | Razer USA       | DeathAdder 2013          | 2.2%   | 3.14.39  | D3BEA910CB |
| 1532:0042 | Razer USA       | Abyssus 2014             | 6.2%   | 4.9.76   | 31E99D9CEA |
| 18d1:4ee7 | Google          | Nexus/Pixel Device (c... | 78.6%  | 5.0.0    | C484F0D58F |
| 18f8:0f97 | [Maxxter]       | Optical Gaming Mouse ... | 0.2%   | 4.1.15   | BEADDBA484 |
| 1c4f:0034 | SiGma Micro     | XM102K Optical Wheel ... | 0.1%   | 3.10.0   | 6834F4BC15 |
| 256c:006e | HUION           | H420                     | 5.7%   | 4.1.16   | 1B290B3823 |
| 413c:8158 | Dell            | Integrated Touchpad /... | 88.6%  | 3.14.44  | 4A26920858 |
| 413c:8162 | Dell            | Integrated Touchpad [... | 82.9%  | 3.14.33  | 36A44664A8 |

### Modem (USB)

9 out of 145 (6.21%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0482:081f | Kyocera         | USB Device               | 100%   |          | 189475C3F5 |
| 04e8:6773 | Samsung Elec... | HSPA Modem               | 50%    | 4.15.0   | 3AD0FF0E13 |
| 0572:cb16 | Conexant Sys... | USB-ADSL Modem           | 100%   |          | 07217A2477 |
| 0baf:00ec | U.S. Robotics   | 56K Faxmodem             | 100%   |          | EF974030B3 |
| 0bdb:1900 | Ericsson Bus... | F3507g Mobile Broadba... | 2.6%   | 3.14.44  | 704DE6C8EA |
| 0bdb:1926 | Ericsson Bus... | H5321 gw Mobile Broad... | 3.7%   | 3.10.0   | 55427995B5 |
| 18d1:d001 | Google          | Nexus 4 (fastboot)       | 100%   |          | CCA77DDA93 |
| 27c6:5301 | Shenzhen Goo... | Fingerprint Reader       | 0.8%   | 4.4.0    | 716CB93844 |
| 27c6:5395 | Shenzhen Goo... | Fingerprint Reader       | 2.9%   | 4.15.0   | D97ED24FB5 |

### Net/ethernet (USB)

1 out of 3 (33.33%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 03f0:0547 | Hewlett-Packard | L2311c LAN7500 Ethernet  | 100%   |          | EBB304F58E |

### Net/wimax (USB)

3 out of 7 (42.86%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 8086:0186 | Intel           | WiMAX Connection 2400m   | 9.1%   | 3.14.44  | 7BA88076ED |
| 8086:1406 | Intel           | WiMAX Connection 2400m   | 4.8%   | 3.10.19  | 3B6AB87F14 |
| 8087:07d6 | Intel           | Centrino Wireless-N +... | 9.8%   | 3.10.34  | 1D8B6BC232 |

### Net/wireless (USB)

111 out of 353 (31.44%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0411:0242 | BUFFALO         | 802.11ac WLAN Adapter    | 40%    | 4.15.0   | D92D4F0666 |
| 0457:0162 | Silicon Inte... | SiS162 usb Wireless L... | 100%   |          | 0A302BFAFD |
| 045e:028f | Microsoft       | Xbox360 Wireless Cont... | 100%   |          | 9EC8A8D087 |
| 045e:0292 | Microsoft       | Xbox360 Wireless Netw... | 100%   |          | 957117D4E3 |
| 045e:02e6 | Microsoft       | Wireless XBox Control... | 62.5%  | 5.0.0    | C1E2E2FC80 |
| 045e:02f9 | Microsoft       | Xbox Embedded Wireless   | 100%   |          | A1A1CE6E00 |
| 045e:02fe | Microsoft       | XBOX ACC                 | 100%   |          | ECC0DF2129 |
| 045e:0719 | Microsoft       | Xbox 360 Wireless Ada... | 0.9%   | 3.14.44  | DA371C4305 |
| 050d:110a | Belkin Compo... | F9L1101v2 802.11abgn ... | 100%   |          | DCE411456D |
| 050d:615a | Belkin Compo... | F7D4101 / F9L1101v1 8... | 100%   |          | 04CE720011 |
| 050d:7050 | Belkin Compo... | F5D7050 Wireless G Ad... | 100%   |          | 7AC6824CEB |
| 057c:8502 | AVM             | FRITZ!WLAN AC 430        | 50%    | 5.1.9    | 7125E8AAA2 |
| 057c:8503 | AVM             | FRITZ!WLAN AC 860        | 9.1%   | 4.15.0   | A8D4B67DE8 |
| 057c:8602 | AVM             | FRITZ!WLAN USB Stick ... | 100%   |          | D4898E4C6A |
| 0586:3425 | ZyXEL Commun... | NWD6505 802.11a/b/g/n... | 75%    | 5.4.0    | 26FD738844 |
| 0586:3426 | ZyXEL Commun... | ZyXEL Dual-Band Wirel... | 66.7%  | 5.3.0    | 0D0564B3D2 |
| 07d1:3a0d | D-Link System   | DWA-120 802.11g Wirel... | 100%   |          | 96DE7C819B |
| 07d1:3b01 | D-Link System   | AirPlus G DWL-G122 Wi... | 100%   |          | A55363D509 |
| 07d1:3b11 | D-Link System   | DWA-130 802.11n Wirel... | 100%   |          | 606522CEDA |
| 07d1:3c09 | D-Link System   | DWA-140 RangeBooster ... | 10%    | 4.1.16   | 211A9802DB |
| 0846:4240 | NetGear         | WG111(v1) rev 2 54 Mb... | 100%   |          | 394B9426A3 |
| 0846:9011 | NetGear         | WNDA3100v2 802.11abgn... | 100%   |          | 49A7547077 |
| 0846:9014 | NetGear         | WNDA3100v3 802.11abgn... | 100%   |          | 64BDDC8167 |
| 0846:9020 | NetGear         | WNA3100(v1) Wireless-... | 100%   |          | 0F910ADD5E |
| 0846:9042 | NetGear         | On Networks N150MA 80... | 100%   |          | 0E5402CD3F |
| 0846:9050 | NetGear         | A6200 802.11a/b/g/n/a... | 100%   |          | B4AFED8FAD |
| 0846:9052 | NetGear         | A6100 AC600 DB Wirele... | 50.7%  | 4.15.0   | CC6CBAE1D4 |
| 0846:9053 | NetGear         | A6210                    | 21.3%  | 4.15.0   | 40AE5C532F |
| 0846:9054 | NetGear         | Nighthawk A7000 802.1... | 62.5%  | 5.0.0    | 41FDB733C0 |
| 0846:9055 | NetGear         | A6150                    | 100%   |          | A573CD6A7C |
| 0a5c:bd11 | Broadcom        | BCM4320 802.11bg Wire... | 100%   |          | CA66B01DF7 |
| 0a5c:bd13 | Broadcom        | BCM4323 802.11abgn Wi... | 100%   |          | B220FD9C11 |
| 0b05:17c9 | ASUSTek Comp... | USB-AC53 802.11a/b/g/... | 100%   |          | C7951A3833 |
| 0b05:17d1 | ASUSTek Comp... | AC51 802.11a/b/g/n/ac... | 52%    | 5.0.0    | ADC4529AFF |
| 0b05:17d2 | ASUSTek Comp... | USB-AC56 802.11a/b/g/... | 21.4%  | 5.0.0    | 62134F37DF |
| 0b05:17db | ASUSTek Comp... | WiFi                     | 100%   |          | 93C92CF446 |
| 0b05:1817 | ASUSTek Comp... | USB-AC68 802.11a/b/g/... | 93.3%  | 4.15.0   | 464709685B |
| 0b05:1841 | ASUSTek Comp... | 802.11ac NIC             | 33.3%  | 4.15.0   | 4B4C28ABBC |
| 0b05:184c | ASUSTek Comp... | 802.11ac NIC             | 84.6%  | 4.15.0   | 5A207F8ECB |
| 0b05:1852 | ASUSTek Comp... | 802.11ac NIC             | 100%   |          | D043FCBC96 |
| 0bda:0811 | Realtek Semi... | Realtek 8812AU/8821AU... | 70.2%  | 4.15.0   | F96E37E18B |
| 0bda:8172 | Realtek Semi... | RTL8191SU 802.11n WLA... | 0.6%   | 3.10.0   | 167CB26122 |
| 0bda:8176 | Realtek Semi... | RTL8188CUS 802.11n WL... | 1.1%   | 3.14.25  | 3635CADDD6 |
| 0bda:8179 | Realtek Semi... | RTL8188EUS 802.11n Wi... | 1.4%   | 3.14.25  | 0B1D1EC461 |
| 0bda:8187 | Realtek Semi... | RTL8187 Wireless Adapter | 0.7%   | 3.14.44  | E5E0D5140E |
| 0bda:818b | Realtek Semi... | RTL8192EU 802.11b/g/n... | 10.4%  | 4.9.0    | DE365730AB |
| 0bda:8812 | Realtek Semi... | RTL8812AU 802.11a/b/g... | 35.2%  | 4.1.38   | 2C3BAD189A |
| 0bda:8813 | Realtek Semi... | RTL8814AU 802.11a/b/g... | 68.8%  | 4.18.16  | A6D833A3B2 |
| 0bda:a811 | Realtek Semi... | RTL8811AU 802.11a/b/g... | 73.9%  | 4.15.0   | 086CFA3F2A |
| 0bda:b711 | Realtek Semi... | 802.11n WLAN Adapter     | 85.7%  | 5.4.0    | 26293FEB91 |
| 0bda:b812 | Realtek Semi... | RTL88x2bu [AC1200 Tec... | 69.6%  | 4.9.155  | FC2411B72F |
| 0bda:c811 | Realtek Semi... | 802.11ac NIC             | 74.1%  | 4.4.0    | D194AC9406 |
| 0bda:f179 | Realtek Semi... | RTL8188FTV 802.11b/g/... | 83%    | 4.15.0   | 0BCF8EAA29 |
| 0bf8:100f | Fujitsu Siem... | miniCard D2301 802.11... | 100%   |          | 0220656F77 |
| 0cde:0015 | Z-Com           | XG-705A 802.11g Wirel... | 100%   |          | B4E374835E |
| 0cf3:9271 | Qualcomm Ath... | AR9271 802.11n           | 0.5%   | 3.14.25  | 02DBB4B982 |
| 0e8d:760c | MediaTek        | 802.11 n WLAN            | 100%   |          | 74DFE126D0 |
| 0e8d:7610 | MediaTek        | WiFi                     | 40.6%  | 4.15.0   | 247B8C1A18 |
| 0e8d:7612 | MediaTek        | MT7612U 802.11a/b/g/n... | 31.2%  | 5.0.0    | 2373345C64 |
| 13b1:000a | Linksys         | WUSB54G v2 802.11g Ad... | 100%   |          | E6B8191910 |
| 13b1:0029 | Linksys         | WUSB300N 802.11bgn Wi... | 100%   |          | 18CF7C0503 |
| 13b1:0039 | Linksys         | AE1200 802.11bgn Wire... | 40%    | 4.18.0   | 7538D3A313 |
| 13b1:003a | Linksys         | AE2500 802.11abgn Wir... | 100%   |          | 05FFB07825 |
| 13b1:003e | Linksys         | AE6000 802.11a/b/g/n/... | 22.2%  | 5.3.0    | C27987482D |
| 13b1:003f | Linksys         | WUSB6300 802.11a/b/g/... | 74.4%  | 4.1.19   | A897C366A9 |
| 13b1:0042 | Linksys         | WUSB6100M 802.11a/b/g... | 10%    | 4.15.0   | 5155142A94 |
| 13b1:0043 | Linksys         | WUSB6400M                | 100%   |          | 1320E8E157 |
| 148f:7601 | Ralink Techn... | MT7601U Wireless Adapter | 10.3%  | 3.14.33  | D14C293BA3 |
| 148f:760b | Ralink Techn... | MT7601U Wireless Adapter | 30.8%  | 3.14.33  | D3D5F51D7A |
| 148f:761a | Ralink Techn... | MT7610U ("Archer T2U"... | 47.1%  | 4.15.0   | 02361185C7 |
| 16f0:0003 | GN ReSound A/S  | Airlink Wireless Prog... | 100%   |          | 7EC6FBAC2B |
| 1eda:2610 | AirTies Wire... | AirTies Wireless Adapter | 100%   |          | 591BDD6E15 |
| 2001:330f | D-Link          | DWA-125 11n Adapter      | 3.1%   | 3.14.44  | 01D21EA756 |
| 2001:3312 | D-Link          | Wireless N Nano USB A... | 100%   |          | 4629800E33 |
| 2001:3314 | D-Link          | DWA-171 AC600 DB Wire... | 40%    | 4.4.0    | 59660A488B |
| 2001:3315 | D-Link          | DWA-182 Wireless AC D... | 16.7%  | 3.14.39  | 77D8F05EB9 |
| 2001:3318 | D-Link          | 11ac adapter             | 70%    | 4.1.34   | DC121E5512 |
| 2001:3319 | D-Link          | DWA-131 Wireless N Na... | 24.6%  | 4.1.38   | 8F4591F672 |
| 2001:331a | D-Link          | 11ac Adapter             | 75%    | 5.3.0    | F2F5232045 |
| 2001:331b | D-Link          | WLAN controller          | 16.7%  | 4.15.0   | F28399B983 |
| 2001:331c | D-Link          | 802.11ac NIC             | 77.8%  | 4.15.0   | E0D5258A66 |
| 2357:0101 | TP-Link         | RTL8812AU Archer T4U ... | 41.2%  | 4.1.25   | D30BC8E081 |
| 2357:0103 | TP-Link         | Archer T4UH wireless ... | 50%    | 3.14.44  | D804242BA9 |
| 2357:0105 | TP-Link         | Archer T1U 802.11a/n/... | 48%    | 5.0.0    | 116FFA29C6 |
| 2357:0106 | TP-Link         | Archer T9UH v1 [Realt... | 87.5%  | 5.3.0    | CA2CE997BD |
| 2357:0107 | TP-Link         | TL-WN821N v5/v6 [RTL8... | 11.9%  | 4.15.0   | EF81BCBD99 |
| 2357:0108 | TP-Link         | TL-WN822N Version 4 R... | 3.1%   | 4.4.0    | 39A0192496 |
| 2357:0109 | TP-Link         | TL WN823N RTL8192EU      | 3.9%   | 3.16.0   | CA04809D83 |
| 2357:010c | TP-Link         | TL-WN722N v2             | 2.1%   | 4.9.41   | 90A8CF6632 |
| 2357:010d | TP-Link         | Archer T4U v2 [Realte... | 48%    | 4.15.0   | F86C7F17DB |
| 2357:010e | TP-Link         | TL-WN722N v2             | 100%   |          | CE020DD17D |
| 2357:0111 | TP-Link         | 802.11n NIC              | 66.7%  | 5.4.0    | 4FFA15CD0F |
| 2357:0115 | TP-Link         | Archer T4U ver.3         | 64.2%  | 4.15.0   | 5D32EB1D75 |
| 2357:011e | TP-Link         | AC600 wireless Realte... | 74.4%  | 4.4.0    | E6ACA4ABAE |
| 2357:011f | TP-Link         | 802.11ac WLAN Adapter    | 66.7%  | 4.15.0   | 81A973FE65 |
| 2357:0120 | TP-Link         | Archer T2U PLUS [RTL8... | 73.7%  | 4.15.0   | 6FF7C7478E |
| 2357:0122 | TP-Link         | 802.11n NIC              | 50%    | 4.18.0   | 7F6510382A |
| 2357:0126 | TP-Link         | 802.11n NIC              | 50%    | 4.18.0   | 71764F18DD |
| 2357:012d | TP-Link         | Archer T3U [Realtek R... | 54.5%  | 4.4.0    | A6F13FD4FA |
| 2604:0012 | Tenda           | U12                      | 56.2%  | 4.15.0   | FC10EB2AA9 |
| 2c4e:0100 | Mercucys        | MW300UM RTL8192EU wifi   | 71.4%  | 4.9.124  | 712B781DB9 |
| 2c4e:0102 | Mercucys        | 802.11n NIC              | 44.4%  | 5.6.1    | CBF18515B3 |
| 2c4e:0103 | MediaTek        | 802.11ac WLAN            | 50%    | 5.5.7    | 9946078BC6 |
| 413c:8102 | Dell            | TrueMobile 1300 802.1... | 100%   |          | 5776ED841E |
| 413c:81b6 | Dell            | DW5811e Snapdragon™... | 3.6%   | 4.1.25   | 568A079F29 |
| 4317:0720 | Broadcom        | Dynex DX-BUSB            | 100%   |          | 806CA649D7 |
| 7392:a812 | Edimax Techn... | AC600 USB                | 40.9%  | 3.14.25  | 28FA360E16 |
| 7392:a822 | Edimax Techn... | AC1200 USB               | 33.3%  | 5.4.0    | 72F4001D32 |
| 7392:a833 | Edimax Techn... | AC1750 USB               | 40%    | 4.15.0   | EADEFAE73E |
| 7392:b822 | Edimax Techn... | EW-7822ULC 802.11ac W... | 76.5%  | 4.18.0   | B61A579F2A |
| a727:6893 | 3Com            | 3CRUSB20075 OfficeCon... | 100%   |          | 968045D52D |

### Network (USB)

7 out of 248 (2.82%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 03f0:411d | Hewlett-Packard | lt2522 Mobile Broadba... | 100%   |          | 1D17C7B04C |
| 03f0:541d | Hewlett-Packard | hs3114 HSPA+ Mobile B... | 100%   |          | E1F4574972 |
| 045e:091e | Microsoft       | XBOX ACC                 | 100%   |          | D0D3D517EF |
| 05ac:12ab | Apple           | iPad 4/Mini1             | 21.4%  | 4.10.0   | 226AD1E0E2 |
| 0bda:8153 | Realtek Semi... | RTL8153 Gigabit Ether... | 0.6%   | 3.10.0   | 61DE8BA8A9 |
| 0bda:b720 | Realtek Semi... | RTL8723BU 802.11b/g/n... | 2.7%   | 4.4.1    | 0F4722247C |
| 2cb7:0210 | Fibocom         | L830-EB-00 LTE WWAN M... | 2.4%   | 4.15.0   | 12B5E06A49 |

### Sound (USB)

5 out of 688 (0.73%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 041e:3232 | Creative Tec... | Sound Blaster Premium... | 10.5%  | 4.1.25   | 4514D59538 |
| 046d:0a46 | Logitech        | Stereo H650e             | 33.3%  | 5.0.0    | 46B504A53C |
| 0763:2012 | M-Audio         | M-Audio Fast Track Pro   | 8.3%   | 4.15.0   | 1D9934126C |
| 0a12:1243 | Cambridge Si... | CSRA64110 USB Audio      | 25%    | 5.2.6    | 2A3F7B30CC |
| 194f:0302 | PreSonus Aud... | AudioBox USB             | 20%    | 4.15.0   | 03EEF2B7D3 |

### Tv card (USB)

7 out of 129 (5.43%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 046d:08a2 | Logitech        | Labtec Webcam Pro        | 16.7%  | 3.14.44  | 51837DE98F |
| 07ca:0889 | AVerMedia Te... | AVerTV Satellite 2       | 100%   |          | 174EC665C6 |
| 093a:2468 | Pixart Imaging  | SoC PC-Camera            | 13.3%  | 3.14.44  | B701C37D96 |
| 0ac8:c002 | Z-Star Micro... | Visual Communication ... | 12.5%  | 4.4.0    | 7F0BB0CC92 |
| 0c45:6030 | Microdia        | VideoCAM ExpressII       | 100%   |          | 6F28F56C47 |
| 0c45:6242 | Microdia        | PC Camera (SN9C201 + ... | 40%    | 4.9.20   | EF01565711 |
| 0c45:627b | Microdia        | PC Camera (SN9C201 + ... | 100%   |          | E5C5CE1445 |

### Ups (USB)

3 out of 22 (13.64%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0592:0002 | Powerware       | UPS (X-Slot)             | 12.5%  | 4.15.0   | 049C18DB44 |
| 06da:0002 | Phoenixtec P... | UPS                      | 100%   |          | 4F5E89A87E |
| 09ae:3016 | Tripp Lite      | UPS                      | 20%    | 5.3.0    | 76299BB9FF |

### Video (USB)

5 out of 8 (62.50%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0fd9:0051 | Elgato Systems  | GameCapture HD           | 100%   |          | 05F988930D |
| 1164:1ee9 | YUAN High-Te... | Polaris AV Capture       | 100%   |          | E1BB0618FD |
| 1b80:a41c | Afatech         | Polaris AV Capture       | 100%   |          | F20674C0B8 |
| 2304:0224 | Pinnacle Sys... | Pinnacle High Speed U... | 100%   |          | B67BBC7E71 |
| 5555:3382 | Epiphan Systems | VGA2USB Frame Grabber    | 100%   |          | 37A831391B |

### Wireless (USB)

1 out of 42 (2.38%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 15a9:003a | Gemtek          | Modem YOTA 4G LTE        | 100%   |          | 02E0DBC8D3 |

Usage of Outdated Kernels
-------------------------

13.1%  of new Linux users encounter hardware compatibility problems due to outdated kernels in Linux distributions.

