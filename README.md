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

    sudo -E hw-probe -all -upload

Total reports: 177135.

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
| 1814:3298 | 103c:18ec | Ralink          | RT3290 Bluetooth         | 96.9%  | 4.15.0   | 91B556E2A3 |
| 1814:3298 | 103c:191c | Ralink          | RT3290 Bluetooth         | 91.3%  | 5.4.0    | A4D6817276 |
| 1814:3298 | 105b:e056 | Ralink          | RT3290 Bluetooth         | 98.5%  | 5.3.0    | 3DC677388A |
| 1814:3298 | 10cf:1772 | Ralink          | RT3290 Bluetooth         | 100%   |          | 1135E21142 |
| 1814:3298 | 1814:3298 | Ralink          | RT3290 Bluetooth         | 100%   |          | AAC37423E5 |
| 1814:3298 | 1a3b:210b | Ralink          | RT3290 Bluetooth         | 100%   |          | 2333E930AF |
| 1814:3298 | 1a3b:2787 | Ralink          | RT3290 Bluetooth         | 100%   |          | A583282400 |
| 1814:3298 | 1a3b:2987 | Ralink          | RT3290 Bluetooth         | 100%   |          | 80DA000793 |
| 1814:3298 | 1a3b:2f87 | Ralink          | RT3290 Bluetooth         | 100%   |          | E60E072319 |

### Card reader (PCI)

83 out of 1328 (6.25%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 10ec:5209 | 103c:1672 | Realtek Semi... | RTS5209 PCI Express C... | 2.9%   | 3.14.44  | 585D199B71 |
| 10ec:5209 | 17aa:21fe | Realtek Semi... | RTS5209 PCI Express C... | 6.7%   | 3.10.0   | 33F0BF2A69 |
| 10ec:5227 | 103c:1940 | Realtek Semi... | RTS5227 PCI Express C... | 5.9%   | 4.15.0   | F440B0000D |
| 10ec:5227 | 103c:1992 | Realtek Semi... | RTS5227 PCI Express C... | 4.2%   | 4.1.25   | 2C52151F77 |
| 10ec:5227 | 103c:2209 | Realtek Semi... | RTS5227 PCI Express C... | 4.7%   | 4.9.20   | 2857EF3B7B |
| 10ec:5227 | 1179:0001 | Realtek Semi... | RTS5227 PCI Express C... | 2.1%   | 4.15.0   | 550460AAAC |
| 10ec:5227 | 1462:10f4 | Realtek Semi... | RTS5227 PCI Express C... | 50%    | 5.8.0    | 852662BDF3 |
| 10ec:5227 | 17aa:220c | Realtek Semi... | RTS5227 PCI Express C... | 0.6%   | 4.1.15   | 54B33D56BB |
| 10ec:5227 | 17aa:5034 | Realtek Semi... | RTS5227 PCI Express C... | 0.7%   | 4.13.0   | 27139478FF |
| 10ec:5229 | 103c:2211 | Realtek Semi... | RTS5229 PCI Express C... | 8.3%   | 4.15.0   | 86CAE084F4 |
| 10ec:5229 | 10ec:5229 | Realtek Semi... | RTS5229 PCI Express C... | 0.6%   | 3.10.51  | 13AB4D878D |
| 10ec:5229 | 17aa:381e | Realtek Semi... | RTS5229 PCI Express C... | 100%   |          | 588AC16C28 |
| 10ec:5229 | 8086:2072 | Realtek Semi... | RTS5229 PCI Express C... | 1.9%   | 4.15.0   | 70FA214165 |
| 10ec:522a | 103c:806e | Realtek Semi... | RTS522A PCI Express C... | 20%    | 5.4.0    | 62A9EF950E |
| 10ec:522a | 103c:8079 | Realtek Semi... | RTS522A PCI Express C... | 2.5%   | 4.4.1    | 15E62C605F |
| 10ec:522a | 103c:80a4 | Realtek Semi... | RTS522A PCI Express C... | 5.3%   | 4.9.60   | B01FB51118 |
| 10ec:522a | 103c:80ff | Realtek Semi... | RTS522A PCI Express C... | 19.4%  | 4.7.2    | B7B039F46E |
| 10ec:522a | 103c:8100 | Realtek Semi... | RTS522A PCI Express C... | 6.2%   | 4.15.0   | 2B56F34E21 |
| 10ec:522a | 103c:8101 | Realtek Semi... | RTS522A PCI Express C... | 7.4%   | 4.9.60   | BC496704F4 |
| 10ec:522a | 103c:820c | Realtek Semi... | RTS522A PCI Express C... | 14.3%  | 4.9.20   | FAE1CD27F3 |
| 10ec:522a | 103c:8377 | Realtek Semi... | RTS522A PCI Express C... | 7.9%   | 4.12.14  | C9A8C10A8F |
| 10ec:522a | 103c:837d | Realtek Semi... | RTS522A PCI Express C... | 1.2%   | 4.9.60   | F343AF14EB |
| 10ec:522a | 103c:8392 | Realtek Semi... | RTS522A PCI Express C... | 28.6%  | 4.9.20   | 142D7492C2 |
| 10ec:522a | 103c:84db | Realtek Semi... | RTS522A PCI Express C... | 8.3%   | 4.15.0   | 06EE78EE4D |
| 10ec:522a | 103c:85dd | Realtek Semi... | RTS522A PCI Express C... | 2.1%   | 5.0.0    | 1169B084AC |
| 10ec:522a | 103c:876f | Realtek Semi... | RTS522A PCI Express C... | 2.4%   | 5.4.0    | 5EAE12F393 |
| 10ec:522a | 10ec:522a | Realtek Semi... | RTS522A PCI Express C... | 0.7%   | 4.4.0    | 6254EDFB10 |
| 10ec:522a | 17aa:22b4 | Realtek Semi... | RTS522A PCI Express C... | 8.3%   | 5.4.0    | 4E68AE7E55 |
| 10ec:522a | 17aa:5048 | Realtek Semi... | RTS522A PCI Express C... | 10%    | 4.4.0    | A549AED5B4 |
| 10ec:522a | 17aa:505d | Realtek Semi... | RTS522A PCI Express C... | 5.6%   | 3.10.0   | 93B236AB24 |
| 10ec:522a | 17aa:506c | Realtek Semi... | RTS522A PCI Express C... | 3.8%   | 4.15.0   | E4205C0A3B |
| 10ec:522a | 17aa:5072 | Realtek Semi... | RTS522A PCI Express C... | 1.6%   | 5.0.0    | 4EE1271923 |
| 10ec:522a | 17aa:5082 | Realtek Semi... | RTS522A PCI Express C... | 1.8%   | 5.4.0    | EF90A9DF54 |
| 10ec:522a | 17aa:5113 | Realtek Semi... | RTS522A PCI Express C... | 12.5%  | 4.15.0   | 32F7318757 |
| 10ec:522a | 1854:0325 | Realtek Semi... | RTS522A PCI Express C... | 12.5%  | 4.15.0   | BF08AA9738 |
| 10ec:5249 | 103c:18e6 | Realtek Semi... | RTS5249 PCI Express C... | 16.7%  | 3.14.44  | CF3ED91B8A |
| 10ec:5249 | 103c:2253 | Realtek Semi... | RTS5249 PCI Express C... | 4.4%   | 4.19.0   | 2B62BC6C8A |
| 10ec:5249 | 17aa:3801 | Realtek Semi... | RTS5249 PCI Express C... | 2.2%   | 3.14.44  | 39A9917502 |
| 10ec:5250 | 1462:11b1 | Realtek Semi... | RTS5250 PCI Express C... | 100%   |          | 99E70D86E2 |
| 10ec:525a | 1028:06de | Realtek Semi... | RTS525A PCI Express C... | 2.4%   | 4.1.25   | 9BAD86D9C9 |
| 10ec:525a | 1028:06df | Realtek Semi... | RTS525A PCI Express C... | 2.3%   | 4.15.0   | 4C46B3C18D |
| 10ec:525a | 1028:075b | Realtek Semi... | RTS525A PCI Express C... | 1.1%   | 4.4.0    | 6695D2A05E |
| 10ec:525a | 1028:079f | Realtek Semi... | RTS525A PCI Express C... | 6.7%   | 4.15.0   | F6081D54B1 |
| 10ec:525a | 1028:07a8 | Realtek Semi... | RTS525A PCI Express C... | 7.1%   | 5.3.0    | EBA5E925B8 |
| 10ec:525a | 1028:07d0 | Realtek Semi... | RTS525A PCI Express C... | 3.1%   | 4.9.9    | D4927A9F76 |
| 10ec:525a | 1028:081b | Realtek Semi... | RTS525A PCI Express C... | 3.2%   | 3.10.0   | 05CDC89A9D |
| 10ec:525a | 1028:081c | Realtek Semi... | RTS525A PCI Express C... | 2.2%   | 4.12.14  | 54E871CA5D |
| 10ec:525a | 1028:08b8 | Realtek Semi... | RTS525A PCI Express C... | 2.5%   | 4.19.0   | 241B649AD1 |
| 10ec:525a | 1028:0905 | Realtek Semi... | RTS525A PCI Express C... | 1.3%   | 4.15.0   | 293A792A22 |
| 10ec:525a | 1028:09be | Realtek Semi... | RTS525A PCI Express C... | 5.9%   | 5.4.0    | AF066AD306 |
| 10ec:525a | 103c:83ba | Realtek Semi... | RTS525A PCI Express C... | 25%    | 4.19.7   | FE8F29171D |
| 10ec:525a | 103c:860f | Realtek Semi... | RTS525A PCI Express C... | 5.9%   | 4.18.0   | BDD15B19B1 |
| 10ec:525a | 17aa:225f | Realtek Semi... | RTS525A PCI Express C... | 2.8%   | 3.10.0   | FFDEE2C6E0 |
| 10ec:525a | 17aa:229b | Realtek Semi... | RTS525A PCI Express C... | 11.1%  | 5.4.0    | 3F3CC6B9D6 |
| 10ec:525a | 17aa:229f | Realtek Semi... | RTS525A PCI Express C... | 2%     | 5.0.0    | 72F3E05699 |
| 10ec:525a | 17aa:22a4 | Realtek Semi... | RTS525A PCI Express C... | 20%    | 5.4.0    | 3103814E46 |
| 10ec:5260 | 1462:12b0 | Realtek Semi... | RTS5260 PCI Express C... | 100%   |          | 35220AE516 |
| 10ec:5287 | 1025:0866 | Realtek Semi... | RTL8411B PCI Express ... | 3%     | 3.14.25  | 84429B1758 |
| 10ec:5287 | 1025:1264 | Realtek Semi... | RTL8411B PCI Express ... | 2%     | 4.1.25   | AAAA4C011C |
| 10ec:5287 | 1558:1404 | Realtek Semi... | RTL8411B PCI Express ... | 1.9%   | 5.0.0    | C1B424BC28 |
| 10ec:5287 | 1558:6509 | Realtek Semi... | RTL8411B PCI Express ... | 9.1%   | 5.0.0    | 13AB4D878D |
| 10ec:5287 | 1558:8550 | Realtek Semi... | RTL8411B PCI Express ... | 9.1%   | 4.18.0   | 04CBCE95B0 |
| 10ec:5288 | 103c:140a | Realtek Semi... | RTS5288 PCI Express C... | 33.3%  | 5.3.0    | A5DF70D8B6 |
| 10ec:5289 | 1025:0724 | Realtek Semi... | RTL8411 PCI Express C... | 1.8%   | 3.14.53  | 6A087DD575 |
| 10ec:5289 | 1043:1447 | Realtek Semi... | RTL8411 PCI Express C... | 3.6%   | 3.14.44  | F23B5BF0DA |
| 1aea:6601 | 0001:0001 | Alcor Micro     | AU6601 PCI-E Flash ca... | 27.3%  | 4.9.0    | E7400380E1 |
| 1aea:6601 | 1179:f900 | Alcor Micro     | AU6601 PCI-E Flash ca... | 16.7%  | 5.0.0    | 43A9D7922A |
| 1aea:6621 | 1aea:6621 | Alcor Micro     | AU6621 PCI-E Flash ca... | 31%    | 5.0.0    | 8564C561BD |
| 1aea:6625 | 103c:8349 | Alcor Micro     | AU6625 PCI-E Flash ca... | 66.7%  | 5.6.10   | 7758717ED0 |
| 1aea:6625 | 103c:834b | Alcor Micro     | AU6625 PCI-E Flash ca... | 66.7%  | 5.8.0    | BD086AB21D |
| 1aea:6625 | 103c:83a9 | Alcor Micro     | AU6625 PCI-E Flash ca... | 50%    | 5.9.10   | 08A47BB260 |
| 1aea:6625 | 103c:8477 | Alcor Micro     | AU6625 PCI-E Flash ca... | 60%    | 5.8.0    | 8721931B25 |
| 1aea:6625 | 103c:8478 | Alcor Micro     | AU6625 PCI-E Flash ca... | 72%    | 5.6.0    | B3C8E240B2 |
| 1aea:6625 | 103c:8479 | Alcor Micro     | AU6625 PCI-E Flash ca... | 100%   |          | 9088E2AAAD |
| 1aea:6625 | 103c:85fa | Alcor Micro     | AU6625 PCI-E Flash ca... | 16.7%  | 5.7.6    | 992E2074FF |
| 1aea:6625 | 103c:85fb | Alcor Micro     | AU6625 PCI-E Flash ca... | 60%    | 5.11.0   | FC1B7D94DC |
| 1aea:6625 | 103c:85fc | Alcor Micro     | AU6625 PCI-E Flash ca... | 77.8%  | 5.6.0    | 3E4D9C8191 |
| 1aea:6625 | 103c:85fd | Alcor Micro     | AU6625 PCI-E Flash ca... | 100%   |          | 5986AC405A |
| 1aea:6625 | 103c:85fe | Alcor Micro     | AU6625 PCI-E Flash ca... | 33.3%  | 5.6.11   | D23BC12452 |
| 1aea:6625 | 103c:85ff | Alcor Micro     | AU6625 PCI-E Flash ca... | 100%   |          | F8AD35BC66 |
| 1aea:6625 | 103c:8741 | Alcor Micro     | AU6625 PCI-E Flash ca... | 42.9%  | 5.8.0    | 90236B54E1 |
| 1aea:6625 | 103c:8744 | Alcor Micro     | AU6625 PCI-E Flash ca... | 28.6%  | 5.8.0    | 38C2A2235E |
| 1aea:6625 | 103c:8745 | Alcor Micro     | AU6625 PCI-E Flash ca... | 21.4%  | 5.6.6    | A181E12F35 |

### Communication controller (PCI)

680 out of 4922 (13.82%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 04f1:2f20 | 04f1:200c |                 | Communication controller | 100%   |          | 6759172767 |
| 104c:8035 | 103c:0934 | Texas Instru... | PCIxx21/PCIxx11 Smart... | 100%   |          | 453696FF5E |
| 104c:8035 | 103c:0938 | Texas Instru... | PCIxx21/PCIxx11 Smart... | 100%   |          | 27E013BC5F |
| 104c:8035 | 103c:0944 | Texas Instru... | PCIxx21/PCIxx11 Smart... | 100%   |          | 7F042FAA64 |
| 104c:8035 | 103c:099c | Texas Instru... | PCIxx21/PCIxx11 Smart... | 100%   |          | 5F105DDA68 |
| 104c:8038 | 1028:0182 | Texas Instru... | PCI6515 SmartCard Con... | 100%   |          | FAAF3B4F3D |
| 104c:8038 | 1028:0186 | Texas Instru... | PCI6515 SmartCard Con... | 100%   |          | CA3886900F |
| 104c:8038 | 1028:0187 | Texas Instru... | PCI6515 SmartCard Con... | 100%   |          | 358447EB4E |
| 104c:8038 | 1028:018f | Texas Instru... | PCI6515 SmartCard Con... | 100%   |          | 26B1A84EFA |
| 104c:803d | 103c:309f | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | 3FFD093A67 |
| 104c:803d | 103c:30a3 | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | A33E615CC5 |
| 104c:803d | 103c:30aa | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | 87BEFC0401 |
| 104c:803d | 103c:30ac | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | 50213B8AAB |
| 104c:803d | 103c:30ad | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | 25FFC80D33 |
| 104c:803d | 103c:30b1 | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | EEDF4BB0CA |
| 104c:803d | 1071:8212 | Texas Instru... | PCIxx12 GemCore based... | 100%   |          | 01F778FE4E |
| 1093:c801 |           | National Ins... | PCI-GPIB                 | 100%   |          | 29A0FC6CE0 |
| 11c1:0480 | 1668:0500 | LSI             | Venus Modem (V90, 56K... | 25%    | 3.14.22  | 0A61436F40 |
| 11c1:048c | 11c1:044c | LSI             | V.92 56K WinModem        | 100%   |          | F5D9A3BA0E |
| 11c1:0620 | 11c1:0620 | LSI             | Lucent V.92 Data/Fax ... | 100%   |          | 0F8A05C749 |
| 11c1:0620 | 11c1:0621 | LSI             | Lucent V.92 Data/Fax ... | 100%   |          | EFAB4D96E9 |
| 11c1:0630 | 11c1:0630 | LSI             | PCI-SV92EX Soft Modem    | 100%   |          | 32AF52ECCD |
| 11c1:0630 | 11c1:0631 | LSI             | PCI-SV92EX Soft Modem    | 100%   |          | 8581DA6FC5 |
| 125d:1989 | 103c:0012 | ESS Technology  | ESS Modem                | 100%   |          | 5E33FEBBC1 |
| 125d:2838 | 125d:2838 | ESS Technology  | ES2838/2839 SuperLink... | 100%   |          | 7F8C6DBB44 |
| 127a:1005 | 127a:1005 | Rockwell Int... | HCF 56k Data/Fax/Voic... | 100%   |          | B3EAB0C7AC |
| 127a:2013 | 1436:2113 | Rockwell Int... | HSF 56k Data/Fax Modem   | 100%   |          | B701C37D96 |
| 127a:2015 | 127a:2015 | Rockwell Int... | HSF 56k Data/Fax/Voic... | 100%   |          | 55EC1147BA |
| 127a:4311 | 1235:4311 | Rockwell Int... | Riptide HSF 56k PCI M... | 100%   |          | 34867AD122 |
| 13b0:0200 | 10b5:9050 | Maxspeed        | Communication controller | 100%   |          | FC54031F7E |
| 13f6:0211 | 13f6:0211 | C-Media Elec... | CM8738                   | 100%   |          | D120BBF41A |
| 14f1:1033 | 1092:0abf | Conexant Sys... | HCF 56k Data/Fax Modem   | 100%   |          | 729981A4D2 |
| 14f1:1033 | 13e0:020d | Conexant Sys... | HCF 56k Data/Fax Modem   | 100%   |          | 87F8B4B22A |
| 14f1:1033 | 13e0:02c0 | Conexant Sys... | HCF 56k Data/Fax Modem   | 100%   |          | 87CFD7513E |
| 14f1:1035 | 148d:1035 | Conexant Sys... | HCF 56k Data/Fax/Voic... | 100%   |          | 68D70F6AA0 |
| 14f1:1056 | 14f1:1056 | Conexant Sys... | HCF 56k Data/Fax/Voic... | 100%   |          | 9F48604FF2 |
| 14f1:10b6 | 14f1:10b6 | Conexant Sys... | CX06834-11 HCF V.92 5... | 100%   |          | 151D253025 |
| 14f1:10b6 | 1b28:c1e0 | Conexant Sys... | CX06834-11 HCF V.92 5... | 100%   |          | 092AE3A8CA |
| 14f1:10b6 | a0a0:00c2 | Conexant Sys... | CX06834-11 HCF V.92 5... | 100%   |          | ABB4E0E0C2 |
| 14f1:2013 | 13e0:0212 | Conexant Sys... | HSF 56k Data/Fax Modem   | 100%   |          | 3ED411EF5C |
| 14f1:2014 | 1048:1540 | Conexant Sys... | HSF 56k Data/Fax/Voic... | 100%   |          | 8BF298A811 |
| 14f1:2014 | 14f1:2014 | Conexant Sys... | HSF 56k Data/Fax/Voic... | 100%   |          | 445429C65F |
| 14f1:2702 | 1028:8d88 | Conexant Sys... | HSFi modem RD01-D270     | 100%   |          | F11822D259 |
| 14f1:2702 | 1028:8d89 | Conexant Sys... | HSFi modem RD01-D270     | 100%   |          | 50914BA2F5 |
| 14f1:2702 | 1043:8d88 | Conexant Sys... | HSFi modem RD01-D270     | 100%   |          | D83C8DDEDF |
| 14f1:2702 | 14f1:2007 | Conexant Sys... | HSFi modem RD01-D270     | 100%   |          | 83629CDF01 |
| 14f1:2f00 | 122d:8d88 | Conexant Sys... | HSF 56k HSFi Modem       | 100%   |          | E29EC46FD7 |
| 14f1:2f00 | 13e0:8d85 | Conexant Sys... | HSF 56k HSFi Modem       | 100%   |          | 1E963ACAC1 |
| 14f1:2f00 | 13e0:8d8b | Conexant Sys... | HSF 56k HSFi Modem       | 100%   |          | 300E280E8C |
| 14f1:2f00 | 13e0:8d8c | Conexant Sys... | HSF 56k HSFi Modem       | 100%   |          | 7B61A183A5 |
| 14f1:2f00 | 14f1:2000 | Conexant Sys... | HSF 56k HSFi Modem       | 100%   |          | 5BB1BF036F |
| 14f1:2f00 | 14f1:2002 | Conexant Sys... | HSF 56k HSFi Modem       | 100%   |          | 20D5A3BD6A |
| 14f1:2f00 | 14f1:2003 | Conexant Sys... | HSF 56k HSFi Modem       | 100%   |          | AF474622B9 |
| 14f1:2f00 | 14f1:2004 | Conexant Sys... | HSF 56k HSFi Modem       | 100%   |          | 171F37F987 |
| 14f1:2f00 | 187e:3409 | Conexant Sys... | HSF 56k HSFi Modem       | 100%   |          | C1BD1568DC |
| 14f1:2f00 | a0a0:02b0 | Conexant Sys... | HSF 56k HSFi Modem       | 100%   |          | B3AA6162D7 |
| 14f1:2f02 | 1767:000b | Conexant Sys... | HSF 56k HSFi Data/Fax    | 100%   |          | DFC83A3DB4 |
| 14f1:2f12 | 16ec:2016 | Conexant Sys... | HSF Data/Fax/Voice (USA) | 100%   |          | 3ADDAB1A1D |
| 14f1:2f20 | 14f1:2000 | Conexant Sys... | HSF 56k Data/Fax Modem   | 100%   |          | 8930791DA4 |
| 14f1:2f20 | 14f1:200c | Conexant Sys... | HSF 56k Data/Fax Modem   | 100%   |          | 7143EF66AF |
| 14f1:2f20 | 14f1:200f | Conexant Sys... | HSF 56k Data/Fax Modem   | 100%   |          | 0C5063C25C |
| 14f1:2f20 | 14f1:2014 | Conexant Sys... | HSF 56k Data/Fax Modem   | 100%   |          | 18C81B7E8B |
| 14f1:2f30 | 14f1:2000 | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | 2E9A342427 |
| 14f1:2f30 | 14f1:2004 | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | 457AB9CF46 |
| 14f1:2f30 | 14f1:200f | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | 6126EB96B3 |
| 14f1:2f30 | 14f1:2014 | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | 1930575F3E |
| 14f1:2f30 | 14f1:2030 | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | B6380B40C3 |
| 14f1:2f30 | 14f1:2051 | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | 01318BF092 |
| 14f1:2f30 | 14f1:205d | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | 21CEB7EB55 |
| 14f1:2f30 | 14f1:2075 | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | B4164233B1 |
| 14f1:2f30 | 14f1:20d5 | Conexant Sys... | SoftV92 SpeakerPhone ... | 100%   |          | C0301AC11D |
| 14f1:2f40 | 14f1:2000 | Conexant Sys... | PCI CX11261 Soft Modem   | 100%   |          | 252BF27B31 |
| 14f1:2f50 | 14f1:205f | Conexant Sys... | Conexant SoftK56 Data... | 100%   |          | 543E8D3501 |
| 14f1:2f50 | 14f1:207c | Conexant Sys... | Conexant SoftK56 Data... | 100%   |          | E13C9CE6FB |
| 14f1:2f81 | 14f1:0000 | Conexant Sys... | PCIe CX95610 Soft Modem  | 100%   |          | 89967DF724 |
| 14f1:2f82 | 14f1:0000 | Conexant Sys... | PCIe CX95610 Soft Modem  | 100%   |          | 039AFB9C35 |
| 1556:1111 | 1556:1111 | PLDA            | XpressRich-AXI Ref De... | 50%    | 4.14.0   | 93785932DD |
| 1813:4000 |           | Ambient Tech... | HaM controllerless modem | 100%   |          | E4FF6ACB83 |
| 1fd4:1999 | 1fd4:0101 | SUNIX           | Multiport serial cont... | 18.2%  | 5.3.0    | 4415A64795 |
| 5372:6870 | 1000:0010 |                 | Communication controller | 100%   |          | 9F8D495876 |
| 8086:02e0 | 1025:1357 | Intel           | Comet Lake Management... | 12%    | 5.4.0    | 8ED7109814 |
| 8086:02e0 | 1028:0950 | Intel           | Comet Lake Management... | 14.3%  | 5.3.0    | 20ABB6DE72 |
| 8086:02e0 | 1028:0954 | Intel           | Comet Lake Management... | 50%    | 5.8.0    | 8740133E10 |
| 8086:02e0 | 1028:0955 | Intel           | Comet Lake Management... | 3.2%   | 5.0.0    | 79CBBE0DFF |
| 8086:02e0 | 1028:0962 | Intel           | Comet Lake Management... | 8.1%   | 5.3.0    | 1683B7E772 |
| 8086:02e0 | 1028:0969 | Intel           | Comet Lake Management... | 100%   |          | 7ABAC766F3 |
| 8086:02e0 | 1028:096a | Intel           | Comet Lake Management... | 14.3%  | 5.4.0    | 6DC830E5A6 |
| 8086:02e0 | 103c:85f1 | Intel           | Comet Lake Management... | 7.1%   | 5.3.0    | 733DA06DF4 |
| 8086:02e0 | 103c:863f | Intel           | Comet Lake Management... | 8.3%   | 5.3.0    | F10553E785 |
| 8086:02e0 | 103c:866e | Intel           | Comet Lake Management... | 7.7%   | 5.3.0    | 8FF42ABD82 |
| 8086:02e0 | 103c:869d | Intel           | Comet Lake Management... | 9.5%   | 5.3.0    | D4A494F550 |
| 8086:02e0 | 103c:86b0 | Intel           | Comet Lake Management... | 16.7%  | 5.0.0    | 43BF3AF429 |
| 8086:02e0 | 103c:86b1 | Intel           | Comet Lake Management... | 15.4%  | 5.3.0    | CEE2AFAE3D |
| 8086:02e0 | 1043:1c71 | Intel           | Comet Lake Management... | 33.3%  | 5.3.0    | 2C64A52714 |
| 8086:02e0 | 1043:1db1 | Intel           | Comet Lake Management... | 100%   |          | F38D5CCA67 |
| 8086:02e0 | 1043:1e31 | Intel           | Comet Lake Management... | 75%    | 5.4.0    | 723BA4E443 |
| 8086:02e0 | 1462:1279 | Intel           | Comet Lake Management... | 16.7%  | 5.3.0    | 27665BDA0E |
| 8086:02e0 | 1462:129c | Intel           | Comet Lake Management... | 2.8%   | 5.3.0    | 754F3C176F |
| 8086:02e0 | 1462:b183 | Intel           | Comet Lake Management... | 54.5%  | 5.3.0    | 3C1185BE29 |
| 8086:02e0 | 1558:1403 | Intel           | Comet Lake Management... | 4.2%   | 5.3.0    | 38CC94083D |
| 8086:02e0 | 1558:1404 | Intel           | Comet Lake Management... | 13%    | 5.3.0    | DAACB350D8 |
| 8086:02e0 | 17aa:3185 | Intel           | Comet Lake Management... | 100%   |          | 324F862858 |
| 8086:02e0 | 17aa:3803 | Intel           | Comet Lake Management... | 2%     | 5.3.0    | 2BD6E7B668 |
| 8086:02e0 | 17aa:3804 | Intel           | Comet Lake Management... | 33.3%  | 5.4.23   | CA529580D5 |
| 8086:02e0 | 17aa:3806 | Intel           | Comet Lake Management... | 5.6%   | 4.18.0   | A1D4CF77BC |
| 8086:02e0 | 17aa:3808 | Intel           | Comet Lake Management... | 40%    | 5.0.0    | 3890D7877D |
| 8086:02e0 | 17aa:382f | Intel           | Comet Lake Management... | 8.3%   | 5.3.0    | E454A0B006 |
| 8086:02e0 | 17aa:5078 | Intel           | Comet Lake Management... | 4%     | 5.0.0    | 6625FCDF3B |
| 8086:02e0 | 17aa:5079 | Intel           | Comet Lake Management... | 1.8%   | 5.3.0    | 43BE642DA5 |
| 8086:02e0 | 17aa:507c | Intel           | Comet Lake Management... | 3.8%   | 5.4.0    | 8C056E4751 |
| 8086:02e0 | 1d05:107a | Intel           | Comet Lake Management... | 14.3%  | 5.4.0    | D412087992 |
| 8086:02e0 | 1d72:1901 | Intel           | Comet Lake Management... | 14.3%  | 5.3.0    | 4D4D89C508 |
| 8086:02e0 | 8086:2081 | Intel           | Comet Lake Management... | 5.7%   | 4.18.0   | A161A19F04 |
| 8086:06a8 | 1028:098f | Intel           | Comet Lake PCH Serial... | 10%    | 5.8.0    | 84387A75F7 |
| 8086:06e0 | 1025:142f | Intel           | Comet Lake HECI Contr... | 20%    | 4.18.0   | CEA1EFD2F4 |
| 8086:06e0 | 1028:097d | Intel           | Comet Lake HECI Contr... | 1.1%   | 5.4.0    | 11B9018EF1 |
| 8086:06e0 | 1028:0984 | Intel           | Comet Lake HECI Contr... | 100%   |          | 3A565370DE |
| 8086:06e0 | 1028:09a4 | Intel           | Comet Lake HECI Contr... | 28.6%  | 4.19.0   | 1E2EC488EE |
| 8086:06e0 | 1028:09c3 | Intel           | Comet Lake HECI Contr... | 5.9%   | 5.4.0    | 9362340E6C |
| 8086:06e0 | 1028:09e1 | Intel           | Comet Lake HECI Contr... | 21.9%  | 5.4.0    | 03AD0892DE |
| 8086:06e0 | 1028:09f6 | Intel           | Comet Lake HECI Contr... | 50%    | 5.4.0    | 1F5B92D91B |
| 8086:06e0 | 103c:8710 | Intel           | Comet Lake HECI Contr... | 33.3%  | 5.4.116  | A862C9D728 |
| 8086:06e0 | 103c:871c | Intel           | Comet Lake HECI Contr... | 100%   |          | 2F7FD6200F |
| 8086:06e0 | 103c:8746 | Intel           | Comet Lake HECI Contr... | 50%    | 5.7.15   | 1174318685 |
| 8086:06e0 | 103c:8755 | Intel           | Comet Lake HECI Contr... | 100%   |          | 334ABF8C53 |
| 8086:06e0 | 1043:1f21 | Intel           | Comet Lake HECI Contr... | 5.3%   | 5.4.0    | 2012AC3D84 |
| 8086:06e0 | 1043:8694 | Intel           | Comet Lake HECI Contr... | 7.5%   | 4.19.0   | F8503ECC3B |
| 8086:06e0 | 1458:1c3a | Intel           | Comet Lake HECI Contr... | 2.7%   | 4.18.0   | 4E23E323DD |
| 8086:06e0 | 1462:12aa | Intel           | Comet Lake HECI Contr... | 7.7%   | 5.4.0    | 9D39878AE6 |
| 8086:06e0 | 1462:7c75 | Intel           | Comet Lake HECI Contr... | 19%    | 4.19.0   | A29449D114 |
| 8086:06e0 | 17aa:380b | Intel           | Comet Lake HECI Contr... | 5.7%   | 5.4.0    | 294FD98C3F |
| 8086:06e0 | 1849:06e0 | Intel           | Comet Lake HECI Contr... | 11.1%  | 5.4.0    | 663E12849D |
| 8086:06e0 | 8086:7270 | Intel           | Comet Lake HECI Contr... | 15.4%  | 5.3.18   | ECF016BAF2 |
| 8086:0801 | 8086:0801 | Intel           | Moorestown SPI Ctrl 1    | 100%   |          | D1874B6708 |
| 8086:0802 | 8086:0802 | Intel           | Moorestown I2C 0         | 100%   |          | D1874B6708 |
| 8086:0803 | 8086:0803 | Intel           | Moorestown I2C 1         | 100%   |          | D1874B6708 |
| 8086:0804 | 8086:0804 | Intel           | Moorestown I2C 2         | 100%   |          | D1874B6708 |
| 8086:1197 |           | Intel           | Communication controller | 100%   |          | D1F5E15D8C |
| 8086:19d3 | 15d9:0969 | Intel           | Atom Processor C3000 ... | 100%   |          | 40E07B4DAD |
| 8086:19d3 | 8086:19d3 | Intel           | Atom Processor C3000 ... | 100%   |          | 50B6A72C0C |
| 8086:1c3a | 1019:99d2 | Intel           | 6 Series/C200 Series ... | 4.9%   | 3.14.44  | AD1B582D15 |
| 8086:1c3a | 1025:0492 | Intel           | 6 Series/C200 Series ... | 1.4%   | 3.10.34  | C0A7DFF96D |
| 8086:1c3a | 1025:0504 | Intel           | 6 Series/C200 Series ... | 0.3%   | 3.10.0   | 8FE3AF49FB |
| 8086:1c3a | 1025:0586 | Intel           | 6 Series/C200 Series ... | 10%    | 4.15.0   | 2138CE4CE5 |
| 8086:1c3a | 1028:0493 | Intel           | 6 Series/C200 Series ... | 0.4%   | 3.14.33  | F33530C32A |
| 8086:1c3a | 1028:0494 | Intel           | 6 Series/C200 Series ... | 1.1%   | 3.14.44  | 24CBAA1C59 |
| 8086:1c3a | 1028:049a | Intel           | 6 Series/C200 Series ... | 1.7%   | 3.14.44  | 1D46B26326 |
| 8086:1c3a | 1028:04a3 | Intel           | 6 Series/C200 Series ... | 1.8%   | 3.10.0   | B88C9F527C |
| 8086:1c3a | 1028:04ad | Intel           | 6 Series/C200 Series ... | 0.5%   | 4.1.25   | 14EDF3BD00 |
| 8086:1c3a | 1028:04b8 | Intel           | 6 Series/C200 Series ... | 15.8%  | 4.15.0   | E3AF15A170 |
| 8086:1c3a | 103c:1495 | Intel           | 6 Series/C200 Series ... | 4%     | 3.10.0   | B1460E1C12 |
| 8086:1c3a | 103c:1659 | Intel           | 6 Series/C200 Series ... | 3.8%   | 4.1.15   | 119A35F980 |
| 8086:1c3a | 103c:1672 | Intel           | 6 Series/C200 Series ... | 2.9%   | 3.14.44  | 585D199B71 |
| 8086:1c3a | 103c:2ac2 | Intel           | 6 Series/C200 Series ... | 4.1%   | 3.14.44  | 436A2CA3CE |
| 8086:1c3a | 1043:11d7 | Intel           | 6 Series/C200 Series ... | 2.6%   | 3.10.34  | A5A0DA657B |
| 8086:1c3a | 1043:844d | Intel           | 6 Series/C200 Series ... | 0.6%   | 3.0.38   | 95722413A6 |
| 8086:1c3a | 10cf:1611 | Intel           | 6 Series/C200 Series ... | 1%     | 4.1.34   | 958D094890 |
| 8086:1c3a | 1179:fc50 | Intel           | 6 Series/C200 Series ... | 1.1%   | 3.14.44  | 046BFED81F |
| 8086:1c3a | 144d:c0c1 | Intel           | 6 Series/C200 Series ... | 4.1%   | 3.14.44  | F79CBC4E24 |
| 8086:1c3a | 144d:c0cd | Intel           | 6 Series/C200 Series ... | 50%    | 5.4.0    | 071C4D8666 |
| 8086:1c3a | 1458:1c3a | Intel           | 6 Series/C200 Series ... | 0.2%   | 3.0.69   | 08EA956BFA |
| 8086:1c3a | 17aa:21cf | Intel           | 6 Series/C200 Series ... | 0.7%   | 3.10.0   | 4CAE7DC78D |
| 8086:1c3a | 17aa:21da | Intel           | 6 Series/C200 Series ... | 1.2%   | 3.14.25  | F9CF2CED7E |
| 8086:1c3a | 17aa:3975 | Intel           | 6 Series/C200 Series ... | 0.7%   | 3.10.34  | 81A1579081 |
| 8086:1c3a | 1849:1c3a | Intel           | 6 Series/C200 Series ... | 0.2%   | 3.10.0   | 7F5766D5DA |
| 8086:1c3a | 8086:1c3a | Intel           | 6 Series/C200 Series ... | 1.1%   | 4.1.15   | A12A2989FD |
| 8086:1c3a | 8086:2017 | Intel           | 6 Series/C200 Series ... | 4.3%   | 3.14.53  | CF6242CACA |
| 8086:1c3a | 8086:2042 | Intel           | 6 Series/C200 Series ... | 12.5%  | 3.14.44  | 7BE6ED70A7 |
| 8086:1c3a | 8086:7270 | Intel           | 6 Series/C200 Series ... | 0.3%   | 3.14.22  | D5C9D589F2 |
| 8086:1c3b |           | Intel           | 6 Series/C200 Series ... | 100%   |          | 22A64B85BE |
| 8086:1c3b | 15d9:0631 | Intel           | 6 Series/C200 Series ... | 100%   |          | 28940AAA42 |
| 8086:1c3b | 1734:11cb | Intel           | 6 Series/C200 Series ... | 100%   |          | 4B6AB99884 |
| 8086:1d3a | 1028:048c | Intel           | C600/X79 series chips... | 12.5%  | 4.15.0   | 77A5A8BF12 |
| 8086:1d3a | 1028:04ce | Intel           | C600/X79 series chips... | 25%    | 4.15.0   | 9977E2B5C3 |
| 8086:1d3a | 1028:04fa | Intel           | C600/X79 series chips... | 46.2%  | 5.0.0    | A4512466F1 |
| 8086:1d3a | 1028:05d2 | Intel           | C600/X79 series chips... | 2.8%   | 4.12.14  | 949DD823D7 |
| 8086:1d3a | 1028:05d4 | Intel           | C600/X79 series chips... | 9.1%   | 4.15.0   | 19FB02CA4E |
| 8086:1d3a | 1043:84ef | Intel           | C600/X79 series chips... | 0.5%   | 3.14.33  | 17ACFC90D4 |
| 8086:1d3a | 15d9:0628 | Intel           | C600/X79 series chips... | 40%    | 3.10.0   | 99E743CA9E |
| 8086:1d3a | 15d9:062b | Intel           | C600/X79 series chips... | 100%   |          | F791C179A5 |
| 8086:1d3a | 15d9:062c | Intel           | C600/X79 series chips... | 25%    | 4.15.0   | FF94B1201C |
| 8086:1d3a | 15d9:0636 | Intel           | C600/X79 series chips... | 94.1%  | 5.4.0    | 53FB02A9EF |
| 8086:1d3a | 15d9:0665 | Intel           | C600/X79 series chips... | 50%    | 4.18.0   | E4A055906A |
| 8086:1d3a | 15d9:0709 | Intel           | C600/X79 series chips... | 42.9%  | 5.3.0    | 9F3D443A21 |
| 8086:1d3a | 15d9:0714 | Intel           | C600/X79 series chips... | 100%   |          | F9D5463C17 |
| 8086:1d3a | 17aa:1026 | Intel           | C600/X79 series chips... | 8.3%   | 4.15.0   | 21286AF23B |
| 8086:1d3a | 1849:1d3a | Intel           | C600/X79 series chips... | 14.8%  | 4.12.14  | CF5FE3DBCE |
| 8086:1d3a | 8086:3582 | Intel           | C600/X79 series chips... | 100%   |          | 9F6D925B73 |
| 8086:1d3b | 1028:048c | Intel           | C600/X79 series chips... | 100%   |          | 4CE6A061A6 |
| 8086:1d3b | 1028:04ce | Intel           | C600/X79 series chips... | 100%   |          | 7A9C742839 |
| 8086:1d3b | 1028:04cf | Intel           | C600/X79 series chips... | 100%   |          | 0343B901D9 |
| 8086:1d3b | 1028:04db | Intel           | C600/X79 series chips... | 100%   |          | 203F23F8D5 |
| 8086:1d3b | 1028:04dc | Intel           | C600/X79 series chips... | 100%   |          | 2A0D285524 |
| 8086:1d3b | 1028:04f7 | Intel           | C600/X79 series chips... | 100%   |          | 6839F6245C |
| 8086:1d3b | 1028:04f8 | Intel           | C600/X79 series chips... | 100%   |          | EA68439F2E |
| 8086:1d3b | 1028:04f9 | Intel           | C600/X79 series chips... | 100%   |          | BB93FE95D1 |
| 8086:1d3b | 1028:04fa | Intel           | C600/X79 series chips... | 100%   |          | 1A32B081A7 |
| 8086:1d3b | 1028:04fe | Intel           | C600/X79 series chips... | 100%   |          | 53AEE4CABC |
| 8086:1d3b | 1028:0528 | Intel           | C600/X79 series chips... | 100%   |          | 31EA0B6D96 |
| 8086:1d3b | 1043:84ef | Intel           | C600/X79 series chips... | 100%   |          | A4C832AB44 |
| 8086:1d3b | 15d9:0626 | Intel           | C600/X79 series chips... | 100%   |          | 2B8813F5C4 |
| 8086:1d3b | 15d9:0628 | Intel           | C600/X79 series chips... | 100%   |          | F7519BF7BE |
| 8086:1d3b | 15d9:062b | Intel           | C600/X79 series chips... | 100%   |          | F791C179A5 |
| 8086:1d3b | 15d9:062c | Intel           | C600/X79 series chips... | 100%   |          | FF94B1201C |
| 8086:1d3b | 15d9:0630 | Intel           | C600/X79 series chips... | 100%   |          | 575A60EDC8 |
| 8086:1d3b | 15d9:0636 | Intel           | C600/X79 series chips... | 100%   |          | DD93F62FFC |
| 8086:1d3b | 15d9:0660 | Intel           | C600/X79 series chips... | 100%   |          | AFE42B7E58 |
| 8086:1d3b | 15d9:0665 | Intel           | C600/X79 series chips... | 100%   |          | E4A055906A |
| 8086:1d3b | 15d9:0667 | Intel           | C600/X79 series chips... | 100%   |          | 8FDC5D8AB4 |
| 8086:1d3b | 15d9:066b | Intel           | C600/X79 series chips... | 100%   |          | 1FF0EE8759 |
| 8086:1d3b | 15d9:0702 | Intel           | C600/X79 series chips... | 100%   |          | E1213C0B05 |
| 8086:1d3b | 15d9:0703 | Intel           | C600/X79 series chips... | 100%   |          | 8C793BB137 |
| 8086:1d3b | 15d9:0705 | Intel           | C600/X79 series chips... | 100%   |          | B3D08DD227 |
| 8086:1d3b | 15d9:0706 | Intel           | C600/X79 series chips... | 100%   |          | AA3D8595BA |
| 8086:1d3b | 15d9:0709 | Intel           | C600/X79 series chips... | 100%   |          | 7D84E25468 |
| 8086:1d3b | 15d9:070a | Intel           | C600/X79 series chips... | 100%   |          | 1F3561AA7D |
| 8086:1d3b | 15d9:070e | Intel           | C600/X79 series chips... | 100%   |          | DABC79444D |
| 8086:1d3b | 15d9:0714 | Intel           | C600/X79 series chips... | 100%   |          | F9D5463C17 |
| 8086:1d3b | 17aa:1026 | Intel           | C600/X79 series chips... | 100%   |          | 21286AF23B |
| 8086:1d3b | 1849:1d3b | Intel           | C600/X79 series chips... | 100%   |          | 957F68F2B7 |
| 8086:1d3b | 8086:1d3b | Intel           | C600/X79 series chips... | 100%   |          | AA487A5EDB |
| 8086:1d3b | 8086:357e | Intel           | C600/X79 series chips... | 100%   |          | 0FADD1EBE3 |
| 8086:1d3b | 8086:3582 | Intel           | C600/X79 series chips... | 100%   |          | 9F6D925B73 |
| 8086:1d3b | 8086:358c | Intel           | C600/X79 series chips... | 100%   |          | D15B8F8758 |
| 8086:1d3b | 8086:3594 | Intel           | C600/X79 series chips... | 100%   |          | FBDCC4D1F5 |
| 8086:1d3b | 8086:35a0 | Intel           | C600/X79 series chips... | 100%   |          | FE1E6CFF79 |
| 8086:1d3b | 8086:35b0 | Intel           | C600/X79 series chips... | 100%   |          | 30CFD7BC18 |
| 8086:1e3a | 1019:99f2 | Intel           | 7 Series/C216 Chipset... | 40%    | 5.0.0    | 45F3B356CF |
| 8086:1e3a | 1025:0647 | Intel           | 7 Series/C216 Chipset... | 0.5%   | 3.10.34  | 86D2D3B0E1 |
| 8086:1e3a | 1025:0649 | Intel           | 7 Series/C216 Chipset... | 0.4%   | 3.14.25  | 344148537E |
| 8086:1e3a | 1025:064b | Intel           | 7 Series/C216 Chipset... | 0.5%   | 3.14.33  | 3290540C34 |
| 8086:1e3a | 1025:0724 | Intel           | 7 Series/C216 Chipset... | 9.1%   | 4.1.16   | 6A087DD575 |
| 8086:1e3a | 1025:0727 | Intel           | 7 Series/C216 Chipset... | 10%    | 3.14.44  | 23E2162B8E |
| 8086:1e3a | 1025:074f | Intel           | 7 Series/C216 Chipset... | 28.6%  | 5.4.0    | 6566319F04 |
| 8086:1e3a | 1028:052c | Intel           | 7 Series/C216 Chipset... | 3%     | 4.15.0   | 779B6B3344 |
| 8086:1e3a | 1028:0534 | Intel           | 7 Series/C216 Chipset... | 0.9%   | 4.1.19   | 2E0EF916C6 |
| 8086:1e3a | 1028:053e | Intel           | 7 Series/C216 Chipset... | 3.4%   | 4.9.124  | F674F91052 |
| 8086:1e3a | 1028:058b | Intel           | 7 Series/C216 Chipset... | 60%    | 5.7.10   | 1DEA8D4332 |
| 8086:1e3a | 103c:1845 | Intel           | 7 Series/C216 Chipset... | 14.3%  | 3.14.44  | 2E60620A98 |
| 8086:1e3a | 103c:3396 | Intel           | 7 Series/C216 Chipset... | 2.2%   | 4.15.0   | 59E4E46994 |
| 8086:1e3a | 1043:100d | Intel           | 7 Series/C216 Chipset... | 3.1%   | 4.1.19   | 385F2BB5DF |
| 8086:1e3a | 1043:1447 | Intel           | 7 Series/C216 Chipset... | 4.5%   | 3.14.44  | F23B5BF0DA |
| 8086:1e3a | 1043:1477 | Intel           | 7 Series/C216 Chipset... | 1%     | 3.14.15  | 731932629B |
| 8086:1e3a | 1043:84ca | Intel           | 7 Series/C216 Chipset... | 1.7%   | 3.10.34  | 7604BCAC72 |
| 8086:1e3a | 1179:fa30 | Intel           | 7 Series/C216 Chipset... | 3.6%   | 4.1.25   | D7B4BF2642 |
| 8086:1e3a | 1179:fb41 | Intel           | 7 Series/C216 Chipset... | 2.2%   | 3.10.42  | 67009EFFAA |
| 8086:1e3a | 1179:ff1e | Intel           | 7 Series/C216 Chipset... | 0.8%   | 3.14.53  | 43DBEEF737 |
| 8086:1e3a | 144d:c0d7 | Intel           | 7 Series/C216 Chipset... | 1.8%   | 3.14.44  | 8784D98684 |
| 8086:1e3a | 1458:1c3a | Intel           | 7 Series/C216 Chipset... | 0.3%   | 3.10.0   | D7DC793C40 |
| 8086:1e3a | 1462:7733 | Intel           | 7 Series/C216 Chipset... | 25%    | 3.14.44  | BF99082E95 |
| 8086:1e3a | 1462:7751 | Intel           | 7 Series/C216 Chipset... | 4.5%   | 4.15.0   | 7A756F5970 |
| 8086:1e3a | 17aa:21f3 | Intel           | 7 Series/C216 Chipset... | 0.4%   | 3.14.44  | 44F6A1F73B |
| 8086:1e3a | 17aa:21f9 | Intel           | 7 Series/C216 Chipset... | 2.9%   | 3.14.15  | B7014678B5 |
| 8086:1e3a | 17aa:21fa | Intel           | 7 Series/C216 Chipset... | 0.8%   | 3.10.42  | 2EBE6149B7 |
| 8086:1e3a | 17aa:21fb | Intel           | 7 Series/C216 Chipset... | 3.2%   | 4.9.20   | 55427995B5 |
| 8086:1e3a | 17aa:3083 | Intel           | 7 Series/C216 Chipset... | 2.9%   | 4.9.111  | E3BF127788 |
| 8086:1e3a | 17aa:3084 | Intel           | 7 Series/C216 Chipset... | 2%     | 4.15.0   | 47BF9CDBA4 |
| 8086:1e3a | 17aa:3977 | Intel           | 7 Series/C216 Chipset... | 0.5%   | 3.10.0   | B5192BE9BF |
| 8086:1e3a | 1849:1e3a | Intel           | 7 Series/C216 Chipset... | 0.7%   | 3.10.0   | 46D7FB23B0 |
| 8086:1e3a | 1ae0:c000 | Intel           | 7 Series/C216 Chipset... | 37.5%  | 5.4.0    | 2E966E7FBA |
| 8086:1e3a | 8086:1e3a | Intel           | 7 Series/C216 Chipset... | 10.8%  | 3.10.34  | 0EE18BF1AE |
| 8086:1e3a | 8086:2035 | Intel           | 7 Series/C216 Chipset... | 6.2%   | 4.15.0   | DEE8F8ADAA |
| 8086:1e3b | 103c:339a | Intel           | 7 Series/C210 Series ... | 100%   |          | C0F1207DE6 |
| 8086:1e3b | 8086:2037 | Intel           | 7 Series/C210 Series ... | 100%   |          | 34CF8C6B04 |
| 8086:2994 | 103c:2801 | Intel           | 82Q963/Q965 HECI Cont... | 2.3%   | 3.14.53  | 097EABE722 |
| 8086:29b4 | 1028:0211 | Intel           | 82Q35 Express MEI Con... | 0.7%   | 3.14.44  | C1582B3202 |
| 8086:29b4 | 103c:2818 | Intel           | 82Q35 Express MEI Con... | 1.1%   | 4.1.15   | 5F350B471F |
| 8086:29b4 | 103c:2819 | Intel           | 82Q35 Express MEI Con... | 4.2%   | 3.14.25  | 1208F22123 |
| 8086:29b4 | 1043:8295 | Intel           | 82Q35 Express MEI Con... | 4.5%   | 3.14.44  | 0CFC87FCD1 |
| 8086:29d4 | 103c:281e | Intel           | 82Q33 Express MEI Con... | 1.1%   | 3.14.44  | 13EF653132 |
| 8086:29e4 | 108e:5351 | Intel           | 82X38/X48 Express MEI... | 66.7%  | 5.4.18   | E4B76F9137 |
| 8086:2a44 | 103c:30e1 | Intel           | Mobile 4 Series Chips... | 7.7%   | 3.14.25  | C384FE6C1C |
| 8086:2a45 |           | Intel           | Mobile 4 Series Chips... | 100%   |          | 55FB907088 |
| 8086:2e14 | 103c:3034 | Intel           | 4 Series Chipset HECI... | 2.1%   | 3.14.44  | A40772FC80 |
| 8086:2e14 | 103c:3048 | Intel           | 4 Series Chipset HECI... | 1.7%   | 3.10.34  | 97B51B0912 |
| 8086:2e14 | 8086:1003 | Intel           | 4 Series Chipset HECI... | 5.9%   | 4.4.0    | 53C6C139DA |
| 8086:2e44 | 8086:0025 | Intel           | 4 Series Chipset HECI... | 100%   |          | 6F88411BC0 |
| 8086:319a | 1043:1181 | Intel           | Celeron/Pentium Silve... | 13.5%  | 4.15.0   | D594314067 |
| 8086:319a | 1043:1df0 | Intel           | Celeron/Pentium Silve... | 23.5%  | 4.19.177 | 5D4E6E95F1 |
| 8086:319a | 1043:1eb0 | Intel           | Celeron/Pentium Silve... | 8%     | 4.15.0   | 47BF81F534 |
| 8086:319a | 1849:319a | Intel           | Celeron/Pentium Silve... | 2.2%   | 4.15.0   | 54F377B79C |
| 8086:319a | 8086:7270 | Intel           | Celeron/Pentium Silve... | 3.1%   | 4.14.71  | 5F4A9F2DC3 |
| 8086:34a8 | 103c:86ab | Intel           | Ice Lake-LP Serial IO... | 10%    | 5.4.0    | 4019B6C1FF |
| 8086:34a8 | 1043:1ec1 | Intel           | Ice Lake-LP Serial IO... | 2%     | 5.3.0    | 347D45179A |
| 8086:34e0 | 1025:141f | Intel           | Ice Lake-LP Managemen... | 11.1%  | 5.4.0    | AA8934716B |
| 8086:34e0 | 1025:1422 | Intel           | Ice Lake-LP Managemen... | 5.9%   | 5.0.0    | 9C0A212B9F |
| 8086:34e0 | 1028:0979 | Intel           | Ice Lake-LP Managemen... | 2.9%   | 5.0.0    | 7F4CE08DF9 |
| 8086:34e0 | 1028:097a | Intel           | Ice Lake-LP Managemen... | 7.7%   | 5.0.0    | 17D09024B3 |
| 8086:34e0 | 1028:097c | Intel           | Ice Lake-LP Managemen... | 5.3%   | 5.0.0    | 90B19AF55F |
| 8086:34e0 | 103c:85f3 | Intel           | Ice Lake-LP Managemen... | 20%    | 5.4.0    | 0B4A5C33EF |
| 8086:34e0 | 103c:868a | Intel           | Ice Lake-LP Managemen... | 25%    | 5.4.0    | 9F4F9A0186 |
| 8086:34e0 | 103c:86ab | Intel           | Ice Lake-LP Managemen... | 10%    | 5.4.0    | 4019B6C1FF |
| 8086:34e0 | 103c:86c8 | Intel           | Ice Lake-LP Managemen... | 3.2%   | 5.3.0    | 16DBE6C7CF |
| 8086:34e0 | 103c:875b | Intel           | Ice Lake-LP Managemen... | 25%    | 5.4.0    | 63ED12357B |
| 8086:34e0 | 1043:1ec1 | Intel           | Ice Lake-LP Managemen... | 2%     | 5.3.0    | 347D45179A |
| 8086:34e0 | 17aa:3801 | Intel           | Ice Lake-LP Managemen... | 2.1%   | 5.4.0    | 35876A09AD |
| 8086:34e0 | 17aa:3a34 | Intel           | Ice Lake-LP Managemen... | 14.3%  | 5.4.61   | 83B0002691 |
| 8086:34e1 | 1854:0361 | Intel           | Communication controller | 100%   |          | BEA6A28EB1 |
| 8086:34e4 | 1414:0039 | Intel           | Communication controller | 92%    | 5.9.13   | BEEF49F713 |
| 8086:34e4 | 1414:0041 | Intel           | Communication controller | 100%   |          | 79D77CFE11 |
| 8086:38a8 | 8086:7270 | Intel           | LPSS: UART #0            | 100%   |          | 27CC77A565 |
| 8086:38e0 | 8086:7270 | Intel           | ME OEM Extension         | 100%   |          | 27CC77A565 |
| 8086:3b64 | 1028:0438 | Intel           | 5 Series/3400 Series ... | 2.5%   | 4.15.0   | F821A0035B |
| 8086:3b64 | 103c:143a | Intel           | 5 Series/3400 Series ... | 1%     | 3.10.51  | 5D1C9AE554 |
| 8086:3b64 | 103c:1521 | Intel           | 5 Series/3400 Series ... | 18.3%  | 4.1.15   | FFC46C9472 |
| 8086:3b64 | 103c:3674 | Intel           | 5 Series/3400 Series ... | 3.1%   | 3.16.0   | F4DE983D96 |
| 8086:3b64 | 103c:7008 | Intel           | 5 Series/3400 Series ... | 1.3%   | 3.10.34  | 5DD7A5FCE1 |
| 8086:3b64 | 1043:1c77 | Intel           | 5 Series/3400 Series ... | 0.3%   | 3.14.25  | 7FDEE4E7BB |
| 8086:3b64 | 105b:0dd5 | Intel           | 5 Series/3400 Series ... | 14.3%  | 4.1.25   | 6B384CAEA8 |
| 8086:3b64 | 10cf:152b | Intel           | 5 Series/3400 Series ... | 1%     | 3.14.44  | 48FC4FF4DB |
| 8086:43e0 | 1043:8694 | Intel           | Tiger Lake-H Manageme... | 8.3%   | 5.8.0    | CB3058760E |
| 8086:43e0 | 1462:7d09 | Intel           | Tiger Lake-H Manageme... | 16.7%  | 5.8.0    | B2CC4333B0 |
| 8086:43e0 | 1849:43e0 | Intel           | Tiger Lake-H Manageme... | 12.5%  | 5.10.0   | FA71CAC850 |
| 8086:5a9a |           | Intel           | Celeron N3350/Pentium... | 0.8%   | 4.4.0    | D0FEF96A1B |
| 8086:5a9a | 1025:1084 | Intel           | Celeron N3350/Pentium... | 4.3%   | 5.8.0    | 171DAB82C1 |
| 8086:5a9a | 1849:5a9a | Intel           | Celeron N3350/Pentium... | 1.6%   | 4.9.0    | 633A8B8ADF |
| 8086:5a9a | 8086:7270 | Intel           | Celeron N3350/Pentium... | 2.6%   | 4.4.0    | 09F3AC6567 |
| 8086:5a9c |           | Intel           | Communication controller | 100%   |          | 23BDDBF63A |
| 8086:5a9c | 1025:1084 | Intel           | Communication controller | 100%   |          | EB24B13C29 |
| 8086:5a9c | 1028:075f | Intel           | Communication controller | 100%   |          | 516D723C41 |
| 8086:5a9c | 103c:832e | Intel           | Communication controller | 100%   |          | 249738C618 |
| 8086:5a9c | 1043:8738 | Intel           | Communication controller | 100%   |          | 48B82345AB |
| 8086:5a9c | 1297:4045 | Intel           | Communication controller | 100%   |          | 340CD4222F |
| 8086:5a9c | 17aa:3802 | Intel           | Communication controller | 100%   |          | 62D04B32F4 |
| 8086:5a9c | 17aa:3803 | Intel           | Communication controller | 100%   |          | 98851C034C |
| 8086:5a9c | 17aa:3809 | Intel           | Communication controller | 100%   |          | 166EE8D0CF |
| 8086:5a9c | 8086:7270 | Intel           | Communication controller | 100%   |          | E5E9A43E32 |
| 8086:5a9e |           | Intel           | Communication controller | 100%   |          | 23BDDBF63A |
| 8086:5a9e | 1025:1084 | Intel           | Communication controller | 100%   |          | EB24B13C29 |
| 8086:5a9e | 1028:075f | Intel           | Communication controller | 100%   |          | 516D723C41 |
| 8086:5a9e | 103c:832e | Intel           | Communication controller | 100%   |          | 249738C618 |
| 8086:5a9e | 1043:8738 | Intel           | Communication controller | 100%   |          | 48B82345AB |
| 8086:5a9e | 17aa:3802 | Intel           | Communication controller | 100%   |          | 62D04B32F4 |
| 8086:5a9e | 17aa:3803 | Intel           | Communication controller | 100%   |          | 98851C034C |
| 8086:5a9e | 17aa:380a | Intel           | Communication controller | 100%   |          | 166EE8D0CF |
| 8086:5a9e | 8086:7270 | Intel           | Communication controller | 100%   |          | E5E9A43E32 |
| 8086:8c3a | 1028:05a4 | Intel           | 8 Series/C220 Series ... | 0.6%   | 3.10.0   | 541846E7D7 |
| 8086:8c3a | 1028:05cd | Intel           | 8 Series/C220 Series ... | 5%     | 4.15.0   | 95FA029C09 |
| 8086:8c3a | 1028:0612 | Intel           | 8 Series/C220 Series ... | 0.7%   | 4.15.0   | D2ECCACD0C |
| 8086:8c3a | 1028:0620 | Intel           | 8 Series/C220 Series ... | 7.7%   | 4.18.0   | F801FAB1AD |
| 8086:8c3a | 1028:0623 | Intel           | 8 Series/C220 Series ... | 25%    | 5.4.0    | 29D0AD2441 |
| 8086:8c3a | 103c:1825 | Intel           | 8 Series/C220 Series ... | 11.8%  | 3.10.0   | 3B6B80DB46 |
| 8086:8c3a | 103c:18e6 | Intel           | 8 Series/C220 Series ... | 14.3%  | 3.14.44  | CF3ED91B8A |
| 8086:8c3a | 103c:18e7 | Intel           | 8 Series/C220 Series ... | 3.4%   | 4.1.25   | 627983AA9A |
| 8086:8c3a | 103c:2253 | Intel           | 8 Series/C220 Series ... | 2.2%   | 4.19.0   | 191021F74E |
| 8086:8c3a | 103c:2af7 | Intel           | 8 Series/C220 Series ... | 9.5%   | 3.14.44  | E0639EA4A5 |
| 8086:8c3a | 1043:8534 | Intel           | 8 Series/C220 Series ... | 0.2%   | 3.14.25  | F5AC359422 |
| 8086:8c3a | 1458:1c3a | Intel           | 8 Series/C220 Series ... | 0.9%   | 3.10.0   | 9EBB974A64 |
| 8086:8c3a | 1462:7816 | Intel           | 8 Series/C220 Series ... | 12.5%  | 3.10.0   | 8FE013F04A |
| 8086:8c3a | 1462:7818 | Intel           | 8 Series/C220 Series ... | 25%    | 4.15.0   | FF6AA3811C |
| 8086:8c3a | 1462:7823 | Intel           | 8 Series/C220 Series ... | 14.7%  | 3.14.25  | 74F473F9BC |
| 8086:8c3a | 1558:0250 | Intel           | 8 Series/C220 Series ... | 100%   |          | 46B44D2D1F |
| 8086:8c3a | 15d9:0921 | Intel           | 8 Series/C220 Series ... | 33.3%  | 4.15.0   | DB25C87154 |
| 8086:8c3a | 17aa:3097 | Intel           | 8 Series/C220 Series ... | 1.4%   | 4.15.0   | 61976E9745 |
| 8086:8c3a | 17aa:3978 | Intel           | 8 Series/C220 Series ... | 1.8%   | 3.14.44  | 39A9917502 |
| 8086:8c3a | 1849:8c3a | Intel           | 8 Series/C220 Series ... | 0.5%   | 3.10.0   | 7E7AD89D55 |
| 8086:8c3a | 8086:204a | Intel           | 8 Series/C220 Series ... | 3.1%   | 4.1.25   | 8C48173C7B |
| 8086:8c3a | 8086:7270 | Intel           | 8 Series/C220 Series ... | 1.3%   | 4.1.25   | A83290B169 |
| 8086:8c3a | 8086:8c3a | Intel           | 8 Series/C220 Series ... | 10%    | 4.1.13   | B364724E53 |
| 8086:8c3b | 1025:0790 | Intel           | 8 Series/C220 Series ... | 100%   |          | CD73F91550 |
| 8086:8c3b | 15d9:0803 | Intel           | 8 Series/C220 Series ... | 100%   |          | 869444ACF6 |
| 8086:8c3b | 15d9:0842 | Intel           | 8 Series/C220 Series ... | 100%   |          | 290C6ED969 |
| 8086:8c3b | 15d9:086d | Intel           | 8 Series/C220 Series ... | 100%   |          | 9AF20F3BA9 |
| 8086:8c3b | 15d9:0921 | Intel           | 8 Series/C220 Series ... | 100%   |          | 34DBD86F7B |
| 8086:8c3b | 15d9:092d | Intel           | 8 Series/C220 Series ... | 100%   |          | ED9D9F347D |
| 8086:8c3b | 1849:8c3b | Intel           | 8 Series/C220 Series ... | 100%   |          | 9E52EE363E |
| 8086:8c3b | 8086:7270 | Intel           | 8 Series/C220 Series ... | 100%   |          | 14C76E0C83 |
| 8086:8cba | 1043:8534 | Intel           | 9 Series Chipset Fami... | 1.7%   | 3.14.25  | BCBCBDF158 |
| 8086:8cba | 1458:1c3a | Intel           | 9 Series Chipset Fami... | 1.2%   | 3.14.22  | AC8250480A |
| 8086:8cba | 1462:7821 | Intel           | 9 Series Chipset Fami... | 16.7%  | 5.3.0    | ADB163E34B |
| 8086:8cba | 1849:8cba | Intel           | 9 Series Chipset Fami... | 0.7%   | 3.14.44  | 5ACBE289AA |
| 8086:8d3a | 1028:0600 | Intel           | C610/X99 series chips... | 33.3%  | 4.15.0   | 018184F964 |
| 8086:8d3a | 1028:0617 | Intel           | C610/X99 series chips... | 2.7%   | 3.10.0   | 375D6B6557 |
| 8086:8d3a | 103c:2129 | Intel           | C610/X99 series chips... | 11.1%  | 5.3.18   | 449A9223A3 |
| 8086:8d3a | 1043:85f6 | Intel           | C610/X99 series chips... | 12%    | 4.4.0    | 4158CB76EF |
| 8086:8d3a | 1043:8600 | Intel           | C610/X99 series chips... | 2.6%   | 3.10.0   | 6054B96BC5 |
| 8086:8d3a | 1458:7270 | Intel           | C610/X99 series chips... | 3%     | 4.1.15   | 6AFD8A5657 |
| 8086:8d3a | 1462:7885 | Intel           | C610/X99 series chips... | 2.1%   | 4.4.0    | 32D5183912 |
| 8086:8d3a | 15d9:0831 | Intel           | C610/X99 series chips... | 16.7%  | 3.10.0   | 52D5275C7F |
| 8086:8d3a | 15d9:0834 | Intel           | C610/X99 series chips... | 25%    | 3.10.0   | FA4BECDE8B |
| 8086:8d3a | 15d9:0852 | Intel           | C610/X99 series chips... | 33.3%  | 5.4.0    | 2E6D79F345 |
| 8086:8d3a | 15d9:0879 | Intel           | C610/X99 series chips... | 100%   |          | 21124E85CC |
| 8086:8d3a | 19e5:2061 | Intel           | C610/X99 series chips... | 100%   |          | 5EB4DFC951 |
| 8086:8d3a | 8086:35c5 | Intel           | C610/X99 series chips... | 100%   |          | 08100751B7 |
| 8086:8d3a | 8086:35c9 | Intel           | C610/X99 series chips... | 100%   |          | 5F9F099F36 |
| 8086:8d3a | 8086:7270 | Intel           | C610/X99 series chips... | 20%    | 3.10.0   | B2AD449201 |
| 8086:8d3b | 1028:0600 | Intel           | C610/X99 series chips... | 100%   |          | A98D12AD3E |
| 8086:8d3b | 1028:0601 | Intel           | C610/X99 series chips... | 100%   |          | C436F9E67A |
| 8086:8d3b | 1028:061b | Intel           | C610/X99 series chips... | 100%   |          | BCD33A41F0 |
| 8086:8d3b | 1028:0627 | Intel           | C610/X99 series chips... | 100%   |          | 51FB8FEE00 |
| 8086:8d3b | 1028:0639 | Intel           | C610/X99 series chips... | 100%   |          | B39BBB71E2 |
| 8086:8d3b | 1028:063a | Intel           | C610/X99 series chips... | 100%   |          | E4DEE6FAF7 |
| 8086:8d3b | 1028:063b | Intel           | C610/X99 series chips... | 100%   |          | 031D1E0BEC |
| 8086:8d3b | 1043:85f6 | Intel           | C610/X99 series chips... | 100%   |          | 4158CB76EF |
| 8086:8d3b | 1458:1000 | Intel           | C610/X99 series chips... | 100%   |          | 0EA40336C5 |
| 8086:8d3b | 15d9:0821 | Intel           | C610/X99 series chips... | 100%   |          | 17BF7A3CBC |
| 8086:8d3b | 15d9:0824 | Intel           | C610/X99 series chips... | 100%   |          | 6C96E4A591 |
| 8086:8d3b | 15d9:0831 | Intel           | C610/X99 series chips... | 100%   |          | 64918C950D |
| 8086:8d3b | 15d9:0833 | Intel           | C610/X99 series chips... | 100%   |          | 6BAC3401A1 |
| 8086:8d3b | 15d9:0834 | Intel           | C610/X99 series chips... | 100%   |          | 72BAE0BDE8 |
| 8086:8d3b | 15d9:0835 | Intel           | C610/X99 series chips... | 100%   |          | 7479576DA8 |
| 8086:8d3b | 15d9:0852 | Intel           | C610/X99 series chips... | 100%   |          | 8A8EA3FF31 |
| 8086:8d3b | 15d9:0879 | Intel           | C610/X99 series chips... | 100%   |          | 21124E85CC |
| 8086:8d3b | 15d9:0924 | Intel           | C610/X99 series chips... | 100%   |          | 3FC4F3458F |
| 8086:8d3b | 15d9:7270 | Intel           | C610/X99 series chips... | 100%   |          | 5F6D0233A8 |
| 8086:8d3b | 19e5:2061 | Intel           | C610/X99 series chips... | 100%   |          | 5EB4DFC951 |
| 8086:8d3b | 19e5:2062 | Intel           | C610/X99 series chips... | 100%   |          | BA0F3C3B41 |
| 8086:8d3b | 1d49:0a00 | Intel           | C610/X99 series chips... | 100%   |          | 3510DD7B10 |
| 8086:8d3b | 8086:35c5 | Intel           | C610/X99 series chips... | 100%   |          | 08100751B7 |
| 8086:8d3b | 8086:35c8 | Intel           | C610/X99 series chips... | 100%   |          | 574D59E89A |
| 8086:8d3b | 8086:35c9 | Intel           | C610/X99 series chips... | 100%   |          | 5F9F099F36 |
| 8086:8d3b | 8086:35cb | Intel           | C610/X99 series chips... | 100%   |          | CC33C2E194 |
| 8086:8d3b | 8086:7270 | Intel           | C610/X99 series chips... | 100%   |          | 937DE612E9 |
| 8086:8d3b | 8086:8d3b | Intel           | C610/X99 series chips... | 100%   |          | 2903921AEB |
| 8086:98a8 | 144d:c18b | Intel           | LPSS: UART Controller #0 | 100%   |          | 6D40FDC958 |
| 8086:98a9 | 144d:c18b | Intel           | LPSS: UART Controller #1 | 100%   |          | 6D40FDC958 |
| 8086:98e0 | 144d:c18b | Intel           | ME OEM Extension         | 100%   |          | 6D40FDC958 |
| 8086:9c3a | 1025:0775 | Intel           | 8 Series HECI #0         | 0.6%   | 3.14.25  | 81B19839F7 |
| 8086:9c3a | 1025:0918 | Intel           | 8 Series HECI #0         | 3%     | 4.1.19   | F970FF6696 |
| 8086:9c3a | 1025:0940 | Intel           | 8 Series HECI #0         | 100%   |          | C730C15BC5 |
| 8086:9c3a | 1028:05e0 | Intel           | 8 Series HECI #0         | 1.9%   | 4.9.9    | 8EA71BA2AE |
| 8086:9c3a | 1028:05eb | Intel           | 8 Series HECI #0         | 2%     | 3.14.33  | F85FC12BFF |
| 8086:9c3a | 1028:0651 | Intel           | 8 Series HECI #0         | 1.3%   | 3.10.0   | AA72A49A15 |
| 8086:9c3a | 103c:2249 | Intel           | 8 Series HECI #0         | 9.1%   | 4.1.25   | 8DCBD3C2B1 |
| 8086:9c3a | 1043:13bd | Intel           | 8 Series HECI #0         | 25%    | 4.15.0   | 4BABC87322 |
| 8086:9c3a | 17aa:220c | Intel           | 8 Series HECI #0         | 4.7%   | 4.1.15   | 1C6A2F5F81 |
| 8086:9c3a | 17aa:3978 | Intel           | 8 Series HECI #0         | 0.9%   | 3.14.25  | 43B95135E2 |
| 8086:9c3a | 8086:9c3a | Intel           | 8 Series HECI #0         | 4%     | 4.1.15   | 36FA5C5584 |
| 8086:9cba | 1025:0962 | Intel           | Wildcat Point-LP MEI ... | 11.1%  | 4.4.0    | 259BFFF741 |
| 8086:9cba | 1028:0665 | Intel           | Wildcat Point-LP MEI ... | 3.3%   | 4.1.25   | 3F67213F5A |
| 8086:9cba | 1028:0675 | Intel           | Wildcat Point-LP MEI ... | 25%    | 4.1.25   | 30ED2641C4 |
| 8086:9cba | 17aa:382a | Intel           | Wildcat Point-LP MEI ... | 1.1%   | 3.19.0   | 9A767F85C2 |
| 8086:9cba | 17aa:390b | Intel           | Wildcat Point-LP MEI ... | 2.6%   | 4.9.60   | AB6BD693BE |
| 8086:9cba | 19da:b282 | Intel           | Wildcat Point-LP MEI ... | 50%    | 5.4.80   | 2EB3FFC86C |
| 8086:9cba | 8086:7270 | Intel           | Wildcat Point-LP MEI ... | 0.6%   | 4.1.25   | 0F915DEE52 |
| 8086:9cba | 8086:9cba | Intel           | Wildcat Point-LP MEI ... | 2.5%   | 4.4.1    | 3D9C3140AD |
| 8086:9d3a | 1025:1094 | Intel           | Sunrise Point-LP CSME... | 2.6%   | 4.9.9    | E7D6077756 |
| 8086:9d3a | 1025:115f | Intel           | Sunrise Point-LP CSME... | 1.8%   | 3.10.0   | B319F99046 |
| 8086:9d3a | 1028:06de | Intel           | Sunrise Point-LP CSME... | 1.9%   | 4.12.14  | AE7AD1E7D9 |
| 8086:9d3a | 1028:06fd | Intel           | Sunrise Point-LP CSME... | 20%    | 4.15.0   | 98D787F0D4 |
| 8086:9d3a | 1028:075b | Intel           | Sunrise Point-LP CSME... | 4.3%   | 4.4.0    | 014FCD25D4 |
| 8086:9d3a | 1028:0782 | Intel           | Sunrise Point-LP CSME... | 4.2%   | 4.15.0   | 49389100FC |
| 8086:9d3a | 1028:079f | Intel           | Sunrise Point-LP CSME... | 13.3%  | 4.15.0   | D18E59C26A |
| 8086:9d3a | 1028:07a7 | Intel           | Sunrise Point-LP CSME... | 1.5%   | 4.9.76   | D0D56FBB1D |
| 8086:9d3a | 1028:07a8 | Intel           | Sunrise Point-LP CSME... | 7.1%   | 5.3.0    | EBA5E925B8 |
| 8086:9d3a | 1028:07dd | Intel           | Sunrise Point-LP CSME... | 3.7%   | 4.19.0   | A3FD17119A |
| 8086:9d3a | 1028:081b | Intel           | Sunrise Point-LP CSME... | 6.5%   | 3.10.0   | D1454B26C6 |
| 8086:9d3a | 1028:081c | Intel           | Sunrise Point-LP CSME... | 3.3%   | 4.12.14  | CE86510D2B |
| 8086:9d3a | 103c:8079 | Intel           | Sunrise Point-LP CSME... | 3.1%   | 4.4.1    | F1A8589F00 |
| 8086:9d3a | 103c:807c | Intel           | Sunrise Point-LP CSME... | 2.9%   | 4.9.0    | 0DCB414448 |
| 8086:9d3a | 103c:80a4 | Intel           | Sunrise Point-LP CSME... | 5.3%   | 4.9.60   | B01FB51118 |
| 8086:9d3a | 103c:80ff | Intel           | Sunrise Point-LP CSME... | 25.8%  | 4.7.2    | C3ACAEB030 |
| 8086:9d3a | 103c:8100 | Intel           | Sunrise Point-LP CSME... | 6.2%   | 4.15.0   | 2B56F34E21 |
| 8086:9d3a | 103c:8101 | Intel           | Sunrise Point-LP CSME... | 7.4%   | 4.9.60   | BC496704F4 |
| 8086:9d3a | 103c:820c | Intel           | Sunrise Point-LP CSME... | 12.5%  | 4.9.20   | FAE1CD27F3 |
| 8086:9d3a | 103c:832a | Intel           | Sunrise Point-LP CSME... | 0.8%   | 4.9.0    | 6B216F692C |
| 8086:9d3a | 103c:8368 | Intel           | Sunrise Point-LP CSME... | 25%    | 4.18.16  | 2C576FB8A9 |
| 8086:9d3a | 103c:8377 | Intel           | Sunrise Point-LP CSME... | 7.7%   | 4.12.14  | C9A8C10A8F |
| 8086:9d3a | 103c:837d | Intel           | Sunrise Point-LP CSME... | 6%     | 4.9.60   | F343AF14EB |
| 8086:9d3a | 103c:83ba | Intel           | Sunrise Point-LP CSME... | 25%    | 4.19.7   | FE8F29171D |
| 8086:9d3a | 103c:84bf | Intel           | Sunrise Point-LP CSME... | 13.6%  | 4.9.60   | D45FF60CD3 |
| 8086:9d3a | 103c:84de | Intel           | Sunrise Point-LP CSME... | 3.8%   | 3.10.0   | B5E9340D85 |
| 8086:9d3a | 1043:1ac0 | Intel           | Sunrise Point-LP CSME... | 4.3%   | 4.18.0   | 97F52734C2 |
| 8086:9d3a | 1043:1ccd | Intel           | Sunrise Point-LP CSME... | 4.5%   | 4.4.0    | A4B26975E9 |
| 8086:9d3a | 1043:1e30 | Intel           | Sunrise Point-LP CSME... | 11.1%  | 4.15.0   | D3B1CF2698 |
| 8086:9d3a | 1043:8744 | Intel           | Sunrise Point-LP CSME... | 100%   |          | 12D0EDEC81 |
| 8086:9d3a | 1179:f820 | Intel           | Sunrise Point-LP CSME... | 25%    | 4.15.0   | B781D8419A |
| 8086:9d3a | 17aa:2238 | Intel           | Sunrise Point-LP CSME... | 5%     | 3.10.0   | E334D68DA2 |
| 8086:9d3a | 17aa:2245 | Intel           | Sunrise Point-LP CSME... | 1.2%   | 4.9.20   | 751DD3BB74 |
| 8086:9d3a | 17aa:224b | Intel           | Sunrise Point-LP CSME... | 3.3%   | 4.15.0   | DFB9858A8F |
| 8086:9d3a | 17aa:225a | Intel           | Sunrise Point-LP CSME... | 2%     | 4.13.0   | 4826998FDA |
| 8086:9d3a | 17aa:225c | Intel           | Sunrise Point-LP CSME... | 0.9%   | 3.10.0   | 4438A85B31 |
| 8086:9d3a | 17aa:225d | Intel           | Sunrise Point-LP CSME... | 1.8%   | 4.12.14  | 7D7E6AD5D5 |
| 8086:9d3a | 17aa:3801 | Intel           | Sunrise Point-LP CSME... | 0.7%   | 4.9.9    | 412EAC636F |
| 8086:9d3a | 17aa:3808 | Intel           | Sunrise Point-LP CSME... | 1.5%   | 4.9.20   | 9B61CC7F7F |
| 8086:9d3a | 17aa:380c | Intel           | Sunrise Point-LP CSME... | 10%    | 4.9.111  | C3352134E9 |
| 8086:9d3a | 17aa:3819 | Intel           | Sunrise Point-LP CSME... | 7.7%   | 4.9.0    | 1AD9E416A0 |
| 8086:9d3a | 17aa:382d | Intel           | Sunrise Point-LP CSME... | 4.7%   | 4.4.0    | 759E13AFC4 |
| 8086:9d3a | 17aa:384e | Intel           | Sunrise Point-LP CSME... | 1.2%   | 4.9.0    | 71BECA8605 |
| 8086:9d3a | 17aa:5048 | Intel           | Sunrise Point-LP CSME... | 6.5%   | 4.4.0    | 842B139FE7 |
| 8086:9d3a | 17aa:5062 | Intel           | Sunrise Point-LP CSME... | 2.3%   | 4.13.0   | C0B7A3C300 |
| 8086:9d3a | 17aa:506c | Intel           | Sunrise Point-LP CSME... | 12.9%  | 4.15.0   | 4FCC54DDAA |
| 8086:9d3a | 1b0a:228a | Intel           | Sunrise Point-LP CSME... | 50%    | 4.9.155  | 4DEB77EF82 |
| 8086:9d3a | 1b0a:229f | Intel           | Sunrise Point-LP CSME... | 33.3%  | 4.15.0   | B857F2B82D |
| 8086:9d3a | 1d72:1808 | Intel           | Sunrise Point-LP CSME... | 33.3%  | 5.3.0    | 8D36FC215C |
| 8086:9d3a | 8086:1999 | Intel           | Sunrise Point-LP CSME... | 0.9%   | 4.9.155  | B1A55C7D69 |
| 8086:9d3a | 8086:9d3a | Intel           | Sunrise Point-LP CSME... | 2.3%   | 4.9.20   | F8A13F3D37 |
| 8086:9d3e |           | Intel           | Skylake-U/Y CSME: HEC... | 70.6%  | 4.18.7   | EF73590627 |
| 8086:9d3e | 103c:82cb | Intel           | Skylake-U/Y CSME: HEC... | 47.1%  | 5.9.3    | 90E70A0F3E |
| 8086:9da8 | 1043:16f1 | Intel           | Cannon Point-LP Seria... | 4.5%   | 4.18.0   | DBDCCC5696 |
| 8086:9de0 | 1028:089d | Intel           | Cannon Point-LP MEI C... | 7.7%   | 4.15.0   | DAF389F21B |
| 8086:9de0 | 1028:08a8 | Intel           | Cannon Point-LP MEI C... | 6.2%   | 4.15.0   | B6DF9FEC5F |
| 8086:9de0 | 1028:08af | Intel           | Cannon Point-LP MEI C... | 1%     | 4.12.14  | 3D7EEAAA37 |
| 8086:9de0 | 1028:08b8 | Intel           | Cannon Point-LP MEI C... | 2.5%   | 4.19.0   | 241B649AD1 |
| 8086:9de0 | 1028:08bc | Intel           | Cannon Point-LP MEI C... | 9.1%   | 4.15.0   | 5ED5F692A4 |
| 8086:9de0 | 1028:08ca | Intel           | Cannon Point-LP MEI C... | 1.1%   | 4.15.0   | 906A07309D |
| 8086:9de0 | 103c:850c | Intel           | Cannon Point-LP MEI C... | 20%    | 5.3.0    | 3396357637 |
| 8086:9de0 | 103c:856e | Intel           | Cannon Point-LP MEI C... | 7.1%   | 4.19.0   | 2928437EAC |
| 8086:9de0 | 103c:857f | Intel           | Cannon Point-LP MEI C... | 16.7%  | 5.3.0    | A838427772 |
| 8086:9de0 | 1043:16f1 | Intel           | Cannon Point-LP MEI C... | 4.5%   | 4.18.0   | DBDCCC5696 |
| 8086:9de0 | 1558:1325 | Intel           | Cannon Point-LP MEI C... | 4.4%   | 4.18.0   | 7C4E814D03 |
| 8086:9de0 | 17aa:2279 | Intel           | Cannon Point-LP MEI C... | 0.7%   | 3.10.0   | B6F9682F0B |
| 8086:9de0 | 17aa:2286 | Intel           | Cannon Point-LP MEI C... | 1.7%   | 4.18.0   | 12B5E06A49 |
| 8086:9de0 | 8086:2074 | Intel           | Cannon Point-LP MEI C... | 0.6%   | 3.10.0   | 7AB72B120C |
| 8086:9de1 | 8086:7270 | Intel           | Communication controller | 100%   |          | DC14D7EC63 |
| 8086:a0e0 | 1028:0a25 | Intel           | Tiger Lake-LP Managem... | 20%    | 5.4.0    | DCC3B1005E |
| 8086:a0e0 | 1558:14a1 | Intel           | Tiger Lake-LP Managem... | 60%    | 5.6.0    | 4D05114173 |
| 8086:a0e0 | 1558:4018 | Intel           | Tiger Lake-LP Managem... | 25%    | 5.8.0    | F630A726E5 |
| 8086:a0e0 | 1558:51a1 | Intel           | Tiger Lake-LP Managem... | 20%    | 5.8.0    | B3B24987E6 |
| 8086:a0e0 | 17aa:3820 | Intel           | Tiger Lake-LP Managem... | 50%    | 5.10.29  | 89AE55D07E |
| 8086:a0e0 | 8086:3004 | Intel           | Tiger Lake-LP Managem... | 33.3%  | 5.10.0   | 93033ED87E |
| 8086:a0e4 | 103c:8847 | Intel           | Tiger Lake-LP Managem... | 100%   |          | 0B8822B65D |
| 8086:a13a | 1019:9bc9 | Intel           | 100 Series/C230 Serie... | 25%    | 5.3.0    | 744A3F2E54 |
| 8086:a13a | 1019:9c56 | Intel           | 100 Series/C230 Serie... | 20%    | 4.15.0   | 093E3BB0DE |
| 8086:a13a | 1025:1000 | Intel           | 100 Series/C230 Serie... | 8%     | 4.9.41   | 644C742328 |
| 8086:a13a | 1025:108e | Intel           | 100 Series/C230 Serie... | 2.9%   | 4.9.0    | 159AFB32C1 |
| 8086:a13a | 1028:06de | Intel           | 100 Series/C230 Serie... | 13.8%  | 4.15.0   | 568A079F29 |
| 8086:a13a | 1028:06f7 | Intel           | 100 Series/C230 Serie... | 12.5%  | 4.15.0   | E2D11AD2AC |
| 8086:a13a | 1028:0708 | Intel           | 100 Series/C230 Serie... | 20%    | 4.15.0   | F9EE772F9E |
| 8086:a13a | 1028:0763 | Intel           | 100 Series/C230 Serie... | 10.5%  | 5.8.0    | 8C4F2F9922 |
| 8086:a13a | 1028:0764 | Intel           | 100 Series/C230 Serie... | 100%   |          | 530CC43BE2 |
| 8086:a13a | 1028:0798 | Intel           | 100 Series/C230 Serie... | 2.4%   | 4.4.0    | 1D461BB9DB |
| 8086:a13a | 1028:07d0 | Intel           | 100 Series/C230 Serie... | 3.1%   | 4.9.9    | D4927A9F76 |
| 8086:a13a | 103c:825f | Intel           | 100 Series/C230 Serie... | 50%    | 4.15.0   | D7A3E1C5BE |
| 8086:a13a | 103c:8275 | Intel           | 100 Series/C230 Serie... | 16.7%  | 4.15.0   | 46EE3CD25C |
| 8086:a13a | 103c:8392 | Intel           | 100 Series/C230 Serie... | 28.6%  | 4.9.20   | 142D7492C2 |
| 8086:a13a | 1043:1080 | Intel           | 100 Series/C230 Serie... | 5.6%   | 4.15.0   | 5B1076EA3C |
| 8086:a13a | 1043:1bb0 | Intel           | 100 Series/C230 Serie... | 6.7%   | 4.19.0   | 743FF3A2AA |
| 8086:a13a | 1043:1c5d | Intel           | 100 Series/C230 Serie... | 5.9%   | 4.13.0   | 1E5DF72D90 |
| 8086:a13a | 1043:1d6d | Intel           | 100 Series/C230 Serie... | 5.9%   | 5.4.0    | 9D6C0DD372 |
| 8086:a13a | 1043:8694 | Intel           | 100 Series/C230 Serie... | 5%     | 4.4.0    | 53020D69CA |
| 8086:a13a | 1458:1c3a | Intel           | 100 Series/C230 Serie... | 4.8%   | 3.10.0   | C983F79AB8 |
| 8086:a13a | 1462:116e | Intel           | 100 Series/C230 Serie... | 20%    | 5.4.0    | 1C47BC90E4 |
| 8086:a13a | 1462:1190 | Intel           | 100 Series/C230 Serie... | 5.9%   | 4.9.9    | 2B70AAB06F |
| 8086:a13a | 1462:7970 | Intel           | 100 Series/C230 Serie... | 11.1%  | 4.9.20   | AC10EFBB42 |
| 8086:a13a | 1462:7977 | Intel           | 100 Series/C230 Serie... | 11.1%  | 4.9.60   | 877BEE4B1A |
| 8086:a13a | 1462:7982 | Intel           | 100 Series/C230 Serie... | 7.7%   | 4.15.0   | AE97650E7C |
| 8086:a13a | 1462:7984 | Intel           | 100 Series/C230 Serie... | 8.3%   | 4.15.0   | E12A573590 |
| 8086:a13a | 1462:7995 | Intel           | 100 Series/C230 Serie... | 33.3%  | 4.15.0   | 7D25E0B2DD |
| 8086:a13a | 1462:7996 | Intel           | 100 Series/C230 Serie... | 4.4%   | 4.4.0    | 9B9C670167 |
| 8086:a13a | 1462:7998 | Intel           | 100 Series/C230 Serie... | 7.7%   | 4.15.0   | 2E49A21374 |
| 8086:a13a | 1462:7a15 | Intel           | 100 Series/C230 Serie... | 4.1%   | 4.9.60   | CD74218E72 |
| 8086:a13a | 1558:850a | Intel           | 100 Series/C230 Serie... | 2.9%   | 4.9.124  | B02C7CD17E |
| 8086:a13a | 1558:9501 | Intel           | 100 Series/C230 Serie... | 33.3%  | 4.15.0   | ADFE862F36 |
| 8086:a13a | 15d9:0884 | Intel           | 100 Series/C230 Serie... | 50%    | 4.15.7   | BB8832ACBD |
| 8086:a13a | 15d9:0886 | Intel           | 100 Series/C230 Serie... | 100%   |          | 80DC2F8936 |
| 8086:a13a | 1734:121d | Intel           | 100 Series/C230 Serie... | 9.1%   | 3.10.0   | F4612BE4FB |
| 8086:a13a | 17aa:222e | Intel           | 100 Series/C230 Serie... | 1.6%   | 4.4.0    | 356758A7D8 |
| 8086:a13a | 17aa:3802 | Intel           | 100 Series/C230 Serie... | 1.5%   | 4.4.16   | 25576A8571 |
| 8086:a13a | 1849:a13a | Intel           | 100 Series/C230 Serie... | 5.4%   | 4.3.3    | 5F8788EE08 |
| 8086:a13a | 8086:1999 | Intel           | 100 Series/C230 Serie... | 11.9%  | 3.10.0   | 98C12554CB |
| 8086:a13a | 8086:2064 | Intel           | 100 Series/C230 Serie... | 2.9%   | 3.10.0   | 0A01176CBE |
| 8086:a13b | 15d9:0884 | Intel           | 100 Series/C230 Serie... | 50%    | 4.15.7   | BB8832ACBD |
| 8086:a13b | 15d9:0886 | Intel           | 100 Series/C230 Serie... | 100%   |          | 80DC2F8936 |
| 8086:a13b | 8086:1999 | Intel           | 100 Series/C230 Serie... | 60%    | 5.0.0    | 98C12554CB |
| 8086:a1ba | 103c:81c7 | Intel           | C620 Series Chipset F... | 9.1%   | 3.10.0   | 0C434691D6 |
| 8086:a1ba | 1043:871e | Intel           | C620 Series Chipset F... | 6.7%   | 4.15.0   | C934F8E023 |
| 8086:a1ba | 17aa:7808 | Intel           | C620 Series Chipset F... | 38.5%  | 4.15.0   | CEE7ED2CE9 |
| 8086:a1ba | 8086:7270 | Intel           | C620 Series Chipset F... | 13.6%  | 4.9.60   | D4827EB6D9 |
| 8086:a1bb | 1028:0715 | Intel           | C620 Series Chipset F... | 100%   |          | E9A1FC86F9 |
| 8086:a1bb | 1028:0716 | Intel           | C620 Series Chipset F... | 100%   |          | E752263E49 |
| 8086:a1bb | 1028:0718 | Intel           | C620 Series Chipset F... | 100%   |          | 1CCB5D67C2 |
| 8086:a1bb | 1028:0737 | Intel           | C620 Series Chipset F... | 100%   |          | DF9A63BE43 |
| 8086:a1bb | 1028:07cb | Intel           | C620 Series Chipset F... | 100%   |          | 5B9EC879FC |
| 8086:a1bb | 1028:07e5 | Intel           | C620 Series Chipset F... | 100%   |          | 4C88B2E09B |
| 8086:a1bb | 1043:871e | Intel           | C620 Series Chipset F... | 100%   |          | AFAB4598A7 |
| 8086:a1bb | 1458:5001 | Intel           | C620 Series Chipset F... | 100%   |          | 7E93E1B694 |
| 8086:a1bb | 15d9:091c | Intel           | C620 Series Chipset F... | 100%   |          | 748FB8054B |
| 8086:a1bb | 15d9:0941 | Intel           | C620 Series Chipset F... | 100%   |          | C619DB847B |
| 8086:a1bb | 15d9:0953 | Intel           | C620 Series Chipset F... | 100%   |          | 7AD1F5EB4E |
| 8086:a1bb | 15d9:095d | Intel           | C620 Series Chipset F... | 100%   |          | C682299C13 |
| 8086:a1bb | 15d9:0962 | Intel           | C620 Series Chipset F... | 100%   |          | 57460AA45B |
| 8086:a1bb | 15d9:096d | Intel           | C620 Series Chipset F... | 100%   |          | F9D0B2BC99 |
| 8086:a1bb | 15d9:096e | Intel           | C620 Series Chipset F... | 100%   |          | 4D0ED95E02 |
| 8086:a1bb | 15d9:0981 | Intel           | C620 Series Chipset F... | 100%   |          | CD543E37E2 |
| 8086:a1bb | 15d9:0987 | Intel           | C620 Series Chipset F... | 100%   |          | 893E9D69F2 |
| 8086:a1bb | 17aa:7800 | Intel           | C620 Series Chipset F... | 100%   |          | 2AE35CF194 |
| 8086:a1bb | 17aa:7808 | Intel           | C620 Series Chipset F... | 100%   |          | CEE7ED2CE9 |
| 8086:a1bb | 1849:a1bb | Intel           | C620 Series Chipset F... | 100%   |          | 35C171899E |
| 8086:a1bb | 8086:35ce | Intel           | C620 Series Chipset F... | 100%   |          | D373AF93CD |
| 8086:a1bb | 8086:7270 | Intel           | C620 Series Chipset F... | 100%   |          | 20EDFBF60B |
| 8086:a1be | 1028:0715 | Intel           | C620 Series Chipset F... | 100%   |          | E9A1FC86F9 |
| 8086:a1be | 1028:0716 | Intel           | C620 Series Chipset F... | 100%   |          | E752263E49 |
| 8086:a1be | 1028:0718 | Intel           | C620 Series Chipset F... | 100%   |          | 1CCB5D67C2 |
| 8086:a1be | 1028:0737 | Intel           | C620 Series Chipset F... | 100%   |          | DF9A63BE43 |
| 8086:a1be | 1028:07cb | Intel           | C620 Series Chipset F... | 100%   |          | 5B9EC879FC |
| 8086:a1be | 1028:07e5 | Intel           | C620 Series Chipset F... | 100%   |          | 4C88B2E09B |
| 8086:a1be | 1043:871e | Intel           | C620 Series Chipset F... | 100%   |          | AFAB4598A7 |
| 8086:a1be | 1458:5001 | Intel           | C620 Series Chipset F... | 100%   |          | 7E93E1B694 |
| 8086:a1be | 1590:00eb | Intel           | C620 Series Chipset F... | 100%   |          | 3120E02C21 |
| 8086:a1be | 15d9:091c | Intel           | C620 Series Chipset F... | 100%   |          | 748FB8054B |
| 8086:a1be | 15d9:0941 | Intel           | C620 Series Chipset F... | 100%   |          | C619DB847B |
| 8086:a1be | 15d9:0953 | Intel           | C620 Series Chipset F... | 100%   |          | 7AD1F5EB4E |
| 8086:a1be | 15d9:095d | Intel           | C620 Series Chipset F... | 100%   |          | C682299C13 |
| 8086:a1be | 15d9:0962 | Intel           | C620 Series Chipset F... | 100%   |          | 57460AA45B |
| 8086:a1be | 15d9:096d | Intel           | C620 Series Chipset F... | 100%   |          | F9D0B2BC99 |
| 8086:a1be | 15d9:096e | Intel           | C620 Series Chipset F... | 100%   |          | 4D0ED95E02 |
| 8086:a1be | 15d9:0981 | Intel           | C620 Series Chipset F... | 100%   |          | CD543E37E2 |
| 8086:a1be | 15d9:0987 | Intel           | C620 Series Chipset F... | 100%   |          | 893E9D69F2 |
| 8086:a1be | 17aa:7800 | Intel           | C620 Series Chipset F... | 100%   |          | 2AE35CF194 |
| 8086:a1be | 17aa:7808 | Intel           | C620 Series Chipset F... | 100%   |          | CEE7ED2CE9 |
| 8086:a1be | 1849:a1be | Intel           | C620 Series Chipset F... | 100%   |          | 35C171899E |
| 8086:a1be | 8086:35ce | Intel           | C620 Series Chipset F... | 100%   |          | D373AF93CD |
| 8086:a1be | 8086:7270 | Intel           | C620 Series Chipset F... | 100%   |          | 20EDFBF60B |
| 8086:a2ba | 1043:8694 | Intel           | 200 Series PCH CSME H... | 0.7%   | 4.4.0    | 07427B8218 |
| 8086:a2ba | 1043:872f | Intel           | 200 Series PCH CSME H... | 1%     | 4.9.9    | AFF27AE264 |
| 8086:a2ba | 1458:1c3a | Intel           | 200 Series PCH CSME H... | 1.2%   | 3.10.0   | FC6C12EB1D |
| 8086:a2ba | 1462:7a70 | Intel           | 200 Series PCH CSME H... | 1.9%   | 4.15.0   | 81F5ABC79D |
| 8086:a2ba | 1462:7a71 | Intel           | 200 Series PCH CSME H... | 9.5%   | 4.9.9    | 309262E3D6 |
| 8086:a2ba | 1462:7b49 | Intel           | 200 Series PCH CSME H... | 6.2%   | 4.15.0   | 6FDFDD701E |
| 8086:a2ba | 8086:1999 | Intel           | 200 Series PCH CSME H... | 6.7%   | 3.10.0   | 63BC2F7D51 |
| 8086:a328 | 1025:1264 | Intel           | Cannon Lake PCH Seria... | 4%     | 4.15.0   | 89497C0F27 |
| 8086:a328 | 1028:088e | Intel           | Cannon Lake PCH Seria... | 50%    | 4.15.0   | 2A87802C58 |
| 8086:a328 | 1028:0890 | Intel           | Cannon Lake PCH Seria... | 66.7%  | 5.8.0    | 9D14FAEDEF |
| 8086:a328 | 1028:08a1 | Intel           | Cannon Lake PCH Seria... | 20%    | 4.18.0   | AACC137FAA |
| 8086:a328 | 103c:843c | Intel           | Cannon Lake PCH Seria... | 7.1%   | 5.0.0    | E5E15DF58D |
| 8086:a328 | 17aa:225f | Intel           | Cannon Lake PCH Seria... | 2.8%   | 3.10.0   | FFDEE2C6E0 |
| 8086:a328 | 17aa:229b | Intel           | Cannon Lake PCH Seria... | 6.7%   | 5.3.0    | 3F3CC6B9D6 |
| 8086:a328 | 17aa:229f | Intel           | Cannon Lake PCH Seria... | 1.2%   | 5.0.0    | 72F3E05699 |
| 8086:a328 | 17aa:3813 | Intel           | Cannon Lake PCH Seria... | 1.3%   | 4.15.0   | C7793F1DAA |
| 8086:a328 | 1849:a328 | Intel           | Cannon Lake PCH Seria... | 66.7%  | 5.4.0    | B2FAC79AFD |
| 8086:a360 | 1019:a4a5 | Intel           | Cannon Lake PCH HECI ... | 16.7%  | 4.18.16  | 3028547DA1 |
| 8086:a360 | 1025:1264 | Intel           | Cannon Lake PCH HECI ... | 4.7%   | 4.15.0   | 99EE0E5718 |
| 8086:a360 | 1025:126c | Intel           | Cannon Lake PCH HECI ... | 100%   |          | C1339E884A |
| 8086:a360 | 1025:1331 | Intel           | Cannon Lake PCH HECI ... | 0.5%   | 4.15.0   | B4580812C2 |
| 8086:a360 | 1025:1338 | Intel           | Cannon Lake PCH HECI ... | 12.5%  | 5.1.0    | 485080DFF0 |
| 8086:a360 | 1028:0818 | Intel           | Cannon Lake PCH HECI ... | 6.7%   | 4.15.0   | F861E71F84 |
| 8086:a360 | 1028:0825 | Intel           | Cannon Lake PCH HECI ... | 1.8%   | 4.15.0   | C99B5F8C72 |
| 8086:a360 | 1028:0851 | Intel           | Cannon Lake PCH HECI ... | 100%   |          | 05D6B79D2F |
| 8086:a360 | 1028:0868 | Intel           | Cannon Lake PCH HECI ... | 11.1%  | 4.15.0   | C4CBEC5B80 |
| 8086:a360 | 1028:086f | Intel           | Cannon Lake PCH HECI ... | 3%     | 4.15.0   | 4E7076F4F9 |
| 8086:a360 | 1028:0877 | Intel           | Cannon Lake PCH HECI ... | 8.7%   | 4.15.0   | 3FBDBB7E9C |
| 8086:a360 | 1028:087c | Intel           | Cannon Lake PCH HECI ... | 0.7%   | 4.15.0   | 7B17868903 |
| 8086:a360 | 1028:088e | Intel           | Cannon Lake PCH HECI ... | 50%    | 4.15.0   | 2A87802C58 |
| 8086:a360 | 1028:0890 | Intel           | Cannon Lake PCH HECI ... | 66.7%  | 5.8.0    | 9D14FAEDEF |
| 8086:a360 | 1028:0905 | Intel           | Cannon Lake PCH HECI ... | 1.3%   | 4.15.0   | 293A792A22 |
| 8086:a360 | 1028:0919 | Intel           | Cannon Lake PCH HECI ... | 7.1%   | 4.15.0   | BCEEEC9520 |
| 8086:a360 | 1028:0930 | Intel           | Cannon Lake PCH HECI ... | 8.3%   | 4.15.0   | C2BF735906 |
| 8086:a360 | 103c:843c | Intel           | Cannon Lake PCH HECI ... | 7.1%   | 5.0.0    | E5E15DF58D |
| 8086:a360 | 103c:844c | Intel           | Cannon Lake PCH HECI ... | 25%    | 5.4.0    | 29F7CF64CE |
| 8086:a360 | 103c:8467 | Intel           | Cannon Lake PCH HECI ... | 33.3%  | 5.4.0    | D20F245092 |
| 8086:a360 | 103c:8478 | Intel           | Cannon Lake PCH HECI ... | 1.3%   | 4.15.0   | 2AF0A44C72 |
| 8086:a360 | 103c:84db | Intel           | Cannon Lake PCH HECI ... | 8.3%   | 4.15.0   | 06EE78EE4D |
| 8086:a360 | 103c:8575 | Intel           | Cannon Lake PCH HECI ... | 9.5%   | 5.0.0    | 1BDD227B6F |
| 8086:a360 | 103c:85a2 | Intel           | Cannon Lake PCH HECI ... | 25%    | 3.10.0   | 5D24D101B0 |
| 8086:a360 | 103c:860f | Intel           | Cannon Lake PCH HECI ... | 6.2%   | 4.18.0   | BDD15B19B1 |
| 8086:a360 | 1043:1041 | Intel           | Cannon Lake PCH HECI ... | 6.2%   | 4.19.1   | F38CA9409C |
| 8086:a360 | 1043:8694 | Intel           | Cannon Lake PCH HECI ... | 2.5%   | 3.10.0   | 8260769B47 |
| 8086:a360 | 1458:1c3a | Intel           | Cannon Lake PCH HECI ... | 4.8%   | 4.12.14  | 7D89BC19FD |
| 8086:a360 | 1462:1222 | Intel           | Cannon Lake PCH HECI ... | 7.7%   | 4.15.0   | 105C3ABAEB |
| 8086:a360 | 1462:126a | Intel           | Cannon Lake PCH HECI ... | 15.4%  | 5.4.0    | 3CEF0087AA |
| 8086:a360 | 1462:7b18 | Intel           | Cannon Lake PCH HECI ... | 14.3%  | 5.0.0    | 77B2CCC8F7 |
| 8086:a360 | 1462:7b23 | Intel           | Cannon Lake PCH HECI ... | 16.7%  | 4.18.0   | 37076CEBE8 |
| 8086:a360 | 1462:7b33 | Intel           | Cannon Lake PCH HECI ... | 5.3%   | 4.15.0   | F08CE9BD47 |
| 8086:a360 | 1462:7b98 | Intel           | Cannon Lake PCH HECI ... | 5.8%   | 4.15.0   | EA7A52FDAC |
| 8086:a360 | 1558:67c1 | Intel           | Cannon Lake PCH HECI ... | 16.7%  | 5.4.0    | 6A8C040FBB |
| 8086:a360 | 1558:8562 | Intel           | Cannon Lake PCH HECI ... | 4.3%   | 5.3.8    | 810C56667D |
| 8086:a360 | 1558:95e6 | Intel           | Cannon Lake PCH HECI ... | 6.1%   | 4.15.0   | 1035C22955 |
| 8086:a360 | 17aa:225f | Intel           | Cannon Lake PCH HECI ... | 11.1%  | 4.15.0   | FFDEE2C6E0 |
| 8086:a360 | 17aa:2267 | Intel           | Cannon Lake PCH HECI ... | 1.6%   | 4.19.11  | AAB68A3B33 |
| 8086:a360 | 17aa:2297 | Intel           | Cannon Lake PCH HECI ... | 1.8%   | 4.18.0   | 8376F889C2 |
| 8086:a360 | 17aa:229b | Intel           | Cannon Lake PCH HECI ... | 6.7%   | 5.3.0    | 3F3CC6B9D6 |
| 8086:a360 | 17aa:229f | Intel           | Cannon Lake PCH HECI ... | 1.2%   | 5.0.0    | 72F3E05699 |
| 8086:a360 | 17aa:3135 | Intel           | Cannon Lake PCH HECI ... | 14.3%  | 4.15.0   | AA1BE9CBEC |
| 8086:a360 | 17aa:3136 | Intel           | Cannon Lake PCH HECI ... | 20%    | 5.0.0    | 02ECA27578 |
| 8086:a360 | 17aa:36e7 | Intel           | Cannon Lake PCH HECI ... | 25%    | 4.15.0   | 1B722DF896 |
| 8086:a360 | 17aa:3810 | Intel           | Cannon Lake PCH HECI ... | 2.6%   | 4.15.0   | C7793F1DAA |
| 8086:a360 | 1849:a360 | Intel           | Cannon Lake PCH HECI ... | 6.8%   | 4.14.222 | 06EB8AFDBC |
| 8086:a360 | 8086:7270 | Intel           | Cannon Lake PCH HECI ... | 0.7%   | 4.15.0   | 4F08E906CA |
| 8086:a361 | 15d9:1a1b | Intel           | 300 Series Chipset HE... | 100%   |          | 16D1B33F25 |
| 8086:a361 | 15d9:1b0f | Intel           | 300 Series Chipset HE... | 100%   |          | D9DA751F0F |
| 8086:a361 | 1849:a361 | Intel           | 300 Series Chipset HE... | 100%   |          | C6E1FF1BED |
| 8086:a361 | 8086:7270 | Intel           | 300 Series Chipset HE... | 100%   |          | 91F3DB65A8 |
| 8086:a364 | 1028:088e | Intel           | Cannon Lake PCH HECI ... | 50%    | 4.15.0   | 2A87802C58 |
| 8086:a364 | 1028:0890 | Intel           | Cannon Lake PCH HECI ... | 66.7%  | 5.8.0    | 9D14FAEDEF |
| 8086:a364 | 1849:a364 | Intel           | Cannon Lake PCH HECI ... | 80%    | 5.4.0    | B2FAC79AFD |
| 8086:a3ba | 1043:8694 | Intel           | Comet Lake PCH-V Mana... | 9.8%   | 4.19.0   | 062FE68B97 |
| 8086:a3ba | 1458:1c3a | Intel           | Comet Lake PCH-V Mana... | 2.6%   | 5.4.0    | ABD511B277 |
| 8086:a3ba | 17aa:317e | Intel           | Comet Lake PCH-V Mana... | 25%    | 5.8.0    | 2CE2A68735 |
| 9710:9900 | a000:2000 | MosChip Semi... | MCS9900 Multi-I/O Con... | 100%   |          | 7D609B3954 |

### Firewire controller (PCI)

38 out of 1000 (3.80%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 004c:8024 |           |                 | FireWire (IEEE 1394)     | 100%   |          | 5837B78F0C |
| 0180:0832 | 003c:30d6 |                 | FireWire (IEEE 1394)     | 100%   |          | 4BDD603282 |
| 01c1:5811 | 0043:8294 |                 | FireWire (IEEE 1394)     | 100%   |          | 44D8BC1D36 |
| 104c:8023 | 108e:5351 | Texas Instru... | TSB43AB22A IEEE-1394a... | 66.7%  | 5.4.18   | E4B76F9137 |
| 104c:8023 | 1297:5106 | Texas Instru... | TSB43AB22A IEEE-1394a... | 14.3%  | 4.12.14  | 35D850590E |
| 104c:8024 | 1458:1000 | Texas Instru... | TSB43AB23 IEEE-1394a-... | 0.1%   | 3.10.0   | 45142A6931 |
| 104c:8024 | 9005:0030 | Texas Instru... | TSB43AB23 IEEE-1394a-... | 25%    | 4.19.57  | D506D4320D |
| 104c:823f |           | Texas Instru... | XIO2213A/B/XIO2221 IE... | 1.2%   | 3.14.44  | E6CC5FBF7F |
| 1102:4001 | 1102:0010 | Creative Labs   | SB Audigy FireWire Port  | 1.1%   | 3.10.0   | 2A34C16AB3 |
| 1106:3044 | 1043:81fe | VIA Technolo... | VT6306/7/8 [Fire II(M... | 0.3%   | 3.0.28   | 35233C6000 |
| 1106:3044 | 1106:3044 | VIA Technolo... | VT6306/7/8 [Fire II(M... | 0.8%   | 3.0.69   | 7EEB446AEE |
| 1106:3044 | 1458:1000 | VIA Technolo... | VT6306/7/8 [Fire II(M... | 0.2%   | 3.14.33  | 746ED0F095 |
| 1106:3044 | 5b10:060c | VIA Technolo... | VT6306/7/8 [Fire II(M... | 100%   |          | A3DF896B35 |
| 1106:3403 | 1025:0158 | VIA Technolo... | VT6315 Series Firewir... | 12.5%  | 4.9.95   | F558E48348 |
| 1106:3403 | 1025:0251 | VIA Technolo... | VT6315 Series Firewir... | 14.3%  | 4.18.0   | DFD78F1056 |
| 1106:3403 | 1043:8384 | VIA Technolo... | VT6315 Series Firewir... | 0.2%   | 3.10.0   | 17ACFC90D4 |
| 1106:3403 | 1106:3403 | VIA Technolo... | VT6315 Series Firewir... | 1.4%   | 3.14.22  | 24CFA19EA6 |
| 1106:3403 | 1849:3403 | VIA Technolo... | VT6315 Series Firewir... | 1.4%   | 3.14.44  | C9529F922D |
| 1180:0832 | 1028:0263 | Ricoh           | R5C832 IEEE 1394 Cont... | 5.1%   | 4.12.14  | A8E17B79CE |
| 1180:0832 | 103c:30db | Ricoh           | R5C832 IEEE 1394 Cont... | 3.2%   | 3.10.0   | B5FBFCF0A5 |
| 1180:0832 | 103c:7008 | Ricoh           | R5C832 IEEE 1394 Cont... | 4.4%   | 3.10.34  | 5DD7A5FCE1 |
| 1180:0832 | 17aa:20c7 | Ricoh           | R5C832 IEEE 1394 Cont... | 0.5%   | 3.10.19  | 28EA2CFCFB |
| 1180:e832 | 1028:040b | Ricoh           | R5C832 PCIe IEEE 1394... | 3.4%   | 3.14.44  | BC65564608 |
| 1180:e832 | 1028:040c | Ricoh           | R5C832 PCIe IEEE 1394... | 4.2%   | 4.9.60   | 919212E67C |
| 1180:e832 | 104d:9089 | Ricoh           | R5C832 PCIe IEEE 1394... | 3%     | 4.1.25   | 44A563D6DB |
| 1180:e832 | 17aa:2136 | Ricoh           | R5C832 PCIe IEEE 1394... | 0.3%   | 3.14.44  | 576FA34B0C |
| 1180:e832 | 17aa:21ce | Ricoh           | R5C832 PCIe IEEE 1394... | 2.2%   | 3.14.25  | 8BDBED7F50 |
| 1180:e832 | 17aa:21cf | Ricoh           | R5C832 PCIe IEEE 1394... | 2.3%   | 3.10.0   | 4CAE7DC78D |
| 11c1:5811 | 103c:130a | LSI             | FW322/323 [TrueFire] ... | 3.7%   | 4.9.60   | 4EF026497F |
| 11c1:5811 | 103c:130b | LSI             | FW322/323 [TrueFire] ... | 6.2%   | 3.10.0   | A1B7A080A8 |
| 11c1:5811 | 103c:158b | LSI             | FW322/323 [TrueFire] ... | 3.7%   | 4.15.0   | 6BC73950DD |
| 11c1:5901 | 11c1:5900 | LSI             | FW643 [TrueFire] PCIe... | 1%     | 3.14.44  | 8A0C5BE794 |
| 1217:00f7 | 1217:00f7 | O2 Micro        | Firewire (IEEE 1394)     | 1.2%   | 3.13.0   | B851103D78 |
| 1217:13f7 | 1028:053e | O2 Micro        | 1394 OHCI Compliant H... | 3.4%   | 4.9.124  | F674F91052 |
| 197b:2380 | 103c:161c | JMicron Tech... | IEEE 1394 Host Contro... | 3.5%   | 4.1.15   | E33B92BBF1 |
| 197b:2380 | 103c:17a7 | JMicron Tech... | IEEE 1394 Host Contro... | 1.8%   | 3.14.44  | 261BB9DE80 |
| 197b:2380 | 1462:522d | JMicron Tech... | IEEE 1394 Host Contro... | 16%    | 4.1.16   | 1FBA25DBCF |
| 197b:2380 | 197b:2380 | JMicron Tech... | IEEE 1394 Host Contro... | 2.2%   | 4.1.19   | 95AF098C68 |

### Flash memory (PCI)

42 out of 77 (54.55%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1524:0500 | 1524:0500 | ENE Technology  | FLASH memory             | 100%   |          | 1312407631 |
| 1524:0520 | 1025:007a | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | E4219525B9 |
| 1524:0520 | 1025:007f | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | 14C016A2F9 |
| 1524:0520 | 1025:0081 | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | 0C32C44824 |
| 1524:0520 | 1025:0090 | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | 4A0EE2EAA5 |
| 1524:0520 | 1025:009f | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | A009C7E619 |
| 1524:0520 | 1025:010f | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | A9D5FB836A |
| 1524:0520 | 1179:ff01 | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | 89C7F0F25E |
| 1524:0520 | 1179:ff10 | ENE Technology  | FLASH memory: ENE Tec... | 100%   |          | 4375F8C26E |
| 1524:0530 | 1025:007a | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | E4219525B9 |
| 1524:0530 | 1025:007f | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 14C016A2F9 |
| 1524:0530 | 1025:0081 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 0C32C44824 |
| 1524:0530 | 1025:0090 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 4A0EE2EAA5 |
| 1524:0530 | 1025:009f | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | A009C7E619 |
| 1524:0530 | 1025:010f | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | A9D5FB836A |
| 1524:0530 | 1179:ff01 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 89C7F0F25E |
| 1524:0530 | 1179:ff10 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 4375F8C26E |
| 1524:0530 | 14c0:0020 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | D1D8A50709 |
| 1524:0530 | 1558:5401 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 8CF7873695 |
| 1524:0530 | 1734:10c1 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 37D02AD16C |
| 1524:0530 | 1734:10d7 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | CA3AC06D30 |
| 1524:0530 | 17aa:2079 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | EDAE63A429 |
| 1524:0720 | 1025:011b | ENE Technology  | Memory Stick Card Rea... | 100%   |          | CD287A7C40 |
| 1524:0720 | 1025:012a | ENE Technology  | Memory Stick Card Rea... | 100%   |          | C95503E7D2 |
| 1524:0720 | 1025:012e | ENE Technology  | Memory Stick Card Rea... | 100%   |          | 6EAAA7BA4F |
| 1524:0720 | 1462:2fb3 | ENE Technology  | Memory Stick Card Rea... | 100%   |          | 5604F2B979 |
| 1524:0720 | 1462:2fbd | ENE Technology  | Memory Stick Card Rea... | 100%   |          | 6502446C70 |
| 1524:0730 | 1025:011b | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | CD287A7C40 |
| 1524:0730 | 1025:012a | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | C95503E7D2 |
| 1524:0730 | 1025:012e | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 6EAAA7BA4F |
| 1524:0730 | 1462:2fb3 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 5604F2B979 |
| 1524:0730 | 1462:2fbd | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 6502446C70 |
| 1524:0730 | 1558:0573 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 95780C2963 |
| 1524:0730 | 1558:0664 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 51E2E84C28 |
| 1524:0730 | 1558:0668 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 41C9811E8B |
| 1524:0730 | 1558:0669 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 66E0793D5B |
| 1524:0730 | 1558:0721 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 4F4A5860A1 |
| 1524:0730 | 1558:0722 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 019E901528 |
| 1524:0730 | 1558:0801 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | BF5F7A5F0A |
| 1524:0730 | 1558:0802 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 44B42FE693 |
| 1524:0730 | 1558:5408 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 01A8AC7CD9 |
| 1524:0730 | 1558:5409 | ENE Technology  | ENE PCI Memory Stick ... | 100%   |          | 00EBCAC258 |

### Graphics card (PCI)

1379 out of 16902 (8.16%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1002:0000 | 17aa:210f | AMD             | VGA compatible contro... | 100%   |          | 7FE76B1B56 |
| 1002:130f | 1849:130f | AMD             | Kaveri [Radeon R7 Gra... | 2.6%   | 3.14.44  | 50841878AE |
| 1002:15d8 | 1002:15d8 | AMD             | Picasso                  | 18%    | 4.18.0   | B246B730F4 |
| 1002:15d8 | 1025:134d | AMD             | Picasso                  | 2.4%   | 5.0.0    | 129A6CF35E |
| 1002:15d8 | 1025:134f | AMD             | Picasso                  | 3.6%   | 5.0.0    | 7721B3FB75 |
| 1002:15d8 | 1025:1456 | AMD             | Picasso                  | 15.4%  | 5.4.0    | 704EC3D66E |
| 1002:15d8 | 103c:85ad | AMD             | Picasso                  | 9.1%   | 5.3.0    | 0D375562BD |
| 1002:15d8 | 103c:85b3 | AMD             | Picasso                  | 7.9%   | 5.0.0    | 89171F1740 |
| 1002:15d8 | 103c:85de | AMD             | Picasso                  | 8.7%   | 5.3.0    | 5DC28F54DD |
| 1002:15d8 | 103c:85ea | AMD             | Picasso                  | 7.1%   | 5.0.0    | 216EB4AF67 |
| 1002:15d8 | 103c:8615 | AMD             | Picasso                  | 3.6%   | 5.0.0    | 7BB8688560 |
| 1002:15d8 | 1043:1821 | AMD             | Picasso                  | 1.2%   | 4.18.0   | 7877A13441 |
| 1002:15d8 | 1043:1831 | AMD             | Picasso                  | 9.5%   | 5.3.0    | F1B9FA59EC |
| 1002:15d8 | 1043:18f1 | AMD             | Picasso                  | 4.2%   | 5.0.0    | 9C797156F9 |
| 1002:15d8 | 1043:876b | AMD             | Picasso                  | 7.1%   | 5.0.0    | F8E204686B |
| 1002:15d8 | 1458:d000 | AMD             | Picasso                  | 11%    | 5.4.0    | 535EA77E4F |
| 1002:15d8 | 1462:7a36 | AMD             | Picasso                  | 16.7%  | 5.3.0    | 70DFCAA6EB |
| 1002:15d8 | 1462:7a40 | AMD             | Picasso                  | 25%    | 5.8.0    | 537F3F8973 |
| 1002:15d8 | 1462:7b87 | AMD             | Picasso                  | 33.3%  | 5.3.11   | 5BCFE2F1CE |
| 1002:15d8 | 1462:7c02 | AMD             | Picasso                  | 7.7%   | 5.4.19   | 893228F4E6 |
| 1002:15d8 | 17aa:3181 | AMD             | Picasso                  | 100%   |          | A203CD8C57 |
| 1002:15d8 | 17aa:3703 | AMD             | Picasso                  | 100%   |          | 91A80D30D0 |
| 1002:15d8 | 17aa:3801 | AMD             | Picasso                  | 4.2%   | 4.19.97  | 7B350A4E79 |
| 1002:15d8 | 17aa:3802 | AMD             | Picasso                  | 4.4%   | 5.0.0    | 33326221E5 |
| 1002:15d8 | 17aa:3805 | AMD             | Picasso                  | 3.6%   | 5.4.0    | 166932E73B |
| 1002:15d8 | 17aa:3808 | AMD             | Picasso                  | 1.1%   | 5.0.0    | 74AB3EBC38 |
| 1002:15d8 | 17aa:5124 | AMD             | Picasso                  | 2.4%   | 4.18.0   | 7B7D62D2A5 |
| 1002:15d8 | 17aa:5125 | AMD             | Picasso                  | 2.4%   | 5.1.17   | BCF2604C43 |
| 1002:15d8 | 17aa:5126 | AMD             | Picasso                  | 4.5%   | 5.0.0    | 44939F005D |
| 1002:15d8 | 19e5:3e0d | AMD             | Picasso                  | 5%     | 5.4.0    | 9F6E79326E |
| 1002:15d8 | 19e5:3e18 | AMD             | Picasso                  | 6.3%   | 5.3.0    | 8956498C75 |
| 1002:15d8 | 1d05:1077 | AMD             | Picasso                  | 5.9%   | 5.4.0    | 4261DD36B1 |
| 1002:15dd | 1002:15dd | AMD             | Raven Ridge [Radeon V... | 2.6%   | 4.12.14  | 05F64AFE14 |
| 1002:15dd | 1028:0812 | AMD             | Raven Ridge [Radeon V... | 15.8%  | 4.18.0   | 1AB4C930EA |
| 1002:15dd | 1028:0884 | AMD             | Raven Ridge [Radeon V... | 4.5%   | 4.18.0   | 3208C17FB3 |
| 1002:15dd | 103c:8434 | AMD             | Raven Ridge [Radeon V... | 25%    | 4.18.0   | E30D68CA01 |
| 1002:15dd | 1043:876b | AMD             | Raven Ridge [Radeon V... | 4.7%   | 4.12.14  | 2A000E48F4 |
| 1002:15dd | 1458:d000 | AMD             | Raven Ridge [Radeon V... | 4.8%   | 3.10.0   | AF4B00F5C3 |
| 1002:15dd | 1462:7a36 | AMD             | Raven Ridge [Radeon V... | 12.5%  | 4.15.0   | 41871808C5 |
| 1002:15dd | 1462:7c02 | AMD             | Raven Ridge [Radeon V... | 6.2%   | 4.15.0   | AD51164983 |
| 1002:15dd | 17aa:36f5 | AMD             | Raven Ridge [Radeon V... | 60%    | 5.5.9    | 7E41940C9C |
| 1002:15dd | 17aa:3801 | AMD             | Raven Ridge [Radeon V... | 1.8%   | 4.15.0   | 2BE2E8C008 |
| 1002:15dd | 17aa:38ef | AMD             | Raven Ridge [Radeon V... | 2.3%   | 4.15.0   | F545576AE9 |
| 1002:1636 | 1002:1636 | AMD             | Renoir                   | 15%    | 5.8.0    | C076095AFB |
| 1002:1636 | 1025:142b | AMD             | Renoir                   | 28.3%  | 5.4.0    | F28C9E243E |
| 1002:1636 | 1025:1461 | AMD             | Renoir                   | 13.2%  | 5.4.0    | 4252D3A477 |
| 1002:1636 | 1028:09f5 | AMD             | Renoir                   | 11.8%  | 5.7.10   | 9D7D4C771B |
| 1002:1636 | 1028:0a1d | AMD             | Renoir                   | 16.7%  | 5.8.0    | 1B291891F4 |
| 1002:1636 | 103c:86ee | AMD             | Renoir                   | 100%   |          | 8579540A18 |
| 1002:1636 | 103c:8730 | AMD             | Renoir                   | 21.5%  | 5.6.14   | 6558DFD5FD |
| 1002:1636 | 103c:8760 | AMD             | Renoir                   | 15.2%  | 5.8.0    | 630337CDE7 |
| 1002:1636 | 103c:876b | AMD             | Renoir                   | 50%    | 5.10.0   | 4149FBF824 |
| 1002:1636 | 103c:876e | AMD             | Renoir                   | 15.5%  | 5.6.15   | 3B48BB4088 |
| 1002:1636 | 103c:876f | AMD             | Renoir                   | 24.4%  | 5.4.0    | FBB923829D |
| 1002:1636 | 103c:8787 | AMD             | Renoir                   | 20%    | 5.8.0    | 548218334C |
| 1002:1636 | 103c:879c | AMD             | Renoir                   | 50%    | 5.8.0    | D8CD629070 |
| 1002:1636 | 103c:87a9 | AMD             | Renoir                   | 40%    | 5.7.2    | F50C02BA9F |
| 1002:1636 | 103c:87b0 | AMD             | Renoir                   | 20%    | 5.8.0    | 05BA81A5EE |
| 1002:1636 | 103c:87b2 | AMD             | Renoir                   | 6.7%   | 5.8.0    | 830C1ED47A |
| 1002:1636 | 103c:87b3 | AMD             | Renoir                   | 16.7%  | 5.8.0    | 6B3DB58438 |
| 1002:1636 | 103c:87cf | AMD             | Renoir                   | 42.9%  | 5.8.0    | 1E8FA91D17 |
| 1002:1636 | 103c:87d0 | AMD             | Renoir                   | 100%   |          | EE4105DF76 |
| 1002:1636 | 103c:87d6 | AMD             | Renoir                   | 40%    | 5.8.0    | 3DA6075B7E |
| 1002:1636 | 103c:8830 | AMD             | Renoir                   | 50%    | 5.8.18   | 4CC6403330 |
| 1002:1636 | 1043:1092 | AMD             | Renoir                   | 33.3%  | 5.10.21  | A3846DB026 |
| 1002:1636 | 1043:1272 | AMD             | Renoir                   | 25%    | 5.4.0    | 47D5B5246F |
| 1002:1636 | 1043:16cf | AMD             | Renoir                   | 15%    | 5.6.0    | 66520B695A |
| 1002:1636 | 1043:16df | AMD             | Renoir                   | 20%    | 5.6.16   | 4657A3E758 |
| 1002:1636 | 1043:16ef | AMD             | Renoir                   | 8.3%   | 5.8.0    | 00373C3EE0 |
| 1002:1636 | 1043:16ff | AMD             | Renoir                   | 22.2%  | 5.6.0    | 08AD28F052 |
| 1002:1636 | 1043:18bf | AMD             | Renoir                   | 20%    | 5.8.5    | 2AAD520134 |
| 1002:1636 | 1043:1e21 | AMD             | Renoir                   | 18.2%  | 5.7.1    | B10D744C6C |
| 1002:1636 | 1043:1f11 | AMD             | Renoir                   | 7.9%   | 5.6.15   | 7FE15CAABF |
| 1002:1636 | 1043:87e1 | AMD             | Renoir                   | 21.4%  | 4.18.0   | 097E77345E |
| 1002:1636 | 1043:87e7 | AMD             | Renoir                   | 29.4%  | 4.18.0   | FCCCC894CA |
| 1002:1636 | 1458:d000 | AMD             | Renoir                   | 4.5%   | 5.8.0    | AC0F996928 |
| 1002:1636 | 1462:12b5 | AMD             | Renoir                   | 38.5%  | 5.8.0    | 08ED0821EF |
| 1002:1636 | 1462:12c8 | AMD             | Renoir                   | 20%    | 5.8.0    | EC110AE347 |
| 1002:1636 | 1558:a500 | AMD             | Renoir                   | 9.1%   | 5.4.0    | 7CAC175BDE |
| 1002:1636 | 17aa:371c | AMD             | Renoir                   | 100%   |          | 65195D0D22 |
| 1002:1636 | 17aa:380d | AMD             | Renoir                   | 10.5%  | 5.4.0    | 406B41E802 |
| 1002:1636 | 17aa:3813 | AMD             | Renoir                   | 1.7%   | 5.4.0    | 8BC1A4D8B0 |
| 1002:1636 | 17aa:381b | AMD             | Renoir                   | 15.6%  | 5.8.0    | F6C13F6EDE |
| 1002:1636 | 17aa:381c | AMD             | Renoir                   | 66.7%  | 5.7.0    | DB1626E471 |
| 1002:1636 | 17aa:3a3f | AMD             | Renoir                   | 12.9%  | 5.7.1    | 9B23B69040 |
| 1002:1636 | 17aa:3a44 | AMD             | Renoir                   | 10%    | 5.8.0    | 96374442C4 |
| 1002:1636 | 17aa:3a45 | AMD             | Renoir                   | 20%    | 5.8.0    | 4B69E8576C |
| 1002:1636 | 17aa:3f1a | AMD             | Renoir                   | 11%    | 5.6.0    | 0341D8D38D |
| 1002:1636 | 17aa:507e | AMD             | Renoir                   | 10.5%  | 5.7.0    | E19A3D01B0 |
| 1002:1636 | 17aa:507f | AMD             | Renoir                   | 12%    | 4.18.0   | 41B0173874 |
| 1002:1636 | 17aa:5081 | AMD             | Renoir                   | 3.3%   | 5.6.0    | 2BF29467E9 |
| 1002:1636 | 17aa:5082 | AMD             | Renoir                   | 9.3%   | 5.4.0    | DF1E1E308B |
| 1002:1636 | 1d05:109f | AMD             | Renoir                   | 8.3%   | 5.6.0    | E651CCB88E |
| 1002:1636 | 1d72:1951 | AMD             | Renoir                   | 25%    | 5.7.0    | E5AAA54863 |
| 1002:1636 | 1d72:1953 | AMD             | Renoir                   | 25%    | 5.7.0    | A52786C26A |
| 1002:1636 | 1e83:3e33 | AMD             | Renoir                   | 4.3%   | 5.8.0    | 7E3892E9B1 |
| 1002:1638 | 1043:128c | AMD             | Cezanne                  | 100%   |          | 6D5882D39F |
| 1002:1638 | 1043:16a2 | AMD             | Cezanne                  | 100%   |          | 1BFCB72AF7 |
| 1002:164c | 17aa:3801 | AMD             | Lucienne                 | 50%    | 5.8.0    | 933D526A12 |
| 1002:164c | 17aa:3f96 | AMD             | Lucienne                 | 33.3%  | 5.11.0   | 47AEF26EC8 |
| 1002:4150 | 1043:005e | AMD             | RV350 [Radeon 9550/96... | 100%   |          | A3DF896B35 |
| 1002:4354 |           | AMD             | 215CT [Mach64 CT PCI]    | 100%   |          | C0709972A2 |
| 1002:4752 | 0e11:001e | AMD             | Rage 3 [Rage XL PCI]     | 100%   |          | BF8AB3D150 |
| 1002:4752 | 103c:3208 | AMD             | Rage 3 [Rage XL PCI]     | 100%   |          | 2C877CF870 |
| 1002:4752 | 8086:341a | AMD             | Rage 3 [Rage XL PCI]     | 100%   |          | 37AA8C0E8E |
| 1002:4752 | 8086:3439 | AMD             | Rage 3 [Rage XL PCI]     | 100%   |          | 0F21E859FA |
| 1002:4752 | 8086:345e | AMD             | Rage 3 [Rage XL PCI]     | 100%   |          | 97CC3C4274 |
| 1002:4756 | 1002:0088 | AMD             | Rage 2 [3D Rage IIC PCI] | 100%   |          | DE464659FE |
| 1002:4756 | 1002:4756 | AMD             | Rage 2 [3D Rage IIC PCI] | 100%   |          | 0B5D843F10 |
| 1002:4c4d | 1002:4c4d | AMD             | Rage Mobility AGP 2x ... | 100%   |          | 5C43AB36E8 |
| 1002:4c4d | 10cf:1074 | AMD             | Rage Mobility AGP 2x ... | 100%   |          | 66D6816956 |
| 1002:4c66 | 1028:011d | AMD             | RV250/M9 GL [Mobility... | 20%    | 3.14.44  | 680157DC8E |
| 1002:5046 | 1002:0014 | AMD             | Rage 4 [Rage 128 PRO ... | 100%   |          | 3C9A2F5DB5 |
| 1002:515e | 103c:31fb | AMD             | ES1000                   | 7.4%   | 2.6.32   | B3175C4255 |
| 1002:5446 | 1002:0408 | AMD             | Rage 128 PRO Ultra AG... | 100%   |          | F254B75397 |
| 1002:5653 | 1043:1122 | AMD             | RV410/M26 [Mobility R... | 33.3%  | 4.15.0   | 79A40B4127 |
| 1002:5975 | 1028:01f5 | AMD             | RS482M [Mobility Rade... | 3.8%   | 3.14.39  | 73260FEC7B |
| 1002:5a62 | 1043:1402 | AMD             | RC410M [Mobility Rade... | 1.2%   | 3.14.25  | 6379E4D092 |
| 1002:5b60 | 1462:0320 | AMD             | RV370 [Radeon X300]      | 38.9%  | 3.10.0   | 41952E666E |
| 1002:6600 | 103c:1947 | AMD             | Mars [Radeon HD 8670A... | 6.2%   | 4.1.33   | 66AABE5A6B |
| 1002:6600 | 103c:194d | AMD             | Mars [Radeon HD 8670A... | 12.9%  | 3.14.25  | 2EDF7E28BE |
| 1002:6600 | 103c:195d | AMD             | Mars [Radeon HD 8670A... | 50%    | 5.7.19   | 1A786FF081 |
| 1002:6601 | 1028:05b8 | AMD             | Mars [Radeon HD 8730M]   | 2.4%   | 3.14.44  | 32AD5A31B9 |
| 1002:6601 | 103c:1990 | AMD             | Mars [Radeon HD 8730M]   | 12%    | 4.18.0   | AF0E04722E |
| 1002:6601 | 103c:2102 | AMD             | Mars [Radeon HD 8730M]   | 16.7%  | 5.0.0    | 9021B90504 |
| 1002:6604 | 1028:066f | AMD             | Opal XT [Radeon R7 M2... | 14.3%  | 4.1.25   | C0697E8F13 |
| 1002:6604 | 103c:8150 | AMD             | Opal XT [Radeon R7 M2... | 5.6%   | 4.15.0   | FD1C0C441E |
| 1002:6606 | 1028:05be | AMD             | Mars XTX [Radeon HD 8... | 4%     | 4.9.20   | FE1F341842 |
| 1002:6610 | 1028:2120 | AMD             | Oland XT [Radeon HD 8... | 21.4%  | 4.15.0   | D246C4D7C9 |
| 1002:6610 | 1043:0462 | AMD             | Oland XT [Radeon HD 8... | 5.3%   | 3.14.44  | 996842CD08 |
| 1002:6610 | 1462:3011 | AMD             | Oland XT [Radeon HD 8... | 7.7%   | 3.10.0   | 1BB044255A |
| 1002:6610 | 1787:2012 | AMD             | Oland XT [Radeon HD 8... | 100%   |          | 50841878AE |
| 1002:6611 | 1028:1002 | AMD             | Oland [Radeon HD 8570... | 12.5%  | 5.0.0    | 21ADB8FC36 |
| 1002:6611 | 174b:4248 | AMD             | Oland [Radeon HD 8570... | 50%    | 5.4.0    | 5F1212E8FF |
| 1002:6613 | 1462:8094 | AMD             | Oland PRO [Radeon R7 ... | 6.4%   | 3.14.44  | 4D6BFB7E09 |
| 1002:6658 | 1043:048f | AMD             | Bonaire XTX [Radeon R... | 20%    | 4.1.34   | 03F855D4C1 |
| 1002:6658 | 1462:2935 | AMD             | Bonaire XTX [Radeon R... | 20%    | 4.15.0   | 62D805686B |
| 1002:6658 | 174b:e258 | AMD             | Bonaire XTX [Radeon R... | 2.7%   | 3.14.44  | 607681A346 |
| 1002:6658 | 1787:200f | AMD             | Bonaire XTX [Radeon R... | 50%    | 5.3.0    | 28E3ED12EF |
| 1002:665c | 1043:0456 | AMD             | Bonaire XT [Radeon HD... | 40%    | 4.15.0   | 8EACB4F7F2 |
| 1002:665f | 1682:7360 | AMD             | Tobago PRO [Radeon R7... | 3.7%   | 3.10.0   | A4E8642513 |
| 1002:66af | 1002:081e | AMD             | Vega 20 [Radeon VII]     | 5.1%   | 4.15.0   | 6F3E76F9C3 |
| 1002:6739 | 1462:2441 | AMD             | Barts PRO [Radeon HD ... | 15.4%  | 4.4.0    | 20AE6B771A |
| 1002:6740 | 103c:1657 | AMD             | Whistler [Radeon HD 6... | 2.8%   | 3.14.44  | D0C6C442EA |
| 1002:6740 | 103c:165a | AMD             | Whistler [Radeon HD 6... | 3.7%   | 4.1.15   | 0261873B10 |
| 1002:6740 | 103c:185e | AMD             | Whistler [Radeon HD 6... | 4.8%   | 4.9.20   | EEA47EE3F6 |
| 1002:6740 | 103c:3388 | AMD             | Whistler [Radeon HD 6... | 16.4%  | 3.14.44  | 5F74F374A8 |
| 1002:6741 | 1025:050e | AMD             | Whistler [Radeon HD 6... | 4.2%   | 4.9.9    | 68C2E2956E |
| 1002:6741 | 1025:059e | AMD             | Whistler [Radeon HD 6... | 14.3%  | 3.14.44  | 7704916E37 |
| 1002:6741 | 1028:04c5 | AMD             | Whistler [Radeon HD 6... | 15.4%  | 4.15.0   | 2C70B99951 |
| 1002:6741 | 1028:04cd | AMD             | Whistler [Radeon HD 6... | 5.9%   | 4.1.13   | 093E631BFB |
| 1002:6741 | 103c:358d | AMD             | Whistler [Radeon HD 6... | 3.1%   | 3.14.44  | AB2744120A |
| 1002:6741 | 103c:3593 | AMD             | Whistler [Radeon HD 6... | 6.2%   | 4.1.13   | 65917EBD9D |
| 1002:6741 | 106b:00e2 | AMD             | Whistler [Radeon HD 6... | 40%    | 5.4.0    | F5B03A2FD9 |
| 1002:6741 | 106b:00e3 | AMD             | Whistler [Radeon HD 6... | 20%    | 5.4.0    | 4FF177B147 |
| 1002:6741 | 106b:00e8 | AMD             | Whistler [Radeon HD 6... | 20%    | 4.9.9    | F5BB829DBB |
| 1002:6741 | 144d:c0b3 | AMD             | Whistler [Radeon HD 6... | 7.7%   | 4.15.0   | 2B3EBD7597 |
| 1002:6741 | 17aa:21ef | AMD             | Whistler [Radeon HD 6... | 14.3%  | 4.18.0   | A8D9E5EF41 |
| 1002:6741 | 17aa:3976 | AMD             | Whistler [Radeon HD 6... | 3.2%   | 4.1.15   | 70A3F923C2 |
| 1002:6742 | 1179:fb31 | AMD             | Whistler LE [Radeon H... | 8.3%   | 3.14.44  | 834D15C08C |
| 1002:6758 | 174b:e194 | AMD             | Turks XT [Radeon HD 6... | 2.3%   | 3.14.44  | AB0866908C |
| 1002:6759 | 1002:0000 | AMD             | Turks PRO [Radeon HD ... | 20%    | 4.15.0   | 168E6322D7 |
| 1002:6759 | 1682:3190 | AMD             | Turks PRO [Radeon HD ... | 50%    | 5.4.0    | 7086B0C8AF |
| 1002:6759 | 174b:e193 | AMD             | Turks PRO [Radeon HD ... | 1.1%   | 3.14.22  | 50DEF7A853 |
| 1002:6759 | 1787:2308 | AMD             | Turks PRO [Radeon HD ... | 1.5%   | 4.1.34   | 1B7D670A36 |
| 1002:675b | 1002:7600 | AMD             | Turks [Radeon HD 7600... | 7.7%   | 4.15.0   | B511052CC4 |
| 1002:6760 | 103c:161e | AMD             | Seymour [Radeon HD 64... | 4.4%   | 4.1.15   | BE8865F154 |
| 1002:6760 | 103c:1659 | AMD             | Seymour [Radeon HD 64... | 8.3%   | 4.1.25   | B7756075FD |
| 1002:6760 | 103c:1663 | AMD             | Seymour [Radeon HD 64... | 4.8%   | 3.14.44  | E7A69B7B4D |
| 1002:6760 | 103c:166c | AMD             | Seymour [Radeon HD 64... | 3.8%   | 3.14.44  | 585D199B71 |
| 1002:6760 | 103c:1672 | AMD             | Seymour [Radeon HD 64... | 3.7%   | 3.14.44  | 4F9C19A9C0 |
| 1002:6760 | 103c:185d | AMD             | Seymour [Radeon HD 64... | 3.8%   | 4.1.15   | 4A453F1EBE |
| 1002:6760 | 103c:3581 | AMD             | Seymour [Radeon HD 64... | 13%    | 4.15.0   | 5D0460ADCE |
| 1002:6760 | 106b:00e1 | AMD             | Seymour [Radeon HD 64... | 12.5%  | 5.3.0    | 772B6F3A59 |
| 1002:6760 | 144d:c625 | AMD             | Seymour [Radeon HD 64... | 5.6%   | 3.14.44  | EEA7A5432D |
| 1002:6761 | 1297:4012 | AMD             | Seymour LP [Radeon HD... | 100%   |          | DE0CC0AB6F |
| 1002:6770 | 17aa:3623 | AMD             | Caicos [Radeon HD 645... | 20%    | 4.1.15   | 02882EF37B |
| 1002:6771 | 174b:a01c | AMD             | Caicos XTX [Radeon HD... | 100%   |          | 665B7470FF |
| 1002:6778 | 1028:2120 | AMD             | Caicos XT [Radeon HD ... | 2.9%   | 3.10.0   | 50650DB6E3 |
| 1002:6779 | 103c:2128 | AMD             | Caicos [Radeon HD 645... | 5.9%   | 4.1.13   | FE2C73039A |
| 1002:6779 | 1043:03da | AMD             | Caicos [Radeon HD 645... | 0.6%   | 3.10.34  | 9734ABB0D4 |
| 1002:6779 | 1043:047b | AMD             | Caicos [Radeon HD 645... | 20%    | 4.15.0   | 423A12D8A5 |
| 1002:6779 | 174b:a004 | AMD             | Caicos [Radeon HD 645... | 1.4%   | 3.14.44  | CD61F6363F |
| 1002:6779 | 174b:e164 | AMD             | Caicos [Radeon HD 645... | 0.6%   | 3.14.33  | 8A4E34A210 |
| 1002:6779 | 1b0a:9097 | AMD             | Caicos [Radeon HD 645... | 7.7%   | 4.15.0   | 05A342E81F |
| 1002:6798 | 174b:3001 | AMD             | Tahiti XT [Radeon HD ... | 2.8%   | 3.14.44  | 7D178DB676 |
| 1002:67b1 | 1002:0b00 | AMD             | Hawaii PRO [Radeon R9... | 6.7%   | 4.19.66  | 2FAE8819F7 |
| 1002:67df | 1002:0b37 | AMD             | Ellesmere [Radeon RX ... | 3.6%   | 4.20.5   | 5CC9EEEBFE |
| 1002:67df | 1043:0537 | AMD             | Ellesmere [Radeon RX ... | 100%   |          | F25E40D620 |
| 1002:67df | 1043:0557 | AMD             | Ellesmere [Radeon RX ... | 50%    | 4.15.0   | A82798AEA1 |
| 1002:67df | 1458:22fc | AMD             | Ellesmere [Radeon RX ... | 1.4%   | 4.15.0   | 6B0F675FD7 |
| 1002:67df | 1462:3413 | AMD             | Ellesmere [Radeon RX ... | 4.1%   | 4.9.87   | 3F7E1BB390 |
| 1002:67df | 1462:3418 | AMD             | Ellesmere [Radeon RX ... | 0.7%   | 4.9.0    | F3A29DDFF9 |
| 1002:67df | 1462:341b | AMD             | Ellesmere [Radeon RX ... | 0.5%   | 4.15.0   | 86FC987528 |
| 1002:67df | 148c:2391 | AMD             | Ellesmere [Radeon RX ... | 6.2%   | 5.4.0    | F61EE20F03 |
| 1002:67df | 1682:c570 | AMD             | Ellesmere [Radeon RX ... | 2.2%   | 4.15.0   | 3A69ABB947 |
| 1002:67df | 174b:e347 | AMD             | Ellesmere [Radeon RX ... | 1.1%   | 4.13.0   | BC7C3F8C4D |
| 1002:67df | 1da2:e366 | AMD             | Ellesmere [Radeon RX ... | 1%     | 4.8.0    | 069769819B |
| 1002:67ef | 1682:9460 | AMD             | Baffin [Radeon RX 460... | 3.1%   | 4.15.0   | 8212CC8601 |
| 1002:67ef | 1682:956d | AMD             | Baffin [Radeon RX 460... | 1.8%   | 4.9.60   | 0E57B37B4E |
| 1002:67ef | 174b:e344 | AMD             | Baffin [Radeon RX 460... | 8.3%   | 4.9.124  | 98A829DCFD |
| 1002:67ef | 174b:e348 | AMD             | Baffin [Radeon RX 460... | 6.2%   | 4.9.20   | 72DD80DA38 |
| 1002:67ff | 1043:052d | AMD             | Baffin [Radeon RX 550... | 6.7%   | 4.15.0   | 0219C1DC48 |
| 1002:67ff | 1da2:e348 | AMD             | Baffin [Radeon RX 550... | 2.1%   | 4.9.60   | CEDA0A30C3 |
| 1002:6800 | 1558:7102 | AMD             | Wimbledon XT [Radeon ... | 50%    | 5.4.0    | B70E28F8B3 |
| 1002:6810 | 174b:e271 | AMD             | Curacao XT / Trinidad... | 2%     | 3.14.44  | E84363FB9C |
| 1002:6818 | 174b:e241 | AMD             | Pitcairn XT [Radeon H... | 3.3%   | 3.14.44  | 7641FD618F |
| 1002:6819 | 1043:042c | AMD             | Pitcairn PRO [Radeon ... | 6.7%   | 3.14.22  | EBBD83B0CA |
| 1002:6819 | 1043:045b | AMD             | Pitcairn PRO [Radeon ... | 11.8%  | 3.14.33  | A12C16610A |
| 1002:6819 | 174b:a001 | AMD             | Pitcairn PRO [Radeon ... | 16.7%  | 4.9.0    | 97B72D7509 |
| 1002:6819 | 1787:2320 | AMD             | Pitcairn PRO [Radeon ... | 2.9%   | 3.14.44  | 56653049B3 |
| 1002:6821 | 1028:05ee | AMD             | Venus XT [Radeon HD 8... | 13%    | 3.14.44  | A4933DBF64 |
| 1002:6823 | 1028:05eb | AMD             | Venus PRO [Radeon HD ... | 11.1%  | 3.14.44  | 1912A7C4EA |
| 1002:682b | 1028:1004 | AMD             | Cape Verde PRO / Venu... | 25%    | 5.3.0    | 0C434691D6 |
| 1002:682f | 1028:0572 | AMD             | Chelsea LP [Radeon HD... | 2.6%   | 3.14.44  | F62BE8057A |
| 1002:683d | 1787:7260 | AMD             | Cape Verde XT [Radeon... | 20%    | 4.1.25   | B0A897D878 |
| 1002:683f | 1682:3246 | AMD             | Cape Verde PRO [Radeo... | 12.5%  | 4.15.0   | D076F8FE03 |
| 1002:6840 | 1028:056a | AMD             | Thames [Radeon HD 750... | 14%    | 3.14.44  | 7617104233 |
| 1002:6840 | 1028:0598 | AMD             | Thames [Radeon HD 750... | 25.5%  | 3.14.25  | E9926664B0 |
| 1002:6840 | 103c:183e | AMD             | Thames [Radeon HD 750... | 2.5%   | 3.14.15  | EB23D17143 |
| 1002:6840 | 103c:1840 | AMD             | Thames [Radeon HD 750... | 6.2%   | 3.14.44  | B0552C0AF2 |
| 1002:6840 | 103c:1842 | AMD             | Thames [Radeon HD 750... | 3.4%   | 3.14.44  | 2266C4AA6C |
| 1002:6840 | 104d:9096 | AMD             | Thames [Radeon HD 750... | 2.9%   | 3.14.25  | 8677002BB3 |
| 1002:6840 | 1179:fb81 | AMD             | Thames [Radeon HD 750... | 11.1%  | 3.14.33  | 611479F524 |
| 1002:6840 | 144d:c0d8 | AMD             | Thames [Radeon HD 750... | 6.5%   | 3.14.22  | F49D288489 |
| 1002:6841 | 1028:057f | AMD             | Thames [Radeon HD 755... | 22.2%  | 4.15.0   | 2CE968AF69 |
| 1002:6841 | 103c:179d | AMD             | Thames [Radeon HD 755... | 17.8%  | 3.14.44  | CE78055795 |
| 1002:6841 | 103c:17f4 | AMD             | Thames [Radeon HD 755... | 8.1%   | 3.14.44  | CF941AF09E |
| 1002:6841 | 104d:90ac | AMD             | Thames [Radeon HD 755... | 5.3%   | 3.10.19  | F5C5B94EB8 |
| 1002:68a1 | 1025:0475 | AMD             | Broadway PRO [Mobilit... | 100%   |          | 3B1F271BB2 |
| 1002:68b8 | 1002:2543 | AMD             | Juniper XT [Radeon HD... | 2.3%   | 3.14.44  | 7EE5C39C1A |
| 1002:68b8 | 174b:1482 | AMD             | Juniper XT [Radeon HD... | 1.6%   | 4.1.15   | 392D4D0E90 |
| 1002:68ba | 1043:0414 | AMD             | Juniper XT [Radeon HD... | 16.7%  | 4.9.124  | 38709AEC79 |
| 1002:68be | 174b:e138 | AMD             | Juniper PRO [Radeon H... | 6.2%   | 4.4.0    | 6C4DA588EA |
| 1002:68bf | 1787:2313 | AMD             | Juniper PRO [Radeon H... | 8.3%   | 4.1.25   | C8888818C9 |
| 1002:68c1 | 1028:0447 | AMD             | Madison [Mobility Rad... | 5%     | 4.1.34   | 313EB1D925 |
| 1002:68c1 | 103c:1448 | AMD             | Madison [Mobility Rad... | 11.1%  | 3.10.34  | 2C1CF2DA53 |
| 1002:68d8 | 1028:68e0 | AMD             | Redwood XT [Radeon HD... | 15.4%  | 4.9.0    | 7155E4EF04 |
| 1002:68d8 | 1462:2201 | AMD             | Redwood XT [Radeon HD... | 20%    | 4.15.0   | DDF9D08A22 |
| 1002:68d8 | 174b:e152 | AMD             | Redwood XT [Radeon HD... | 4.3%   | 4.1.15   | D67A015497 |
| 1002:68da | 174b:e930 | AMD             | Redwood LE [Radeon HD... | 12.5%  | 4.1.19   | EEC47F990C |
| 1002:68e0 | 103c:143a | AMD             | Park [Mobility Radeon... | 4.6%   | 3.10.51  | 78A2215DD4 |
| 1002:68e0 | 1043:1bf2 | AMD             | Park [Mobility Radeon... | 0.8%   | 3.14.44  | A092284909 |
| 1002:68e0 | 104d:9071 | AMD             | Park [Mobility Radeon... | 4.3%   | 4.1.34   | F28BA85F16 |
| 1002:68e4 | 103c:162c | AMD             | Robson CE [Radeon HD ... | 33.3%  | 4.15.0   | D563465019 |
| 1002:68e4 | 1043:1c92 | AMD             | Robson CE [Radeon HD ... | 3.9%   | 3.14.44  | 021C8D3567 |
| 1002:68e4 | 17aa:397a | AMD             | Robson CE [Radeon HD ... | 6.5%   | 3.10.34  | AF0EC73528 |
| 1002:68f9 | 1028:2126 | AMD             | Cedar [Radeon HD 5000... | 2.4%   | 4.1.34   | D5A5261203 |
| 1002:68f9 | 1462:2127 | AMD             | Cedar [Radeon HD 5000... | 1.5%   | 4.15.0   | 3E9F988A30 |
| 1002:68f9 | 1462:2133 | AMD             | Cedar [Radeon HD 5000... | 20%    | 5.0.0    | E6AC4BAD03 |
| 1002:68f9 | 1462:2181 | AMD             | Cedar [Radeon HD 5000... | 7.1%   | 5.2.17   | DA73296417 |
| 1002:68f9 | 1462:2340 | AMD             | Cedar [Radeon HD 5000... | 3.8%   | 4.1.22   | 75CAA3FF6A |
| 1002:68f9 | 1682:3030 | AMD             | Cedar [Radeon HD 5000... | 4.5%   | 4.9.0    | 761DD67D16 |
| 1002:6900 | 1179:f933 | AMD             | Topaz XT [Radeon R7 M... | 66.7%  | 5.4.0    | 16C913AC5F |
| 1002:6901 | 103c:224a | AMD             | Topaz PRO [Radeon R5 ... | 8.3%   | 4.9.155  | 00E2C13F56 |
| 1002:6938 | 1043:04f5 | AMD             | Tonga XT / Amethyst X... | 33.3%  | 4.5.5    | 0E1E35C6E2 |
| 1002:6938 | 174b:e308 | AMD             | Tonga XT / Amethyst X... | 10%    | 4.15.0   | 358922D8FF |
| 1002:6939 | 1682:9380 | AMD             | Tonga PRO [Radeon R9 ... | 7.1%   | 4.15.0   | A3F6229CAA |
| 1002:6939 | 174b:e308 | AMD             | Tonga PRO [Radeon R9 ... | 2.9%   | 4.9.60   | 77EF398855 |
| 1002:6981 | 1002:0b0d | AMD             | Lexa XT [Radeon PRO W... | 50%    | 5.4.0    | A21B63E491 |
| 1002:6981 | 1028:0926 | AMD             | Lexa XT [Radeon PRO W... | 25%    | 5.4.0    | 218EFD739A |
| 1002:699f | 1002:0b04 | AMD             | Lexa PRO [Radeon 540/... | 4.3%   | 4.15.0   | 54B3E00EE6 |
| 1002:699f | 1043:0511 | AMD             | Lexa PRO [Radeon 540/... | 1.4%   | 4.12.14  | A994473A14 |
| 1002:699f | 1458:22f3 | AMD             | Lexa PRO [Radeon 540/... | 10%    | 4.15.0   | 03EEED62F1 |
| 1002:699f | 1462:8a90 | AMD             | Lexa PRO [Radeon 540/... | 7.9%   | 3.10.0   | 28B8E9271B |
| 1002:699f | 148c:2380 | AMD             | Lexa PRO [Radeon 540/... | 13%    | 4.15.0   | F48405DCFD |
| 1002:699f | 1682:9550 | AMD             | Lexa PRO [Radeon 540/... | 5.6%   | 4.15.0   | C32123B3A9 |
| 1002:7187 | 1043:0174 | AMD             | RV516 [Radeon X1300/X... | 20%    | 3.14.22  | CE881D4659 |
| 1002:71c5 | 1033:8816 | AMD             | RV530/M56-P [Mobility... | 50%    | 4.18.16  | 76BEC35362 |
| 1002:731f | 1043:0577 | AMD             | Navi 10 [Radeon RX 56... | 7.7%   | 5.3.18   | A4C45E5869 |
| 1002:731f | 1043:05a5 | AMD             | Navi 10 [Radeon RX 56... | 100%   |          | 15F9EE179C |
| 1002:731f | 1458:2313 | AMD             | Navi 10 [Radeon RX 56... | 2.4%   | 5.3.0    | DE7CD1F262 |
| 1002:731f | 1458:2316 | AMD             | Navi 10 [Radeon RX 56... | 32%    | 5.4.0    | 0FAED02AF4 |
| 1002:731f | 1462:3810 | AMD             | Navi 10 [Radeon RX 56... | 12.5%  | 5.3.6    | 07C97FA660 |
| 1002:731f | 1462:3811 | AMD             | Navi 10 [Radeon RX 56... | 33.3%  | 5.4.0    | 84D8CC558D |
| 1002:731f | 148c:2399 | AMD             | Navi 10 [Radeon RX 56... | 11.8%  | 5.3.0    | 2F9E637529 |
| 1002:731f | 1682:5701 | AMD             | Navi 10 [Radeon RX 56... | 4.3%   | 5.3.0    | 97E4FAABF9 |
| 1002:731f | 1682:5710 | AMD             | Navi 10 [Radeon RX 56... | 6.2%   | 5.4.0    | DD30E29DA1 |
| 1002:731f | 1da2:e409 | AMD             | Navi 10 [Radeon RX 56... | 1.7%   | 5.3.0    | 40061999CC |
| 1002:731f | 1da2:e410 | AMD             | Navi 10 [Radeon RX 56... | 6.7%   | 5.4.0    | 9A71B52057 |
| 1002:731f | 1da2:e411 | AMD             | Navi 10 [Radeon RX 56... | 2.3%   | 5.3.0    | 8D44C5EE07 |
| 1002:7340 | 1043:04e6 | AMD             | Navi 14 [Radeon RX 55... | 12.5%  | 5.4.0    | A53152418D |
| 1002:7340 | 1458:2319 | AMD             | Navi 14 [Radeon RX 55... | 25%    | 5.4.0    | 6C7CCE8852 |
| 1002:7340 | 1462:3820 | AMD             | Navi 14 [Radeon RX 55... | 60%    | 5.4.0    | AE3376CD9B |
| 1002:7340 | 1462:3822 | AMD             | Navi 14 [Radeon RX 55... | 4%     | 4.15.0   | A96ADDDFC3 |
| 1002:7340 | 1682:5501 | AMD             | Navi 14 [Radeon RX 55... | 12.5%  | 5.4.0    | B7550DC9FC |
| 1002:7340 | 1849:5116 | AMD             | Navi 14 [Radeon RX 55... | 28.6%  | 5.4.0    | A30F82D383 |
| 1002:7340 | 1da2:e421 | AMD             | Navi 14 [Radeon RX 55... | 5.9%   | 5.4.0    | 72D2BD3597 |
| 1002:73bf | 1002:0e3a | AMD             | Navi 21 [Radeon RX 68... | 7.1%   | 5.9.13   | 448EEDB174 |
| 1002:73bf | 1462:3951 | AMD             | Navi 21 [Radeon RX 68... | 100%   |          | 604E65FE47 |
| 1002:73bf | 148c:2406 | AMD             | Navi 21 [Radeon RX 68... | 33.3%  | 5.11.0   | C5010E1348 |
| 1002:73bf | 1da2:e438 | AMD             | Navi 21 [Radeon RX 68... | 9.1%   | 5.9.16   | B6DD3AD958 |
| 1002:73bf | 1da2:e439 | AMD             | Navi 21 [Radeon RX 68... | 33.3%  | 5.11.0   | 3C17BD1B57 |
| 1002:791e | 105b:0e0a | AMD             | RS690 [Radeon X1200]     | 14.3%  | 4.9.155  | A0E95916C3 |
| 1002:791e | 1462:7327 | AMD             | RS690 [Radeon X1200]     | 11.1%  | 4.1.15   | 03A49D47F8 |
| 1002:791f | 1043:14f2 | AMD             | RS690M [Radeon Xpress... | 7.7%   | 3.14.44  | 31DD762F09 |
| 1002:791f | 1462:6b30 | AMD             | RS690M [Radeon Xpress... | 100%   |          | 4940058A56 |
| 1002:944a | 106b:00b5 | AMD             | RV770/M98L [Mobility ... | 66.7%  | 4.16.12  | D90C44B813 |
| 1002:9460 | 1682:2700 | AMD             | RV790 [Radeon HD 4890]   | 100%   |          | 335083A19F |
| 1002:9480 | 1025:017e | AMD             | RV730/M96 [Mobility R... | 75%    | 5.4.0    | 6D1385653B |
| 1002:9488 | 106b:00b6 | AMD             | RV730/M96-XT [Mobilit... | 16.7%  | 4.9.0    | 65E6848B8A |
| 1002:9490 | 1787:2268 | AMD             | RV730 XT [Radeon HD 4... | 6.2%   | 4.1.15   | 0ADCFFB219 |
| 1002:9495 | 1458:0028 | AMD             | RV730 [Radeon HD 4600... | 7.1%   | 4.9.20   | 7DE59C54E2 |
| 1002:9498 | 1458:21c5 | AMD             | RV730 PRO [Radeon HD ... | 12.5%  | 3.14.44  | 7082E7CD50 |
| 1002:9498 | 174b:9498 | AMD             | RV730 PRO [Radeon HD ... | 20%    | 3.14.44  | 5A0B34CAC9 |
| 1002:9498 | 174b:e109 | AMD             | RV730 PRO [Radeon HD ... | 7.1%   | 4.1.19   | 58A3E6E8ED |
| 1002:94c1 | 1458:2190 | AMD             | RV610 [Radeon HD 2400... | 50%    | 4.18.16  | 45FA5763DC |
| 1002:94c3 | 1028:0402 | AMD             | RV610 [Radeon HD 2400... | 18.8%  | 4.15.0   | 9434F7214C |
| 1002:94c8 | 1025:011f | AMD             | RV610/M74 [Mobility R... | 7.7%   | 3.14.44  | B5EDE5C96B |
| 1002:9540 | 1458:21ae | AMD             | RV710 [Radeon HD 4550]   | 8.3%   | 4.15.0   | F2FB2391A2 |
| 1002:954f | 1043:02a8 | AMD             | RV710 [Radeon HD 4350... | 2.7%   | 3.13.0   | 9EB845703C |
| 1002:954f | 1043:02ca | AMD             | RV710 [Radeon HD 4350... | 66.7%  | 3.14.33  | AD36100CE4 |
| 1002:954f | 1458:21ed | AMD             | RV710 [Radeon HD 4350... | 50%    | 4.18.16  | 3FA9D8EBCB |
| 1002:954f | 1462:1618 | AMD             | RV710 [Radeon HD 4350... | 8.3%   | 3.14.53  | 51837DE98F |
| 1002:954f | 174b:e990 | AMD             | RV710 [Radeon HD 4350... | 2.3%   | 3.14.25  | 7A1BE51DAF |
| 1002:9552 | 103c:3074 | AMD             | RV710/M92 [Mobility R... | 5.1%   | 3.14.25  | 764886854E |
| 1002:9553 | 1025:0293 | AMD             | RV710/M92 [Mobility R... | 33.3%  | 4.4.0    | B61F73224F |
| 1002:9553 | 103c:3628 | AMD             | RV710/M92 [Mobility R... | 3.7%   | 4.1.38   | 5A2F390FC9 |
| 1002:9553 | 1043:1b32 | AMD             | RV710/M92 [Mobility R... | 6.2%   | 3.14.44  | 78420C272F |
| 1002:9553 | 1043:1c42 | AMD             | RV710/M92 [Mobility R... | 3%     | 4.1.15   | 6D866DDF45 |
| 1002:9553 | 1179:ff82 | AMD             | RV710/M92 [Mobility R... | 66.7%  | 3.14.44  | E710B01A79 |
| 1002:9553 | 1462:1055 | AMD             | RV710/M92 [Mobility R... | 100%   |          | EAAB14866E |
| 1002:9581 | 103c:30c5 | AMD             | RV630/M76 [Mobility R... | 3.7%   | 3.14.25  | 64A60F9E6A |
| 1002:9583 | 106b:0083 | AMD             | RV630/M76 [Mobility R... | 1.3%   | 4.4.0    | 29FDFC8C36 |
| 1002:9588 | 174b:2e42 | AMD             | RV630 XT [Radeon HD 2... | 4.3%   | 3.14.44  | 69171F27D3 |
| 1002:9589 | 174b:e410 | AMD             | RV630 PRO [Radeon HD ... | 3.8%   | 3.14.44  | C4119749D3 |
| 1002:9591 | 17aa:2126 | AMD             | RV635/M86 [Mobility R... | 6.2%   | 4.9.0    | 7C29A97DFF |
| 1002:9598 | 1043:01d6 | AMD             | RV635 [Radeon HD 3650... | 33.3%  | 4.1.19   | 68A53D1511 |
| 1002:95c0 | 1028:3243 | AMD             | RV620 PRO [Radeon HD ... | 30%    | 4.15.0   | BEA8F18224 |
| 1002:95c4 | 1043:19e2 | AMD             | RV620/M82 [Mobility R... | 2.1%   | 4.1.34   | A13580724B |
| 1002:95c4 | 17aa:210f | AMD             | RV620/M82 [Mobility R... | 12.5%  | 4.4.0    | 906EA1B277 |
| 1002:95c5 | 1462:1371 | AMD             | RV620 LE [Radeon HD 3... | 50%    | 4.9.20   | E76B366E33 |
| 1002:9610 | 1458:d000 | AMD             | RS780 [Radeon HD 3200]   | 12.5%  | 3.10.0   | 52F139CC1C |
| 1002:9611 | 103c:3029 | AMD             | RS780C [Radeon 3100]     | 4.8%   | 4.1.25   | AD816C7052 |
| 1002:9612 | 103c:308c | AMD             | RS780M [Mobility Rade... | 5.9%   | 4.1.6    | 1A6FC28BDC |
| 1002:9614 | 1462:7550 | AMD             | RS780D [Radeon HD 3300]  | 100%   |          | 0B976BCE4C |
| 1002:9616 | 1043:8388 | AMD             | RS780L [Radeon 3000]     | 1.4%   | 3.10.0   | 2FBE460B8A |
| 1002:9616 | 1458:d000 | AMD             | RS780L [Radeon 3000]     | 1.6%   | 3.10.0   | 5232DD577C |
| 1002:9641 | 1025:059e | AMD             | Sumo [Radeon HD 6620G]   | 16.7%  | 3.17.8   | 7704916E37 |
| 1002:9647 | 103c:1663 | AMD             | Sumo [Radeon HD 6520G]   | 11.1%  | 4.1.15   | E7A69B7B4D |
| 1002:9647 | 103c:358d | AMD             | Sumo [Radeon HD 6520G]   | 7.1%   | 3.14.44  | AB2744120A |
| 1002:9647 | 1179:fc80 | AMD             | Sumo [Radeon HD 6520G]   | 100%   |          | 82C4813A13 |
| 1002:9647 | 144d:c625 | AMD             | Sumo [Radeon HD 6520G]   | 33.3%  | 4.15.0   | EEA7A5432D |
| 1002:964a | 1043:84c8 | AMD             | Sumo [Radeon HD 6530D]   | 5.9%   | 4.1.25   | 277AED7ED9 |
| 1002:9710 | 1043:83a2 | AMD             | RS880 [Radeon HD 4200]   | 1.7%   | 3.14.33  | 997274B093 |
| 1002:9710 | 1458:d000 | AMD             | RS880 [Radeon HD 4200]   | 2.5%   | 4.1.25   | 9FF481D661 |
| 1002:9710 | 1565:1704 | AMD             | RS880 [Radeon HD 4200]   | 12.5%  | 4.1.15   | 646309CB22 |
| 1002:9712 | 103c:1455 | AMD             | RS880M [Mobility Rade... | 7.7%   | 4.1.15   | 699CD52B2C |
| 1002:9712 | 103c:1609 | AMD             | RS880M [Mobility Rade... | 17.4%  | 3.10.0   | EF11B1D600 |
| 1002:9714 | 1458:d000 | AMD             | RS880 [Radeon HD 4290]   | 7.1%   | 4.18.16  | 888FF52208 |
| 1002:9714 | 1849:9714 | AMD             | RS880 [Radeon HD 4290]   | 25%    | 4.1.25   | CAFF866F87 |
| 1002:9715 | 1025:0444 | AMD             | RS880 [Radeon HD 4250]   | 14.3%  | 4.7.0    | 52BBC50495 |
| 1002:9715 | 1458:d000 | AMD             | RS880 [Radeon HD 4250]   | 2.6%   | 3.14.44  | 4967060223 |
| 1002:9802 | 103c:3577 | AMD             | Wrestler [Radeon HD 6... | 1.7%   | 3.14.44  | DB6A9D6546 |
| 1002:9802 | 17aa:3619 | AMD             | Wrestler [Radeon HD 6... | 100%   |          | 79C67392D7 |
| 1002:9802 | 17aa:397f | AMD             | Wrestler [Radeon HD 6... | 23.1%  | 5.0.0    | 29B045E703 |
| 1002:9806 | 1002:9806 | AMD             | Wrestler [Radeon HD 6... | 20%    | 4.15.0   | 5FB055C8BB |
| 1002:9806 | 1025:0690 | AMD             | Wrestler [Radeon HD 6... | 100%   |          | 5AAA403DEE |
| 1002:9806 | 103c:17e2 | AMD             | Wrestler [Radeon HD 6... | 17.6%  | 4.15.0   | 67884140AF |
| 1002:9806 | 103c:3577 | AMD             | Wrestler [Radeon HD 6... | 1.6%   | 3.14.33  | 2B13402314 |
| 1002:9806 | 104d:9082 | AMD             | Wrestler [Radeon HD 6... | 3.4%   | 3.14.44  | F116097E48 |
| 1002:9807 | 1002:9807 | AMD             | Wrestler [Radeon HD 6... | 100%   |          | 3027B15C31 |
| 1002:9808 | 17aa:397b | AMD             | Wrestler [Radeon HD 7... | 33.3%  | 5.3.0    | 1EB94811FC |
| 1002:9809 | 17aa:3668 | AMD             | Wrestler [Radeon HD 7... | 50%    | 4.1.15   | 3FDBCC01BC |
| 1002:9830 | 1043:8623 | AMD             | Kabini [Radeon HD 840... | 1%     | 3.14.44  | 7A3C73F361 |
| 1002:9830 | 1849:9830 | AMD             | Kabini [Radeon HD 840... | 11.1%  | 3.10.0   | 19E04F01E6 |
| 1002:9833 | 103c:21b4 | AMD             | Kabini [Radeon HD 8330E] | 22.2%  | 5.4.0    | BAB965C49D |
| 1002:9837 | 103c:2187 | AMD             | Kabini [Radeon HD 8280E] | 16.7%  | 4.19.0   | 0E816C8EE5 |
| 1002:9838 | 1025:0800 | AMD             | Kabini [Radeon HD 824... | 23.5%  | 4.15.0   | 370BD439D7 |
| 1002:9838 | 103c:2b56 | AMD             | Kabini [Radeon HD 824... | 50%    | 4.9.155  | 3DB64C4252 |
| 1002:9838 | 103c:8133 | AMD             | Kabini [Radeon HD 824... | 22.2%  | 4.15.0   | 9311532F56 |
| 1002:9839 | 1179:fae1 | AMD             | Kabini [Radeon HD 8180]  | 100%   |          | 7F18F2F6E4 |
| 1002:9850 | 1025:108a | AMD             | Mullins [Radeon R3 Gr... | 16.7%  | 4.9.20   | E335200DD8 |
| 1002:9850 | 17aa:3804 | AMD             | Mullins [Radeon R3 Gr... | 25%    | 5.3.0    | 2D8AAC7989 |
| 1002:9851 | 1025:088c | AMD             | Mullins [Radeon R4/R5... | 100%   |          | D0E8E1E8D9 |
| 1002:9851 | 1025:104b | AMD             | Mullins [Radeon R4/R5... | 4.2%   | 4.1.33   | 792F04996F |
| 1002:9851 | 1025:108a | AMD             | Mullins [Radeon R4/R5... | 15.8%  | 4.9.60   | E0AFAC617E |
| 1002:9851 | 103c:2269 | AMD             | Mullins [Radeon R4/R5... | 10.5%  | 4.9.20   | B83DC673FD |
| 1002:9851 | 103c:226b | AMD             | Mullins [Radeon R4/R5... | 10%    | 4.1.34   | 8016AF5575 |
| 1002:9851 | 103c:22cd | AMD             | Mullins [Radeon R4/R5... | 3.8%   | 4.15.0   | 46004F2E8E |
| 1002:9851 | 17aa:3801 | AMD             | Mullins [Radeon R4/R5... | 8.1%   | 4.1.15   | 8FE8A781D0 |
| 1002:9852 | 1025:0865 | AMD             | Mullins [Radeon R2 Gr... | 36.4%  | 4.9.9    | 31DAE0F477 |
| 1002:9853 | 1028:0657 | AMD             | Mullins [Radeon R2 Gr... | 50%    | 5.10.14  | FDA4EB0499 |
| 1002:9853 | 1458:d000 | AMD             | Mullins [Radeon R2 Gr... | 25%    | 5.4.0    | 1635D5DB86 |
| 1002:9853 | 17aa:3801 | AMD             | Mullins [Radeon R2 Gr... | 2.5%   | 4.1.16   | 18EDCF9CC0 |
| 1002:9874 | 1002:1871 | AMD             | Wani [Radeon R5/R6/R7... | 15.4%  | 4.15.0   | 56E685A6F9 |
| 1002:9874 | 103c:80b6 | AMD             | Wani [Radeon R5/R6/R7... | 33.3%  | 4.18.0   | C7EEDACBF5 |
| 1002:9874 | 103c:8158 | AMD             | Wani [Radeon R5/R6/R7... | 33.3%  | 4.18.16  | 5818C39DC4 |
| 1002:9874 | 1458:d000 | AMD             | Wani [Radeon R5/R6/R7... | 3.4%   | 4.15.0   | EF2A18EF64 |
| 1002:9874 | 1462:7721 | AMD             | Wani [Radeon R5/R6/R7... | 66.7%  | 4.9.155  | 452B661F11 |
| 1002:9874 | 1565:1708 | AMD             | Wani [Radeon R5/R6/R7... | 100%   |          | C2727E98B9 |
| 1002:9874 | 17aa:5113 | AMD             | Wani [Radeon R5/R6/R7... | 25%    | 4.15.0   | 32F7318757 |
| 1002:9874 | 1849:9901 | AMD             | Wani [Radeon R5/R6/R7... | 66.7%  | 4.15.0   | 08FA2E917A |
| 1002:98e4 | 1002:1ca0 | AMD             | Stoney [Radeon R2/R3/... | 57.1%  | 5.4.0    | 5BBB4B610A |
| 1002:98e4 | 1002:1eb0 | AMD             | Stoney [Radeon R2/R3/... | 100%   |          | 5DFC619144 |
| 1002:98e4 | 1025:1087 | AMD             | Stoney [Radeon R2/R3/... | 9.1%   | 4.15.0   | AF870DDF65 |
| 1002:98e4 | 103c:84ac | AMD             | Stoney [Radeon R2/R3/... | 1.5%   | 4.15.0   | 1FB2A53C6D |
| 1002:98e4 | 17aa:39f3 | AMD             | Stoney [Radeon R2/R3/... | 0.8%   | 4.9.60   | CB06DA42F6 |
| 1002:98e4 | 17aa:39f5 | AMD             | Stoney [Radeon R2/R3/... | 1.3%   | 4.9.60   | 07D8074592 |
| 1002:98e4 | 17aa:39f9 | AMD             | Stoney [Radeon R2/R3/... | 4%     | 4.9.60   | C23D0EF968 |
| 1002:9900 | 103c:1849 | AMD             | Trinity [Radeon HD 76... | 10%    | 3.14.44  | FE4579E9D1 |
| 1002:9901 | 1002:9901 | AMD             | Trinity [Radeon HD 76... | 12.5%  | 4.9.60   | 23A46F007D |
| 1002:9901 | 1043:8526 | AMD             | Trinity [Radeon HD 76... | 2.6%   | 3.10.0   | AB0866908C |
| 1002:9901 | 1458:d000 | AMD             | Trinity [Radeon HD 76... | 22.2%  | 5.4.0    | 54B4B243AF |
| 1002:9908 | 103c:193b | AMD             | Trinity [Radeon HD 76... | 58.8%  | 4.15.0   | B7C9817495 |
| 1002:990c | 1043:8526 | AMD             | Richland [Radeon HD 8... | 2%     | 3.17.8   | 2B812202FC |
| 1002:990d | 17aa:3804 | AMD             | Richland [Radeon HD 8... | 2.6%   | 3.16.0   | BCE345B263 |
| 1002:990e | 1849:990e | AMD             | Richland [Radeon HD 8... | 1.6%   | 4.1.19   | 9875911102 |
| 1002:9990 | 1179:fb28 | AMD             | Trinity 2 [Radeon HD ... | 7.1%   | 4.15.0   | 053C350BEA |
| 1002:9991 | 103c:1850 | AMD             | Trinity 2 [Radeon HD ... | 28.6%  | 4.9.60   | 517C6137A3 |
| 1002:9993 | 103c:1850 | AMD             | Trinity 2 [Radeon HD ... | 10%    | 4.18.16  | A92E22AF3C |
| 1002:9996 | 1462:7721 | AMD             | Richland [Radeon HD 8... | 10%    | 3.14.44  | 373FA45C3B |
| 1002:9998 | 1462:7721 | AMD             | Richland [Radeon HD 8... | 33.3%  | 4.1.19   | 64E88CC13B |
| 10de:00cd | 10de:029b | Nvidia          | NV42GL [Quadro FX 345... | 25%    | 3.14.25  | E4D149FE76 |
| 10de:00ce | 10de:0243 | Nvidia          | NV41GL [Quadro FX 1400]  | 28.6%  | 4.15.0   | 43DA00D022 |
| 10de:0140 | 1458:3126 | Nvidia          | NV43 [GeForce 6600 GT]   | 50%    | 4.9.155  | 9F8066CA65 |
| 10de:0141 | 1043:81ee | Nvidia          | NV43 [GeForce 6600]      | 16.7%  | 4.1.38   | 71BC5B9631 |
| 10de:0141 | 1458:3124 | Nvidia          | NV43 [GeForce 6600]      | 7.7%   | 4.9.20   | F70B1CE07F |
| 10de:0141 | 1458:3126 | Nvidia          | NV43 [GeForce 6600]      | 16.7%  | 4.9.60   | 7E447609BE |
| 10de:0142 | 1462:9818 | Nvidia          | NV43 [GeForce 6600 LE]   | 60%    | 5.4.0    | 209ECB3837 |
| 10de:0148 | 1179:0001 | Nvidia          | NV43M [GeForce Go 6600]  | 100%   |          | D5D7DAB02F |
| 10de:0160 |           | Nvidia          | NV44 [GeForce 6500]      | 100%   |          | E776B2D4E9 |
| 10de:0161 |           | Nvidia          | NV44 [GeForce 6200 Tu... | 25%    | 4.9.60   | 10788B7DD6 |
| 10de:0161 | 1682:208f | Nvidia          | NV44 [GeForce 6200 Tu... | 100%   |          | 65D7B7AD14 |
| 10de:0163 | 1043:8205 | Nvidia          | NV44 [GeForce 6200 LE]   | 66.7%  | 5.4.0    | 41D3825923 |
| 10de:0163 | 1043:827b | Nvidia          | NV44 [GeForce 6200 LE]   | 100%   |          | 92059B060A |
| 10de:016a | 1043:8222 | Nvidia          | NV44 [GeForce 7100 GS]   | 50%    | 5.3.0    | E63CDF17ED |
| 10de:016a | 1462:0273 | Nvidia          | NV44 [GeForce 7100 GS]   | 80%    | 4.15.0   | 2116D4313C |
| 10de:0181 | 10de:016e | Nvidia          | NV18 [GeForce4 MX 440... | 100%   |          | D25A89846D |
| 10de:0191 | 10de:039c | Nvidia          | G80 [GeForce 8800 GTX]   | 16.7%  | 5.0.0    | F62172105C |
| 10de:01d1 | 1028:0405 | Nvidia          | G72 [GeForce 7300 LE]    | 12.5%  | 3.14.13  | D866167EB1 |
| 10de:01d1 | 1043:0346 | Nvidia          | G72 [GeForce 7300 LE]    | 20%    | 4.15.0   | 06FA187755 |
| 10de:01d1 | 1462:0345 | Nvidia          | G72 [GeForce 7300 LE]    | 100%   |          | B60543E7D3 |
| 10de:01d3 |           | Nvidia          | G72 [GeForce 7200 GS ... | 10.5%  | 4.1.25   | 45142A6931 |
| 10de:01d3 | 1458:3469 | Nvidia          | G72 [GeForce 7200 GS ... | 33.3%  | 5.0.0    | 67D8647DF7 |
| 10de:01d3 | 1682:227e | Nvidia          | G72 [GeForce 7200 GS ... | 15%    | 3.14.44  | 400AAFA751 |
| 10de:01d3 | 19da:5001 | Nvidia          | G72 [GeForce 7200 GS ... | 100%   |          | 7F950EC2F7 |
| 10de:01d7 | 1025:0090 | Nvidia          | G72M [Quadro NVS 110M... | 7.7%   | 4.9.9    | 26E90CD431 |
| 10de:01d7 | 1028:01c2 | Nvidia          | G72M [Quadro NVS 110M... | 20%    | 3.10.51  | 3832D0C33E |
| 10de:01d7 | 1043:1101 | Nvidia          | G72M [Quadro NVS 110M... | 50%    | 5.3.0    | F68C00B849 |
| 10de:01d7 | 1179:ff31 | Nvidia          | G72M [Quadro NVS 110M... | 14.3%  | 4.15.0   | 60E53B8E68 |
| 10de:01d7 | 17aa:3839 | Nvidia          | G72M [Quadro NVS 110M... | 11.1%  | 4.1.15   | 233A47535C |
| 10de:01d8 | 104d:81ef | Nvidia          | G72M [GeForce Go 7400]   | 25%    | 4.9.9    | 82BD19C032 |
| 10de:01d8 | 104d:81fd | Nvidia          | G72M [GeForce Go 7400]   | 66.7%  | 5.3.0    | 52E6107C87 |
| 10de:01df | 1acc:0804 | Nvidia          | G72 [GeForce 7300 GS]    | 100%   |          | F0F594BAAF |
| 10de:0241 | 1028:01ec | Nvidia          | C51 [GeForce 6150 LE]    | 9.1%   | 3.14.44  | 9F87C05C90 |
| 10de:0241 | 1462:3290 | Nvidia          | C51 [GeForce 6150 LE]    | 75%    | 4.15.0   | D67A4DF7D0 |
| 10de:0244 | 103c:30b7 | Nvidia          | C51 [GeForce Go 6150]    | 4.2%   | 3.10.34  | 0CA0AF6291 |
| 10de:0244 | 103c:30bf | Nvidia          | C51 [GeForce Go 6150]    | 27.3%  | 4.15.0   | BAD7484C1A |
| 10de:0247 | 1025:0112 | Nvidia          | C51 [GeForce Go 6100]    | 30.8%  | 5.0.0    | AF7A2A10E6 |
| 10de:0247 | 1462:373d | Nvidia          | C51 [GeForce Go 6100]    | 66.7%  | 4.19.69  | 154009C211 |
| 10de:0290 | 1682:2210 | Nvidia          | G71 [GeForce 7900 GTX]   | 33.3%  | 4.15.0   | DD42A7E94C |
| 10de:0291 | 1682:4000 | Nvidia          | G71 [GeForce 7900 GT/... | 100%   |          | C48FFB770E |
| 10de:0292 | 105b:0f03 | Nvidia          | G71 [GeForce 7900 GS]    | 50%    | 4.1.15   | 7296E03F32 |
| 10de:0298 | 1028:019b | Nvidia          | G71M [GeForce Go 7900... | 50%    | 4.15.0   | D04B1D869E |
| 10de:0298 | 1179:ff31 | Nvidia          | G71M [GeForce Go 7900... | 50%    | 5.4.0    | EF145B7CA4 |
| 10de:0299 | 1028:019b | Nvidia          | G71M [GeForce Go 7900... | 50%    | 5.3.0    | DD02475780 |
| 10de:029d | 10de:032b | Nvidia          | G71GL [Quadro FX 3500]   | 9.1%   | 3.14.44  | 22179970F5 |
| 10de:029e | 10de:032c | Nvidia          | G71GL [Quadro FX 1500]   | 40%    | 4.9.60   | 2CA2293675 |
| 10de:031a | 104d:814f | Nvidia          | NV31M [GeForce FX Go5... | 100%   |          | 88ABDEBE09 |
| 10de:0322 |           | Nvidia          | NV34 [GeForce FX 5200]   | 4.5%   | 3.14.44  | 61193F39C7 |
| 10de:0326 |           | Nvidia          | NV34 [GeForce FX 5500]   | 7.1%   | 3.18.16  | 3B62A9558D |
| 10de:0326 | 1462:911a | Nvidia          | NV34 [GeForce FX 5500]   | 25%    | 4.9.41   | FFD7AFA075 |
| 10de:0329 | 10de:0010 | Nvidia          | NV34M [GeForce FX Go5... | 50%    | 5.4.48   | 3AB679A1A1 |
| 10de:032c | 17c0:206f | Nvidia          | NV34M [GeForce FX Go5... | 100%   |          | 289D2B0685 |
| 10de:0344 | 1462:9573 | Nvidia          | NV36 [GeForce FX 5700VE] | 100%   |          | 303C1AC636 |
| 10de:0392 |           | Nvidia          | G73 [GeForce 7600 GS]    | 17.1%  | 3.14.25  | 2897AEB958 |
| 10de:0392 | 1458:341a | Nvidia          | G73 [GeForce 7600 GS]    | 12.5%  | 3.14.44  | 820510871C |
| 10de:0392 | 1462:0620 | Nvidia          | G73 [GeForce 7600 GS]    | 100%   |          | E757A87E51 |
| 10de:0393 |           | Nvidia          | G73 [GeForce 7300 GT]    | 16.7%  | 3.14.44  | 655B4A64A7 |
| 10de:0393 | 1043:820e | Nvidia          | G73 [GeForce 7300 GT]    | 12.5%  | 4.15.0   | 2A0BD07CFA |
| 10de:0398 | 1025:006c | Nvidia          | G73M [GeForce Go 7600]   | 33.3%  | 5.3.0    | 2D3698DEC2 |
| 10de:0398 | 103c:30bb | Nvidia          | G73M [GeForce Go 7600]   | 55.6%  | 4.15.0   | F39A330574 |
| 10de:0398 | 1179:0001 | Nvidia          | G73M [GeForce Go 7600]   | 100%   |          | 0BAD664989 |
| 10de:0398 | 1179:ff10 | Nvidia          | G73M [GeForce Go 7600]   | 44.4%  | 4.1.25   | 51128D9716 |
| 10de:0398 | 1179:ff31 | Nvidia          | G73M [GeForce Go 7600]   | 66.7%  | 4.18.16  | 9AD8511991 |
| 10de:0398 | 14c0:0020 | Nvidia          | G73M [GeForce Go 7600]   | 16.7%  | 4.1.38   | 41FD098E10 |
| 10de:03d0 | 1025:0153 | Nvidia          | C61 [GeForce 6150SE n... | 40%    | 5.1.0    | A62A5A1516 |
| 10de:03d0 | 1025:0181 | Nvidia          | C61 [GeForce 6150SE n... | 16.7%  | 4.15.0   | 9685CED5FE |
| 10de:03d0 | 1025:0394 | Nvidia          | C61 [GeForce 6150SE n... | 10.3%  | 3.14.44  | 95BCA495A4 |
| 10de:03d0 | 103c:2a6c | Nvidia          | C61 [GeForce 6150SE n... | 11.1%  | 4.1.15   | 4618DD21FE |
| 10de:03d0 | 103c:2a6d | Nvidia          | C61 [GeForce 6150SE n... | 36.4%  | 4.15.0   | 5E5FD822C7 |
| 10de:03d0 | 1043:8234 | Nvidia          | C61 [GeForce 6150SE n... | 11.1%  | 3.14.53  | 7A7933F5D5 |
| 10de:03d0 | 105b:0efe | Nvidia          | C61 [GeForce 6150SE n... | 20%    | 4.15.0   | 8776D239B4 |
| 10de:03d0 | 1458:d000 | Nvidia          | C61 [GeForce 6150SE n... | 7.7%   | 4.1.15   | B9E294218B |
| 10de:03d0 | 1462:7309 | Nvidia          | C61 [GeForce 6150SE n... | 23.1%  | 3.14.44  | DC2D2CA478 |
| 10de:03d0 | 1565:1405 | Nvidia          | C61 [GeForce 6150SE n... | 7.1%   | 3.14.53  | 43719F7617 |
| 10de:03d0 | 1849:03d0 | Nvidia          | C61 [GeForce 6150SE n... | 13.3%  | 4.8.13   | DD876BA784 |
| 10de:03d1 | 1019:2601 | Nvidia          | C61 [GeForce 6100 nFo... | 11.1%  | 4.1.38   | 54B2A67E58 |
| 10de:03d1 | 1019:2609 | Nvidia          | C61 [GeForce 6100 nFo... | 5%     | 4.4.0    | 5343BC19E6 |
| 10de:03d1 | 1462:7309 | Nvidia          | C61 [GeForce 6100 nFo... | 33.3%  | 3.14.44  | AE124F45F6 |
| 10de:03d1 | 1565:1404 | Nvidia          | C61 [GeForce 6100 nFo... | 12.5%  | 4.9.60   | C071FA24D8 |
| 10de:03d6 | 1043:83a4 | Nvidia          | C61 [GeForce 7025 / n... | 9.8%   | 3.14.44  | 9065FDC5CF |
| 10de:03d6 | 1458:d000 | Nvidia          | C61 [GeForce 7025 / n... | 2.6%   | 3.14.44  | 47DEFF8A39 |
| 10de:03d6 | 1462:7597 | Nvidia          | C61 [GeForce 7025 / n... | 37.5%  | 4.1.25   | 916B2D5B72 |
| 10de:03d6 | 1565:1405 | Nvidia          | C61 [GeForce 7025 / n... | 50%    | 4.9.20   | 1E4D89CAFE |
| 10de:03d6 | 1849:03d6 | Nvidia          | C61 [GeForce 7025 / n... | 13.1%  | 3.14.44  | 694D230820 |
| 10de:0400 | 3842:c765 | Nvidia          | G84 [GeForce 8600 GTS]   | 50%    | 5.3.0    | 9E38311ABE |
| 10de:0402 | 1043:8258 | Nvidia          | G84 [GeForce 8600 GT]    | 28.6%  | 4.1.25   | 8CDD8FFE23 |
| 10de:0402 | 10de:0505 | Nvidia          | G84 [GeForce 8600 GT]    | 100%   |          | AB0E072F1E |
| 10de:0402 | 10de:050e | Nvidia          | G84 [GeForce 8600 GT]    | 83.3%  | 4.9.124  | 87142BF4F1 |
| 10de:0402 | 3842:c755 | Nvidia          | G84 [GeForce 8600 GT]    | 33.3%  | 4.1.38   | C7DBE1E979 |
| 10de:0405 | 1043:15d2 | Nvidia          | G84M [GeForce 9500M GS]  | 11.1%  | 3.14.44  | 4137AC8F54 |
| 10de:0407 | 1028:01f2 | Nvidia          | G84M [GeForce 8600M GT]  | 17.6%  | 4.1.15   | 5BBAB2BC27 |
| 10de:0407 | 1028:022e | Nvidia          | G84M [GeForce 8600M GT]  | 4.5%   | 4.9.20   | AE0878FAD3 |
| 10de:0407 | 106b:00a4 | Nvidia          | G84M [GeForce 8600M GT]  | 33.3%  | 5.4.0    | 8FA09C0988 |
| 10de:0407 | 1462:3fad | Nvidia          | G84M [GeForce 8600M GT]  | 50%    | 4.1.15   | DF24AE7647 |
| 10de:040d | 1028:019b | Nvidia          | G84GLM [Quadro FX 1600M] | 6.7%   | 4.4.0    | 5B6CA806FB |
| 10de:040e | 10de:0474 | Nvidia          | G84GL [Quadro FX 570]    | 11.1%  | 4.9.60   | 520EF22702 |
| 10de:040f | 10de:049a | Nvidia          | G84GL [Quadro FX 1700]   | 5.1%   | 4.1.25   | E46F368705 |
| 10de:0421 | 1acc:0857 | Nvidia          | G86 [GeForce 8500 GT]    | 50%    | 4.18.0   | 629F7B490A |
| 10de:0423 | 10de:0494 | Nvidia          | G86 [GeForce 8300 GS]    | 40%    | 4.19.0   | C803923E0B |
| 10de:0425 | 1043:1514 | Nvidia          | G86M [GeForce 8600M GS]  | 40%    | 4.1.19   | 785A42EB5B |
| 10de:0425 | 1734:110c | Nvidia          | G86M [GeForce 8600M GS]  | 50%    | 4.15.0   | 7F69D38EE2 |
| 10de:0426 | 104d:9005 | Nvidia          | G86M [GeForce 8400M GT]  | 50%    | 4.15.0   | 664743C2A1 |
| 10de:0426 | 104d:9016 | Nvidia          | G86M [GeForce 8400M GT]  | 12.5%  | 4.15.0   | B7E36C53A4 |
| 10de:0426 | 104d:9018 | Nvidia          | G86M [GeForce 8400M GT]  | 100%   |          | 8A814A5779 |
| 10de:0427 | 1028:022e | Nvidia          | G86M [GeForce 8400M GS]  | 100%   |          | 95BBC5463F |
| 10de:0427 | 103c:30cd | Nvidia          | G86M [GeForce 8400M GS]  | 50%    | 3.14.44  | 109CAEF651 |
| 10de:0427 | 103c:30cf | Nvidia          | G86M [GeForce 8400M GS]  | 11.1%  | 3.14.53  | 5EDC5F1DD9 |
| 10de:0427 | 104d:9008 | Nvidia          | G86M [GeForce 8400M GS]  | 66.7%  | 4.15.0   | D61D45BA24 |
| 10de:0428 | 1043:1513 | Nvidia          | G86M [GeForce 8400M G]   | 11.1%  | 4.1.15   | E0EEE8D1CC |
| 10de:0428 | 1631:c103 | Nvidia          | G86M [GeForce 8400M G]   | 100%   |          | AFDAAF53BA |
| 10de:0429 | 17aa:20d8 | Nvidia          | G86M [Quadro NVS 140M]   | 3%     | 3.10.42  | CCD11DEBCB |
| 10de:042e | 1043:17c2 | Nvidia          | G86M [GeForce 9300M G]   | 6.2%   | 3.14.33  | 4E30CC5479 |
| 10de:042f | 10de:0492 | Nvidia          | G86 [Quadro NVS 290]     | 8%     | 4.4.0    | 520EF22702 |
| 10de:0531 | 103c:30cf | Nvidia          | C67 [GeForce 7150M / ... | 51.1%  | 4.1.15   | 4D4583E9D7 |
| 10de:0533 | 1025:0126 | Nvidia          | C67 [GeForce 7000M / ... | 13.6%  | 4.1.34   | B79B98D390 |
| 10de:0533 | 1043:1692 | Nvidia          | C67 [GeForce 7000M / ... | 16.7%  | 4.1.15   | 5A1B1F9F7A |
| 10de:0533 | 1631:c106 | Nvidia          | C67 [GeForce 7000M / ... | 100%   |          | BC2AD0771E |
| 10de:053b | 1565:1406 | Nvidia          | C68 [GeForce 7050 PV ... | 50%    | 4.15.0   | 0B8A392B30 |
| 10de:05e2 | 10b0:0801 | Nvidia          | GT200 [GeForce GTX 260]  | 33.3%  | 4.1.25   | 2ACCE8DC12 |
| 10de:05e2 | 3842:1255 | Nvidia          | GT200 [GeForce GTX 260]  | 100%   |          | 947267E711 |
| 10de:0602 | 10de:057c | Nvidia          | G92 [GeForce 8800 GT]    | 42.9%  | 4.15.0   | DA7914FBED |
| 10de:0610 | 1682:2385 | Nvidia          | G92 [GeForce 9600 GSO]   | 40%    | 5.3.0    | DF029EB2A3 |
| 10de:0611 | 10b0:0401 | Nvidia          | G92 [GeForce 8800 GT]    | 33.3%  | 3.14.44  | 2147D0B585 |
| 10de:0611 | 1458:3468 | Nvidia          | G92 [GeForce 8800 GT]    | 50%    | 4.9.9    | 5EF7A4CB4F |
| 10de:0611 | 3842:c802 | Nvidia          | G92 [GeForce 8800 GT]    | 100%   |          | D342FEF56E |
| 10de:0614 | 1043:8314 | Nvidia          | G92 [GeForce 9800 GT]    | 16.7%  | 3.14.44  | A3AFA44F01 |
| 10de:0614 | 10b0:0401 | Nvidia          | G92 [GeForce 9800 GT]    | 8.3%   | 3.14.44  | 5121186A98 |
| 10de:0614 | 1acc:913c | Nvidia          | G92 [GeForce 9800 GT]    | 100%   |          | 530D99F1D6 |
| 10de:0615 | 1458:34e7 | Nvidia          | G92 [GeForce GTS 250]    | 25%    | 3.14.33  | 3EEFCF4B58 |
| 10de:0615 | 19da:1103 | Nvidia          | G92 [GeForce GTS 250]    | 33.3%  | 3.14.44  | 5534D6517F |
| 10de:0615 | 3842:1158 | Nvidia          | G92 [GeForce GTS 250]    | 100%   |          | 0B0B863932 |
| 10de:0618 | 1028:02a1 | Nvidia          | G92M [GeForce GTX 260M]  | 50%    | 5.9.16   | 4A26920858 |
| 10de:061a | 10de:055f | Nvidia          | G92GL [Quadro FX 3700]   | 25%    | 5.3.0    | 2C436DD9BF |
| 10de:0622 | 1043:8304 | Nvidia          | G94 [GeForce 9600 GT]    | 11.1%  | 4.1.13   | CDE1C20A36 |
| 10de:0622 | 10b0:0401 | Nvidia          | G94 [GeForce 9600 GT]    | 16.7%  | 3.14.44  | 3D2F901492 |
| 10de:0622 | 10de:058f | Nvidia          | G94 [GeForce 9600 GT]    | 33.3%  | 4.9.60   | 43C2648D7F |
| 10de:0622 | 1458:3481 | Nvidia          | G94 [GeForce 9600 GT]    | 12.5%  | 4.18.16  | 1610C2FAB2 |
| 10de:0627 | 1462:127b | Nvidia          | G94 [GeForce GT 140]     | 33.3%  | 4.15.0   | 3EF5D8D387 |
| 10de:062f | 10de:060e | Nvidia          | G94 [GeForce 9800 S]     | 100%   |          | D677F0444F |
| 10de:0638 | 10de:062c | Nvidia          | G94GL [Quadro FX 1800]   | 9.1%   | 3.14.44  | 2162A4B852 |
| 10de:0640 |           | Nvidia          | G96C [GeForce 9500 GT]   | 1.8%   | 3.14.44  | 5BFCEDE830 |
| 10de:0640 | 19da:7046 | Nvidia          | G96C [GeForce 9500 GT]   | 5.6%   | 3.14.44  | 4AF0E060E6 |
| 10de:0641 |           | Nvidia          | G96C [GeForce 9400 GT]   | 1.6%   | 4.1.15   | 761D76FE04 |
| 10de:0641 | 10b0:1401 | Nvidia          | G96C [GeForce 9400 GT]   | 50%    | 5.4.0    | 966575FD13 |
| 10de:0641 | 1458:349b | Nvidia          | G96C [GeForce 9400 GT]   | 12.5%  | 3.14.44  | 193ECC62CF |
| 10de:0641 | 1462:1572 | Nvidia          | G96C [GeForce 9400 GT]   | 25%    | 4.9.124  | FE27BC79EE |
| 10de:0641 | 196d:0000 | Nvidia          | G96C [GeForce 9400 GT]   | 100%   |          | 9E63F07AED |
| 10de:0647 | 106b:00a9 | Nvidia          | G96CM [GeForce 9600M GT] | 10%    | 4.9.20   | 238564A9FC |
| 10de:0647 | 106b:00b0 | Nvidia          | G96CM [GeForce 9600M GT] | 66.7%  | 4.9.60   | D2F97E2295 |
| 10de:0647 | 106b:00bc | Nvidia          | G96CM [GeForce 9600M GT] | 16.7%  | 4.18.0   | EF054DD726 |
| 10de:0648 | 152d:0776 | Nvidia          | G96CM [GeForce 9600M GS] | 100%   |          | 705E766496 |
| 10de:0655 | 106b:0633 | Nvidia          | G96 [GeForce GT 120 M... | 16.7%  | 4.18.0   | A3BF786E45 |
| 10de:0659 | 10de:063a | Nvidia          | G96CGL [Quadro FX 580]   | 5.7%   | 4.1.25   | C3C620590F |
| 10de:065b | 1682:236d | Nvidia          | G96C [GeForce 9400 GT]   | 25%    | 5.0.0    | 5B28B44909 |
| 10de:06cd | 19da:1153 | Nvidia          | GF100 [GeForce GTX 470]  | 66.7%  | 4.1.15   | 9B0D9C1623 |
| 10de:06cd | 3842:1470 | Nvidia          | GF100 [GeForce GTX 470]  | 50%    | 4.15.0   | A0225AA660 |
| 10de:06d1 | 10de:0771 | Nvidia          | GF100GL [Tesla C2050 ... | 100%   |          | 1BEF5D0065 |
| 10de:06dd | 103c:0780 | Nvidia          | GF100GL [Quadro 4000]    | 10%    | 4.15.0   | 21308638C4 |
| 10de:06dd | 10de:0780 | Nvidia          | GF100GL [Quadro 4000]    | 9.1%   | 3.14.44  | 330066219D |
| 10de:06e0 | 10de:060c | Nvidia          | G98 [GeForce 9300 GE]    | 20%    | 4.9.111  | 830A379C75 |
| 10de:06e4 |           | Nvidia          | G98 [GeForce 8400 GS ... | 3.2%   | 3.14.44  | 583ACD1F2E |
| 10de:06e4 | 1043:82bc | Nvidia          | G98 [GeForce 8400 GS ... | 50%    | 4.15.0   | 0220656F77 |
| 10de:06e4 | 1458:349c | Nvidia          | G98 [GeForce 8400 GS ... | 100%   |          | 1BB2DCA709 |
| 10de:06e4 | 1462:2060 | Nvidia          | G98 [GeForce 8400 GS ... | 5.9%   | 4.1.25   | 4AC8C18E85 |
| 10de:06e4 | 1462:a165 | Nvidia          | G98 [GeForce 8400 GS ... | 100%   |          | 5E666A6D07 |
| 10de:06e4 | 1682:2354 | Nvidia          | G98 [GeForce 8400 GS ... | 20%    | 4.15.0   | ADF0D7D6E5 |
| 10de:06e4 | 1acc:853d | Nvidia          | G98 [GeForce 8400 GS ... | 20%    | 4.15.0   | DEAF2D6855 |
| 10de:06e8 | 103c:3603 | Nvidia          | G98M [GeForce 9200M GS]  | 37.5%  | 4.9.20   | F5A369D166 |
| 10de:06e9 | 1043:19b2 | Nvidia          | G98M [GeForce 9300M GS]  | 4.7%   | 3.10.34  | 8ABF85E052 |
| 10de:06e9 | 144d:c520 | Nvidia          | G98M [GeForce 9300M GS]  | 100%   |          | F9CD84FA75 |
| 10de:06e9 | 1558:0802 | Nvidia          | G98M [GeForce 9300M GS]  | 33.3%  | 4.9.9    | 44B42FE693 |
| 10de:06eb | 1028:0233 | Nvidia          | G98M [Quadro NVS 160M]   | 3.9%   | 3.14.44  | C7BF47C450 |
| 10de:06ef | 103c:306a | Nvidia          | G98M [GeForce G 103M]    | 12.5%  | 4.1.34   | 7393752623 |
| 10de:07e1 | 1025:0137 | Nvidia          | C73 [GeForce 7100 / n... | 50%    | 5.3.0    | C75B63EB1A |
| 10de:07e1 | 1025:0158 | Nvidia          | C73 [GeForce 7100 / n... | 10%    | 4.9.20   | BEB70C1FC5 |
| 10de:07e1 | 1025:026c | Nvidia          | C73 [GeForce 7100 / n... | 100%   |          | 066559EA13 |
| 10de:07e1 | 103c:2a65 | Nvidia          | C73 [GeForce 7100 / n... | 16.7%  | 3.14.44  | E35C61490A |
| 10de:07e3 | 1019:2145 | Nvidia          | C73 [GeForce 7050 / n... | 20%    | 4.1.15   | C29CA24015 |
| 10de:07e5 | 1025:0137 | Nvidia          | C73 [GeForce 7100 / n... | 50%    | 4.15.0   | B50872CAF4 |
| 10de:0845 | 103c:360a | Nvidia          | C77 [GeForce 8200M G]    | 5.1%   | 3.14.44  | 43E7FDECE6 |
| 10de:0848 | 1043:82e2 | Nvidia          | C77 [GeForce 8300]       | 5.6%   | 3.10.19  | E1B7D175A1 |
| 10de:0849 | 1043:82f2 | Nvidia          | C77 [GeForce 8200]       | 33.3%  | 3.14.44  | A36944300C |
| 10de:084b | 1025:0153 | Nvidia          | C77 [GeForce 8200]       | 28.6%  | 4.15.0   | 9E32F34F8E |
| 10de:0862 | 1028:02a1 | Nvidia          | C79 [GeForce 9400M G]    | 50%    | 5.9.16   | 4A26920858 |
| 10de:0863 | 106b:00aa | Nvidia          | C79 [GeForce 9400M]      | 7.5%   | 4.9.60   | 880E7D527C |
| 10de:0863 | 106b:00ac | Nvidia          | C79 [GeForce 9400M]      | 10%    | 4.9.20   | 238564A9FC |
| 10de:0863 | 106b:00af | Nvidia          | C79 [GeForce 9400M]      | 66.7%  | 4.9.60   | D2F97E2295 |
| 10de:0863 | 106b:00b9 | Nvidia          | C79 [GeForce 9400M]      | 10.5%  | 4.9.60   | E22CD8013E |
| 10de:0863 | 106b:00bb | Nvidia          | C79 [GeForce 9400M]      | 20%    | 4.18.0   | EF054DD726 |
| 10de:0863 | 106b:00bd | Nvidia          | C79 [GeForce 9400M]      | 17.6%  | 4.1.16   | FB5F956CA2 |
| 10de:0866 | 106b:00b1 | Nvidia          | C79 [GeForce 9400M G]    | 5.3%   | 4.1.15   | 1D7D57E70A |
| 10de:0867 | 106b:00ad | Nvidia          | C79 [GeForce 9400]       | 21.1%  | 4.9.20   | 24BB1E05DF |
| 10de:0868 | 103c:2a83 | Nvidia          | C79 [nForce 760i SLI]    | 100%   |          | D677F0444F |
| 10de:0869 | 106b:00b4 | Nvidia          | MCP7A [GeForce 9400]     | 5%     | 3.14.44  | FF93728268 |
| 10de:086c | 1043:8356 | Nvidia          | C79 [GeForce 9300 / n... | 50%    | 4.9.20   | AAF6FAFAD6 |
| 10de:086e | 1462:7621 | Nvidia          | C79 [GeForce 9100M G]    | 11.1%  | 4.9.60   | 70CF4C2F6B |
| 10de:086f | 1043:16b2 | Nvidia          | MCP79 [GeForce 8200M G]  | 100%   |          | 03675A2262 |
| 10de:086f | 1462:71f0 | Nvidia          | MCP79 [GeForce 8200M G]  | 100%   |          | FB8A0F79C4 |
| 10de:0871 | 1028:02b6 | Nvidia          | C79 [GeForce 9200]       | 100%   |          | 85AAFD27C3 |
| 10de:087d | 1043:83e9 | Nvidia          | C79 [ION]                | 50%    | 5.10.14  | 95A54C7D29 |
| 10de:08a0 | 106b:00c2 | Nvidia          | MCP89 [GeForce 320M]     | 11.1%  | 4.8.0    | 6E1DF6E5B2 |
| 10de:08a0 | 106b:00ce | Nvidia          | MCP89 [GeForce 320M]     | 2.9%   | 4.1.15   | 241E284E59 |
| 10de:08a2 | 106b:00d4 | Nvidia          | MCP89 [GeForce 320M]     | 30%    | 4.9.155  | A3168C57EA |
| 10de:08a4 | 106b:00c0 | Nvidia          | MCP89 [GeForce 320M]     | 22.2%  | 4.9.60   | 76695B955A |
| 10de:0a20 | 1043:830f | Nvidia          | GT216 [GeForce GT 220]   | 11.8%  | 3.14.22  | 73DDC0D056 |
| 10de:0a20 | 10b0:0801 | Nvidia          | GT216 [GeForce GT 220]   | 14.3%  | 4.1.38   | 3C402E56A5 |
| 10de:0a20 | 1458:34d6 | Nvidia          | GT216 [GeForce GT 220]   | 9.5%   | 3.14.44  | 517B90D6F4 |
| 10de:0a20 | 174b:2160 | Nvidia          | GT216 [GeForce GT 220]   | 6.2%   | 5.0.0    | 60F738965A |
| 10de:0a20 | 3842:1225 | Nvidia          | GT216 [GeForce GT 220]   | 33.3%  | 4.15.0   | 6542FC1F81 |
| 10de:0a22 | 174b:1141 | Nvidia          | GT216 [GeForce 315]      | 12.5%  | 4.15.0   | 74E55BB86A |
| 10de:0a23 | 1043:833f | Nvidia          | GT216 [GeForce 210]      | 25%    | 4.15.0   | B6E97B7A0E |
| 10de:0a28 | 103c:363c | Nvidia          | GT216M [GeForce GT 230M] | 16.7%  | 4.19.0   | 662A781C83 |
| 10de:0a28 | 103c:7001 | Nvidia          | GT216M [GeForce GT 230M] | 9.1%   | 3.10.34  | 2E7C7E635C |
| 10de:0a2c | 103c:1521 | Nvidia          | GT216M [NVS 5100M]       | 13.3%  | 4.15.0   | 45852B242B |
| 10de:0a2d | 1025:036d | Nvidia          | GT216M [GeForce GT 320M] | 11.8%  | 3.14.44  | 2A4C7DD1D5 |
| 10de:0a34 | 1025:0299 | Nvidia          | GT216M [GeForce GT 240M] | 33.3%  | 4.1.15   | 7B66B4DC9F |
| 10de:0a34 | 1642:3928 | Nvidia          | GT216M [GeForce GT 240M] | 100%   |          | 0921BB94E0 |
| 10de:0a34 | 1734:118d | Nvidia          | GT216M [GeForce GT 240M] | 50%    | 4.1.16   | A54F523EAE |
| 10de:0a38 | 10de:0893 | Nvidia          | GT216GL [Quadro 400]     | 66.7%  | 5.10.13  | 903973759D |
| 10de:0a3c | 1028:040c | Nvidia          | GT216GLM [Quadro FX 8... | 5.9%   | 4.15.0   | 321BF92263 |
| 10de:0a3c | 17aa:2145 | Nvidia          | GT216GLM [Quadro FX 8... | 1.9%   | 4.8.0    | ED0088F25E |
| 10de:0a65 |           | Nvidia          | GT218 [GeForce 210]      | 2.8%   | 3.14.25  | 0F6037A19E |
| 10de:0a65 | 1043:8334 | Nvidia          | GT218 [GeForce 210]      | 3.6%   | 4.1.15   | C26157F6A1 |
| 10de:0a65 | 1043:8354 | Nvidia          | GT218 [GeForce 210]      | 4.1%   | 3.14.44  | E9ACF54209 |
| 10de:0a65 | 1043:847f | Nvidia          | GT218 [GeForce 210]      | 3.7%   | 4.15.0   | F195015CF8 |
| 10de:0a65 | 1043:8490 | Nvidia          | GT218 [GeForce 210]      | 36.4%  | 4.4.0    | 24CFA19EA6 |
| 10de:0a65 | 1043:852d | Nvidia          | GT218 [GeForce 210]      | 3.3%   | 4.4.0    | A242B5B90B |
| 10de:0a65 | 10de:0000 | Nvidia          | GT218 [GeForce 210]      | 16.7%  | 4.15.0   | 50EFF49465 |
| 10de:0a65 | 10de:048b | Nvidia          | GT218 [GeForce 210]      | 28.6%  | 4.9.60   | 662EC4F699 |
| 10de:0a65 | 10de:080a | Nvidia          | GT218 [GeForce 210]      | 8.3%   | 4.9.41   | D48C515893 |
| 10de:0a65 | 1458:34d5 | Nvidia          | GT218 [GeForce 210]      | 14.3%  | 4.1.15   | 83BD0D970C |
| 10de:0a65 | 1458:34d7 | Nvidia          | GT218 [GeForce 210]      | 100%   |          | 916B2D5B72 |
| 10de:0a65 | 1458:3525 | Nvidia          | GT218 [GeForce 210]      | 3.4%   | 4.1.25   | EA3398787C |
| 10de:0a65 | 1458:3629 | Nvidia          | GT218 [GeForce 210]      | 3.8%   | 4.1.15   | 8C3172A9F3 |
| 10de:0a65 | 1462:229d | Nvidia          | GT218 [GeForce 210]      | 100%   |          | 4C42FB5573 |
| 10de:0a65 | 1462:8094 | Nvidia          | GT218 [GeForce 210]      | 4.4%   | 3.14.44  | 290838C751 |
| 10de:0a65 | 19da:7214 | Nvidia          | GT218 [GeForce 210]      | 30%    | 4.9.0    | 88150BC6CD |
| 10de:0a65 | 3842:1215 | Nvidia          | GT218 [GeForce 210]      | 66.7%  | 5.3.0    | 08F4C825CC |
| 10de:0a65 | 3842:1310 | Nvidia          | GT218 [GeForce 210]      | 75%    | 4.9.124  | 8388FBE3B4 |
| 10de:0a65 | 3842:1312 | Nvidia          | GT218 [GeForce 210]      | 3.6%   | 4.1.34   | 7052D8B8E5 |
| 10de:0a65 | 3842:1313 | Nvidia          | GT218 [GeForce 210]      | 8.8%   | 4.1.15   | FA386D9577 |
| 10de:0a66 | 1b0a:9060 | Nvidia          | GT218 [GeForce 310]      | 18.2%  | 4.15.0   | 5C7E0A86DF |
| 10de:0a68 | 144d:c059 | Nvidia          | GT218M [GeForce G 105M]  | 6.7%   | 3.14.44  | 7579CC4303 |
| 10de:0a6c | 1028:040a | Nvidia          | GT218M [NVS 3100M]       | 4.1%   | 4.1.22   | 2DC4747689 |
| 10de:0a6c | 1028:040b | Nvidia          | GT218M [NVS 3100M]       | 18.2%  | 4.9.0    | CA17782E8F |
| 10de:0a6c | 103c:172b | Nvidia          | GT218M [NVS 3100M]       | 10%    | 4.1.15   | 1CE4689041 |
| 10de:0a6c | 17aa:215c | Nvidia          | GT218M [NVS 3100M]       | 14.3%  | 4.15.0   | 41C93BB503 |
| 10de:0a70 | 17aa:396d | Nvidia          | GT218M [GeForce 310M]    | 3.4%   | 3.14.44  | B3A54D7DD5 |
| 10de:0a74 | 1025:0296 | Nvidia          | GT218M [GeForce G210M]   | 60%    | 4.18.0   | 64727A44DB |
| 10de:0a75 | 1043:1c22 | Nvidia          | GT218M [GeForce 310M]    | 27.3%  | 4.9.20   | 4C59EB856A |
| 10de:0a75 | 104d:9067 | Nvidia          | GT218M [GeForce 310M]    | 14.3%  | 5.3.0    | E28ABD6F23 |
| 10de:0a7a | 1179:fc90 | Nvidia          | GT218M [GeForce 315M]    | 8.3%   | 3.14.44  | 38C32074A0 |
| 10de:0ca3 | 1043:8326 | Nvidia          | GT215 [GeForce GT 240]   | 15.4%  | 4.1.25   | 70AC8E5D0B |
| 10de:0ca3 | 1458:34e5 | Nvidia          | GT215 [GeForce GT 240]   | 33.3%  | 4.9.7    | 8F408A7FEC |
| 10de:0ca3 | 196e:0789 | Nvidia          | GT215 [GeForce GT 240]   | 40%    | 4.18.16  | EBA84AFC5E |
| 10de:0ca3 | 1acc:30d3 | Nvidia          | GT215 [GeForce GT 240]   | 20%    | 3.14.44  | 64C8A84081 |
| 10de:0ca5 |           | Nvidia          | GT215 [GeForce GT 220]   | 5.6%   | 3.14.33  | 2B809785CB |
| 10de:0caf | 1028:0443 | Nvidia          | GT215M [GeForce GT 335M] | 14.3%  | 4.1.25   | 931486D93C |
| 10de:0cb1 | 1043:203c | Nvidia          | GT215M [GeForce GTS 3... | 50%    | 5.0.0    | E193018885 |
| 10de:0dc0 | 1462:2310 | Nvidia          | GF106 [GeForce GT 440]   | 100%   |          | 78CE34058B |
| 10de:0dc4 |           | Nvidia          | GF106 [GeForce GTS 450]  | 2.6%   | 3.14.44  | 45EC5E9B13 |
| 10de:0dc6 | 1462:2362 | Nvidia          | GF106 [GeForce GTS 45... | 33.3%  | 4.1.16   | 3FEACD8F08 |
| 10de:0dd1 | 1043:2048 | Nvidia          | GF106M [GeForce GTX 4... | 12.5%  | 4.18.16  | E738441ADB |
| 10de:0dd8 | 103c:084a | Nvidia          | GF106GL [Quadro 2000]    | 16.7%  | 4.9.41   | CED13A5341 |
| 10de:0dd8 | 10de:084a | Nvidia          | GF106GL [Quadro 2000]    | 2.4%   | 3.14.44  | 0AEE9744E0 |
| 10de:0de0 |           | Nvidia          | GF108 [GeForce GT 440]   | 1.4%   | 3.14.44  | 412BBB55C4 |
| 10de:0de0 | 1043:83b7 | Nvidia          | GF108 [GeForce GT 440]   | 20%    | 3.14.44  | C24FEBEB28 |
| 10de:0de0 | 1458:353b | Nvidia          | GF108 [GeForce GT 440]   | 80%    | 4.1.15   | 453120855B |
| 10de:0de1 |           | Nvidia          | GF108 [GeForce GT 430]   | 2.8%   | 3.14.44  | 93671F3ECC |
| 10de:0de1 | 10b0:0401 | Nvidia          | GF108 [GeForce GT 430]   | 6.7%   | 3.14.44  | F8C2960A69 |
| 10de:0de1 | 10de:0828 | Nvidia          | GF108 [GeForce GT 430]   | 22.2%  | 3.14.33  | 7FECBF8628 |
| 10de:0de1 | 1acc:43c1 | Nvidia          | GF108 [GeForce GT 430]   | 100%   |          | E40FE3768D |
| 10de:0de1 | 3842:1335 | Nvidia          | GF108 [GeForce GT 430]   | 33.3%  | 4.18.0   | 3036B319AB |
| 10de:0de2 | 10de:0000 | Nvidia          | GF108 [GeForce GT 420]   | 100%   |          | 330F595A12 |
| 10de:0de2 | 10de:0988 | Nvidia          | GF108 [GeForce GT 420]   | 100%   |          | 2813977A91 |
| 10de:0de2 | 1458:368c | Nvidia          | GF108 [GeForce GT 420]   | 25%    | 4.9.155  | 8E47098AD1 |
| 10de:0dec | 1179:fcd0 | Nvidia          | GF108M [GeForce GT 525M] | 50%    | 5.10.14  | 8F86800C3C |
| 10de:0def | 17aa:21f6 | Nvidia          | GF108M [NVS 5400M]       | 50%    | 5.10.0   | 2D24A0CF83 |
| 10de:0df0 | 104d:907a | Nvidia          | GF108M [GeForce GT 425M] | 13.3%  | 4.15.0   | 961089FAB7 |
| 10de:0df8 | 103c:0835 | Nvidia          | GF108GL [Quadro 600]     | 5.3%   | 4.9.60   | 8ABFAE9D0B |
| 10de:0df8 | 10de:0835 | Nvidia          | GF108GL [Quadro 600]     | 11.8%  | 3.10.0   | 6C5626EE38 |
| 10de:0dfa | 1028:04a3 | Nvidia          | GF108GLM [Quadro 1000M]  | 42.9%  | 4.18.0   | EA97B61280 |
| 10de:0dfa | 103c:1631 | Nvidia          | GF108GLM [Quadro 1000M]  | 8.3%   | 4.18.0   | C5C3EA52C7 |
| 10de:0dfc | 1028:0534 | Nvidia          | GF108GLM [NVS 5200M]     | 33.3%  | 4.15.0   | 303A078ABD |
| 10de:0dfc | 1028:0535 | Nvidia          | GF108GLM [NVS 5200M]     | 20.8%  | 3.14.25  | 059C31B683 |
| 10de:0e22 | 1043:835d | Nvidia          | GF104 [GeForce GTX 460]  | 4.5%   | 3.14.44  | C20498908C |
| 10de:0e22 | 10de:0804 | Nvidia          | GF104 [GeForce GTX 460]  | 100%   |          | CB7598899F |
| 10de:0e22 | 3842:1362 | Nvidia          | GF104 [GeForce GTX 460]  | 25%    | 4.1.15   | F59CE557E1 |
| 10de:0e22 | 3842:1370 | Nvidia          | GF104 [GeForce GTX 460]  | 80%    | 4.15.0   | 001ADC9156 |
| 10de:0e3b | 103c:1630 | Nvidia          | GF104GLM [Quadro 4000M]  | 25%    | 4.15.0   | 59247A25B1 |
| 10de:0f00 |           | Nvidia          | GF108 [GeForce GT 630]   | 20%    | 3.14.25  | 013FDFC708 |
| 10de:0f00 | 1043:8400 | Nvidia          | GF108 [GeForce GT 630]   | 4.8%   | 3.14.25  | 846F436311 |
| 10de:0f00 | 1458:3543 | Nvidia          | GF108 [GeForce GT 630]   | 1.8%   | 3.14.44  | D6AA70D2A0 |
| 10de:0f00 | 1458:3544 | Nvidia          | GF108 [GeForce GT 630]   | 2.4%   | 3.14.44  | CA483B940F |
| 10de:0f00 | 1462:8a90 | Nvidia          | GF108 [GeForce GT 630]   | 5.3%   | 3.14.44  | 64D092BAC7 |
| 10de:0f00 | 19da:5199 | Nvidia          | GF108 [GeForce GT 630]   | 11.1%  | 4.1.15   | 0EEE02F427 |
| 10de:0f00 | 3842:2639 | Nvidia          | GF108 [GeForce GT 630]   | 20%    | 4.18.0   | 1509FC7671 |
| 10de:0f01 | 1043:83fe | Nvidia          | GF108 [GeForce GT 620]   | 16.7%  | 3.14.44  | E12E8BD518 |
| 10de:0f02 |           | Nvidia          | GF108 [GeForce GT 730]   | 6.2%   | 4.9.60   | 8DEBFEF4D1 |
| 10de:0f02 | 1043:84d9 | Nvidia          | GF108 [GeForce GT 730]   | 16.7%  | 3.14.44  | 88C289D589 |
| 10de:0f02 | 1043:84f6 | Nvidia          | GF108 [GeForce GT 730]   | 20%    | 3.14.44  | 93A29298D7 |
| 10de:0f02 | 1043:858e | Nvidia          | GF108 [GeForce GT 730]   | 12.5%  | 4.9.20   | 0EC5C79EB8 |
| 10de:0f02 | 10de:0825 | Nvidia          | GF108 [GeForce GT 730]   | 50%    | 5.4.0    | 9627CF5EEF |
| 10de:0f02 | 10de:8399 | Nvidia          | GF108 [GeForce GT 730]   | 100%   |          | 3CC8E9E496 |
| 10de:0f02 | 1458:365b | Nvidia          | GF108 [GeForce GT 730]   | 6.1%   | 3.14.44  | 19795140C8 |
| 10de:0fc1 | 1043:83f3 | Nvidia          | GK107 [GeForce GT 640]   | 3.2%   | 3.14.44  | 3B6F246900 |
| 10de:0fc2 | 10de:093c | Nvidia          | GK107 [GeForce GT 630... | 50%    | 4.9.20   | 84224B6ADA |
| 10de:0fc6 |           | Nvidia          | GK107 [GeForce GTX 650]  | 25%    | 4.1.15   | CDEAE8E065 |
| 10de:0fc6 | 1043:8427 | Nvidia          | GK107 [GeForce GTX 650]  | 10%    | 3.14.44  | 4E0DC79606 |
| 10de:0fc6 | 10b0:0fc6 | Nvidia          | GK107 [GeForce GTX 650]  | 7.7%   | 3.14.33  | 41FA59AD16 |
| 10de:0fc6 | 10de:0973 | Nvidia          | GK107 [GeForce GTX 650]  | 1.1%   | 3.10.51  | CF8A32D6BF |
| 10de:0fc6 | 1458:3555 | Nvidia          | GK107 [GeForce GTX 650]  | 9.7%   | 3.14.13  | FE2C088EA6 |
| 10de:0fc6 | 1462:2802 | Nvidia          | GK107 [GeForce GTX 650]  | 28.6%  | 4.18.0   | 128A90D3B7 |
| 10de:0fc6 | 1462:8a96 | Nvidia          | GK107 [GeForce GTX 650]  | 3%     | 3.14.44  | 1A53A82660 |
| 10de:0fc6 | 19da:1288 | Nvidia          | GK107 [GeForce GTX 650]  | 50%    | 4.9.60   | E6F9B2CF07 |
| 10de:0fc6 | 3842:2650 | Nvidia          | GK107 [GeForce GTX 650]  | 50%    | 4.15.0   | 9E45B155AC |
| 10de:0fc8 | 1043:84d8 | Nvidia          | GK107 [GeForce GT 740]   | 6.7%   | 4.1.15   | A1AF850C30 |
| 10de:0fc8 | 1458:3654 | Nvidia          | GK107 [GeForce GT 740]   | 18.2%  | 4.9.20   | 2A545CAC20 |
| 10de:0fcd | 17aa:3800 | Nvidia          | GK107M [GeForce GT 755M] | 16.7%  | 5.0.0    | 01CCFAFE86 |
| 10de:0fea | 106b:011f | Nvidia          | GK107M [GeForce GT 75... | 66.7%  | 5.2.11   | 58432EB50F |
| 10de:0ff3 | 10de:1162 | Nvidia          | GK107GL [Quadro K420]    | 25%    | 4.9.76   | BEA2C0B6F8 |
| 10de:0ffa | 103c:094b | Nvidia          | GK107GL [Quadro K600]    | 7.7%   | 4.9.0    | 5B3AF441AE |
| 10de:0ffa | 10de:094b | Nvidia          | GK107GL [Quadro K600]    | 25%    | 4.1.15   | EB3B40AD4F |
| 10de:100a | 1462:2983 | Nvidia          | GK110B [GeForce GTX 7... | 100%   |          | 91D43B6213 |
| 10de:102d | 10de:106c | Nvidia          | GK210GL [Tesla K80]      | 100%   |          | 33281F109C |
| 10de:1040 | 1043:83a0 | Nvidia          | GF119 [GeForce GT 520]   | 6.7%   | 3.14.44  | 17392A1FE7 |
| 10de:1040 | 10de:0000 | Nvidia          | GF119 [GeForce GT 520]   | 6.2%   | 4.1.38   | F6B55F7969 |
| 10de:1040 | 10de:0915 | Nvidia          | GF119 [GeForce GT 520]   | 16.7%  | 4.15.0   | C05FF50573 |
| 10de:1040 | 1462:2630 | Nvidia          | GF119 [GeForce GT 520]   | 7.7%   | 3.14.15  | C1F02780E4 |
| 10de:1040 | 174b:3214 | Nvidia          | GF119 [GeForce GT 520]   | 14.3%  | 4.9.60   | 610EB308AC |
| 10de:1040 | 19da:1222 | Nvidia          | GF119 [GeForce GT 520]   | 20%    | 3.14.44  | 26CB6EBFBB |
| 10de:1049 | 10de:0977 | Nvidia          | GF119 [GeForce GT 620... | 18.2%  | 4.1.25   | 11D88B0256 |
| 10de:104a |           | Nvidia          | GF119 [GeForce GT 610]   | 33.3%  | 4.9.60   | 016D2F25A7 |
| 10de:104a | 1043:840d | Nvidia          | GF119 [GeForce GT 610]   | 8.3%   | 3.14.15  | 6F49C2288D |
| 10de:104a | 1043:8411 | Nvidia          | GF119 [GeForce GT 610]   | 66.7%  | 4.15.0   | 9E30F90134 |
| 10de:104a | 1462:809f | Nvidia          | GF119 [GeForce GT 610]   | 2.1%   | 3.14.44  | 114E38FD23 |
| 10de:104a | 196e:104a | Nvidia          | GF119 [GeForce GT 610]   | 7.7%   | 3.14.53  | 4A237E25C2 |
| 10de:104a | 19da:2219 | Nvidia          | GF119 [GeForce GT 610]   | 100%   |          | 6E35626719 |
| 10de:104a | 19da:5228 | Nvidia          | GF119 [GeForce GT 610]   | 100%   |          | FF621CB51A |
| 10de:104a | 19da:6222 | Nvidia          | GF119 [GeForce GT 610]   | 9.5%   | 4.1.16   | EC33C42906 |
| 10de:104c | 1462:b593 | Nvidia          | GF119 [GeForce GT 705]   | 100%   |          | E999E28C5B |
| 10de:1055 | 104d:908b | Nvidia          | GF119M [GeForce 410M]    | 1.4%   | 3.14.44  | D304BAAD85 |
| 10de:1056 | 1028:0494 | Nvidia          | GF119M [NVS 4200M]       | 14.3%  | 3.14.44  | 132C1F74FC |
| 10de:1058 | 1043:8536 | Nvidia          | GF119M [GeForce 610M]    | 40%    | 4.1.22   | C3694759D1 |
| 10de:107c | 10de:102f | Nvidia          | GF119 [NVS 315]          | 10%    | 4.18.0   | 9E55C4BDEE |
| 10de:107d | 10de:094e | Nvidia          | GF119 [NVS 310]          | 33.3%  | 4.15.0   | 90871ECFF1 |
| 10de:1081 | 10de:087e | Nvidia          | GF110 [GeForce GTX 570]  | 14.3%  | 3.14.44  | 3A3874784C |
| 10de:1086 | 1043:8387 | Nvidia          | GF110 [GeForce GTX 57... | 20%    | 3.14.22  | 6AFCF2F51C |
| 10de:1086 | 1462:2571 | Nvidia          | GF110 [GeForce GTX 57... | 50%    | 5.8.0    | 3717F79D0B |
| 10de:10d8 | 103c:0862 | Nvidia          | GT218 [NVS 300]          | 16.7%  | 4.15.0   | 4F9670DA15 |
| 10de:1183 | 1043:841f | Nvidia          | GK104 [GeForce GTX 66... | 33.3%  | 4.9.20   | 6CB5707322 |
| 10de:1184 | 3842:3778 | Nvidia          | GK104 [GeForce GTX 770]  | 100%   |          | C22EF5B009 |
| 10de:1185 | 1462:2841 | Nvidia          | GK104 [GeForce GTX 66... | 50%    | 5.4.0    | D4FC6A6F52 |
| 10de:1187 | 3842:2768 | Nvidia          | GK104 [GeForce GTX 760]  | 100%   |          | FC4C28F995 |
| 10de:119e | 106b:0121 | Nvidia          | GK104M [GeForce GTX 7... | 33.3%  | 5.4.0    | D53F359250 |
| 10de:119f | 1043:213e | Nvidia          | GK104M [GeForce GTX 7... | 20%    | 4.4.0    | 30FBA8E75C |
| 10de:11c0 | 1043:8422 | Nvidia          | GK106 [GeForce GTX 660]  | 4.2%   | 3.14.33  | 4C444B85D5 |
| 10de:11c0 | 1043:843b | Nvidia          | GK106 [GeForce GTX 660]  | 10%    | 3.14.44  | B197E3E4CC |
| 10de:11c2 | 3842:3656 | Nvidia          | GK106 [GeForce GTX 65... | 100%   |          | B96B88613A |
| 10de:11c6 | 1043:8446 | Nvidia          | GK106 [GeForce GTX 65... | 18.2%  | 3.14.44  | 3730F9BE71 |
| 10de:11c8 | 1569:11c8 | Nvidia          | GK106 [GeForce GTX 65... | 6.2%   | 4.1.15   | CE85A9AD63 |
| 10de:11e0 | 1043:21bb | Nvidia          | GK106M [GeForce GTX 7... | 100%   |          | E10390E908 |
| 10de:11fa | 10de:097c | Nvidia          | GK106GL [Quadro K4000]   | 16.7%  | 4.18.16  | 088A4C0DEC |
| 10de:1200 | 1043:838b | Nvidia          | GF114 [GeForce GTX 56... | 18.2%  | 3.14.44  | 5C1D6C3562 |
| 10de:1200 | 1043:83ac | Nvidia          | GF114 [GeForce GTX 56... | 75%    | 4.18.0   | A2755006BE |
| 10de:1200 | 10b0:0801 | Nvidia          | GF114 [GeForce GTX 56... | 100%   |          | 02FFA180C8 |
| 10de:1200 | 19da:1209 | Nvidia          | GF114 [GeForce GTX 56... | 33.3%  | 3.14.44  | C96ED1C03E |
| 10de:1200 | 19da:4227 | Nvidia          | GF114 [GeForce GTX 56... | 100%   |          | F7FD155DD3 |
| 10de:1200 | 3842:1568 | Nvidia          | GF114 [GeForce GTX 56... | 100%   |          | A623E40CE4 |
| 10de:1208 | 1462:232a | Nvidia          | GF114 [GeForce GTX 56... | 50%    | 4.9.60   | BAEFCCEA96 |
| 10de:1210 | 1462:10bd | Nvidia          | GF114M [GeForce GTX 5... | 11.1%  | 4.1.15   | 7CEA76DF9B |
| 10de:1213 | 1043:2119 | Nvidia          | GF114M [GeForce GTX 6... | 14.3%  | 3.14.15  | CC1A212C60 |
| 10de:1244 |           | Nvidia          | GF116 [GeForce GTX 55... | 4.1%   | 3.14.44  | 3736215480 |
| 10de:1244 | 1043:83be | Nvidia          | GF116 [GeForce GTX 55... | 3.8%   | 3.14.44  | 87FA5760D1 |
| 10de:1244 | 1043:83c2 | Nvidia          | GF116 [GeForce GTX 55... | 5%     | 3.14.44  | 61C80798A5 |
| 10de:1244 | 1458:351a | Nvidia          | GF116 [GeForce GTX 55... | 22.2%  | 3.14.44  | 99C4748650 |
| 10de:1244 | 1462:2612 | Nvidia          | GF116 [GeForce GTX 55... | 11.1%  | 4.9.60   | 5B7AE4F768 |
| 10de:1244 | 1462:809d | Nvidia          | GF116 [GeForce GTX 55... | 25%    | 3.14.44  | 0842ADE22D |
| 10de:1244 | 174b:5194 | Nvidia          | GF116 [GeForce GTX 55... | 33.3%  | 5.4.28   | 84DF613461 |
| 10de:1244 | 196e:089c | Nvidia          | GF116 [GeForce GTX 55... | 100%   |          | A425AB20CA |
| 10de:1244 | 1acc:55a1 | Nvidia          | GF116 [GeForce GTX 55... | 100%   |          | 6C3F49421D |
| 10de:1244 | 1b0a:90a2 | Nvidia          | GF116 [GeForce GTX 55... | 33.3%  | 4.1.16   | 1F9450CF86 |
| 10de:1244 | 3842:1556 | Nvidia          | GF116 [GeForce GTX 55... | 25%    | 4.15.0   | 8094FDE100 |
| 10de:1244 | 3842:1557 | Nvidia          | GF116 [GeForce GTX 55... | 100%   |          | 33B473FD04 |
| 10de:1244 | 3842:1559 | Nvidia          | GF116 [GeForce GTX 55... | 16.7%  | 4.18.0   | 0E49C860E0 |
| 10de:1244 | 3842:2059 | Nvidia          | GF116 [GeForce GTX 55... | 100%   |          | 3BE6CEF510 |
| 10de:1245 |           | Nvidia          | GF116 [GeForce GTS 45... | 2%     | 3.14.39  | 41C215F59C |
| 10de:1245 | 10b0:0401 | Nvidia          | GF116 [GeForce GTS 45... | 4.3%   | 3.10.34  | 38906FFC03 |
| 10de:1245 | 3842:1351 | Nvidia          | GF116 [GeForce GTS 45... | 100%   |          | 385BAE92A5 |
| 10de:1251 | 10de:0000 | Nvidia          | GF116M [GeForce GT 560M] | 100%   |          | BBF8BA233B |
| 10de:1284 | 1043:8461 | Nvidia          | GK208 [GeForce GT 630... | 10%    | 3.14.44  | 9B458CFF70 |
| 10de:1286 | 1462:2928 | Nvidia          | GK208 [GeForce GT 720]   | 40%    | 5.0.0    | B0C02D52C9 |
| 10de:1287 | 1043:84f5 | Nvidia          | GK208B [GeForce GT 730]  | 35.7%  | 4.1.16   | 5D93D067D7 |
| 10de:1287 | 1043:8501 | Nvidia          | GK208B [GeForce GT 730]  | 10%    | 4.1.15   | 930D8056C3 |
| 10de:1287 | 1043:850c | Nvidia          | GK208B [GeForce GT 730]  | 20%    | 4.15.0   | 6CF789DF63 |
| 10de:1287 | 1043:858b | Nvidia          | GK208B [GeForce GT 730]  | 100%   |          | 60C99711B8 |
| 10de:1287 | 10de:1083 | Nvidia          | GK208B [GeForce GT 730]  | 33.3%  | 4.9.60   | 5E5919C697 |
| 10de:1287 | 10de:1287 | Nvidia          | GK208B [GeForce GT 730]  | 13.8%  | 4.1.25   | 8286FE4F06 |
| 10de:1287 | 1642:3e56 | Nvidia          | GK208B [GeForce GT 730]  | 20%    | 4.9.60   | 2F126B4841 |
| 10de:1287 | 19da:730b | Nvidia          | GK208B [GeForce GT 730]  | 5%     | 4.9.60   | 355600CF2F |
| 10de:1288 | 1462:8c90 | Nvidia          | GK208B [GeForce GT 720]  | 26.7%  | 4.1.15   | 665E2E1F1B |
| 10de:1288 | 1569:1288 | Nvidia          | GK208B [GeForce GT 720]  | 50%    | 4.9.60   | 7E9CD09A5D |
| 10de:1288 | 19da:720a | Nvidia          | GK208B [GeForce GT 720]  | 40%    | 4.15.0   | AD88B9D524 |
| 10de:128b | 1043:8572 | Nvidia          | GK208B [GeForce GT 710]  | 3.6%   | 4.1.25   | 7902B95176 |
| 10de:128b | 1043:85f7 | Nvidia          | GK208B [GeForce GT 710]  | 13.3%  | 4.9.60   | A628F16E75 |
| 10de:128b | 1043:86df | Nvidia          | GK208B [GeForce GT 710]  | 20%    | 4.15.0   | 585A8B80A8 |
| 10de:128b | 10de:118b | Nvidia          | GK208B [GeForce GT 710]  | 5.9%   | 4.9.0    | 872ADD2D9C |
| 10de:128b | 10de:128b | Nvidia          | GK208B [GeForce GT 710]  | 4.2%   | 4.9.20   | 5F0D30FFA0 |
| 10de:128b | 1458:36f7 | Nvidia          | GK208B [GeForce GT 710]  | 9.1%   | 4.1.25   | A3EF9588AD |
| 10de:128b | 1458:375a | Nvidia          | GK208B [GeForce GT 710]  | 8.3%   | 4.9.155  | 509ECC6BFA |
| 10de:128b | 1458:375b | Nvidia          | GK208B [GeForce GT 710]  | 33.3%  | 4.15.0   | 8D923C87E6 |
| 10de:128b | 1458:376c | Nvidia          | GK208B [GeForce GT 710]  | 5%     | 4.9.155  | D1A51A8680 |
| 10de:128b | 1462:8c93 | Nvidia          | GK208B [GeForce GT 710]  | 3.1%   | 4.9.0    | A77184C9C7 |
| 10de:1380 | 1019:1028 | Nvidia          | GM107 [GeForce GTX 75... | 66.7%  | 5.4.0    | A4A5ED082D |
| 10de:1380 | 1043:84bb | Nvidia          | GM107 [GeForce GTX 75... | 11.6%  | 4.4.0    | 6400689A90 |
| 10de:1380 | 1043:84bc | Nvidia          | GM107 [GeForce GTX 75... | 16.7%  | 4.1.25   | 59CCFFE44E |
| 10de:1380 | 10de:0401 | Nvidia          | GM107 [GeForce GTX 75... | 25%    | 4.18.16  | 08FBE2F45C |
| 10de:1380 | 10de:8412 | Nvidia          | GM107 [GeForce GTX 75... | 100%   |          | 3A624021F2 |
| 10de:1380 | 1458:362d | Nvidia          | GM107 [GeForce GTX 75... | 18.8%  | 4.1.25   | 84A36237D0 |
| 10de:1380 | 1458:3667 | Nvidia          | GM107 [GeForce GTX 75... | 25%    | 4.9.20   | EEB7663AF0 |
| 10de:1380 | 1462:3102 | Nvidia          | GM107 [GeForce GTX 75... | 11.1%  | 4.1.15   | 6158505A7F |
| 10de:1380 | 1642:3e32 | Nvidia          | GM107 [GeForce GTX 75... | 25%    | 4.15.0   | E5BFC5E8A5 |
| 10de:1380 | 1acc:752e | Nvidia          | GM107 [GeForce GTX 75... | 100%   |          | 356C1804FA |
| 10de:1381 | 1019:1026 | Nvidia          | GM107 [GeForce GTX 750]  | 100%   |          | 90BFCE836F |
| 10de:1381 | 1043:84f0 | Nvidia          | GM107 [GeForce GTX 750]  | 9.1%   | 4.1.15   | 8E80E31C5C |
| 10de:1381 | 10de:1073 | Nvidia          | GM107 [GeForce GTX 750]  | 9.1%   | 4.9.20   | 02666C5333 |
| 10de:1381 | 1458:362e | Nvidia          | GM107 [GeForce GTX 750]  | 36.4%  | 4.1.16   | FED7D6BB61 |
| 10de:1381 | 1458:3642 | Nvidia          | GM107 [GeForce GTX 750]  | 9.1%   | 4.1.15   | 8276D533D6 |
| 10de:1381 | 1462:8a9c | Nvidia          | GM107 [GeForce GTX 750]  | 31.8%  | 4.1.25   | 0000FF019E |
| 10de:13b1 | 17aa:2230 | Nvidia          | GM107GLM [Quadro M1000M] | 33.3%  | 4.18.0   | 3908B619CA |
| 10de:13b6 | 1028:17b0 | Nvidia          | GM107GLM [Quadro M120... | 100%   |          | 9C4C70327E |
| 10de:13bb | 103c:1098 | Nvidia          | GM107GL [Quadro K620]    | 20%    | 5.3.0    | E5B45EED8D |
| 10de:13bb | 10de:1098 | Nvidia          | GM107GL [Quadro K620]    | 11.1%  | 4.13.0   | A0294F08B7 |
| 10de:13c0 | 1043:8506 | Nvidia          | GM204 [GeForce GTX 980]  | 100%   |          | 3063855C7C |
| 10de:13c2 |           | Nvidia          | GM204 [GeForce GTX 970]  | 66.7%  | 5.4.0    | 10CE1EF592 |
| 10de:13c2 | 1019:1029 | Nvidia          | GM204 [GeForce GTX 970]  | 100%   |          | F39DBBFB9A |
| 10de:13c2 | 1043:8508 | Nvidia          | GM204 [GeForce GTX 970]  | 7.4%   | 4.15.0   | 5A72089FCC |
| 10de:13c2 | 10de:1131 | Nvidia          | GM204 [GeForce GTX 970]  | 40%    | 4.1.15   | 4CC243C7EF |
| 10de:13c2 | 1458:367a | Nvidia          | GM204 [GeForce GTX 970]  | 5%     | 4.1.15   | 3E15147646 |
| 10de:13c2 | 1458:367b | Nvidia          | GM204 [GeForce GTX 970]  | 33.3%  | 5.4.0    | 37FD9139AF |
| 10de:13c2 | 1462:3160 | Nvidia          | GM204 [GeForce GTX 970]  | 3.8%   | 4.15.0   | 7980C33879 |
| 10de:13c2 | 19da:1366 | Nvidia          | GM204 [GeForce GTX 970]  | 36.4%  | 4.15.0   | 68C2299CCC |
| 10de:13c2 | 19da:2370 | Nvidia          | GM204 [GeForce GTX 970]  | 100%   |          | 143214DBAB |
| 10de:13c2 | 3842:2974 | Nvidia          | GM204 [GeForce GTX 970]  | 11.1%  | 4.15.0   | 3251848CE3 |
| 10de:13c2 | 3842:2978 | Nvidia          | GM204 [GeForce GTX 970]  | 20%    | 4.1.15   | 3251848CE3 |
| 10de:13f1 | 10de:1153 | Nvidia          | GM204GL [Quadro M4000]   | 25%    | 5.4.0    | B8D85B966B |
| 10de:1401 |           | Nvidia          | GM206 [GeForce GTX 960]  | 50%    | 4.15.0   | 653A2DFA38 |
| 10de:1401 | 1043:8520 | Nvidia          | GM206 [GeForce GTX 960]  | 5.9%   | 4.9.20   | 7114DE29ED |
| 10de:1401 | 1043:8526 | Nvidia          | GM206 [GeForce GTX 960]  | 50%    | 5.4.0    | 05A4F713EA |
| 10de:1401 | 1043:8678 | Nvidia          | GM206 [GeForce GTX 960]  | 40%    | 5.4.0    | 0966F43D9E |
| 10de:1401 | 1458:36aa | Nvidia          | GM206 [GeForce GTX 960]  | 100%   |          | 1CFE050B29 |
| 10de:1401 | 1458:36ad | Nvidia          | GM206 [GeForce GTX 960]  | 50%    | 5.0.0    | A8A89AC09A |
| 10de:1401 | 1458:36b0 | Nvidia          | GM206 [GeForce GTX 960]  | 100%   |          | B99D4A956B |
| 10de:1401 | 1458:36be | Nvidia          | GM206 [GeForce GTX 960]  | 10%    | 4.9.60   | DA333CA37B |
| 10de:1401 | 1462:3202 | Nvidia          | GM206 [GeForce GTX 960]  | 11.8%  | 4.1.15   | 1532D55BA0 |
| 10de:1401 | 1462:3205 | Nvidia          | GM206 [GeForce GTX 960]  | 6.7%   | 4.18.16  | 7D2485C593 |
| 10de:1401 | 196e:1138 | Nvidia          | GM206 [GeForce GTX 960]  | 28.6%  | 4.15.0   | C94384F620 |
| 10de:1401 | 3842:2966 | Nvidia          | GM206 [GeForce GTX 960]  | 25%    | 5.4.0    | 33DA9C195D |
| 10de:1406 | 1028:072b | Nvidia          | GM206 [GeForce GTX 96... | 100%   |          | 4B9D75483A |
| 10de:1427 | 1558:1502 | Nvidia          | GM206M [GeForce GTX 9... | 100%   |          | B551F83C2C |
| 10de:1617 | 1043:1ced | Nvidia          | GM204M [GeForce GTX 9... | 25%    | 4.18.16  | 6BCCA7D246 |
| 10de:1619 | 1043:1ced | Nvidia          | GM204M [GeForce GTX 9... | 33.3%  | 5.3.0    | 670040946B |
| 10de:17c2 | 10de:1132 | Nvidia          | GM200 [GeForce GTX TI... | 33.3%  | 5.7.5    | 2369E0376D |
| 10de:1b06 | 1043:85e2 | Nvidia          | GP102 [GeForce GTX 10... | 33.3%  | 5.5.15   | 5D1A48EE4E |
| 10de:1b06 | 1458:374c | Nvidia          | GP102 [GeForce GTX 10... | 40%    | 4.18.16  | E1EBFFB1F6 |
| 10de:1b06 | 1458:3752 | Nvidia          | GP102 [GeForce GTX 10... | 20%    | 5.0.0    | 5B7738AF52 |
| 10de:1b06 | 3842:6696 | Nvidia          | GP102 [GeForce GTX 10... | 36.4%  | 4.18.0   | 9FBBF0498F |
| 10de:1b80 | 1043:8592 | Nvidia          | GP104 [GeForce GTX 1080] | 66.7%  | 4.15.0   | 925EC1C4FD |
| 10de:1b80 | 1043:859b | Nvidia          | GP104 [GeForce GTX 1080] | 25%    | 4.15.0   | CFA898D2DF |
| 10de:1b80 | 10de:1b80 | Nvidia          | GP104 [GeForce GTX 1080] | 16.7%  | 4.18.0   | F7D08CE703 |
| 10de:1b80 | 1458:3717 | Nvidia          | GP104 [GeForce GTX 1080] | 33.3%  | 4.15.0   | 4723903BE4 |
| 10de:1b80 | 1462:3367 | Nvidia          | GP104 [GeForce GTX 1080] | 25%    | 4.12.14  | A81EFB1774 |
| 10de:1b80 | 3842:5180 | Nvidia          | GP104 [GeForce GTX 1080] | 100%   |          | 31BF3FAE67 |
| 10de:1b80 | 4426:19da | Nvidia          | GP104 [GeForce GTX 1080] | 100%   |          | 3F63AB158D |
| 10de:1b81 |           | Nvidia          | GP104 [GeForce GTX 1070] | 50%    | 4.9.20   | D326BF619F |
| 10de:1b81 | 1043:8597 | Nvidia          | GP104 [GeForce GTX 1070] | 50%    | 5.8.0    | 90D8E62525 |
| 10de:1b81 | 1043:8598 | Nvidia          | GP104 [GeForce GTX 1070] | 20%    | 4.15.0   | 7CE03AF897 |
| 10de:1b81 | 1043:859f | Nvidia          | GP104 [GeForce GTX 1070] | 100%   |          | D68BCE418A |
| 10de:1b81 | 1043:85a0 | Nvidia          | GP104 [GeForce GTX 1070] | 16.7%  | 4.15.0   | 42E012B0E1 |
| 10de:1b81 | 10b0:1b81 | Nvidia          | GP104 [GeForce GTX 1070] | 100%   |          | 8FB6824328 |
| 10de:1b81 | 1458:36fc | Nvidia          | GP104 [GeForce GTX 1070] | 33.3%  | 4.9.20   | CD8505D488 |
| 10de:1b81 | 19da:1435 | Nvidia          | GP104 [GeForce GTX 1070] | 33.3%  | 5.9.11   | 2FB0F5003D |
| 10de:1b81 | 3842:6173 | Nvidia          | GP104 [GeForce GTX 1070] | 20%    | 5.9.15   | D6318C05CD |
| 10de:1b81 | 3842:6276 | Nvidia          | GP104 [GeForce GTX 1070] | 66.7%  | 4.15.0   | 2162A4B852 |
| 10de:1b82 | 1043:861d | Nvidia          | GP104 [GeForce GTX 10... | 100%   |          | B03C78FE4F |
| 10de:1b82 | 1043:8623 | Nvidia          | GP104 [GeForce GTX 10... | 33.3%  | 5.0.0    | 510B031CE9 |
| 10de:1b82 | 1462:c307 | Nvidia          | GP104 [GeForce GTX 10... | 50%    | 5.4.0    | 17BCC983CA |
| 10de:1b82 | 19da:2445 | Nvidia          | GP104 [GeForce GTX 10... | 33.3%  | 5.2.4    | B499AA651F |
| 10de:1b82 | 3842:5671 | Nvidia          | GP104 [GeForce GTX 10... | 14.3%  | 4.15.0   | BFDE779CB2 |
| 10de:1bb1 | 1028:11a3 | Nvidia          | GP104GL [Quadro P4000]   | 100%   |          | 52B7CECCFF |
| 10de:1be1 | 103c:846a | Nvidia          | GP104BM [GeForce GTX ... | 100%   |          | 28EE5CFE8C |
| 10de:1be1 | 1043:1470 | Nvidia          | GP104BM [GeForce GTX ... | 16.7%  | 4.18.0   | D1FEF3959B |
| 10de:1be1 | 1043:1660 | Nvidia          | GP104BM [GeForce GTX ... | 40%    | 5.3.0    | 21CC811FE0 |
| 10de:1be1 | 1462:11ff | Nvidia          | GP104BM [GeForce GTX ... | 50%    | 5.3.0    | C2E855B5BC |
| 10de:1be1 | 1558:67a4 | Nvidia          | GP104BM [GeForce GTX ... | 33.3%  | 4.18.0   | ADFAFBA25E |
| 10de:1c02 |           | Nvidia          | GP106 [GeForce GTX 10... | 53.8%  | 4.15.0   | A248371C4D |
| 10de:1c02 | 103c:82fc | Nvidia          | GP106 [GeForce GTX 10... | 50%    | 4.15.0   | B084532F5D |
| 10de:1c02 | 1043:85b1 | Nvidia          | GP106 [GeForce GTX 10... | 33.3%  | 4.15.0   | 39F3C43A6B |
| 10de:1c02 | 1043:85b9 | Nvidia          | GP106 [GeForce GTX 10... | 16.7%  | 4.15.0   | A0E30E712F |
| 10de:1c02 | 10de:11c2 | Nvidia          | GP106 [GeForce GTX 10... | 20%    | 4.15.0   | 85E312192E |
| 10de:1c02 | 10de:1c02 | Nvidia          | GP106 [GeForce GTX 10... | 21.4%  | 4.15.0   | 2C46451B47 |
| 10de:1c02 | 1458:3722 | Nvidia          | GP106 [GeForce GTX 10... | 2.9%   | 4.15.0   | CC9A8D1703 |
| 10de:1c02 | 1458:3724 | Nvidia          | GP106 [GeForce GTX 10... | 17.5%  | 4.15.0   | C74C010C1B |
| 10de:1c02 | 1462:3287 | Nvidia          | GP106 [GeForce GTX 10... | 3.8%   | 4.13.0   | CCB4D48D08 |
| 10de:1c02 | 1462:8c95 | Nvidia          | GP106 [GeForce GTX 10... | 37.5%  | 4.18.16  | 778D35D82D |
| 10de:1c02 | 3842:6162 | Nvidia          | GP106 [GeForce GTX 10... | 50%    | 4.18.16  | B58089CDC0 |
| 10de:1c03 |           | Nvidia          | GP106 [GeForce GTX 10... | 16.7%  | 4.15.0   | 8FC4603F6C |
| 10de:1c03 | 1043:85a4 | Nvidia          | GP106 [GeForce GTX 10... | 12.5%  | 4.15.0   | 725B24FE69 |
| 10de:1c03 | 1043:85a6 | Nvidia          | GP106 [GeForce GTX 10... | 50%    | 5.4.0    | EB6CD37E93 |
| 10de:1c03 | 1043:85ab | Nvidia          | GP106 [GeForce GTX 10... | 66.7%  | 5.4.0    | 8A1C4909D6 |
| 10de:1c03 | 1043:85ae | Nvidia          | GP106 [GeForce GTX 10... | 60%    | 5.4.0    | 5385F57036 |
| 10de:1c03 | 1043:85e0 | Nvidia          | GP106 [GeForce GTX 10... | 16.7%  | 4.18.16  | 2C9527A545 |
| 10de:1c03 | 10de:0401 | Nvidia          | GP106 [GeForce GTX 10... | 75%    | 5.3.0    | B7ED1BD518 |
| 10de:1c03 | 10de:0921 | Nvidia          | GP106 [GeForce GTX 10... | 28.6%  | 5.4.0    | 975CF16BE2 |
| 10de:1c03 | 10de:1c03 | Nvidia          | GP106 [GeForce GTX 10... | 17.6%  | 4.15.0   | 186DBB4515 |
| 10de:1c03 | 1458:3716 | Nvidia          | GP106 [GeForce GTX 10... | 16.7%  | 4.15.0   | 8E3EE6F0BA |
| 10de:1c03 | 1458:371a | Nvidia          | GP106 [GeForce GTX 10... | 6.2%   | 4.15.0   | 740AB53EE9 |
| 10de:1c03 | 1458:3739 | Nvidia          | GP106 [GeForce GTX 10... | 25%    | 4.15.0   | 1DDF0EC6EC |
| 10de:1c03 | 1458:3776 | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | 28D68A2C46 |
| 10de:1c03 | 1462:3281 | Nvidia          | GP106 [GeForce GTX 10... | 15.8%  | 4.15.0   | E044F153CE |
| 10de:1c03 | 1462:3283 | Nvidia          | GP106 [GeForce GTX 10... | 3.6%   | 4.13.0   | 9043D81B30 |
| 10de:1c03 | 196e:119f | Nvidia          | GP106 [GeForce GTX 10... | 50%    | 5.0.0    | 8ED2B2284E |
| 10de:1c03 | 19da:1438 | Nvidia          | GP106 [GeForce GTX 10... | 30%    | 4.15.0   | 68C2299CCC |
| 10de:1c03 | 3842:6163 | Nvidia          | GP106 [GeForce GTX 10... | 16.7%  | 4.15.0   | D94180D023 |
| 10de:1c03 | 3842:6267 | Nvidia          | GP106 [GeForce GTX 10... | 100%   |          | B01E929F22 |
| 10de:1c06 | 1043:862c | Nvidia          | GP106 [GeForce GTX 10... | 20%    | 4.15.0   | 9C309002D1 |
| 10de:1c30 | 1028:11b3 | Nvidia          | GP106GL [Quadro P2000]   | 50%    | 5.4.0    | 7149315F22 |
| 10de:1c81 | 103c:8338 | Nvidia          | GP107 [GeForce GTX 1050] | 10%    | 4.15.0   | 3673691CB2 |
| 10de:1c81 | 10de:11c0 | Nvidia          | GP107 [GeForce GTX 1050] | 40%    | 4.15.0   | 1276D33239 |
| 10de:1c81 | 10de:1c81 | Nvidia          | GP107 [GeForce GTX 1050] | 28.6%  | 4.18.0   | 6E08766029 |
| 10de:1c81 | 1458:372c | Nvidia          | GP107 [GeForce GTX 1050] | 33.3%  | 4.15.0   | 1A7DB52C9A |
| 10de:1c81 | 1458:372d | Nvidia          | GP107 [GeForce GTX 1050] | 37.5%  | 4.15.0   | CAFF866F87 |
| 10de:1c81 | 1458:3765 | Nvidia          | GP107 [GeForce GTX 1050] | 14.3%  | 4.15.0   | 2FEBF6828E |
| 10de:1c81 | 1458:3766 | Nvidia          | GP107 [GeForce GTX 1050] | 36.4%  | 4.15.0   | AE2AD389DA |
| 10de:1c81 | 1462:3354 | Nvidia          | GP107 [GeForce GTX 1050] | 25%    | 5.3.0    | 844A6EF03C |
| 10de:1c81 | 1462:8c97 | Nvidia          | GP107 [GeForce GTX 1050] | 20.6%  | 4.15.0   | 96406ED8E3 |
| 10de:1c81 | 174b:5454 | Nvidia          | GP107 [GeForce GTX 1050] | 50%    | 4.15.0   | 42EF2AA13B |
| 10de:1c81 | 19da:2454 | Nvidia          | GP107 [GeForce GTX 1050] | 16.7%  | 4.15.0   | F67985779A |
| 10de:1c81 | 3842:6150 | Nvidia          | GP107 [GeForce GTX 1050] | 33.3%  | 5.7.14   | F2560038AF |
| 10de:1c82 |           | Nvidia          | GP107 [GeForce GTX 10... | 20%    | 4.9.60   | 9D3A142A54 |
| 10de:1c82 | 1043:85cd | Nvidia          | GP107 [GeForce GTX 10... | 42.9%  | 4.15.0   | F8158B205A |
| 10de:1c82 | 1043:85d3 | Nvidia          | GP107 [GeForce GTX 10... | 66.7%  | 4.15.0   | 79B1E21D1A |
| 10de:1c82 | 1043:85d6 | Nvidia          | GP107 [GeForce GTX 10... | 20%    | 4.15.0   | E48D3747A9 |
| 10de:1c82 | 1043:85fb | Nvidia          | GP107 [GeForce GTX 10... | 100%   |          | 16C69C53FF |
| 10de:1c82 | 1043:85ff | Nvidia          | GP107 [GeForce GTX 10... | 14.3%  | 4.15.0   | 4FF6F8B306 |
| 10de:1c82 | 1043:8613 | Nvidia          | GP107 [GeForce GTX 10... | 12.5%  | 4.15.0   | 4F0A8E2C5B |
| 10de:1c82 | 1043:8627 | Nvidia          | GP107 [GeForce GTX 10... | 8.3%   | 4.15.0   | 70C1FC426A |
| 10de:1c82 | 1043:862a | Nvidia          | GP107 [GeForce GTX 10... | 18.2%  | 4.15.0   | 0A27F87F0C |
| 10de:1c82 | 10b0:1c82 | Nvidia          | GP107 [GeForce GTX 10... | 8.3%   | 4.18.16  | 85FF8C6337 |
| 10de:1c82 | 10de:0000 | Nvidia          | GP107 [GeForce GTX 10... | 33.3%  | 4.15.0   | EF93E0C52C |
| 10de:1c82 | 10de:11bf | Nvidia          | GP107 [GeForce GTX 10... | 11.1%  | 4.15.0   | 2244646450 |
| 10de:1c82 | 10de:1c82 | Nvidia          | GP107 [GeForce GTX 10... | 17.1%  | 4.15.0   | F2CA33243F |
| 10de:1c82 | 1458:3729 | Nvidia          | GP107 [GeForce GTX 10... | 33.3%  | 4.15.0   | F71DD78128 |
| 10de:1c82 | 1458:3733 | Nvidia          | GP107 [GeForce GTX 10... | 14.3%  | 4.15.0   | E510EC2AB5 |
| 10de:1c82 | 1458:3746 | Nvidia          | GP107 [GeForce GTX 10... | 50%    | 5.4.0    | D961C79493 |
| 10de:1c82 | 1458:3763 | Nvidia          | GP107 [GeForce GTX 10... | 11.1%  | 4.15.0   | 3DDAB16FAC |
| 10de:1c82 | 1462:3351 | Nvidia          | GP107 [GeForce GTX 10... | 14.3%  | 4.12.14  | B2CD0963B2 |
| 10de:1c82 | 1462:8c96 | Nvidia          | GP107 [GeForce GTX 10... | 8.5%   | 4.15.0   | 9578024712 |
| 10de:1c82 | 19da:2454 | Nvidia          | GP107 [GeForce GTX 10... | 14.3%  | 4.15.0   | 1FE17AADBB |
| 10de:1c8d | 1043:11d1 | Nvidia          | GP107M [GeForce GTX 1... | 28.6%  | 4.15.0   | 47123299D4 |
| 10de:1c91 | 103c:86d4 | Nvidia          | GP107M [GeForce GTX 1... | 33.3%  | 5.4.0    | 9E3950795E |
| 10de:1c91 | 103c:87b0 | Nvidia          | GP107M [GeForce GTX 1... | 50%    | 5.11.12  | C9B7B9393C |
| 10de:1c91 | 1043:18f1 | Nvidia          | GP107M [GeForce GTX 1... | 83.3%  | 5.0.0    | FDE4BFBB76 |
| 10de:1c92 | 1043:1bb1 | Nvidia          | GP107M [GeForce GTX 1... | 100%   |          | 6343267AB7 |
| 10de:1cb1 | 10de:11bc | Nvidia          | GP107GL [Quadro P1000]   | 14.3%  | 4.18.16  | 555F102847 |
| 10de:1cb3 | 1028:11be | Nvidia          | GP107GL [Quadro P400]    | 50%    | 5.4.0    | 6E177D8EC9 |
| 10de:1cb3 | 103c:11be | Nvidia          | GP107GL [Quadro P400]    | 28.6%  | 3.10.0   | AF25E34016 |
| 10de:1cb6 | 1028:1264 | Nvidia          | GP107GL [Quadro P620]    | 85.7%  | 5.9.16   | AD29AF92C2 |
| 10de:1cba | 103c:8451 | Nvidia          | GP107GLM [Quadro P200... | 100%   |          | 04873C768C |
| 10de:1cbb | 103c:842f | Nvidia          | GP107GLM [Quadro P100... | 100%   |          | 93F2B3D9A8 |
| 10de:1cbb | 17aa:2262 | Nvidia          | GP107GLM [Quadro P100... | 50%    | 5.9.12   | 0A2CA85DDC |
| 10de:1cbd | 103c:87da | Nvidia          | GP107GLM [Quadro P620]   | 100%   |          | A57EA6C772 |
| 10de:1d01 | 1043:85f4 | Nvidia          | GP108 [GeForce GT 1030]  | 12.1%  | 4.15.0   | 04C0BFBF31 |
| 10de:1d01 | 1043:85f5 | Nvidia          | GP108 [GeForce GT 1030]  | 8.3%   | 4.15.0   | C9B3B14E25 |
| 10de:1d01 | 1043:8642 | Nvidia          | GP108 [GeForce GT 1030]  | 100%   |          | 1AD00E6974 |
| 10de:1d01 | 10de:11c7 | Nvidia          | GP108 [GeForce GT 1030]  | 9.1%   | 4.15.0   | 20E91A55F2 |
| 10de:1d01 | 10de:1d01 | Nvidia          | GP108 [GeForce GT 1030]  | 10%    | 4.15.0   | C97547ED2D |
| 10de:1d01 | 1458:375c | Nvidia          | GP108 [GeForce GT 1030]  | 13.3%  | 4.15.0   | 228BBE0E9B |
| 10de:1d01 | 1462:8c98 | Nvidia          | GP108 [GeForce GT 1030]  | 10.3%  | 4.15.0   | 1F02E0A2E4 |
| 10de:1d01 | 19da:1476 | Nvidia          | GP108 [GeForce GT 1030]  | 50%    | 4.18.0   | 2B0D032DAD |
| 10de:1e02 | 10de:12a3 | Nvidia          | TU102 [TITAN RTX]        | 33.3%  | 5.4.0    | 30502C41DE |
| 10de:1e04 | 1458:37c4 | Nvidia          | TU102 [GeForce RTX 20... | 100%   |          | 931EA9A398 |
| 10de:1e07 | 1028:3718 | Nvidia          | TU102 [GeForce RTX 20... | 100%   |          | 0496499AA5 |
| 10de:1e07 | 10de:12a4 | Nvidia          | TU102 [GeForce RTX 20... | 100%   |          | 95132AF36E |
| 10de:1e07 | 1462:3711 | Nvidia          | TU102 [GeForce RTX 20... | 100%   |          | 62128222FA |
| 10de:1e07 | 1462:3715 | Nvidia          | TU102 [GeForce RTX 20... | 100%   |          | CE19512CBB |
| 10de:1e07 | 19da:1503 | Nvidia          | TU102 [GeForce RTX 20... | 50%    | 5.11.11  | C8FDC5E958 |
| 10de:1e07 | 3842:2382 | Nvidia          | TU102 [GeForce RTX 20... | 100%   |          | F89E4AD849 |
| 10de:1e07 | 3842:2487 | Nvidia          | TU102 [GeForce RTX 20... | 100%   |          | C3DCC51002 |
| 10de:1e30 | 1028:12ba | Nvidia          | TU102GL [Quadro RTX 6... | 28.6%  | 5.3.0    | 33FDE2B5FB |
| 10de:1e81 | 1458:4003 | Nvidia          | TU104 [GeForce RTX 20... | 100%   |          | 7E6AC3D0C4 |
| 10de:1e81 | 1462:372d | Nvidia          | TU104 [GeForce RTX 20... | 40%    | 5.4.0    | 531975EDD5 |
| 10de:1e81 | 196e:1342 | Nvidia          | TU104 [GeForce RTX 20... | 100%   |          | 1466E1B169 |
| 10de:1e81 | 3842:3287 | Nvidia          | TU104 [GeForce RTX 20... | 100%   |          | 3DA3A9D9AD |
| 10de:1e82 | 1043:8676 | Nvidia          | TU104 [GeForce RTX 2080] | 100%   |          | 48041296CA |
| 10de:1e82 | 10b0:1e87 | Nvidia          | TU104 [GeForce RTX 2080] | 100%   |          | 73CF7CEE79 |
| 10de:1e82 | 1462:3722 | Nvidia          | TU104 [GeForce RTX 2080] | 100%   |          | ACBAD1E6CE |
| 10de:1e84 | 1458:4001 | Nvidia          | TU104 [GeForce RTX 20... | 33.3%  | 5.4.38   | 3A856A26D1 |
| 10de:1e87 | 1458:37a8 | Nvidia          | TU104 [GeForce RTX 20... | 100%   |          | AAD0551E27 |
| 10de:1e87 | 1458:37b3 | Nvidia          | TU104 [GeForce RTX 20... | 100%   |          | F27C124F98 |
| 10de:1e87 | 3842:2183 | Nvidia          | TU104 [GeForce RTX 20... | 50%    | 5.4.18   | 3F2E438AAF |
| 10de:1e89 | 10de:1e89 | Nvidia          | TU104 [GeForce RTX 2060] | 100%   |          | 74E3DEC02B |
| 10de:1eb1 | 1028:12a0 | Nvidia          | TU104GL [Quadro RTX 4... | 100%   |          | 845D92DA91 |
| 10de:1eb1 | 10de:12a0 | Nvidia          | TU104GL [Quadro RTX 4... | 33.3%  | 5.8.0    | B95F8101E5 |
| 10de:1f02 | 1043:8679 | Nvidia          | TU106 [GeForce RTX 2070] | 100%   |          | C1BF2C43E1 |
| 10de:1f02 | 10de:1f02 | Nvidia          | TU106 [GeForce RTX 2070] | 100%   |          | C8C1A01026 |
| 10de:1f02 | 1458:37c8 | Nvidia          | TU106 [GeForce RTX 2070] | 100%   |          | 69F2264D39 |
| 10de:1f02 | 1458:3fda | Nvidia          | TU106 [GeForce RTX 2070] | 33.3%  | 5.4.0    | 70DFCAA6EB |
| 10de:1f02 | 3842:1171 | Nvidia          | TU106 [GeForce RTX 2070] | 100%   |          | 9B509BE358 |
| 10de:1f06 | 10de:13a3 | Nvidia          | TU106 [GeForce RTX 20... | 9.1%   | 4.18.0   | 59145CA9E6 |
| 10de:1f06 | 1458:3ff1 | Nvidia          | TU106 [GeForce RTX 20... | 20%    | 5.4.0    | C4B822A843 |
| 10de:1f06 | 1462:c753 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | 3700FF2DD4 |
| 10de:1f06 | 1462:c757 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | 1F8B296CCC |
| 10de:1f06 | 196e:133b | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | EA4CD0299C |
| 10de:1f06 | 7377:0000 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | 3FA9B2D5A3 |
| 10de:1f07 | 1043:8670 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | AF6DA5211E |
| 10de:1f07 | 1043:8671 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | AC29A018F8 |
| 10de:1f07 | 10de:12ad | Nvidia          | TU106 [GeForce RTX 20... | 50%    | 5.10.6   | 55119E58D9 |
| 10de:1f07 | 1462:3732 | Nvidia          | TU106 [GeForce RTX 20... | 37.5%  | 5.0.0    | 95EB08349E |
| 10de:1f08 | 10de:1f08 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | 3CF95EC244 |
| 10de:1f08 | 1458:37d9 | Nvidia          | TU106 [GeForce RTX 20... | 33.3%  | 5.4.0    | 364918C615 |
| 10de:1f08 | 1458:3fc2 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | 8DF2C93C38 |
| 10de:1f08 | 1458:3fd1 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | 4BF53BD278 |
| 10de:1f08 | 1462:3755 | Nvidia          | TU106 [GeForce RTX 20... | 66.7%  | 5.3.0    | EAA00F4B65 |
| 10de:1f08 | 196e:130f | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | 328F236B37 |
| 10de:1f08 | 3842:2063 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | E4512CE4FC |
| 10de:1f08 | 3842:2167 | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | 32073E3911 |
| 10de:1f11 | 103c:8574 | Nvidia          | TU106M [GeForce RTX 2... | 100%   |          | 5A99A3A590 |
| 10de:1f11 | 1043:140f | Nvidia          | TU106M [GeForce RTX 2... | 50%    | 5.3.0    | EFC1AC12C7 |
| 10de:1f12 | 1043:1f11 | Nvidia          | TU106M [GeForce RTX 2... | 33.3%  | 5.10.14  | A50F9ABD26 |
| 10de:1f15 | 1043:1e21 | Nvidia          | TU106M [GeForce RTX 2... | 80%    | 5.9.16   | B10D744C6C |
| 10de:1f15 | 17aa:3a47 | Nvidia          | TU106M [GeForce RTX 2... | 100%   |          | F707B24713 |
| 10de:1f15 | 1d05:1100 | Nvidia          | TU106M [GeForce RTX 2... | 50%    | 5.8.13   | 4DD6F9EE66 |
| 10de:1f47 | 10de:13ad | Nvidia          | TU106 [GeForce RTX 20... | 100%   |          | E0192EBFC1 |
| 10de:1f50 | 103c:8574 | Nvidia          | TU106BM [GeForce RTX ... | 50%    | 4.18.0   | E31EFEB24C |
| 10de:1f50 | 103c:8600 | Nvidia          | TU106BM [GeForce RTX ... | 100%   |          | 2153033D3A |
| 10de:1f50 | 103c:8603 | Nvidia          | TU106BM [GeForce RTX ... | 50%    | 5.8.10   | 8295B3DB5F |
| 10de:1f82 | 103c:8558 | Nvidia          | TU117 [GeForce GTX 1650] | 33.3%  | 5.10.14  | 6C0504F168 |
| 10de:1f82 | 10de:1320 | Nvidia          | TU117 [GeForce GTX 1650] | 62.5%  | 5.6.6    | 6EC3B6B77E |
| 10de:1f82 | 1458:3fca | Nvidia          | TU117 [GeForce GTX 1650] | 33.3%  | 5.4.32   | 736B24E183 |
| 10de:1f82 | 1458:3fcb | Nvidia          | TU117 [GeForce GTX 1650] | 37.5%  | 5.4.0    | 71F658769F |
| 10de:1f82 | 1458:3fcc | Nvidia          | TU117 [GeForce GTX 1650] | 33.3%  | 5.8.11   | 97755E07C8 |
| 10de:1f82 | 1462:3800 | Nvidia          | TU117 [GeForce GTX 1650] | 66.7%  | 5.9.11   | 9C0406B489 |
| 10de:1f91 | 103c:86d5 | Nvidia          | TU117M [GeForce GTX 1... | 75%    | 5.3.0    | 209887E993 |
| 10de:1f91 | 1043:109f | Nvidia          | TU117M [GeForce GTX 1... | 69.6%  | 5.3.0    | 10A2F7DBA4 |
| 10de:1f91 | 1043:10cf | Nvidia          | TU117M [GeForce GTX 1... | 50%    | 5.9.3    | 916D4B225B |
| 10de:1f91 | 17aa:3a41 | Nvidia          | TU117M [GeForce GTX 1... | 33.3%  | 4.18.0   | A70D38C48C |
| 10de:1f91 | 17aa:3ffb | Nvidia          | TU117M [GeForce GTX 1... | 42.9%  | 5.3.0    | 09DA46F5D5 |
| 10de:1f95 | 1025:1447 | Nvidia          | TU117M [GeForce GTX 1... | 100%   |          | 19F0A0EEED |
| 10de:1f95 | 103c:87b2 | Nvidia          | TU117M [GeForce GTX 1... | 50%    | 5.13.0   | FAB2C07BC0 |
| 10de:1f95 | 1043:16df | Nvidia          | TU117M [GeForce GTX 1... | 87.5%  | 5.8.0    | D27007007F |
| 10de:1f95 | 1043:16ef | Nvidia          | TU117M [GeForce GTX 1... | 33.3%  | 5.8.1    | CBC872E471 |
| 10de:1f95 | 17aa:3a3e | Nvidia          | TU117M [GeForce GTX 1... | 71.4%  | 5.10.13  | 1F2752F00F |
| 10de:1f95 | 17aa:3a44 | Nvidia          | TU117M [GeForce GTX 1... | 100%   |          | 3A0EDBA2D3 |
| 10de:1f99 | 1025:1447 | Nvidia          | TU117M                   | 100%   |          | C58E02D129 |
| 10de:1f99 | 103c:87b1 | Nvidia          | TU117M                   | 60%    | 5.7.12   | 508213FD9C |
| 10de:1f99 | 17aa:3a43 | Nvidia          | TU117M                   | 33.3%  | 5.4.0    | 8CCBC14BCA |
| 10de:1fb9 | 103c:860e | Nvidia          | TU117GLM [Quadro T100... | 100%   |          | DC6E4DA9DE |
| 10de:2182 | 1043:86a3 | Nvidia          | TU116 [GeForce GTX 16... | 50%    | 5.4.0    | E891AAE560 |
| 10de:2182 | 10de:2182 | Nvidia          | TU116 [GeForce GTX 16... | 37.5%  | 5.4.0    | 00F710FA13 |
| 10de:2182 | 1458:3fbe | Nvidia          | TU116 [GeForce GTX 16... | 54.5%  | 5.4.0    | F50C460937 |
| 10de:2182 | 1462:3750 | Nvidia          | TU116 [GeForce GTX 16... | 66.7%  | 5.8.13   | 9E2420DAD2 |
| 10de:2182 | 1462:375a | Nvidia          | TU116 [GeForce GTX 16... | 11.1%  | 5.3.0    | CA561AA481 |
| 10de:2184 | 10de:1324 | Nvidia          | TU116 [GeForce GTX 1660] | 60%    | 5.4.32   | 50AFAA10C6 |
| 10de:2184 | 10de:1366 | Nvidia          | TU116 [GeForce GTX 1660] | 100%   |          | 2F657D538C |
| 10de:2184 | 10de:2184 | Nvidia          | TU116 [GeForce GTX 1660] | 100%   |          | A011A6EF0E |
| 10de:2184 | 1458:3fc7 | Nvidia          | TU116 [GeForce GTX 1660] | 100%   |          | C4C123186E |
| 10de:2184 | 1462:3792 | Nvidia          | TU116 [GeForce GTX 1660] | 6.2%   | 5.3.0    | 705949F6E0 |
| 10de:2184 | 1462:8d91 | Nvidia          | TU116 [GeForce GTX 1660] | 66.7%  | 5.3.11   | F81F24D3E6 |
| 10de:2184 | 7377:150a | Nvidia          | TU116 [GeForce GTX 1660] | 100%   |          | 30939907C1 |
| 10de:2187 | 1043:8750 | Nvidia          | TU116 [GeForce GTX 16... | 100%   |          | 5214390AB5 |
| 10de:2187 | 1043:8769 | Nvidia          | TU116 [GeForce GTX 16... | 40%    | 5.10.9   | 01B19A01D9 |
| 10de:2187 | 10de:2187 | Nvidia          | TU116 [GeForce GTX 16... | 100%   |          | F1D2507C90 |
| 10de:2187 | 3842:1357 | Nvidia          | TU116 [GeForce GTX 16... | 33.3%  | 5.8.0    | F36075AAA0 |
| 10de:2188 | 10de:2188 | Nvidia          | TU116 [GeForce GTX 1650] | 100%   |          | 07EE20E1CA |
| 10de:2191 | 103c:8574 | Nvidia          | TU116M [GeForce GTX 1... | 50%    | 5.7.8    | A85470AC70 |
| 10de:2191 | 103c:8786 | Nvidia          | TU116M [GeForce GTX 1... | 33.3%  | 5.10.0   | 2E1D9BDA67 |
| 10de:2191 | 103c:87b3 | Nvidia          | TU116M [GeForce GTX 1... | 50%    | 5.8.0    | 6B3DB58438 |
| 10de:2191 | 1043:10af | Nvidia          | TU116M [GeForce GTX 1... | 50%    | 5.6.7    | 85703241B5 |
| 10de:2191 | 1043:16cf | Nvidia          | TU116M [GeForce GTX 1... | 67.9%  | 5.6.14   | 9D9C3E89A5 |
| 10de:2191 | 1043:16ff | Nvidia          | TU116M [GeForce GTX 1... | 62.5%  | 5.8.0    | D7899F0224 |
| 10de:2191 | 1043:171f | Nvidia          | TU116M [GeForce GTX 1... | 100%   |          | 23EC9F2747 |
| 10de:2191 | 1043:18d1 | Nvidia          | TU116M [GeForce GTX 1... | 50%    | 5.8.0    | C6FD48FE3F |
| 10de:2191 | 17aa:3a46 | Nvidia          | TU116M [GeForce GTX 1... | 14.3%  | 5.8.0    | 24CD377743 |
| 10de:21c4 | 1043:8752 | Nvidia          | TU116 [GeForce GTX 16... | 100%   |          | 0F16D1F407 |
| 10de:21c4 | 1458:4013 | Nvidia          | TU116 [GeForce GTX 16... | 28.6%  | 5.3.0    | EF19F435BE |
| 10de:21c4 | 1462:8d94 | Nvidia          | TU116 [GeForce GTX 16... | 60%    | 5.6.15   | 0DF80890C0 |
| 10de:21c4 | 1462:c757 | Nvidia          | TU116 [GeForce GTX 16... | 66.7%  | 5.6.14   | 406E2C08D2 |
| 10de:21c4 | 3842:1061 | Nvidia          | TU116 [GeForce GTX 16... | 100%   |          | 8CA3789A9E |
| 10de:2204 | 1028:3880 | Nvidia          | GA102 [GeForce RTX 3090] | 100%   |          | 2CA79D800A |
| 10de:2204 | 10de:147d | Nvidia          | GA102 [GeForce RTX 3090] | 100%   |          | 33281F109C |
| 10de:2206 | 1043:87b0 | Nvidia          | GA102 [GeForce RTX 3080] | 100%   |          | 35D97E2D21 |
| 10de:2206 | 1462:3892 | Nvidia          | GA102 [GeForce RTX 3080] | 33.3%  | 5.4.32   | 70DFCAA6EB |
| 10de:2206 | 1462:3896 | Nvidia          | GA102 [GeForce RTX 3080] | 100%   |          | B2DE3AF507 |
| 10de:2206 | 1462:3897 | Nvidia          | GA102 [GeForce RTX 3080] | 100%   |          | FAFE6F69B5 |
| 10de:2486 | 10de:2486 | Nvidia          | GA104 [GeForce RTX 30... | 100%   |          | EFCE67D492 |
| 10de:2486 | 1462:3903 | Nvidia          | GA104 [GeForce RTX 30... | 100%   |          | AE807DEDAC |
| 10de:249d | 1043:118c | Nvidia          | GA104M [GeForce RTX 3... | 100%   |          | A488AFB982 |
| 10de:249d | 1043:128c | Nvidia          | GA104M [GeForce RTX 3... | 100%   |          | 6D5882D39F |
| 10de:2503 | 1458:4074 | Nvidia          | GA106 [GeForce RTX 3060] | 100%   |          | 84BE0D6978 |
| 10de:2503 | 1462:3976 | Nvidia          | GA106 [GeForce RTX 3060] | 100%   |          | CCC507D50B |
| 10de:2520 | 1043:16a2 | Nvidia          | GA106M [GeForce RTX 3... | 100%   |          | 1BFCB72AF7 |
| 8086:0042 | 1849:0042 | Intel           | Core Processor Integr... | 4.5%   | 3.14.33  | 1D9934126C |
| 8086:0046 | 1179:0003 | Intel           | Core Processor Integr... | 33.3%  | 5.4.0    | 1C8D8216C0 |
| 8086:0102 | 1025:0586 | Intel           | 2nd Generation Core P... | 100%   |          | 59F759C146 |
| 8086:0102 | 103c:2ac5 | Intel           | 2nd Generation Core P... | 3.8%   | 4.1.34   | 7E85D95373 |
| 8086:0102 | 17aa:3078 | Intel           | 2nd Generation Core P... | 5.3%   | 4.15.0   | 735EE0A048 |
| 8086:0102 | 1849:0102 | Intel           | 2nd Generation Core P... | 0.9%   | 3.10.0   | 7F5766D5DA |
| 8086:0106 | 1025:0504 | Intel           | 2nd Generation Core P... | 2.4%   | 4.1.38   | 8FE3AF49FB |
| 8086:0106 | 103c:177c | Intel           | 2nd Generation Core P... | 100%   |          | AD79605A2B |
| 8086:0116 | 1028:0493 | Intel           | 2nd Generation Core P... | 2.9%   | 4.9.60   | CAC07212DD |
| 8086:0116 | 1179:fc50 | Intel           | 2nd Generation Core P... | 4%     | 4.4.0    | 046BFED81F |
| 8086:0116 | 144d:c0b3 | Intel           | 2nd Generation Core P... | 11.1%  | 4.15.0   | 2B3EBD7597 |
| 8086:0116 | 144d:c0d3 | Intel           | 2nd Generation Core P... | 100%   |          | EF995FD5BC |
| 8086:0152 | 1028:0577 | Intel           | Xeon E3-1200 v2/3rd G... | 0.8%   | 4.1.38   | CF1915F31B |
| 8086:0152 | 1043:84ca | Intel           | Xeon E3-1200 v2/3rd G... | 0.8%   | 3.10.34  | 44E0CE8FC8 |
| 8086:0156 | 103c:218b | Intel           | 3rd Gen Core processo... | 50%    | 5.4.0    | 0C2506DFCB |
| 8086:0162 | 1028:052c | Intel           | Xeon E3-1200 v2/3rd G... | 5%     | 4.15.0   | 29A0FC6CE0 |
| 8086:0162 | 1043:84ca | Intel           | Xeon E3-1200 v2/3rd G... | 6.5%   | 3.14.44  | C7C6CD6D36 |
| 8086:0162 | 1458:d000 | Intel           | Xeon E3-1200 v2/3rd G... | 0.9%   | 3.10.0   | A282EBEBE6 |
| 8086:0166 | 1025:0647 | Intel           | 3rd Gen Core processo... | 0.5%   | 3.10.34  | 86D2D3B0E1 |
| 8086:0166 | 17aa:21fb | Intel           | 3rd Gen Core processo... | 3.8%   | 4.15.0   | 55427995B5 |
| 8086:0166 | 1854:0167 | Intel           | 3rd Gen Core processo... | 20%    | 5.0.0    | D0CF0BEEA8 |
| 8086:0402 | 1028:0620 | Intel           | Xeon E3-1200 v3/4th G... | 50%    | 4.5.4    | 470703F4AF |
| 8086:0402 | 1458:d000 | Intel           | Xeon E3-1200 v3/4th G... | 0.5%   | 3.14.44  | A3FA543C65 |
| 8086:0412 | 1028:05b0 | Intel           | Xeon E3-1200 v3/4th G... | 50%    | 5.3.0    | BDF125B54E |
| 8086:0412 | 103c:18e6 | Intel           | Xeon E3-1200 v3/4th G... | 20%    | 5.6.14   | CF3ED91B8A |
| 8086:0412 | 1458:d000 | Intel           | Xeon E3-1200 v3/4th G... | 0.2%   | 2.6.32   | CD61F6363F |
| 8086:0412 | 1462:7816 | Intel           | Xeon E3-1200 v3/4th G... | 25%    | 4.9.20   | 1D08943078 |
| 8086:0412 | 17aa:30a3 | Intel           | Xeon E3-1200 v3/4th G... | 4.2%   | 4.9.20   | C9E1E1AD57 |
| 8086:0416 | 103c:1993 | Intel           | 4th Gen Core Processo... | 0.9%   | 4.4.0    | FE47E4E62A |
| 8086:0416 | 1558:5455 | Intel           | 4th Gen Core Processo... | 11.8%  | 3.14.22  | 32F4FB7C0C |
| 8086:0416 | 8086:0416 | Intel           | 4th Gen Core Processo... | 21.4%  | 4.18.0   | B364724E53 |
| 8086:041a | 1462:7823 | Intel           | Xeon E3-1200 v3 Proce... | 100%   |          | 7755195EF6 |
| 8086:0a06 | 1025:0888 | Intel           | Haswell-ULT Integrate... | 33.3%  | 4.9.60   | F19B7DB6C0 |
| 8086:0a16 | 1025:0775 | Intel           | Haswell-ULT Integrate... | 1%     | 3.14.53  | 81B19839F7 |
| 8086:0a16 | 1028:0651 | Intel           | Haswell-ULT Integrate... | 0.9%   | 3.14.44  | AA72A49A15 |
| 8086:0a16 | 17aa:380d | Intel           | Haswell-ULT Integrate... | 1%     | 3.14.25  | B3B3794709 |
| 8086:0be2 | 8086:2012 | Intel           | Atom Processor D2xxx/... | 50%    | 3.14.44  | AC8E827D44 |
| 8086:0f31 | 1025:0936 | Intel           | Atom Processor Z36xxx... | 2.3%   | 4.12.14  | 1718CF1D36 |
| 8086:0f31 | 1458:d000 | Intel           | Atom Processor Z36xxx... | 14.5%  | 3.10.0   | 18EECC3CF2 |
| 8086:0f31 | 17aa:3695 | Intel           | Atom Processor Z36xxx... | 16.7%  | 4.15.0   | 08BB09B100 |
| 8086:0f31 | 1849:0f31 | Intel           | Atom Processor Z36xxx... | 0.8%   | 3.10.0   | 78F7E1012F |
| 8086:1616 | 1025:1019 | Intel           | HD Graphics 5500         | 100%   |          | 5DBE9649A7 |
| 8086:1626 | 106b:011b | Intel           | HD Graphics 6000         | 3.3%   | 4.15.0   | 0789DA98E3 |
| 8086:1902 | 1043:8694 | Intel           | HD Graphics 510          | 5.1%   | 4.8.14   | A91734714E |
| 8086:1902 | 1462:7996 | Intel           | HD Graphics 510          | 6.7%   | 4.9.20   | BFAA613B9E |
| 8086:1902 | 8086:2212 | Intel           | HD Graphics 510          | 33.3%  | 4.15.0   | FF56929B10 |
| 8086:1912 | 1043:8694 | Intel           | HD Graphics 530          | 3.9%   | 4.4.0    | AF1F86E610 |
| 8086:1912 | 1458:d000 | Intel           | HD Graphics 530          | 10.2%  | 4.9.41   | 53E6A4F263 |
| 8086:1912 | 1734:121c | Intel           | HD Graphics 530          | 50%    | 4.12.14  | B363AEA94A |
| 8086:1912 | 1849:1912 | Intel           | HD Graphics 530          | 2.7%   | 4.3.3    | 42FACB50D6 |
| 8086:1916 | 1025:0985 | Intel           | Skylake GT2 [HD Graph... | 14.3%  | 5.3.0    | 01210C0B0E |
| 8086:1916 | 1025:1094 | Intel           | Skylake GT2 [HD Graph... | 2.6%   | 4.9.9    | E7D6077756 |
| 8086:1916 | 1028:06de | Intel           | Skylake GT2 [HD Graph... | 1.9%   | 4.12.14  | AE7AD1E7D9 |
| 8086:1916 | 1028:06fd | Intel           | Skylake GT2 [HD Graph... | 11.1%  | 4.15.0   | 569785286A |
| 8086:1916 | 1028:070a | Intel           | Skylake GT2 [HD Graph... | 2.1%   | 4.4.0    | 09095E1ECF |
| 8086:1916 | 103c:8079 | Intel           | Skylake GT2 [HD Graph... | 1.3%   | 4.1.15   | 82F5250E0D |
| 8086:1916 | 103c:807c | Intel           | Skylake GT2 [HD Graph... | 2.9%   | 4.9.0    | 0DCB414448 |
| 8086:1916 | 103c:80a4 | Intel           | Skylake GT2 [HD Graph... | 5.3%   | 4.9.60   | B01FB51118 |
| 8086:1916 | 103c:80ff | Intel           | Skylake GT2 [HD Graph... | 18.5%  | 4.7.2    | B7B039F46E |
| 8086:1916 | 103c:8100 | Intel           | Skylake GT2 [HD Graph... | 6.7%   | 4.15.0   | 2B56F34E21 |
| 8086:1916 | 103c:8101 | Intel           | Skylake GT2 [HD Graph... | 2%     | 4.9.60   | BC496704F4 |
| 8086:1916 | 103c:820c | Intel           | Skylake GT2 [HD Graph... | 12.5%  | 4.9.20   | FAE1CD27F3 |
| 8086:1916 | 1043:1020 | Intel           | Skylake GT2 [HD Graph... | 40%    | 4.19.31  | C0A516F3EC |
| 8086:1916 | 1043:1ccd | Intel           | Skylake GT2 [HD Graph... | 4.7%   | 4.9.20   | A4B26975E9 |
| 8086:1916 | 1179:f822 | Intel           | Skylake GT2 [HD Graph... | 25%    | 4.15.0   | B781D8419A |
| 8086:1916 | 17aa:3824 | Intel           | Skylake GT2 [HD Graph... | 2.1%   | 4.9.9    | 412EAC636F |
| 8086:1916 | 17aa:382c | Intel           | Skylake GT2 [HD Graph... | 6.2%   | 4.9.0    | 18379EBD5C |
| 8086:1916 | 17aa:5048 | Intel           | Skylake GT2 [HD Graph... | 10%    | 4.15.0   | 842B139FE7 |
| 8086:1916 | 8086:1916 | Intel           | Skylake GT2 [HD Graph... | 20%    | 4.15.0   | 253718AA9E |
| 8086:1916 | 8086:2063 | Intel           | Skylake GT2 [HD Graph... | 16.7%  | 4.15.0   | 001888ED9C |
| 8086:1916 | 8086:2212 | Intel           | Skylake GT2 [HD Graph... | 12.5%  | 4.9.124  | 9DE5E32B25 |
| 8086:191b | 1028:06de | Intel           | HD Graphics 530          | 3.4%   | 4.15.0   | BC4C6EBBA7 |
| 8086:191b | 1043:1080 | Intel           | HD Graphics 530          | 5.6%   | 4.15.0   | 5B1076EA3C |
| 8086:191b | 1043:1d6d | Intel           | HD Graphics 530          | 6.2%   | 5.4.0    | 9D6C0DD372 |
| 8086:191b | 1462:1190 | Intel           | HD Graphics 530          | 5.9%   | 4.9.9    | 2B70AAB06F |
| 8086:191b | 17aa:222e | Intel           | HD Graphics 530          | 2.3%   | 4.4.0    | 356758A7D8 |
| 8086:1921 | 17aa:39e8 | Intel           | HD Graphics 520          | 20%    | 4.9.111  | C3352134E9 |
| 8086:22b0 | 1043:8705 | Intel           | Atom/Celeron/Pentium ... | 50%    | 5.4.80   | 71D7F6E110 |
| 8086:22b0 | 8086:7270 | Intel           | Atom/Celeron/Pentium ... | 0.3%   | 3.10.0   | D40BF2CFA6 |
| 8086:22b1 | 1025:1012 | Intel           | Atom/Celeron/Pentium ... | 2.6%   | 4.9.20   | 16D1C62342 |
| 8086:22b1 | 1028:06ac | Intel           | Atom/Celeron/Pentium ... | 1.2%   | 4.4.0    | 8F537DF4E3 |
| 8086:22b1 | 1028:0725 | Intel           | Atom/Celeron/Pentium ... | 7.7%   | 4.9.20   | 92DCC778AC |
| 8086:22b1 | 1043:10c0 | Intel           | Atom/Celeron/Pentium ... | 1.4%   | 4.9.9    | E6AFAB9B56 |
| 8086:22b1 | 1458:1000 | Intel           | Atom/Celeron/Pentium ... | 3.1%   | 4.4.0    | 970493CF1B |
| 8086:22b1 | 1458:d000 | Intel           | Atom/Celeron/Pentium ... | 10%    | 4.9.9    | 2FD537312F |
| 8086:22b1 | 1558:0945 | Intel           | Atom/Celeron/Pentium ... | 4.5%   | 4.1.15   | BDAF59B6EB |
| 8086:2572 | 103c:12bc | Intel           | 82865G Integrated Gra... | 8.3%   | 4.1.34   | DD4DD47556 |
| 8086:2582 | 1028:01c7 | Intel           | 82915G/GV/910GL Integ... | 50%    | 4.9.60   | AA18FB386C |
| 8086:2772 | 1028:01ad | Intel           | 82945G/GZ Integrated ... | 1.5%   | 3.14.22  | D8D0898E8C |
| 8086:2772 | 1297:3166 | Intel           | 82945G/GZ Integrated ... | 100%   |          | 14A841B718 |
| 8086:2772 | 1462:7418 | Intel           | 82945G/GZ Integrated ... | 33.3%  | 4.18.16  | AF5AB7C73F |
| 8086:2772 | 1849:2772 | Intel           | 82945G/GZ Integrated ... | 3%     | 4.1.15   | F919A6006E |
| 8086:2772 | 8086:464c | Intel           | 82945G/GZ Integrated ... | 28.6%  | 3.10.0   | 947354716F |
| 8086:27a2 | 1025:0107 | Intel           | Mobile 945GM/GMS, 943... | 42.9%  | 4.1.34   | 290DB67DA7 |
| 8086:27a2 | 1025:012e | Intel           | Mobile 945GM/GMS, 943... | 3.3%   | 4.1.16   | 7138F65A56 |
| 8086:27a2 | 104d:81ef | Intel           | Mobile 945GM/GMS, 943... | 22.2%  | 4.15.0   | CA251E5028 |
| 8086:27a2 | 104d:820f | Intel           | Mobile 945GM/GMS, 943... | 30%    | 3.14.44  | 811EFEE1FC |
| 8086:27a2 | 1462:0341 | Intel           | Mobile 945GM/GMS, 943... | 18.2%  | 4.1.15   | C71F72F074 |
| 8086:27a2 | 14c0:0020 | Intel           | Mobile 945GM/GMS, 943... | 22.2%  | 4.1.15   | D1D8A50709 |
| 8086:27ae | 1179:ff1e | Intel           | Mobile 945GSE Express... | 8.3%   | 4.9.20   | 7876CCA0BB |
| 8086:2992 | 1028:01da | Intel           | 82Q963/Q965 Integrate... | 1.3%   | 4.4.0    | B41D37ED11 |
| 8086:2992 | 1734:10b5 | Intel           | 82Q963/Q965 Integrate... | 11.8%  | 4.1.15   | BF1BADE95D |
| 8086:29b2 | 1028:0211 | Intel           | 82Q35 Express Integra... | 3.2%   | 3.14.44  | 8B35A68B60 |
| 8086:29c2 | 1019:2683 | Intel           | 82G33/G31 Express Int... | 3%     | 4.1.25   | 4B118F08F0 |
| 8086:29c2 | 103c:2a5d | Intel           | 82G33/G31 Express Int... | 7.7%   | 4.15.0   | 8EAD41D349 |
| 8086:29c2 | 1043:82b0 | Intel           | 82G33/G31 Express Int... | 0.5%   | 3.14.44  | D0F087D90E |
| 8086:29c2 | 1458:d000 | Intel           | 82G33/G31 Express Int... | 1.3%   | 3.14.44  | FAE0FA711B |
| 8086:29c2 | 1849:29c2 | Intel           | 82G33/G31 Express Int... | 0.6%   | 3.14.44  | 948B6142EC |
| 8086:2a02 | 103c:30cd | Intel           | Mobile GM965/GL960 In... | 4%     | 4.18.16  | 312D41F446 |
| 8086:2a02 | 10cf:13f8 | Intel           | Mobile GM965/GL960 In... | 33.3%  | 4.12.14  | 19DF86707E |
| 8086:2a02 | 1734:1118 | Intel           | Mobile GM965/GL960 In... | 11.1%  | 4.1.25   | 989E87E18E |
| 8086:2a12 | 103c:3618 | Intel           | Mobile GME965/GLE960 ... | 6.1%   | 3.14.44  | 13824A2872 |
| 8086:2a42 | 1025:020e | Intel           | Mobile 4 Series Chips... | 50%    | 4.9.0    | 298F046639 |
| 8086:2a42 | 103c:3676 | Intel           | Mobile 4 Series Chips... | 16.7%  | 4.1.25   | 031B9CF2AF |
| 8086:2a42 | 1631:018b | Intel           | Mobile 4 Series Chips... | 11.8%  | 5.0.0    | 96A6F21797 |
| 8086:2e12 | 1025:0151 | Intel           | 4 Series Chipset Inte... | 25%    | 4.9.20   | 96ED3B9CA2 |
| 8086:2e12 | 1028:027f | Intel           | 4 Series Chipset Inte... | 1.4%   | 3.14.44  | FCFB060CFE |
| 8086:2e12 | 17aa:3048 | Intel           | 4 Series Chipset Inte... | 15.8%  | 4.1.15   | B57213E97F |
| 8086:2e22 | 1025:0251 | Intel           | 4 Series Chipset Inte... | 11.1%  | 4.18.0   | DFD78F1056 |
| 8086:2e32 |           | Intel           | 4 Series Chipset Inte... | 28.6%  | 5.0.0    | 37B1114873 |
| 8086:2e32 | 1025:0390 | Intel           | 4 Series Chipset Inte... | 9.1%   | 4.15.0   | 112E50B08C |
| 8086:2e32 | 8086:5756 | Intel           | 4 Series Chipset Inte... | 2.9%   | 4.9.60   | AF606A347F |
| 8086:2e32 | 8086:d612 | Intel           | 4 Series Chipset Inte... | 20%    | 4.15.0   | 48AB47DFE5 |
| 8086:3184 | 1458:1000 | Intel           | GeminiLake [UHD Graph... | 20%    | 4.15.0   | C7F8A0A39C |
| 8086:3185 | 1849:2212 | Intel           | GeminiLake [UHD Graph... | 3.3%   | 4.15.0   | 54F377B79C |
| 8086:3e90 | 1458:d000 | Intel           | CoffeeLake-S GT1 [UHD... | 18.2%  | 4.15.0   | A174DA5BA2 |
| 8086:3e91 | 1043:8694 | Intel           | CoffeeLake-S GT2 [UHD... | 3.9%   | 4.15.0   | DA54361164 |
| 8086:3e91 | 1458:d000 | Intel           | CoffeeLake-S GT2 [UHD... | 1.8%   | 4.13.0   | EE50586259 |
| 8086:3e91 | 1849:3e91 | Intel           | CoffeeLake-S GT2 [UHD... | 3.3%   | 4.15.0   | 59151791CF |
| 8086:3e92 | 1025:126c | Intel           | CometLake-S GT2 [UHD ... | 100%   |          | C1339E884A |
| 8086:3e92 | 1028:0851 | Intel           | CometLake-S GT2 [UHD ... | 100%   |          | 05D6B79D2F |
| 8086:3e92 | 1028:0930 | Intel           | CometLake-S GT2 [UHD ... | 20%    | 4.15.0   | C2BF735906 |
| 8086:3e92 | 103c:843c | Intel           | CometLake-S GT2 [UHD ... | 50%    | 5.1.3    | E5E15DF58D |
| 8086:3e92 | 1043:8694 | Intel           | CometLake-S GT2 [UHD ... | 1.9%   | 4.15.0   | 66A90BEA5D |
| 8086:3e92 | 1458:d000 | Intel           | CometLake-S GT2 [UHD ... | 0.9%   | 4.14.0   | DA58706E3D |
| 8086:3e98 | 1043:8694 | Intel           | CoffeeLake-S GT2 [UHD... | 2.6%   | 4.15.0   | DC32FE8000 |
| 8086:3e98 | 1462:7b98 | Intel           | CoffeeLake-S GT2 [UHD... | 14.3%  | 5.3.0    | 297E534CF0 |
| 8086:3e98 | 1849:3e98 | Intel           | CoffeeLake-S GT2 [UHD... | 2.6%   | 4.15.0   | 06EB8AFDBC |
| 8086:3e9b | 1025:1264 | Intel           | CoffeeLake-H GT2 [UHD... | 1.3%   | 4.15.0   | C4FA903BED |
| 8086:3e9b | 1462:126a | Intel           | CoffeeLake-H GT2 [UHD... | 7.7%   | 3.10.0   | 039A05F3EB |
| 8086:3e9b | 1558:95e6 | Intel           | CoffeeLake-H GT2 [UHD... | 5.9%   | 4.15.0   | 1035C22955 |
| 8086:3ea0 | 1028:08a8 | Intel           | WhiskeyLake-U GT2 [UH... | 6.2%   | 4.15.0   | B6DF9FEC5F |
| 8086:3ea0 | 1028:08b8 | Intel           | WhiskeyLake-U GT2 [UH... | 2.5%   | 4.19.0   | 241B649AD1 |
| 8086:3ea0 | 1028:08bc | Intel           | WhiskeyLake-U GT2 [UH... | 3%     | 4.15.0   | 5ED5F692A4 |
| 8086:3ea0 | 103c:8533 | Intel           | WhiskeyLake-U GT2 [UH... | 3.3%   | 4.15.0   | 66C8150E0D |
| 8086:3ea0 | 103c:856e | Intel           | WhiskeyLake-U GT2 [UH... | 7.1%   | 4.19.0   | 2928437EAC |
| 8086:3ea0 | 17aa:2279 | Intel           | WhiskeyLake-U GT2 [UH... | 1.2%   | 4.15.0   | B6F9682F0B |
| 8086:3ea0 | 1849:3ea0 | Intel           | WhiskeyLake-U GT2 [UH... | 33.3%  | 5.4.0    | 2F6164BD1D |
| 8086:3ea1 | 1028:08ca | Intel           | Coffee Lake UHD 610 G... | 6.7%   | 4.15.0   | 906A07309D |
| 8086:3ea5 | 8086:2074 | Intel           | CoffeeLake-U GT3e [Ir... | 0.6%   | 3.10.0   | 7AB72B120C |
| 8086:4905 | 1028:09de | Intel           | DG1 [Iris Xe MAX Grap... | 100%   |          | 65286CB6D4 |
| 8086:4c8a | 1043:8694 | Intel           | RocketLake-S GT1 [UHD... | 66.7%  | 5.11.12  | 9E40A428C6 |
| 8086:4c8a | 1458:d000 | Intel           | RocketLake-S GT1 [UHD... | 25%    | 5.11.0   | 8A81B827C0 |
| 8086:4c8a | 1849:4c8a | Intel           | RocketLake-S GT1 [UHD... | 75%    | 5.10.0   | ADC5D5D836 |
| 8086:4e71 | 1025:1516 | Intel           | JasperLake [UHD Graph... | 66.7%  | 5.10.0   | E1AE43D711 |
| 8086:5902 | 1849:5902 | Intel           | HD Graphics 610          | 7.1%   | 4.9.60   | 9E7024131D |
| 8086:5912 | 1028:0764 | Intel           | HD Graphics 630          | 100%   |          | 530CC43BE2 |
| 8086:5912 | 1043:8694 | Intel           | HD Graphics 630          | 0.5%   | 4.4.0    | B0DE2CBA6A |
| 8086:5912 | 1462:7a15 | Intel           | HD Graphics 630          | 4.3%   | 4.9.95   | CD74218E72 |
| 8086:5912 | 1734:121c | Intel           | HD Graphics 630          | 9.1%   | 4.12.14  | D9EA4A7B7A |
| 8086:5912 | 17aa:310c | Intel           | HD Graphics 630          | 33.3%  | 5.8.0    | 60877665B6 |
| 8086:5916 | 1028:075b | Intel           | HD Graphics 620          | 1.5%   | 4.4.0    | 6695D2A05E |
| 8086:5916 | 1028:0768 | Intel           | HD Graphics 620          | 4.3%   | 4.9.9    | 2BB9B79D2E |
| 8086:5916 | 1028:0782 | Intel           | HD Graphics 620          | 4.3%   | 4.15.0   | 49389100FC |
| 8086:5916 | 1028:078b | Intel           | HD Graphics 620          | 0.9%   | 4.15.0   | D074E75C19 |
| 8086:5916 | 1028:07a8 | Intel           | HD Graphics 620          | 8.3%   | 5.3.0    | EBA5E925B8 |
| 8086:5916 | 17aa:39f1 | Intel           | HD Graphics 620          | 3.8%   | 4.4.0    | 32F19AB04D |
| 8086:5916 | 8086:2212 | Intel           | HD Graphics 620          | 2%     | 4.9.41   | B1A55C7D69 |
| 8086:5917 | 1028:081c | Intel           | UHD Graphics 620         | 2.3%   | 4.12.14  | 54E871CA5D |
| 8086:5917 | 1028:0841 | Intel           | UHD Graphics 620         | 11.1%  | 4.19.0   | A3D09E7D2F |
| 8086:5917 | 103c:837d | Intel           | UHD Graphics 620         | 1.4%   | 4.9.60   | 757C263C73 |
| 8086:5917 | 1558:1313 | Intel           | UHD Graphics 620         | 23.1%  | 4.15.0   | B72558F93C |
| 8086:5917 | 17aa:225e | Intel           | UHD Graphics 620         | 2.8%   | 4.12.14  | 7D7E6AD5D5 |
| 8086:591b | 1025:118a | Intel           | HD Graphics 630          | 1.3%   | 4.9.60   | 018F6EE8E7 |
| 8086:591b | 1028:07bf | Intel           | HD Graphics 630          | 4.2%   | 4.15.0   | 26DBEC9F3A |
| 8086:591b | 1028:07d0 | Intel           | HD Graphics 630          | 4.5%   | 4.9.9    | D4927A9F76 |
| 8086:5a84 | 17aa:39fd | Intel           | Celeron N3350/Pentium... | 9.1%   | 4.18.16  | 8597CD19C4 |
| 8086:5a85 | 8086:7270 | Intel           | HD Graphics 500          | 10%    | 4.4.59   | 622CED4019 |
| 8086:8108 | 1028:02b1 | Intel           | US15W/US15X SCH [Poul... | 100%   |          | 7D4473A4A5 |
| 8086:8a52 | 1025:136f | Intel           | Iris Plus Graphics G7    | 33.3%  | 5.5.2    | F56B772338 |
| 8086:8a52 | 1028:0979 | Intel           | Iris Plus Graphics G7    | 2.9%   | 5.0.0    | 43A70E3901 |
| 8086:8a52 | 1028:097c | Intel           | Iris Plus Graphics G7    | 28.6%  | 5.3.0    | 66554C2B07 |
| 8086:8a52 | 103c:86c9 | Intel           | Iris Plus Graphics G7    | 6.7%   | 5.3.0    | 19D3840414 |
| 8086:8a52 | 17aa:3ff1 | Intel           | Iris Plus Graphics G7    | 15.4%  | 5.3.0    | 3F4D79EA3B |
| 8086:8a56 | 1025:1422 | Intel           | Iris Plus Graphics G1... | 11.8%  | 5.3.0    | 9C0A212B9F |
| 8086:8a56 | 1028:0979 | Intel           | Iris Plus Graphics G1... | 5.7%   | 5.0.0    | 7F4CE08DF9 |
| 8086:8a56 | 1028:097a | Intel           | Iris Plus Graphics G1... | 22.2%  | 5.0.0    | 17D09024B3 |
| 8086:8a56 | 103c:868a | Intel           | Iris Plus Graphics G1... | 25%    | 5.4.0    | 9F4F9A0186 |
| 8086:8a56 | 103c:86ab | Intel           | Iris Plus Graphics G1... | 25%    | 5.4.0    | 4019B6C1FF |
| 8086:8a56 | 103c:875b | Intel           | Iris Plus Graphics G1... | 33.3%  | 5.8.0    | 63ED12357B |
| 8086:8a56 | 1043:1ec1 | Intel           | Iris Plus Graphics G1... | 2.9%   | 5.3.0    | 347D45179A |
| 8086:8a56 | 17aa:3852 | Intel           | Iris Plus Graphics G1... | 4%     | 5.4.0    | 0426A1C07E |
| 8086:8a56 | 17aa:3fdc | Intel           | Iris Plus Graphics G1... | 2%     | 5.3.0    | 24F6BEC1FE |
| 8086:8a5a | 103c:86c8 | Intel           | Iris Plus Graphics G4... | 20%    | 5.4.8    | 16DBE6C7CF |
| 8086:9840 | 144d:c18b | Intel           | UHD Graphics, LKF        | 100%   |          | 6D40FDC958 |
| 8086:9a40 | 17aa:22c7 | Intel           | Tiger Lake Iris Xe Gr... | 50%    | 5.8.0    | 49AAD4B320 |
| 8086:9a49 | 1025:1464 | Intel           | TigerLake-LP GT2 [Iri... | 40%    | 5.8.0    | 731F04B1C6 |
| 8086:9a49 | 1025:1507 | Intel           | TigerLake-LP GT2 [Iri... | 66.7%  | 5.8.0    | 9A7CCA485D |
| 8086:9a49 | 1028:0991 | Intel           | TigerLake-LP GT2 [Iri... | 2.2%   | 5.6.0    | 5A7035D3AC |
| 8086:9a49 | 1028:09de | Intel           | TigerLake-LP GT2 [Iri... | 66.7%  | 5.8.0    | 65286CB6D4 |
| 8086:9a49 | 1028:09ff | Intel           | TigerLake-LP GT2 [Iri... | 4.2%   | 5.8.0    | 20E30AE2DE |
| 8086:9a49 | 1028:0a02 | Intel           | TigerLake-LP GT2 [Iri... | 25%    | 5.8.0    | F82797555A |
| 8086:9a49 | 1028:0a03 | Intel           | TigerLake-LP GT2 [Iri... | 50%    | 5.8.0    | 03AA94F52F |
| 8086:9a49 | 1028:0a05 | Intel           | TigerLake-LP GT2 [Iri... | 25%    | 5.8.0    | 7DBDF36326 |
| 8086:9a49 | 1028:0a25 | Intel           | TigerLake-LP GT2 [Iri... | 40%    | 5.8.0    | 84B300D969 |
| 8086:9a49 | 103c:87c9 | Intel           | TigerLake-LP GT2 [Iri... | 33.3%  | 5.11.0   | 865565B3CF |
| 8086:9a49 | 103c:87e1 | Intel           | TigerLake-LP GT2 [Iri... | 25%    | 5.8.0    | 17973D035D |
| 8086:9a49 | 103c:87f4 | Intel           | TigerLake-LP GT2 [Iri... | 16.7%  | 5.8.0    | CA6170372F |
| 8086:9a49 | 103c:87fe | Intel           | TigerLake-LP GT2 [Iri... | 20%    | 5.8.0    | 888E055121 |
| 8086:9a49 | 103c:881d | Intel           | TigerLake-LP GT2 [Iri... | 50%    | 5.11.18  | 2FF3765461 |
| 8086:9a49 | 103c:8823 | Intel           | TigerLake-LP GT2 [Iri... | 50%    | 5.10.14  | 4FDB80F31D |
| 8086:9a49 | 1043:1452 | Intel           | TigerLake-LP GT2 [Iri... | 25%    | 5.6.0    | A9E2DF4121 |
| 8086:9a49 | 1043:1ebf | Intel           | TigerLake-LP GT2 [Iri... | 33.3%  | 5.6.0    | 942ABB0546 |
| 8086:9a49 | 1462:12d2 | Intel           | TigerLake-LP GT2 [Iri... | 30%    | 5.8.0    | 465BEDF341 |
| 8086:9a49 | 17aa:3f19 | Intel           | TigerLake-LP GT2 [Iri... | 50%    | 5.10.29  | 89AE55D07E |
| 8086:9a49 | 17aa:5088 | Intel           | TigerLake-LP GT2 [Iri... | 12%    | 5.8.0    | C5ED725F00 |
| 8086:9a49 | 17aa:508f | Intel           | TigerLake-LP GT2 [Iri... | 100%   |          | 241B13488E |
| 8086:9a49 | 1e39:a025 | Intel           | TigerLake-LP GT2 [Iri... | 16.7%  | 5.9.11   | D34DDAC4F0 |
| 8086:9a78 | 103c:87cb | Intel           | Tiger Lake UHD Graphics  | 100%   |          | 0020768470 |
| 8086:9a78 | 103c:881d | Intel           | Tiger Lake UHD Graphics  | 100%   |          | 8889DC5AD5 |
| 8086:9b21 | 103c:85f1 | Intel           | Comet Lake UHD Graphics  | 20%    | 5.4.0    | 733DA06DF4 |
| 8086:9b41 | 1028:0954 | Intel           | CometLake-U GT2 [UHD ... | 50%    | 5.8.0    | 8740133E10 |
| 8086:9b41 | 1028:0962 | Intel           | CometLake-U GT2 [UHD ... | 1.6%   | 4.15.0   | E69F835F2B |
| 8086:9b41 | 1028:0969 | Intel           | CometLake-U GT2 [UHD ... | 100%   |          | 7ABAC766F3 |
| 8086:9b41 | 1028:096a | Intel           | CometLake-U GT2 [UHD ... | 14.3%  | 5.4.0    | 6DC830E5A6 |
| 8086:9b41 | 103c:869d | Intel           | CometLake-U GT2 [UHD ... | 5%     | 5.0.0    | 2230D28A9A |
| 8086:9b41 | 103c:86b1 | Intel           | CometLake-U GT2 [UHD ... | 15.4%  | 5.3.0    | CEE2AFAE3D |
| 8086:9b41 | 1043:156f | Intel           | CometLake-U GT2 [UHD ... | 6.7%   | 5.0.0    | 2C64A52714 |
| 8086:9b41 | 1462:1279 | Intel           | CometLake-U GT2 [UHD ... | 8.3%   | 5.3.0    | 27665BDA0E |
| 8086:9b41 | 1462:b183 | Intel           | CometLake-U GT2 [UHD ... | 54.5%  | 5.3.0    | 3C1185BE29 |
| 8086:9b41 | 17aa:3185 | Intel           | CometLake-U GT2 [UHD ... | 100%   |          | 324F862858 |
| 8086:9b41 | 17aa:382f | Intel           | CometLake-U GT2 [UHD ... | 4.2%   | 5.3.0    | E6E2F26ADE |
| 8086:9b41 | 17aa:3fb2 | Intel           | CometLake-U GT2 [UHD ... | 66.7%  | 5.0.0    | 3890D7877D |
| 8086:9b41 | 17aa:5079 | Intel           | CometLake-U GT2 [UHD ... | 1.7%   | 5.0.0    | 43BE642DA5 |
| 8086:9b41 | 17aa:507c | Intel           | CometLake-U GT2 [UHD ... | 3.8%   | 5.4.0    | 8C056E4751 |
| 8086:9b41 | 1d05:107a | Intel           | CometLake-U GT2 [UHD ... | 14.3%  | 5.4.0    | D412087992 |
| 8086:9b41 | 8086:2081 | Intel           | CometLake-U GT2 [UHD ... | 2.9%   | 5.4.0    | D942ED05B5 |
| 8086:9ba8 | 1458:d000 | Intel           | Comet Lake UHD Graphics  | 20%    | 5.4.0    | ABD511B277 |
| 8086:9bc4 | 1025:142f | Intel           | CometLake-H GT2 [UHD ... | 20%    | 4.18.0   | CEA1EFD2F4 |
| 8086:9bc4 | 1028:098f | Intel           | CometLake-H GT2 [UHD ... | 2.6%   | 5.4.0    | 84387A75F7 |
| 8086:9bc4 | 1028:09c3 | Intel           | CometLake-H GT2 [UHD ... | 6.7%   | 5.4.0    | 9362340E6C |
| 8086:9bc4 | 1028:09e1 | Intel           | CometLake-H GT2 [UHD ... | 12.5%  | 5.4.0    | 387113EA62 |
| 8086:9bc4 | 1462:12aa | Intel           | CometLake-H GT2 [UHD ... | 7.7%   | 5.4.0    | 9D39878AE6 |
| 8086:9bc4 | 17aa:3fa2 | Intel           | CometLake-H GT2 [UHD ... | 11.1%  | 5.4.57   | 66DE8410B3 |
| 8086:9bc5 | 1043:8694 | Intel           | CometLake-S GT2 [UHD ... | 9.1%   | 5.4.0    | 9B055BD98D |
| 8086:9bc5 | 1462:7c75 | Intel           | CometLake-S GT2 [UHD ... | 33.3%  | 5.4.0    | A29449D114 |
| 8086:9bc5 | 8086:2212 | Intel           | CometLake-S GT2 [UHD ... | 16.7%  | 5.4.0    | ECF016BAF2 |
| 8086:9bc6 | 1028:09f6 | Intel           | UHD P630 Graphics        | 100%   |          | 1F5B92D91B |
| 8086:9bc6 | 103c:8755 | Intel           | UHD P630 Graphics        | 100%   |          | 334ABF8C53 |
| 8086:9bc8 | 1028:0984 | Intel           | CometLake-S GT2 [UHD ... | 50%    | 5.0.0    | 3A565370DE |
| 8086:9bc8 | 103c:8710 | Intel           | CometLake-S GT2 [UHD ... | 33.3%  | 5.4.116  | A862C9D728 |
| 8086:9bc8 | 103c:871c | Intel           | CometLake-S GT2 [UHD ... | 100%   |          | 2F7FD6200F |
| 8086:9bc8 | 1043:8694 | Intel           | CometLake-S GT2 [UHD ... | 8.7%   | 5.4.0    | 062FE68B97 |
| 8086:9bc8 | 17aa:317e | Intel           | CometLake-S GT2 [UHD ... | 75%    | 5.11.10  | B2E207F67B |
| 8086:9bca | 1028:09a0 | Intel           | Comet Lake UHD Graphics  | 50%    | 5.9.0    | 916DB21F7F |
| 8086:9bca | 1462:129c | Intel           | Comet Lake UHD Graphics  | 2.9%   | 5.3.0    | 754F3C176F |
| 8086:9bca | 8086:2081 | Intel           | Comet Lake UHD Graphics  | 7.5%   | 4.18.0   | A161A19F04 |
| 8086:a001 | 1043:83e6 | Intel           | Atom Processor D4xx/D... | 21.4%  | 4.9.20   | 47E870B0B9 |
| 8086:a001 | 1458:d000 | Intel           | Atom Processor D4xx/D... | 14.8%  | 3.10.0   | 4C598BFFF1 |
| 8086:a001 | 1849:a001 | Intel           | Atom Processor D4xx/D... | 5.9%   | 3.10.0   | 20089C34B5 |
| 8086:a001 | 8086:4f4d | Intel           | Atom Processor D4xx/D... | 5%     | 3.10.0   | A8297FFB6C |
| 8086:a001 | 8086:a001 | Intel           | Atom Processor D4xx/D... | 6.7%   | 3.14.44  | B672C68361 |
| 8086:a011 | 1025:0349 | Intel           | Atom Processor D4xx/D... | 0.7%   | 3.14.44  | CACD668025 |
| 8086:a011 | 1462:104e | Intel           | Atom Processor D4xx/D... | 20%    | 4.1.15   | 5F15F028A8 |

### Modem (PCI)

86 out of 145 (59.31%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1002:4378 | 103c:3085 | AMD             | IXP SB400 AC'97 Modem... | 68%    | 4.15.0   | 8B13FEAD92 |
| 1039:7013 | 1025:0082 | Silicon Inte... | AC'97 Modem Controller   | 100%   |          | EDF0363AFE |
| 1039:7013 | 1025:0083 | Silicon Inte... | AC'97 Modem Controller   | 92.9%  | 4.19.0   | 464DA49516 |
| 1039:7013 | 1043:1696 | Silicon Inte... | AC'97 Modem Controller   | 100%   |          | D385784B22 |
| 1039:7013 | 1043:1816 | Silicon Inte... | AC'97 Modem Controller   | 58.3%  | 3.14.25  | AA92B168C5 |
| 1039:7013 | 104d:814e | Silicon Inte... | AC'97 Modem Controller   | 50%    | 3.14.44  | 11D39BBA01 |
| 1039:7013 | 1558:4201 | Silicon Inte... | AC'97 Modem Controller   | 100%   |          | 5B191FE82E |
| 1039:7013 | 1584:4003 | Silicon Inte... | AC'97 Modem Controller   | 60%    | 3.10.0   | E9BC9B3C8A |
| 1039:7013 | 1734:106c | Silicon Inte... | AC'97 Modem Controller   | 100%   |          | BFFEEEDE0D |
| 1057:3052 | 1057:3020 | Motorola        | SM56 Data Fax Modem      | 100%   |          | 5850550628 |
| 1057:3052 | 1631:3034 | Motorola        | SM56 Data Fax Modem      | 100%   |          | B7CEC1644D |
| 10b9:5457 | 103c:0850 | ULi Electronics | M5457 AC'97 Modem Con... | 100%   |          | 4E9D284D9C |
| 10b9:5457 | 104d:8158 | ULi Electronics | M5457 AC'97 Modem Con... | 100%   |          | 7E4F74E16A |
| 10b9:5457 | 1071:8351 | ULi Electronics | M5457 AC'97 Modem Con... | 100%   |          | 7806C7E5CD |
| 10b9:5457 | 10cf:130f | ULi Electronics | M5457 AC'97 Modem Con... | 100%   |          | 347EB6B747 |
| 10de:00d9 | 103c:006d | Nvidia          | nForce3 Audio            | 100%   |          | 564B583FED |
| 10de:00d9 | 1043:1856 | Nvidia          | nForce3 Audio            | 50%    | 4.9.60   | 0A302BFAFD |
| 1106:3068 |           | VIA Technolo... | AC'97 Modem Controller   | 3.7%   | 3.14.44  | C469D16946 |
| 11c1:0440 | 11c1:0440 | LSI             | 56k WinModem             | 100%   |          | 31EAA72C65 |
| 11c1:0448 | 1014:0131 | LSI             | WinModem 56k             | 100%   |          | F004231106 |
| 11c1:0449 | 1468:0410 | LSI             | L56xM+S [Mars-2] WinM... | 100%   |          | A8A13EFBA0 |
| 11c1:044c | 11c1:044c | LSI             | LT WinModem              | 100%   |          | 34D12D37FD |
| 11c1:044e | 11c1:044e | LSI             | LT WinModem              | 100%   |          | DA6AB84289 |
| 11c1:044e | 1235:044e | LSI             | LT WinModem              | 100%   |          | C22EB5394A |
| 11c1:044e | 13e0:0401 | LSI             | LT WinModem              | 100%   |          | E9ACA9663F |
| 11c1:0450 | 144f:1515 | LSI             | LT WinModem              | 100%   |          | 32D5B1A614 |
| 134d:7890 | 134d:0001 | PCTel           | HSP MicroModem 56        | 33.3%  | 5.3.0    | 332DDF27C1 |
| 1543:3052 | 1543:3000 | SILICON Labo... | Intel 537 [Winmodem]     | 100%   |          | 6B3BFC1719 |
| 2000:2800 | 122d:2800 | Smart Link      | SmartPCI2800 V.92 PCI... | 100%   |          | 3BC558699A |
| 2000:2800 | 163c:2800 | Smart Link      | SmartPCI2800 V.92 PCI... | 100%   |          | 9DEE04D2CB |
| 2003:8800 | 16ef:2800 | Smart Link      | LM-I56N                  | 100%   |          | 8B4AE6CF41 |
| 2003:8800 | 1801:2800 | Smart Link      | LM-I56N                  | 100%   |          | 62AFB6C0F6 |
| 8086:1040 | 8086:1000 | Intel           | 536EP Data Fax Modem     | 100%   |          | F2CC8FAE4D |
| 8086:2446 | 1025:1027 | Intel           | 82801BA/BAM AC'97 Mod... | 100%   |          | E0A83557FF |
| 8086:2446 | 1179:0001 | Intel           | 82801BA/BAM AC'97 Mod... | 100%   |          | 89EB89D54A |
| 8086:2486 | 1014:0223 | Intel           | 82801CA/CAM AC'97 Mod... | 50%    | 4.9.0    | B6D0B8758E |
| 8086:2486 | 1014:0227 | Intel           | 82801CA/CAM AC'97 Mod... | 100%   |          | 65D3C4C3C2 |
| 8086:2486 | 1043:1496 | Intel           | 82801CA/CAM AC'97 Mod... | 100%   |          | 1E7DA431AF |
| 8086:2486 | 134d:4c21 | Intel           | 82801CA/CAM AC'97 Mod... | 100%   |          | 5489DF545B |
| 8086:2486 | 14f1:5421 | Intel           | 82801CA/CAM AC'97 Mod... | 100%   |          | 4F9273C63C |
| 8086:24c6 | 1014:0524 | Intel           | 82801DB/DBL/DBM (ICH4... | 54.5%  | 4.9.200  | 71DAF2C5B4 |
| 8086:24c6 | 1014:0525 | Intel           | 82801DB/DBL/DBM (ICH4... | 100%   |          | ED7FD6C653 |
| 8086:24c6 | 1014:0559 | Intel           | 82801DB/DBL/DBM (ICH4... | 85.7%  | 3.14.53  | 58F9CE5671 |
| 8086:24c6 | 1014:055a | Intel           | 82801DB/DBL/DBM (ICH4... | 16.7%  | 3.14.44  | 190737F754 |
| 8086:24c6 | 1025:005a | Intel           | 82801DB/DBL/DBM (ICH4... | 100%   |          | 21602D608F |
| 8086:24c6 | 1025:0064 | Intel           | 82801DB/DBL/DBM (ICH4... | 100%   |          | C7045484B1 |
| 8086:24c6 | 103c:0890 | Intel           | 82801DB/DBL/DBM (ICH4... | 100%   |          | 44DF53B183 |
| 8086:24c6 | 103c:3080 | Intel           | 82801DB/DBL/DBM (ICH4... | 50%    | 4.19.0   | 6802B34FDD |
| 8086:24c6 | 103c:3084 | Intel           | 82801DB/DBL/DBM (ICH4... | 100%   |          | 24A093E347 |
| 8086:24c6 | 107b:0360 | Intel           | 82801DB/DBL/DBM (ICH4... | 100%   |          | 53EC93715E |
| 8086:24c6 | 10cf:10d1 | Intel           | 82801DB/DBL/DBM (ICH4... | 66.7%  | 3.14.25  | EA732BEA27 |
| 8086:24c6 | 1179:0001 | Intel           | 82801DB/DBL/DBM (ICH4... | 80%    | 4.9.0    | FBF8640D2E |
| 8086:24c6 | 1179:ff31 | Intel           | 82801DB/DBL/DBM (ICH4... | 80%    | 4.1.38   | E9BD04F647 |
| 8086:24c6 | 14f1:5422 | Intel           | 82801DB/DBL/DBM (ICH4... | 35.7%  | 3.14.44  | 60A32F7736 |
| 8086:24c6 | 1584:4007 | Intel           | 82801DB/DBL/DBM (ICH4... | 100%   |          | F13A21C874 |
| 8086:24c6 | 1631:d004 | Intel           | 82801DB/DBL/DBM (ICH4... | 100%   |          | 2EE7FA4DA9 |
| 8086:24c6 | 1734:103c | Intel           | 82801DB/DBL/DBM (ICH4... | 100%   |          | 6F452862B4 |
| 8086:24d6 | 1025:0045 | Intel           | 82801EB/ER (ICH5/ICH5... | 100%   |          | 41CC7EB08C |
| 8086:24d6 | 103c:006a | Intel           | 82801EB/ER (ICH5/ICH5... | 100%   |          | 66FC1D68B2 |
| 8086:24d6 | 104d:816f | Intel           | 82801EB/ER (ICH5/ICH5... | 100%   |          | AB742E4CF2 |
| 8086:24d6 | 1179:0001 | Intel           | 82801EB/ER (ICH5/ICH5... | 100%   |          | A7D4DEEF9E |
| 8086:24d6 | 14e4:4d64 | Intel           | 82801EB/ER (ICH5/ICH5... | 100%   |          | A30A53108B |
| 8086:266d |           | Intel           | 82801FB/FBM/FR/FW/FRW... | 100%   |          | D8653C0683 |
| 8086:266d | 1014:0574 | Intel           | 82801FB/FBM/FR/FW/FRW... | 75%    | 4.9.20   | DAB32CED08 |
| 8086:266d | 1014:0576 | Intel           | 82801FB/FBM/FR/FW/FRW... | 60%    | 3.14.33  | E323E5FE53 |
| 8086:266d | 1025:0066 | Intel           | 82801FB/FBM/FR/FW/FRW... | 66.7%  | 3.14.44  | 10A0D7E3A2 |
| 8086:266d | 1025:006a | Intel           | 82801FB/FBM/FR/FW/FRW... | 53.3%  | 3.14.25  | 93DAE491F3 |
| 8086:266d | 1033:8293 | Intel           | 82801FB/FBM/FR/FW/FRW... | 50%    | 4.19.0   | C65BC992C6 |
| 8086:266d | 103c:0934 | Intel           | 82801FB/FBM/FR/FW/FRW... | 100%   |          | 453696FF5E |
| 8086:266d | 103c:0944 | Intel           | 82801FB/FBM/FR/FW/FRW... | 66.7%  | 3.14.44  | 7F042FAA64 |
| 8086:266d | 103c:099c | Intel           | 82801FB/FBM/FR/FW/FRW... | 27.3%  | 3.14.44  | 932C3D4CC2 |
| 8086:266d | 103c:3080 | Intel           | 82801FB/FBM/FR/FW/FRW... | 50%    | 4.9.9    | 0572E8425C |
| 8086:266d | 103c:3081 | Intel           | 82801FB/FBM/FR/FW/FRW... | 40%    | 5.3.0    | DC4B912BFC |
| 8086:266d | 103c:3082 | Intel           | 82801FB/FBM/FR/FW/FRW... | 100%   |          | C98B9CF200 |
| 8086:266d | 103c:309d | Intel           | 82801FB/FBM/FR/FW/FRW... | 33.3%  | 4.1.16   | 837230178B |
| 8086:266d | 103c:30c4 | Intel           | 82801FB/FBM/FR/FW/FRW... | 80%    | 4.1.25   | FE8A07348F |
| 8086:266d | 107b:0215 | Intel           | 82801FB/FBM/FR/FW/FRW... | 100%   |          | 15D8283384 |
| 8086:266d | 107b:0460 | Intel           | 82801FB/FBM/FR/FW/FRW... | 100%   |          | B62ECA10E8 |
| 8086:266d | 1179:0001 | Intel           | 82801FB/FBM/FR/FW/FRW... | 85.7%  | 3.14.44  | B99ABFD9D6 |
| 8086:266d | 1179:ff31 | Intel           | 82801FB/FBM/FR/FW/FRW... | 25%    | 4.1.34   | FBAEC7A912 |
| 8086:266d | 144d:2115 | Intel           | 82801FB/FBM/FR/FW/FRW... | 40%    | 4.1.22   | 88BAF3B388 |
| 8086:266d | 14f1:5423 | Intel           | 82801FB/FBM/FR/FW/FRW... | 61.5%  | 3.14.44  | CA3886900F |
| 8086:266d | 161f:204f | Intel           | 82801FB/FBM/FR/FW/FRW... | 100%   |          | 07CC1E0952 |
| 8086:266d | 1631:c00b | Intel           | 82801FB/FBM/FR/FW/FRW... | 100%   |          | CCD46D5757 |
| 8086:266d | 17aa:207c | Intel           | 82801FB/FBM/FR/FW/FRW... | 100%   |          | EDAE63A429 |
| 8086:27dd |           | Intel           | 82801G (ICH7 Family) ... | 100%   |          | 151F16B506 |

### Multimedia controller (PCI)

331 out of 436 (75.92%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 0002:8290 | 107d:2609 |                 | Multimedia controller    | 100%   |          | 95D420F37F |
| 1002:4d51 | 1002:b041 | AMD             | Unified AVStream         | 100%   |          | E0EE188631 |
| 1002:4d52 | 1002:a346 | AMD             | Theater 550 PRO PCI [... | 100%   |          | FDE418F259 |
| 1002:4d53 | 1028:a503 | AMD             | Theater 550 PRO PCIe     | 100%   |          | A8D52F4DF8 |
| 1002:ac02 | 1002:b300 | AMD             | TV Wonder HD 600 PCIe    | 100%   |          | 47AC62397C |
| 1002:ac12 | 1002:b539 | AMD             | Theater HD T507 (DVB-... | 100%   |          | 01463318AC |
| 1002:ac12 | 1002:b935 | AMD             | Theater HD T507 (DVB-... | 100%   |          | B4CD2CBC1E |
| 1002:ac12 | 12ab:0003 | AMD             | Theater HD T507 (DVB-... | 100%   |          | 4E3343DADF |
| 1002:ad18 | 1682:ad18 | AMD             | Multimedia controller    | 100%   |          | 829182B838 |
| 1022:15e2 | 1022:15e2 | AMD             | Raven/Raven2/FireFlig... | 40.6%  | 4.18.0   | 3F202F2D16 |
| 1022:15e2 | 1025:1233 | AMD             | Raven/Raven2/FireFlig... | 38.9%  | 5.0.0    | A94A021F5E |
| 1022:15e2 | 1025:134d | AMD             | Raven/Raven2/FireFlig... | 22.9%  | 5.0.0    | 1D914DF010 |
| 1022:15e2 | 1025:134f | AMD             | Raven/Raven2/FireFlig... | 25.8%  | 5.0.0    | A368A3C0C8 |
| 1022:15e2 | 1025:1378 | AMD             | Raven/Raven2/FireFlig... | 20%    | 5.3.0    | FDE9376452 |
| 1022:15e2 | 1025:1455 | AMD             | Raven/Raven2/FireFlig... | 12.5%  | 5.4.0    | 19F0A0EEED |
| 1022:15e2 | 1025:1456 | AMD             | Raven/Raven2/FireFlig... | 30.8%  | 5.4.0    | E156DE8003 |
| 1022:15e2 | 1025:1461 | AMD             | Raven/Raven2/FireFlig... | 11.4%  | 5.4.0    | EFD658792F |
| 1022:15e2 | 1028:09f5 | AMD             | Raven/Raven2/FireFlig... | 16.7%  | 5.8.0    | 9D7D4C771B |
| 1022:15e2 | 1028:0a12 | AMD             | Raven/Raven2/FireFlig... | 33.3%  | 5.8.0    | 3B4E5DC713 |
| 1022:15e2 | 1028:0a1e | AMD             | Raven/Raven2/FireFlig... | 11.1%  | 5.4.0    | 5DAC15D30A |
| 1022:15e2 | 103c:8433 | AMD             | Raven/Raven2/FireFlig... | 22.7%  | 5.0.0    | 32C974B562 |
| 1022:15e2 | 103c:8434 | AMD             | Raven/Raven2/FireFlig... | 50%    | 5.0.0    | E2E650868B |
| 1022:15e2 | 103c:8496 | AMD             | Raven/Raven2/FireFlig... | 33.3%  | 5.0.0    | A36C150859 |
| 1022:15e2 | 103c:84a2 | AMD             | Raven/Raven2/FireFlig... | 11.1%  | 5.3.0    | 220E290FCB |
| 1022:15e2 | 103c:84a3 | AMD             | Raven/Raven2/FireFlig... | 100%   |          | 6A706DA421 |
| 1022:15e2 | 103c:84ae | AMD             | Raven/Raven2/FireFlig... | 54.1%  | 5.0.0    | B243C0380F |
| 1022:15e2 | 103c:84af | AMD             | Raven/Raven2/FireFlig... | 66.7%  | 5.0.0    | 8A858D88D0 |
| 1022:15e2 | 103c:84d2 | AMD             | Raven/Raven2/FireFlig... | 68%    | 5.3.0    | F83DDC3D9D |
| 1022:15e2 | 103c:85b1 | AMD             | Raven/Raven2/FireFlig... | 25%    | 5.3.0    | 87CABD058E |
| 1022:15e2 | 103c:85b3 | AMD             | Raven/Raven2/FireFlig... | 31.7%  | 5.0.0    | F492073A06 |
| 1022:15e2 | 103c:85dd | AMD             | Raven/Raven2/FireFlig... | 14.6%  | 5.0.0    | ABF11EF628 |
| 1022:15e2 | 103c:85de | AMD             | Raven/Raven2/FireFlig... | 16%    | 5.3.0    | C764C0655E |
| 1022:15e2 | 103c:85e0 | AMD             | Raven/Raven2/FireFlig... | 31.8%  | 5.0.0    | BFCA277988 |
| 1022:15e2 | 103c:85ea | AMD             | Raven/Raven2/FireFlig... | 29.2%  | 5.0.0    | E5A505D84F |
| 1022:15e2 | 103c:86d4 | AMD             | Raven/Raven2/FireFlig... | 37.5%  | 5.4.0    | 0C1B37ACD2 |
| 1022:15e2 | 103c:86d5 | AMD             | Raven/Raven2/FireFlig... | 27.8%  | 5.3.0    | 11DD7F0A3B |
| 1022:15e2 | 103c:86d6 | AMD             | Raven/Raven2/FireFlig... | 37.5%  | 5.4.0    | 9BE60C8533 |
| 1022:15e2 | 103c:86fd | AMD             | Raven/Raven2/FireFlig... | 32.6%  | 5.3.18   | 2AE02BC53F |
| 1022:15e2 | 103c:8706 | AMD             | Raven/Raven2/FireFlig... | 45.5%  | 5.4.0    | DF7F4634BC |
| 1022:15e2 | 103c:8730 | AMD             | Raven/Raven2/FireFlig... | 22.1%  | 5.4.0    | ED8C410826 |
| 1022:15e2 | 103c:8735 | AMD             | Raven/Raven2/FireFlig... | 29.2%  | 5.8.0    | 85C7810586 |
| 1022:15e2 | 103c:8760 | AMD             | Raven/Raven2/FireFlig... | 6.4%   | 5.3.18   | 50B75A0212 |
| 1022:15e2 | 103c:876e | AMD             | Raven/Raven2/FireFlig... | 5.2%   | 5.4.0    | 12A3ADEDE5 |
| 1022:15e2 | 103c:876f | AMD             | Raven/Raven2/FireFlig... | 2.4%   | 5.4.0    | 5EAE12F393 |
| 1022:15e2 | 103c:879c | AMD             | Raven/Raven2/FireFlig... | 66.7%  | 5.8.0    | EA09357867 |
| 1022:15e2 | 103c:879e | AMD             | Raven/Raven2/FireFlig... | 40%    | 5.4.0    | 44F3BFB1B0 |
| 1022:15e2 | 103c:87b0 | AMD             | Raven/Raven2/FireFlig... | 20%    | 5.4.0    | 8B778E7903 |
| 1022:15e2 | 103c:87b1 | AMD             | Raven/Raven2/FireFlig... | 45.8%  | 5.7.12   | 1D95F1FECA |
| 1022:15e2 | 103c:87b2 | AMD             | Raven/Raven2/FireFlig... | 33.3%  | 5.4.0    | 56BAAFF907 |
| 1022:15e2 | 103c:87cf | AMD             | Raven/Raven2/FireFlig... | 12.5%  | 5.4.0    | 530BE6CE7B |
| 1022:15e2 | 103c:87da | AMD             | Raven/Raven2/FireFlig... | 75%    | 5.11.0   | 8647F6F8FB |
| 1022:15e2 | 1043:11f2 | AMD             | Raven/Raven2/FireFlig... | 80%    | 5.8.0    | 974B8F73D1 |
| 1022:15e2 | 1043:1e8e | AMD             | Raven/Raven2/FireFlig... | 33.3%  | 5.10.32  | A488AFB982 |
| 1022:15e2 | 1462:12b5 | AMD             | Raven/Raven2/FireFlig... | 31.8%  | 5.4.0    | 649DBCEEFF |
| 1022:15e2 | 1462:12c8 | AMD             | Raven/Raven2/FireFlig... | 20%    | 5.4.0    | 67ABD4509A |
| 1022:15e2 | 1558:a500 | AMD             | Raven/Raven2/FireFlig... | 33.3%  | 5.4.0    | C38A7587DB |
| 1022:15e2 | 17aa:36f5 | AMD             | Raven/Raven2/FireFlig... | 60%    | 5.5.9    | 7E41940C9C |
| 1022:15e2 | 17aa:3708 | AMD             | Raven/Raven2/FireFlig... | 66.7%  | 5.8.0    | F8BAB84CFF |
| 1022:15e2 | 17aa:371c | AMD             | Raven/Raven2/FireFlig... | 100%   |          | 65195D0D22 |
| 1022:15e2 | 17aa:3807 | AMD             | Raven/Raven2/FireFlig... | 39.3%  | 5.4.0    | A36A726BBA |
| 1022:15e2 | 17aa:380b | AMD             | Raven/Raven2/FireFlig... | 57.1%  | 5.3.0    | 932B22C52A |
| 1022:15e2 | 17aa:380f | AMD             | Raven/Raven2/FireFlig... | 28.6%  | 5.4.0    | A91B62859A |
| 1022:15e2 | 17aa:3811 | AMD             | Raven/Raven2/FireFlig... | 50%    | 5.0.0    | 3CC715F92A |
| 1022:15e2 | 17aa:3812 | AMD             | Raven/Raven2/FireFlig... | 20.9%  | 5.0.0    | F2B808BDD1 |
| 1022:15e2 | 17aa:3813 | AMD             | Raven/Raven2/FireFlig... | 30.8%  | 5.0.0    | BD4A9E7910 |
| 1022:15e2 | 17aa:3814 | AMD             | Raven/Raven2/FireFlig... | 28.4%  | 5.0.0    | FC8C52785D |
| 1022:15e2 | 17aa:381b | AMD             | Raven/Raven2/FireFlig... | 22.9%  | 5.4.0    | 5287CEEF8D |
| 1022:15e2 | 17aa:381c | AMD             | Raven/Raven2/FireFlig... | 15.9%  | 5.4.0    | 3F4B15A31D |
| 1022:15e2 | 17aa:381f | AMD             | Raven/Raven2/FireFlig... | 42.1%  | 5.4.0    | DB1626E471 |
| 1022:15e2 | 17aa:3821 | AMD             | Raven/Raven2/FireFlig... | 19.2%  | 5.4.0    | 7C2EF960B5 |
| 1022:15e2 | 17aa:3822 | AMD             | Raven/Raven2/FireFlig... | 3.4%   | 5.4.0    | CE6E4E8A2D |
| 1022:15e2 | 17aa:3823 | AMD             | Raven/Raven2/FireFlig... | 16%    | 5.4.0    | 8355EE2CD4 |
| 1022:15e2 | 17aa:3824 | AMD             | Raven/Raven2/FireFlig... | 20%    | 5.8.0    | AAC20E8DCE |
| 1022:15e2 | 17aa:507e | AMD             | Raven/Raven2/FireFlig... | 20.5%  | 5.4.0    | E19A3D01B0 |
| 1022:15e2 | 17aa:507f | AMD             | Raven/Raven2/FireFlig... | 21.4%  | 5.4.0    | DC95288D50 |
| 1022:15e2 | 17aa:5081 | AMD             | Raven/Raven2/FireFlig... | 2.7%   | 5.4.0    | 8A19941FFE |
| 1022:15e2 | 17aa:5082 | AMD             | Raven/Raven2/FireFlig... | 25%    | 5.4.0    | 0E719D2807 |
| 1022:15e2 | 17aa:5083 | AMD             | Raven/Raven2/FireFlig... | 9.1%   | 5.8.9    | 1913C60408 |
| 1022:15e2 | 17aa:5084 | AMD             | Raven/Raven2/FireFlig... | 4%     | 5.4.0    | DE9EA1422C |
| 1022:15e2 | 17aa:5124 | AMD             | Raven/Raven2/FireFlig... | 17.4%  | 5.0.0    | D7FED90840 |
| 1022:15e2 | 17aa:5125 | AMD             | Raven/Raven2/FireFlig... | 27.9%  | 5.1.17   | BCF2604C43 |
| 1022:15e2 | 17aa:5126 | AMD             | Raven/Raven2/FireFlig... | 40.9%  | 5.0.0    | EB33727EFF |
| 1022:15e2 | 17aa:5127 | AMD             | Raven/Raven2/FireFlig... | 23.1%  | 5.3.0    | 643E539134 |
| 1022:15e2 | 19e5:3e06 | AMD             | Raven/Raven2/FireFlig... | 53.1%  | 5.0.0    | 7D8EF49865 |
| 1022:15e2 | 19e5:3e10 | AMD             | Raven/Raven2/FireFlig... | 18.8%  | 5.3.0    | 473A4DEBAC |
| 1022:15e2 | 19e5:3e14 | AMD             | Raven/Raven2/FireFlig... | 19.2%  | 5.4.0    | D029AEADEB |
| 1022:15e2 | 19e5:3e18 | AMD             | Raven/Raven2/FireFlig... | 29.1%  | 5.3.0    | 8D09FD5FAD |
| 1022:15e2 | 19e5:3e19 | AMD             | Raven/Raven2/FireFlig... | 11.2%  | 5.3.0    | C56A98FF8A |
| 1022:15e2 | 1a0e:1043 | AMD             | Raven/Raven2/FireFlig... | 32.3%  | 5.3.0    | DBAD55C117 |
| 1022:15e2 | 1d05:109f | AMD             | Raven/Raven2/FireFlig... | 40.7%  | 5.3.7    | EC0CB83241 |
| 1022:15e2 | 1d72:1951 | AMD             | Raven/Raven2/FireFlig... | 12.5%  | 5.4.0    | D609A6C4A1 |
| 1022:15e2 | 1d72:1953 | AMD             | Raven/Raven2/FireFlig... | 16.7%  | 5.4.0    | E38BDAE28D |
| 1022:15e2 | 1e21:1043 | AMD             | Raven/Raven2/FireFlig... | 24.4%  | 5.0.0    | 285DFADDB2 |
| 1022:15e2 | 1e83:3e33 | AMD             | Raven/Raven2/FireFlig... | 8.3%   | 5.4.0    | E6A375087E |
| 102b:8350 | 102b:9000 | Matrox Elect... | Matrox Multimedia con... | 100%   |          | B3EE98B7CC |
| 1057:1801 |           | Motorola        | DSP56301 Digital Sign... | 100%   |          | BA572256B0 |
| 1057:3410 | 1057:ffff | Motorola        | DSP56361 Digital Sign... | 100%   |          | 16A7890585 |
| 1057:3410 | 11af:eed2 | Motorola        | DSP56361 Digital Sign... | 100%   |          | 16A7890585 |
| 1057:3410 | 11af:eee1 | Motorola        | DSP56361 Digital Sign... | 100%   |          | 16A7890585 |
| 109e:037e | 1554:4001 | Brooktree       | Multimedia controller    | 100%   |          | 30BC79956D |
| 109e:0868 | 1554:4001 | Brooktree       | Multimedia controller    | 100%   |          | 30BC79956D |
| 109e:0878 |           | Brooktree       | Bt878 Audio Capture      | 97.8%  | 5.3.0    | 53A8C28AED |
| 109e:0878 | 0070:13e9 | Brooktree       | Bt878 Audio Capture      | 100%   |          | 10B0CA2195 |
| 109e:0878 | 0070:ff02 | Brooktree       | Bt878 Audio Capture      | 100%   |          | 84495E0FB8 |
| 109e:0878 | 0070:ff04 | Brooktree       | Bt878 Audio Capture      | 100%   |          | 2C877CF870 |
| 109e:0878 | 1002:0003 | Brooktree       | Bt878 Audio Capture      | 100%   |          | B03897D3E4 |
| 109e:0878 | 1047:f331 | Brooktree       | Bt878 Audio Capture      | 100%   |          | 444FFBC8A6 |
| 109e:0878 | 107d:6607 | Brooktree       | Bt878 Audio Capture      | 75%    | 4.9.20   | 502C4EB91B |
| 109e:0878 | 107d:6609 | Brooktree       | Bt878 Audio Capture      | 100%   |          | 31DFECDF4A |
| 109e:0878 | 11bd:0012 | Brooktree       | Bt878 Audio Capture      | 16.7%  | 4.1.34   | ECA8E2E768 |
| 109e:0878 | 1461:0001 | Brooktree       | Bt878 Audio Capture      | 100%   |          | E8072B6F3A |
| 109e:0878 | 1461:0002 | Brooktree       | Bt878 Audio Capture      | 100%   |          | A22609B54B |
| 109e:0878 | 1461:0003 | Brooktree       | Bt878 Audio Capture      | 4%     | 3.14.25  | 7A69435C43 |
| 109e:0878 | 1461:0004 | Brooktree       | Bt878 Audio Capture      | 100%   |          | F2B7867CAA |
| 109e:0878 | 153b:1118 | Brooktree       | Bt878 Audio Capture      | 100%   |          | DDFD3CC319 |
| 109e:0878 | 1852:1852 | Brooktree       | Bt878 Audio Capture      | 100%   |          | C560D2AA9B |
| 109e:0878 | 800a:763d | Brooktree       | Bt878 Audio Capture      | 100%   |          | 7E72574FF4 |
| 109e:0878 | 800b:763d | Brooktree       | Bt878 Audio Capture      | 100%   |          | 7E72574FF4 |
| 109e:0878 | 800c:763d | Brooktree       | Bt878 Audio Capture      | 100%   |          | 7E72574FF4 |
| 109e:0878 | 800d:763d | Brooktree       | Bt878 Audio Capture      | 100%   |          | 7E72574FF4 |
| 109e:0878 | aa03:1433 | Brooktree       | Bt878 Audio Capture      | 100%   |          | ABDBF93DB4 |
| 109e:0878 | aaff:1431 | Brooktree       | Bt878 Audio Capture      | 100%   |          | ABDBF93DB4 |
| 109e:0878 | bd11:4100 | Brooktree       | Bt878 Audio Capture      | 100%   |          | 34BC4E6EF8 |
| 109e:0878 | ffff:ffff | Brooktree       | Bt878 Audio Capture      | 100%   |          | A4B2A57CC3 |
| 10b5:9056 | 1a0e:006f | PLX Technology  | PCI9056 32-bit 66MHz ... | 100%   |          | C6B09D560F |
| 10b5:9056 | 1a0e:0073 | PLX Technology  | PCI9056 32-bit 66MHz ... | 50%    | 4.15.0   | 5122F7EE54 |
| 10cf:2026 | 1718:10c0 | Fujitsu Limi... | Fujitsu Multimedia co... | 100%   |          | 347EB6B747 |
| 10cf:202a | 104d:81fa | Fujitsu Limi... | Integrated MPEG Encoder  | 100%   |          | 7F0BB0CC92 |
| 10cf:202a | ffff:ffff | Fujitsu Limi... | Integrated MPEG Encoder  | 100%   |          | 911280F4FC |
| 10cf:2030 | 104d:9053 | Fujitsu Limi... | Fujitsu Multimedia co... | 100%   |          | CFDCAC5734 |
| 10cf:2030 | 104d:9062 | Fujitsu Limi... | Fujitsu Multimedia co... | 100%   |          | 2628EBE1BB |
| 10cf:2036 | 104d:906e | Fujitsu Limi... | DT-XXX                   | 100%   |          | 68937CF6BB |
| 10cf:2036 | 10fc:d05f | Fujitsu Limi... | DT-XXX                   | 100%   |          | F8D281DB4B |
| 10cf:2036 | 1718:190d | Fujitsu Limi... | DT-XXX                   | 100%   |          | 15202A6CAE |
| 10cf:2049 | 13fe:8701 | Fujitsu Limi... | Fujitsu Multimedia co... | 100%   |          | CFBB1B9F64 |
| 1105:8300 |           | Sigma Designs   | REALmagic Hollywood P... | 100%   |          | 3F170135D2 |
| 1131:5134 | 1019:4cb4 | Philips Semi... | Multimedia controller    | 100%   |          | E677B96DBA |
| 1131:5402 | 4954:5434 | Philips Semi... | TriMedia TM1300          | 100%   |          | 64A9C1D635 |
| 1131:7146 | 114b:201e | Philips Semi... | SAA7146                  | 100%   |          | 5681B93AAF |
| 1131:7146 | 11bd:0805 | Philips Semi... | SAA7146                  | 100%   |          | 60F6C8F96D |
| 1131:7160 | 1043:48b5 | Philips Semi... | SAA7160                  | 100%   |          | 6B30DD9FF7 |
| 1131:7160 | 107d:6686 | Philips Semi... | SAA7160                  | 100%   |          | 5BA05AC282 |
| 1131:7160 | 1131:0002 | Philips Semi... | SAA7160                  | 100%   |          | 0861B33243 |
| 1131:7160 | 1461:0455 | Philips Semi... | SAA7160                  | 100%   |          | F85808C04C |
| 1131:7160 | 1461:0555 | Philips Semi... | SAA7160                  | 100%   |          | C47AD5ED50 |
| 1131:7160 | 1461:0655 | Philips Semi... | SAA7160                  | 100%   |          | 58A8ECB02A |
| 1131:7160 | 1461:0855 | Philips Semi... | SAA7160                  | 100%   |          | BBDA8BED86 |
| 1131:7160 | 1461:0955 | Philips Semi... | SAA7160                  | 100%   |          | 613C8A1900 |
| 1131:7160 | 1461:0a55 | Philips Semi... | SAA7160                  | 100%   |          | 6F6DE0E938 |
| 1131:7160 | 1461:0e55 | Philips Semi... | SAA7160                  | 100%   |          | 08CED52205 |
| 1131:7160 | 1461:0f55 | Philips Semi... | SAA7160                  | 100%   |          | 7985ADDC49 |
| 1131:7160 | 1461:1055 | Philips Semi... | SAA7160                  | 100%   |          | 47374D1B5F |
| 1131:7160 | 1461:1455 | Philips Semi... | SAA7160                  | 100%   |          | 2D08F702CF |
| 1131:7160 | 1461:1855 | Philips Semi... | SAA7160                  | 100%   |          | FA070462FC |
| 1131:7160 | 1461:1e55 | Philips Semi... | SAA7160                  | 100%   |          | 06582DF260 |
| 1131:7160 | 1461:1f55 | Philips Semi... | SAA7160                  | 100%   |          | 0812A4EFC1 |
| 1131:7160 | 1461:2155 | Philips Semi... | SAA7160                  | 100%   |          | 27E7D42D53 |
| 1131:7160 | 1461:2355 | Philips Semi... | SAA7160                  | 100%   |          | 0574C9D2F7 |
| 1131:7160 | 1461:2655 | Philips Semi... | SAA7160                  | 100%   |          | A74B989748 |
| 1131:7160 | 1461:7561 | Philips Semi... | SAA7160                  | 100%   |          | 1CBEE8A7EF |
| 1131:7160 | 1461:7992 | Philips Semi... | SAA7160                  | 100%   |          | 3ACD33354F |
| 1131:7160 | 16be:0034 | Philips Semi... | SAA7160                  | 100%   |          | 2B8D93B7EC |
| 1131:7160 | 17de:7542 | Philips Semi... | SAA7160                  | 100%   |          | AAA454AA30 |
| 1131:7160 | 185b:e750 | Philips Semi... | SAA7160                  | 100%   |          | 262A709D45 |
| 1131:7160 | 1ae4:0700 | Philips Semi... | SAA7160                  | 100%   |          | FA3005B3D4 |
| 1131:7160 | 6221:0001 | Philips Semi... | SAA7160                  | 100%   |          | 1CDCECADAB |
| 1131:7160 | 6281:0001 | Philips Semi... | SAA7160                  | 15.8%  | 4.9.76   | 21E6F57AC5 |
| 1131:7160 | 6925:0001 | Philips Semi... | SAA7160                  | 100%   |          | B4E45EAE99 |
| 1131:7160 | 6928:0001 | Philips Semi... | SAA7160                  | 100%   |          | 8C8F8EFAB1 |
| 1131:7160 | 6928:0002 | Philips Semi... | SAA7160                  | 100%   |          | 2F7F236AF3 |
| 1131:7160 | e517:12ab | Philips Semi... | SAA7160                  | 100%   |          | 786069DE60 |
| 1131:7160 | e519:12ab | Philips Semi... | SAA7160                  | 100%   |          | 786069DE60 |
| 1131:7160 | f501:12ab | Philips Semi... | SAA7160                  | 100%   |          | E5F24075E5 |
| 1131:7162 | 11bd:0100 | Philips Semi... | SAA7162                  | 100%   |          | D495DD5272 |
| 1131:7162 | 11bd:0101 | Philips Semi... | SAA7162                  | 100%   |          | 3C6DF0441A |
| 1131:7162 | 14c7:3540 | Philips Semi... | SAA7162                  | 100%   |          | A084E40027 |
| 1131:7164 | 0070:8851 | Philips Semi... | SAA7164                  | 12.5%  | 3.14.22  | 9E32F34F8E |
| 1131:7231 | 0070:0810 | Philips Semi... | SAA7231                  | 100%   |          | 6CB625FE85 |
| 1131:7231 | 0070:49d1 | Philips Semi... | SAA7231                  | 100%   |          | 043F4AB102 |
| 1131:7231 | 12ab:0762 | Philips Semi... | SAA7231                  | 100%   |          | 29398A5494 |
| 1131:7231 | 12ab:0763 | Philips Semi... | SAA7231                  | 100%   |          | 20768D0E33 |
| 1131:7231 | 1461:0607 | Philips Semi... | SAA7231                  | 100%   |          | AE889D26D4 |
| 1131:7231 | 1461:0b07 | Philips Semi... | SAA7231                  | 100%   |          | C1EDE2C7D9 |
| 1131:7231 | 1461:0b0f | Philips Semi... | SAA7231                  | 100%   |          | 6752A255CA |
| 1131:7231 | 1461:110f | Philips Semi... | SAA7231                  | 100%   |          | 90DFBFB6FA |
| 1131:7231 | 1461:1400 | Philips Semi... | SAA7231                  | 100%   |          | 70C319B3C6 |
| 1131:7231 | 1461:1807 | Philips Semi... | SAA7231                  | 100%   |          | 7979049FAF |
| 1131:7231 | 1461:2a0f | Philips Semi... | SAA7231                  | 100%   |          | BEB8F313F7 |
| 1131:7231 | 1461:2b07 | Philips Semi... | SAA7231                  | 100%   |          | 8672A3F85D |
| 1131:7231 | 1461:2b0f | Philips Semi... | SAA7231                  | 100%   |          | 42BC05AF33 |
| 1131:7231 | 1461:3301 | Philips Semi... | SAA7231                  | 100%   |          | 7E1176A7C2 |
| 1131:7231 | 1461:7981 | Philips Semi... | SAA7231                  | 100%   |          | 928BFFA7DF |
| 1131:7231 | 1461:7983 | Philips Semi... | SAA7231                  | 100%   |          | 4365F32962 |
| 1131:7231 | 1461:890f | Philips Semi... | SAA7231                  | 100%   |          | 4C97361FFD |
| 1131:7231 | 16be:0002 | Philips Semi... | SAA7231                  | 100%   |          | 751F3FAAFA |
| 1131:7231 | 16be:0008 | Philips Semi... | SAA7231                  | 100%   |          | 9D7D398CC1 |
| 1131:7231 | 16be:0013 | Philips Semi... | SAA7231                  | 100%   |          | 157E1F057D |
| 1131:7231 | 1b0a:3001 | Philips Semi... | SAA7231                  | 100%   |          | 5EFEDE21E2 |
| 1131:7231 | 5ace:8000 | Philips Semi... | SAA7231                  | 100%   |          | FA070462FC |
| 1131:7231 | 5ace:8150 | Philips Semi... | SAA7231                  | 100%   |          | 8603D5BDF5 |
| 1131:7231 | 5ace:8201 | Philips Semi... | SAA7231                  | 100%   |          | 75F255A4E2 |
| 116e:00d0 | 116e:0000 | Electronics ... | Multimedia controller    | 100%   |          | 7823D71E26 |
| 116e:0600 | 116e:0012 | Electronics ... | Multimedia controller    | 100%   |          | 7823D71E26 |
| 11bd:0040 | 11bd:0045 | Pinnacle Sys... | Royal TS Function 1      | 100%   |          | 7793E267F5 |
| 11bd:0041 | 11bd:0045 | Pinnacle Sys... | RoyalTS Function 2       | 100%   |          | 7793E267F5 |
| 11bd:0042 | 11bd:0045 | Pinnacle Sys... | Royal TS Function 3      | 100%   |          | 7793E267F5 |
| 11bd:bed6 | 11bd:0022 | Pinnacle Sys... | Pinnacle Multimedia c... | 100%   |          | D805D39715 |
| 11bd:bede | 11bd:0022 | Pinnacle Sys... | AV/DV Studio Capture ... | 100%   |          | E4F384C278 |
| 11bd:bede | 11bd:0023 | Pinnacle Sys... | AV/DV Studio Capture ... | 100%   |          | FD7DE4EB5A |
| 11bd:bede | 11bd:0024 | Pinnacle Sys... | AV/DV Studio Capture ... | 100%   |          | D6BD28C216 |
| 123f:8120 | 10de:01e1 | LSI Logic       | DVxplore Codec           | 100%   |          | BF588FC977 |
| 123f:8120 | 11bd:0805 | LSI Logic       | DVxplore Codec           | 100%   |          | E4D5F651E2 |
| 123f:8120 | 123f:8120 | LSI Logic       | DVxplore Codec           | 100%   |          | 60F6C8F96D |
| 127e:0010 | 127e:0010 | Winnov, L.P.    | Videum 1000 Plus         | 100%   |          | 37BC71433C |
| 12ab:0371 | 1cfa:000b | YUAN High-Te... | Game Capture 4K60 Pro    | 100%   |          | 508BC3DCEE |
| 12ab:0371 | 1cfa:000c | YUAN High-Te... | Game Capture 4K60 Pro    | 100%   |          | 508BC3DCEE |
| 12ab:0380 | 1cfa:0006 | YUAN High-Te... | Game Capture 4K60 Pro    | 100%   |          | 7A840D41B2 |
| 12ab:0710 | f718:0001 | YUAN High-Te... | Multimedia controller    | 100%   |          | 4E0D80B779 |
| 13fe:0059 | 13fe:0059 | Advantech       | Multimedia controller    | 100%   |          | CFBB1B9F64 |
| 14b5:0200 |           | Creamware       | Scope                    | 100%   |          | 0FB4C2BDDA |
| 14b5:0300 |           | Creamware       | Pulsar                   | 100%   |          | 0FB4C2BDDA |
| 14b5:0600 | 14b5:0600 | Creamware       | Pulsar2                  | 100%   |          | 0FB4C2BDDA |
| 14e4:1570 | 14e4:1570 | Broadcom        | 720p FaceTime HD Camera  | 33%    | 4.15.0   | 020810CB9B |
| 14e4:1612 | 14e4:2612 | Broadcom        | BCM70012 Video Decode... | 100%   |          | 6FCADF1396 |
| 14e4:1615 | 1028:048b | Broadcom Lim... | BCM70015 Video Decode... | 100%   |          | 86E4BDCDFF |
| 14e4:1615 | 105b:0d57 | Broadcom        | BCM70015 Video Decode... | 100%   |          | BDCE37F0A6 |
| 14e4:1615 | 105b:0d77 | Broadcom        | BCM70015 Video Decode... | 100%   |          | B036D312E6 |
| 14e4:1615 | 14e4:1615 | Broadcom        | BCM70015 Video Decode... | 96%    | 5.3.0    | 85DEF78A94 |
| 14f1:8002 | 14f1:0084 | Conexant Sys... | Conexant Multimedia c... | 100%   |          | 380140EB8D |
| 14f1:8803 | 14f1:0084 | Conexant Sys... | CX2388x TV Capture Chip  | 100%   |          | 2EE541928A |
| 14f1:8803 | 185b:e000 | Conexant Sys... | CX2388x TV Capture Chip  | 100%   |          | 5B85C2F248 |
| 14f1:8804 | 0070:1402 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | BC782F5E67 |
| 14f1:8804 | 0070:6902 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | B2A993FF98 |
| 14f1:8804 | 0070:6906 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | B4E45EAE99 |
| 14f1:8804 | 0070:9002 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | 1351C7B098 |
| 14f1:8804 | 0070:9202 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | 3323601EEF |
| 14f1:8804 | 0070:9402 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | 0A7AB4D43E |
| 14f1:8804 | 14f1:0084 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | 2EE541928A |
| 14f1:8804 | 1822:0023 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | AB36F565A4 |
| 14f1:8804 | 7063:5500 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 100%   |          | BC5631611B |
| 1745:2100 | 1043:48b0 | ViXS Systems    | XCode 2100 Series        | 100%   |          | AD1D92439F |
| 1745:2100 | 1043:48d1 | ViXS Systems    | XCode 2100 Series        | 100%   |          | AAA454AA30 |
| 1745:3000 | 0070:d180 | ViXS Systems    | Colossus Encoder         | 100%   |          | 3A3874784C |
| 1745:3000 | 104d:9049 | ViXS Systems    | Colossus Encoder         | 100%   |          | 2628EBE1BB |
| 1745:3000 | 1bcf:a023 | ViXS Systems    | Colossus Encoder         | 100%   |          | 1494683BB9 |
| 1797:6805 |           | Intersil Tec... | HV4000 DVR card          | 100%   |          | 9800E2F253 |
| 1797:6805 | 1797:6804 | Intersil Tec... | HV4000 DVR card          | 100%   |          | B2C845B843 |
| 1797:6814 | 000a:6814 | Intersil Tec... | TW6816 multimedia vid... | 100%   |          | D455CC3322 |
| 1797:6815 | 000a:6815 | Intersil Tec... | TW6816 multimedia vid... | 100%   |          | D455CC3322 |
| 1797:6816 | 000a:6816 | Intersil Tec... | TW6816 multimedia vid... | 100%   |          | D455CC3322 |
| 1797:6817 | 000a:6817 | Intersil Tec... | TW6816 multimedia vid... | 100%   |          | D455CC3322 |
| 1797:6869 |           | Intersil Tec... | C968 PCIe SD Capture     | 66.7%  | 4.15.0   | B364724E53 |
| 1822:4e35 | 1822:0048 | Twinhan Tech... | Mantis DTV PCI Bridge... | 100%   |          | CB1A0D9CDD |
| 1a00:0001 | 1a00:0001 |                 | Multimedia controller    | 100%   |          | 16796AF2C3 |
| 544d:6178 | 6205:0001 | TBS Technolo... | DVB Tuner PCIe Card      | 100%   |          | 7FE42C31D7 |
| 544d:6178 | 6209:0001 | TBS Technolo... | DVB Tuner PCIe Card      | 100%   |          | C7E1E32971 |
| 544d:6178 | 6281:0002 | TBS Technolo... | DVB Tuner PCIe Card      | 50%    | 5.4.0    | 6971A673EC |
| 544d:6178 | 6522:0002 | TBS Technolo... | DVB Tuner PCIe Card      | 100%   |          | 732336834F |
| 544d:6178 | 6902:0002 | TBS Technolo... | DVB Tuner PCIe Card      | 100%   |          | 012B402EAC |
| 544d:6178 | 6908:0001 | TBS Technolo... | DVB Tuner PCIe Card      | 100%   |          | 2F71E9B242 |
| 8086:0f38 | 8086:0f31 | Intel           | Atom Processor Z36xxx... | 66.7%  | 4.12.4   | 0A0191D0D3 |
| 8086:0f38 | 8086:7270 | Intel           | Atom Processor Z36xxx... | 87.5%  | 5.0.0    | 0A96B79D5F |
| 8086:1919 | 1025:111e | Intel           | Xeon E3-1200 v5/E3-15... | 80%    | 5.4.11   | 2D71938FC4 |
| 8086:1919 | 1028:06d6 | Intel           | Xeon E3-1200 v5/E3-15... | 40%    | 5.4.0    | 7A9C92F242 |
| 8086:1919 | 1028:06e6 | Intel           | Xeon E3-1200 v5/E3-15... | 23.1%  | 5.0.0    | 33FE389598 |
| 8086:1919 | 1028:0702 | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | 229409A8DC |
| 8086:1919 | 1028:07a4 | Intel           | Xeon E3-1200 v5/E3-15... | 17.4%  | 5.0.0    | C5396B5734 |
| 8086:1919 | 1028:07a5 | Intel           | Xeon E3-1200 v5/E3-15... | 42.9%  | 5.4.0    | 87A44EF029 |
| 8086:1919 | 1028:081d | Intel           | Xeon E3-1200 v5/E3-15... | 20%    | 5.4.0    | B1CC9FA911 |
| 8086:1919 | 103c:80fc | Intel           | Xeon E3-1200 v5/E3-15... | 25%    | 5.4.0    | 4957115CEC |
| 8086:1919 | 103c:8146 | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | 3C4E95F3C6 |
| 8086:1919 | 103c:828b | Intel           | Xeon E3-1200 v5/E3-15... | 75%    | 5.3.0    | 3196DC7C2A |
| 8086:1919 | 103c:82ca | Intel           | Xeon E3-1200 v5/E3-15... | 38.5%  | 5.4.0    | D6AB5352B8 |
| 8086:1919 | 103c:82cb | Intel           | Xeon E3-1200 v5/E3-15... | 29.4%  | 5.8.0    | 5783B64146 |
| 8086:1919 | 144d:c135 | Intel           | Xeon E3-1200 v5/E3-15... | 85.7%  | 5.4.0    | 4E4EF907A0 |
| 8086:1919 | 144d:c14f | Intel           | Xeon E3-1200 v5/E3-15... | 33.3%  | 5.0.0    | C9D869A6A8 |
| 8086:1919 | 152d:1182 | Intel           | Xeon E3-1200 v5/E3-15... | 33.3%  | 5.0.0    | E88C6D9780 |
| 8086:1919 | 152d:1237 | Intel           | Xeon E3-1200 v5/E3-15... | 25%    | 5.4.0    | 88C7E28521 |
| 8086:1919 | 17aa:2241 | Intel           | Xeon E3-1200 v5/E3-15... | 36.4%  | 5.4.0    | EC046B0E9C |
| 8086:1919 | 17aa:2244 | Intel           | Xeon E3-1200 v5/E3-15... | 50%    | 5.4.0    | 7A3A0603E5 |
| 8086:1919 | 17aa:3812 | Intel           | Xeon E3-1200 v5/E3-15... | 66.7%  | 5.3.0    | AAEF1C5AE7 |
| 8086:1919 | 17aa:3825 | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | 14DC838F85 |
| 8086:1919 | 17aa:382f | Intel           | Xeon E3-1200 v5/E3-15... | 100%   |          | F78D607B1F |
| 8086:1919 | 19e5:3e00 | Intel           | Xeon E3-1200 v5/E3-15... | 66.7%  | 5.8.0    | A76E9D9514 |
| 8086:1919 | 8086:1919 | Intel           | Xeon E3-1200 v5/E3-15... | 37.9%  | 5.0.0    | BAF839D246 |
| 8086:1919 | 8086:2015 | Intel           | Xeon E3-1200 v5/E3-15... | 44.5%  | 4.4.232  | 7A294509DE |
| 8086:1a88 |           | Intel           | Imaging Signal Proces... | 100%   |          | 555A26F0D1 |
| 8086:22b8 | 1025:1021 | Intel           | Atom/Celeron/Pentium ... | 45.5%  | 4.19.0   | 663247803F |
| 8086:22b8 | 1025:106e | Intel           | Atom/Celeron/Pentium ... | 16.7%  | 5.4.0    | 425D589D65 |
| 8086:22b8 | 1025:113a | Intel           | Atom/Celeron/Pentium ... | 100%   |          | FBF9B74A34 |
| 8086:22b8 | 1028:06ea | Intel           | Atom/Celeron/Pentium ... | 71.4%  | 4.20.1   | 57FDB94877 |
| 8086:22b8 | 103c:8042 | Intel           | Atom/Celeron/Pentium ... | 16.7%  | 5.6.19   | 45359B58FC |
| 8086:22b8 | 103c:813e | Intel           | Atom/Celeron/Pentium ... | 28.3%  | 5.0.0    | 92BE7FA2D2 |
| 8086:22b8 | 103c:827c | Intel           | Atom/Celeron/Pentium ... | 33.3%  | 5.0.0    | 163F3173C7 |
| 8086:22b8 | 103c:82f4 | Intel           | Atom/Celeron/Pentium ... | 12.5%  | 5.1.15   | 1C188B150F |
| 8086:22b8 | 1043:13a0 | Intel           | Atom/Celeron/Pentium ... | 28.2%  | 5.0.0    | B5A52077BB |
| 8086:22b8 | 1043:1400 | Intel           | Atom/Celeron/Pentium ... | 27.6%  | 5.0.0    | 56BDBE35F8 |
| 8086:22b8 | 1043:1bdd | Intel           | Atom/Celeron/Pentium ... | 10.7%  | 5.0.0    | 12E1B01848 |
| 8086:22b8 | 1043:1c60 | Intel           | Atom/Celeron/Pentium ... | 12.5%  | 5.0.0    | 5FCF1662DB |
| 8086:22b8 | 1071:a126 | Intel           | Atom/Celeron/Pentium ... | 100%   |          | F2981C1775 |
| 8086:22b8 | 10cf:1925 | Intel           | Atom/Celeron/Pentium ... | 100%   |          | 6D19311F7E |
| 8086:22b8 | 1179:f860 | Intel           | Atom/Celeron/Pentium ... | 100%   |          | 1148737572 |
| 8086:22b8 | 1297:2063 | Intel           | Atom/Celeron/Pentium ... | 27.8%  | 4.19.0   | 589328FA17 |
| 8086:22b8 | 1414:0009 | Intel           | Atom/Celeron/Pentium ... | 14.3%  | 5.3.0    | 76A25407DE |
| 8086:22b8 | 17aa:222a | Intel           | Atom/Celeron/Pentium ... | 40%    | 5.10.33  | 42B9111B9B |
| 8086:22b8 | 17aa:3809 | Intel           | Atom/Celeron/Pentium ... | 10.4%  | 5.0.0    | 00CDB13890 |
| 8086:22b8 | 17aa:38e3 | Intel           | Atom/Celeron/Pentium ... | 28%    | 4.19.110 | B99FF99A2F |
| 8086:22b8 | 1854:0280 | Intel           | Atom/Celeron/Pentium ... | 100%   |          | A6AB074BB5 |
| 8086:22b8 | 1bfd:0001 | Intel           | Atom/Celeron/Pentium ... | 100%   |          | 1BA20022CB |
| 8086:22b8 | 8086:7270 | Intel           | Atom/Celeron/Pentium ... | 40.7%  | 4.19.0   | 044D8CA250 |
| 8086:5a88 |           | Intel           | Celeron N3350/Pentium... | 100%   |          | AC530E40AD |
| 8086:8a19 | 1028:08b0 | Intel           | Image Signal Processor   | 100%   |          | CD3B8F3BCA |
| 8086:8a19 | 8086:7270 | Intel           | Image Signal Processor   | 100%   |          | 4265905516 |
| 8086:9830 | 144d:c18b | Intel           | Multimedia controller    | 100%   |          | 6D40FDC958 |
| 8086:9a19 | 17aa:508b | Intel           | Multimedia controller    | 100%   |          | AAC22AF3A1 |
| 8086:9a19 | 8086:2097 | Intel           | Multimedia controller    | 100%   |          | 9519AF9ABA |
| 8086:9d32 |           | Intel           | CSI-2 Host Controller    | 5.9%   | 4.4.232  | C596B50DF9 |
| 8086:9d32 | 1028:06e6 | Intel           | CSI-2 Host Controller    | 19.2%  | 4.18.0   | 33FE389598 |
| 8086:9d32 | 1028:07a4 | Intel           | CSI-2 Host Controller    | 8.7%   | 4.18.0   | AA661DFC05 |
| 8086:9d32 | 1028:07a5 | Intel           | CSI-2 Host Controller    | 42.9%  | 5.4.0    | 87A44EF029 |
| 8086:9d32 | 103c:80fc | Intel           | CSI-2 Host Controller    | 8.3%   | 5.4.0    | 931B6970F2 |
| 8086:9d32 | 103c:8146 | Intel           | CSI-2 Host Controller    | 75%    | 5.4.0    | 70ACFD512F |
| 8086:9d32 | 103c:82cb | Intel           | CSI-2 Host Controller    | 5.9%   | 5.0.0    | 5783B64146 |
| 8086:9d32 | 1043:1410 | Intel           | CSI-2 Host Controller    | 50%    | 5.8.0    | 0B5AD4104E |
| 8086:9d32 | 144d:c135 | Intel           | CSI-2 Host Controller    | 14.3%  | 4.18.0   | 4E4EF907A0 |
| 8086:9d32 | 17aa:2241 | Intel           | CSI-2 Host Controller    | 27.3%  | 4.18.0   | EC046B0E9C |
| 8086:9d32 | 17aa:380c | Intel           | CSI-2 Host Controller    | 50%    | 4.18.0   | F78D607B1F |
| 8086:9d32 | 17aa:3812 | Intel           | CSI-2 Host Controller    | 16.7%  | 5.0.3    | 508333A652 |
| 8086:9d32 | 8086:7270 | Intel           | CSI-2 Host Controller    | 15%    | 4.18.0   | AE3077AF50 |
| 8086:9d32 | 8086:9d32 | Intel           | CSI-2 Host Controller    | 12.5%  | 4.18.0   | 422797E8D2 |
| dd01:0006 | dd01:0022 | Digital Devices | Cine V7                  | 100%   |          | FCF4AFE5C6 |

### Net/ethernet (PCI)

177 out of 6078 (2.91%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 0000:0200 | 002c:0200 |                 | Ethernet controller      | 100%   |          | 32AE4212DF |
| 000c:0000 | 1043:83a3 |                 | Ethernet controller      | 100%   |          | B5189C3BF2 |
| 1039:0900 | 1584:5002 | Silicon Inte... | SiS900 PCI Fast Ethernet | 50%    | 4.15.0   | CC188D0F25 |
| 10ec:0139 | 10bd:0320 | Realtek Semi... | RTL-8139/8139C/8139C+... | 100%   |          | 305C35F50C |
| 10ec:2600 | 098e:1028 | Realtek Semi... | Killer E2600 Gigabit ... | 12.5%  | 5.4.0    | 0496499AA5 |
| 10ec:3000 | 1025:132d | Realtek Semi... | Killer E3000 2.5GbE C... | 36.4%  | 5.4.0    | 17674B4CBD |
| 10ec:3000 | 1025:1375 | Realtek Semi... | Killer E3000 2.5GbE C... | 44.4%  | 5.4.5    | 8396C1D9E6 |
| 10ec:3000 | 1028:08c4 | Realtek Semi... | Killer E3000 2.5GbE C... | 33.3%  | 5.4.0    | BA3ACE6663 |
| 10ec:3000 | 1028:093c | Realtek Semi... | Killer E3000 2.5GbE C... | 60%    | 5.4.25   | 5FCBF716A6 |
| 10ec:3000 | 1462:7c34 | Realtek Semi... | Killer E3000 2.5GbE C... | 30%    | 5.3.18   | EDC31CEC40 |
| 10ec:3000 | 1558:7714 | Realtek Semi... | Killer E3000 2.5GbE C... | 27.3%  | 5.8.0    | EB5AF1BBD3 |
| 10ec:3000 | 1849:3000 | Realtek Semi... | Killer E3000 2.5GbE C... | 33.3%  | 5.10.12  | 1B9FC852A6 |
| 10ec:8125 | 1043:879b | Realtek Semi... | RTL8125 2.5GbE Contro... | 10.3%  | 5.4.0    | B1F5EAC9A6 |
| 10ec:8125 | 1462:7c76 | Realtek Semi... | RTL8125 2.5GbE Contro... | 40%    | 5.8.0    | 6F93F2376D |
| 10ec:8131 | 10ec:8131 | Realtek Semi... | RTL8131 PCIe Fast Eth... | 100%   |          | 4E43962152 |
| 10ec:8136 | 1025:061f | Realtek Semi... | RTL810xE PCI Express ... | 1.8%   | 3.14.44  | ADD6CC4F5F |
| 10ec:8136 | 1028:0555 | Realtek Semi... | RTL810xE PCI Express ... | 3%     | 4.1.15   | A7211B4E35 |
| 10ec:8136 | 1028:0597 | Realtek Semi... | RTL810xE PCI Express ... | 2.3%   | 3.14.25  | 0DD732A269 |
| 10ec:8136 | 1028:06b2 | Realtek Semi... | RTL810xE PCI Express ... | 1.1%   | 4.9.20   | A2E2A6CF66 |
| 10ec:8136 | 1028:0768 | Realtek Semi... | RTL810xE PCI Express ... | 4.3%   | 4.9.9    | 32E3129638 |
| 10ec:8136 | 1028:0810 | Realtek Semi... | RTL810xE PCI Express ... | 1.4%   | 4.4.0    | BE05348BE2 |
| 10ec:8136 | 1028:08fa | Realtek Semi... | RTL810xE PCI Express ... | 2.9%   | 4.18.16  | 738E03E488 |
| 10ec:8136 | 1028:0969 | Realtek Semi... | RTL810xE PCI Express ... | 100%   |          | 7ABAC766F3 |
| 10ec:8136 | 1028:097c | Realtek Semi... | RTL810xE PCI Express ... | 7.9%   | 5.0.0    | 1E5A862091 |
| 10ec:8136 | 103c:1484 | Realtek Semi... | RTL810xE PCI Express ... | 4%     | 4.9.60   | C7734FBAE0 |
| 10ec:8136 | 103c:148a | Realtek Semi... | RTL810xE PCI Express ... | 7.1%   | 4.1.38   | A8A7B70079 |
| 10ec:8136 | 103c:184a | Realtek Semi... | RTL810xE PCI Express ... | 1.3%   | 3.14.33  | 581C3578E1 |
| 10ec:8136 | 103c:2212 | Realtek Semi... | RTL810xE PCI Express ... | 13.3%  | 4.9.41   | 3930E9BFE0 |
| 10ec:8136 | 103c:2213 | Realtek Semi... | RTL810xE PCI Express ... | 3.4%   | 3.14.25  | C4E7564FC7 |
| 10ec:8136 | 103c:226a | Realtek Semi... | RTL810xE PCI Express ... | 15%    | 3.14.44  | 9CEDFB1B3B |
| 10ec:8136 | 103c:306b | Realtek Semi... | RTL810xE PCI Express ... | 5.6%   | 3.14.44  | 93C0EF7223 |
| 10ec:8136 | 103c:80c7 | Realtek Semi... | RTL810xE PCI Express ... | 16.7%  | 5.3.0    | FE4C2B1CA0 |
| 10ec:8136 | 103c:8137 | Realtek Semi... | RTL810xE PCI Express ... | 1.4%   | 4.1.15   | 9070448ACE |
| 10ec:8136 | 103c:81f5 | Realtek Semi... | RTL810xE PCI Express ... | 2.3%   | 4.1.34   | 045809FB67 |
| 10ec:8136 | 103c:81f6 | Realtek Semi... | RTL810xE PCI Express ... | 3%     | 4.1.25   | 142457C9EA |
| 10ec:8136 | 103c:820c | Realtek Semi... | RTL810xE PCI Express ... | 12.5%  | 4.1.25   | 21A7695D56 |
| 10ec:8136 | 10ec:0123 | Realtek Semi... | RTL810xE PCI Express ... | 0.4%   | 3.14.25  | 37B1114873 |
| 10ec:8136 | 1179:f920 | Realtek Semi... | RTL810xE PCI Express ... | 5.9%   | 4.9.9    | 0BC2465C23 |
| 10ec:8136 | 1179:fbb0 | Realtek Semi... | RTL810xE PCI Express ... | 9.1%   | 4.15.0   | DCF4CE8AA3 |
| 10ec:8136 | 1179:ff1e | Realtek Semi... | RTL810xE PCI Express ... | 0.5%   | 3.14.44  | 9A6A86E7FC |
| 10ec:8136 | 1462:7529 | Realtek Semi... | RTL810xE PCI Express ... | 3.2%   | 3.14.44  | 99777B72F9 |
| 10ec:8136 | 17aa:381f | Realtek Semi... | RTL810xE PCI Express ... | 3.2%   | 4.1.34   | 1952B1CCF3 |
| 10ec:8136 | 17aa:3861 | Realtek Semi... | RTL810xE PCI Express ... | 0.7%   | 4.9.60   | C2D5094A2D |
| 10ec:8161 | 10ec:8168 | Realtek Semi... | RTL8111/8168/8411 PCI... | 4.8%   | 4.15.0   | 3C4C6C8BD0 |
| 10ec:8168 | 1019:99e7 | Realtek Semi... | RTL8111/8168/8411 PCI... | 50%    | 5.3.0    | 974F5398CA |
| 10ec:8168 | 1025:0866 | Realtek Semi... | RTL8111/8168/8411 PCI... | 1.7%   | 3.10.51  | 8B133744C1 |
| 10ec:8168 | 1025:0918 | Realtek Semi... | RTL8111/8168/8411 PCI... | 8.1%   | 4.1.19   | 68E659C87D |
| 10ec:8168 | 1025:0936 | Realtek Semi... | RTL8111/8168/8411 PCI... | 2%     | 3.8.0    | A2C7011157 |
| 10ec:8168 | 1025:0987 | Realtek Semi... | RTL8111/8168/8411 PCI... | 2.9%   | 4.1.34   | 89237E04FC |
| 10ec:8168 | 1025:1094 | Realtek Semi... | RTL8111/8168/8411 PCI... | 1.4%   | 3.10.0   | B319F99046 |
| 10ec:8168 | 1025:1238 | Realtek Semi... | RTL8111/8168/8411 PCI... | 1.4%   | 4.15.0   | 3520CCDFCF |
| 10ec:8168 | 1025:125c | Realtek Semi... | RTL8111/8168/8411 PCI... | 0.9%   | 4.15.0   | 6AEFA7E06C |
| 10ec:8168 | 1025:1266 | Realtek Semi... | RTL8111/8168/8411 PCI... | 22.2%  | 5.0.0    | 5737732BB0 |
| 10ec:8168 | 1028:04b8 | Realtek Semi... | RTL8111/8168/8411 PCI... | 4.8%   | 4.15.0   | A993CB7099 |
| 10ec:8168 | 1028:04d9 | Realtek Semi... | RTL8111/8168/8411 PCI... | 9.1%   | 4.15.0   | 6ECDF91891 |
| 10ec:8168 | 1028:068d | Realtek Semi... | RTL8111/8168/8411 PCI... | 16.7%  | 5.4.0    | 6DFB5101A1 |
| 10ec:8168 | 1028:0763 | Realtek Semi... | RTL8111/8168/8411 PCI... | 5.3%   | 5.8.0    | 8C4F2F9922 |
| 10ec:8168 | 1028:0870 | Realtek Semi... | RTL8111/8168/8411 PCI... | 7.7%   | 4.15.0   | B0DF3027CF |
| 10ec:8168 | 103c:180d | Realtek Semi... | RTL8111/8168/8411 PCI... | 2.8%   | 3.10.42  | 41A6D6B87B |
| 10ec:8168 | 103c:1968 | Realtek Semi... | RTL8111/8168/8411 PCI... | 8.3%   | 4.9.9    | 18B8D3D480 |
| 10ec:8168 | 103c:1992 | Realtek Semi... | RTL8111/8168/8411 PCI... | 4.2%   | 4.1.25   | 2C52151F77 |
| 10ec:8168 | 103c:2a94 | Realtek Semi... | RTL8111/8168/8411 PCI... | 3.3%   | 4.1.25   | 33AE5EBABC |
| 10ec:8168 | 103c:80e6 | Realtek Semi... | RTL8111/8168/8411 PCI... | 100%   |          | 4F20314E69 |
| 10ec:8168 | 103c:831c | Realtek Semi... | RTL8111/8168/8411 PCI... | 9.1%   | 4.9.60   | 854604BDAD |
| 10ec:8168 | 103c:8328 | Realtek Semi... | RTL8111/8168/8411 PCI... | 4.3%   | 4.9.20   | 4E7C532C73 |
| 10ec:8168 | 103c:837d | Realtek Semi... | RTL8111/8168/8411 PCI... | 1.2%   | 4.9.60   | 4EAD1B8C73 |
| 10ec:8168 | 103c:8467 | Realtek Semi... | RTL8111/8168/8411 PCI... | 33.3%  | 5.4.0    | D20F245092 |
| 10ec:8168 | 103c:84ac | Realtek Semi... | RTL8111/8168/8411 PCI... | 2%     | 4.15.0   | 7E7AD00D75 |
| 10ec:8168 | 103c:8615 | Realtek Semi... | RTL8111/8168/8411 PCI... | 3.4%   | 4.15.0   | C3DDCBBE38 |
| 10ec:8168 | 103c:872e | Realtek Semi... | RTL8111/8168/8411 PCI... | 33.3%  | 5.10.9   | 95939E2AED |
| 10ec:8168 | 1043:1447 | Realtek Semi... | RTL8111/8168/8411 PCI... | 4.5%   | 3.14.44  | F23B5BF0DA |
| 10ec:8168 | 1043:1477 | Realtek Semi... | RTL8111/8168/8411 PCI... | 8.8%   | 4.9.60   | 9998E51D1C |
| 10ec:8168 | 1043:14f7 | Realtek Semi... | RTL8111/8168/8411 PCI... | 3.7%   | 3.14.44  | CE99670CEB |
| 10ec:8168 | 1043:200f | Realtek Semi... | RTL8111/8168/8411 PCI... | 0.2%   | 3.10.34  | 4D035C5605 |
| 10ec:8168 | 1043:208f | Realtek Semi... | RTL8111/8168/8411 PCI... | 0.2%   | 4.13.0   | 3C4DEC3B5D |
| 10ec:8168 | 1043:8432 | Realtek Semi... | RTL8111/8168/8411 PCI... | 0.1%   | 3.0.38   | 58F57667EE |
| 10ec:8168 | 1043:8677 | Realtek Semi... | RTL8111/8168/8411 PCI... | 0.1%   | 2.6.32   | 9578024712 |
| 10ec:8168 | 1043:8783 | Realtek Semi... | RTL8111/8168/8411 PCI... | 6.2%   | 5.0.0    | 7329CF3BE4 |
| 10ec:8168 | 10ec:0123 | Realtek Semi... | RTL8111/8168/8411 PCI... | 0.1%   | 3.10.0   | C47774CC75 |
| 10ec:8168 | 10ec:8168 | Realtek Semi... | RTL8111/8168/8411 PCI... | 0.4%   | 3.10.0   | 7BB7690B49 |
| 10ec:8168 | 1297:2033 | Realtek Semi... | RTL8111/8168/8411 PCI... | 3%     | 4.9.20   | 51273F53DF |
| 10ec:8168 | 1458:e000 | Realtek Semi... | RTL8111/8168/8411 PCI... | 0.1%   | 3.10.0   | 4B6B54B926 |
| 10ec:8168 | 1462:10b8 | Realtek Semi... | RTL8111/8168/8411 PCI... | 1.2%   | 4.1.25   | 1E515A2EC5 |
| 10ec:8168 | 14c0:0059 | Realtek Semi... | RTL8111/8168/8411 PCI... | 20%    | 4.19.0   | 42B3F11A1E |
| 10ec:8168 | 1558:1323 | Realtek Semi... | RTL8111/8168/8411 PCI... | 8%     | 4.15.0   | 75848692B4 |
| 10ec:8168 | 1558:1404 | Realtek Semi... | RTL8111/8168/8411 PCI... | 3.7%   | 5.0.0    | 4275F330AF |
| 10ec:8168 | 1558:1550 | Realtek Semi... | RTL8111/8168/8411 PCI... | 2.1%   | 3.14.33  | A0EB5DA51A |
| 10ec:8168 | 1558:8680 | Realtek Semi... | RTL8111/8168/8411 PCI... | 20%    | 5.4.0    | 4D0B64CD52 |
| 10ec:8168 | 17aa:21dd | Realtek Semi... | RTL8111/8168/8411 PCI... | 2.2%   | 3.14.44  | DB0C1FE4C4 |
| 10ec:8168 | 17aa:21fe | Realtek Semi... | RTL8111/8168/8411 PCI... | 6.7%   | 3.10.0   | E17730F707 |
| 10ec:8168 | 17aa:2219 | Realtek Semi... | RTL8111/8168/8411 PCI... | 7.1%   | 4.9.60   | 39F6DECF99 |
| 10ec:8168 | 17aa:2224 | Realtek Semi... | RTL8111/8168/8411 PCI... | 2.8%   | 4.15.0   | C163822056 |
| 10ec:8168 | 17aa:380b | Realtek Semi... | RTL8111/8168/8411 PCI... | 0.9%   | 3.14.25  | B3B3794709 |
| 10ec:8168 | 17aa:3831 | Realtek Semi... | RTL8111/8168/8411 PCI... | 2.9%   | 4.4.6    | 9E5B4C92F4 |
| 10ec:8168 | 17aa:383a | Realtek Semi... | RTL8111/8168/8411 PCI... | 10%    | 4.1.25   | 8AEDFD9F4C |
| 10ec:8168 | 17aa:38c7 | Realtek Semi... | RTL8111/8168/8411 PCI... | 1.1%   | 4.15.0   | E030A286C2 |
| 10ec:8168 | 17aa:5123 | Realtek Semi... | RTL8111/8168/8411 PCI... | 33.3%  | 5.4.0    | 4DABCB8D3F |
| 10ec:8168 | 17aa:5126 | Realtek Semi... | RTL8111/8168/8411 PCI... | 2.1%   | 4.15.0   | E720C77930 |
| 10ec:8168 | 1849:8168 | Realtek Semi... | RTL8111/8168/8411 PCI... | 0.1%   | 2.6.32   | 5ACBE289AA |
| 10ec:8168 | 1d05:109f | Realtek Semi... | RTL8111/8168/8411 PCI... | 1.9%   | 5.3.7    | EC0CB83241 |
| 10ec:8168 | 7470:3468 | Realtek Semi... | RTL8111/8168/8411 PCI... | 0.2%   | 3.10.0   | 7A756F5970 |
| 10ec:8169 | 10ec:8169 | Realtek Semi... | RTL8169 PCI Gigabit E... | 0.4%   | 3.10.0   | 2DBD467937 |
| 1106:3106 | 1186:1403 | VIA Technolo... | VT6105/VT6106S [Rhine... | 3.1%   | 3.14.44  | D142F54A38 |
| 1186:4200 | 1186:1103 | D-Link System   | DFE-520TX Fast Ethern... | 100%   |          | 790E740601 |
| 1186:4300 | 1186:4300 | D-Link System   | DGE-528T Gigabit Ethe... | 1.3%   | 3.10.0   | 6BA672F50B |
| 1186:4300 | 1186:4c00 | D-Link System   | DGE-528T Gigabit Ethe... | 5.6%   | 3.14.44  | 1611967F74 |
| 1186:4b01 | 1186:4b01 | D-Link System   | DGE-530T Gigabit Ethe... | 2.4%   | 3.14.44  | F195015CF8 |
| 11ab:4362 | 1043:8142 | Marvell Tech... | 88E8053 PCI-E Gigabit... | 1%     | 3.14.33  | 193ECC62CF |
| 11ab:4363 | 144d:c03f | Marvell Tech... | 88E8055 PCI-E Gigabit... | 5.3%   | 3.12.23  | 4D35B24594 |
| 11ab:4380 | 104d:907a | Marvell Tech... | 88E8057 PCI-E Gigabit... | 9.4%   | 4.9.155  | E6E4689D4B |
| 11ab:4381 | 104d:9071 | Marvell Tech... | Yukon Optima 88E8059 ... | 0.9%   | 3.14.44  | 1744D5DB17 |
| 1374:0038 | 1374:0038 | Silicom         | Quad port Copper Ethe... | 100%   |          | 8BE6B42FC7 |
| 14e4:1680 | 1028:0263 | Broadcom        | NetXtreme BCM5761e Gi... | 3.2%   | 4.12.14  | 079101F502 |
| 14e4:1698 | 105b:0e34 | Broadcom        | NetLink BCM5784M Giga... | 33.3%  | 4.15.0   | F75D2CD0A7 |
| 14e4:16a3 | 14e4:16a3 | Broadcom        | NetXtreme BCM57786 Gi... | 100%   |          | FF18F266EE |
| 14e4:16a3 | 14e4:16b4 | Broadcom        | NetXtreme BCM57786 Gi... | 100%   |          | 5372B6674E |
| 14e4:16b5 | 1025:0504 | Broadcom        | NetLink BCM57785 Giga... | 0.5%   | 3.10.0   | B377A89C57 |
| 14e4:52a3 | d3a6:afcd | Broadcom Lim... | Ethernet controller      | 100%   |          | 191BA97155 |
| 168c:abcd |           | Qualcomm Ath... | Osprey Emulation Wire... | 100%   |          | 08EC3E2E3D |
| 168c:ff1a |           | Qualcomm Ath... | Ethernet controller      | 100%   |          | 962E760F3B |
| 1969:1083 | 1025:0686 | Qualcomm Ath... | AR8151 v2.0 Gigabit E... | 1%     | 3.14.44  | 910279B054 |
| 1969:1083 | 1179:fc50 | Qualcomm Ath... | AR8151 v2.0 Gigabit E... | 3.3%   | 3.14.44  | 046BFED81F |
| 1969:1090 | 17aa:3979 | Qualcomm Ath... | AR8162 Fast Ethernet     | 0.9%   | 3.14.15  | A9D699C1F6 |
| 1969:10a0 | 1179:fa30 | Qualcomm Ath... | QCA8172 Fast Ethernet    | 2.8%   | 3.14.15  | D7B4BF2642 |
| 1969:e0a1 | 1462:7977 | Qualcomm Ath... | Killer E2400 Gigabit ... | 3.7%   | 4.9.60   | 877BEE4B1A |
| 1969:e0b1 | 1462:11f2 | Qualcomm Ath... | Killer E2500 Gigabit ... | 11.1%  | 5.4.0    | 3DDF7394D8 |
| 197b:0250 | 1558:4120 | JMicron Tech... | JMC250 PCI Express Gi... | 8.3%   | 4.15.0   | DBA823C7CC |
| 1a47:0003 | 0000:0200 | 3DSP            | WLAN and Bluetooth Card  | 100%   |          | 3A17145633 |
| 1d6a:00b1 | 1043:874a | Aquantia        | AQC100 10G Ethernet M... | 33.3%  | 5.8.0    | F5152B2EC1 |
| 1d6a:07b1 | 1043:8757 | Aquantia        | AQC107 NBase-T/IEEE 8... | 12.1%  | 4.15.0   | 656256DB83 |
| 1d6a:07b1 | 1462:7c59 | Aquantia        | AQC107 NBase-T/IEEE 8... | 57.1%  | 5.4.0    | 7539DA519D |
| 1d6a:07b1 | 1849:d107 | Aquantia        | AQC107 NBase-T/IEEE 8... | 5.4%   | 3.10.0   | DD14B01C46 |
| 1d6a:d107 | 1458:e000 | Aquantia        | AQC107 NBase-T/IEEE 8... | 7.4%   | 5.0.0    | 78D71EC4A3 |
| 1fc9:4022 | 1432:8103 | Tehuti Networks | TN9310 10GbE SFP+ Eth... | 100%   |          | 72C72698D3 |
| 1fc9:4027 | 1432:8104 | Tehuti Networks | TN9710P 10GBase-T/NBA... | 100%   |          | 4B605582DF |
| 1fc9:4027 | 1fc9:3015 | Tehuti Networks | TN9710P 10GBase-T/NBA... | 50%    | 4.2.8    | 1DDC8C7398 |
| 8086:0000 | 8086:0000 | Intel           | PROSet/Wireless WiFi ... | 100%   |          | 418C3E7B73 |
| 8086:0d4c | 1028:09f6 | Intel           | Ethernet Connection (... | 50%    | 5.4.0    | 1F5B92D91B |
| 8086:0d4c | 103c:8755 | Intel           | Ethernet Connection (... | 100%   |          | 334ABF8C53 |
| 8086:0d4d | 1043:8672 | Intel           | Ethernet Connection (... | 2.9%   | 4.19.0   | F8503ECC3B |
| 8086:0d4f | 1043:200f | Intel           | Ethernet Connection (... | 50%    | 5.10.7   | 42CDDE5346 |
| 8086:0d4f | 17aa:2292 | Intel           | Ethernet Connection (... | 29.7%  | 5.0.0    | BCBC0E3494 |
| 8086:0d4f | 17aa:5078 | Intel           | Ethernet Connection (... | 8%     | 5.0.0    | 3BB77F19C3 |
| 8086:0d4f | 8086:2081 | Intel           | Ethernet Connection (... | 1.1%   | 4.15.0   | F2BFE6BFB3 |
| 8086:107c | 8086:1376 | Intel           | 82541PI Gigabit Ether... | 1.2%   | 2.6.32   | F801FAB1AD |
| 8086:109a | 8086:0000 | Intel           | 82573L Gigabit Ethern... | 22.2%  | 4.15.0   | ED27C7AA81 |
| 8086:10aa | 8086:0000 | Intel           | Ethernet controller      | 100%   |          | CBBE408AAC |
| 8086:10fb | 1028:1f72 | Intel           | 82599ES 10-Gigabit SF... | 100%   |          | 77A5A8BF12 |
| 8086:10fb | 8086:000c | Intel           | 82599ES 10-Gigabit SF... | 7.7%   | 4.15.0   | AC9EE9A2A3 |
| 8086:1229 | 1014:005c | Intel           | 82557/8/9/0/1 Etherne... | 50%    | 4.9.60   | 3BE565CCFD |
| 8086:1229 | 8086:0050 | Intel           | 82557/8/9/0/1 Etherne... | 8.7%   | 3.10.0   | E568C873E2 |
| 8086:153b | 1558:0940 | Intel           | Ethernet Connection I... | 100%   |          | D9819DC4AA |
| 8086:153b | 8086:0000 | Intel           | Ethernet Connection I... | 16.7%  | 3.14.44  | 4C63D890BC |
| 8086:154b | 8086:0000 | Intel           | Ethernet controller      | 100%   |          | 2F03DC661B |
| 8086:1572 | 8086:0000 | Intel           | Ethernet Controller X... | 4.3%   | 3.10.0   | 4158CB76EF |
| 8086:1572 | 8086:0001 | Intel           | Ethernet Controller X... | 12.5%  | 3.10.0   | 4158CB76EF |
| 8086:158b | 1374:0000 | Intel           | Ethernet Controller X... | 100%   |          | 4158CB76EF |
| 8086:158b | 1374:023a | Intel           | Ethernet Controller X... | 100%   |          | 4158CB76EF |
| 8086:15a0 | 103c:2129 | Intel           | Ethernet Connection (... | 2%     | 4.15.0   | 71CFEF0293 |
| 8086:15a1 | 1458:e000 | Intel           | Ethernet Connection (... | 1.7%   | 4.1.15   | F2EDD659F0 |
| 8086:15b7 | 17aa:310b | Intel           | Ethernet Connection (... | 20%    | 5.4.0    | 9B4C82CD04 |
| 8086:15b8 | 1043:8672 | Intel           | Ethernet Connection (... | 0.1%   | 4.1.15   | 51B31F180E |
| 8086:15bc | 1028:0851 | Intel           | Ethernet Connection (... | 100%   |          | 05D6B79D2F |
| 8086:15bc | 1462:7b23 | Intel           | Ethernet Connection (... | 16.7%  | 4.18.0   | 37076CEBE8 |
| 8086:15bc | 1849:15bc | Intel           | Ethernet Connection (... | 1.7%   | 4.13.0   | BA39531B87 |
| 8086:15be | 17aa:2286 | Intel           | Ethernet Connection (... | 2.8%   | 4.18.0   | 12B5E06A49 |
| 8086:15f3 | 1043:87d2 | Intel           | Ethernet Controller I... | 2.2%   | 5.4.0    | BE8CD1AF8B |
| 8086:15f3 | 1458:e000 | Intel           | Ethernet Controller I... | 4.3%   | 5.4.0    | 58DCE1215C |
| 8086:15fc | 17aa:508f | Intel           | Ethernet Connection (... | 100%   |          | 241B13488E |
| 8086:3100 | 8086:0000 | Intel           | Ethernet controller      | 22.2%  | 5.4.0    | D18CD6B320 |
| 8086:3101 | 1028:0a74 | Intel           | Ethernet controller      | 100%   |          | 5B2250FC19 |
| 8086:3101 | 8086:0000 | Intel           | Ethernet controller      | 37.5%  | 5.8.0    | D1444D8EF3 |
| 8086:37cc | 103c:81c6 | Intel           | Ethernet Connection X722 | 100%   |          | 9D6E46ECA9 |
| 8086:37cc | 103c:81c7 | Intel           | Ethernet Connection X722 | 100%   |          | 0C434691D6 |
| 8086:37cc | 15d9:0000 | Intel           | Ethernet Connection X722 | 100%   |          | 2794B14FEE |
| 8086:37cc | 1734:1230 | Intel           | Ethernet Connection X722 | 100%   |          | 86AB491564 |
| 8086:37cc | 17aa:4020 | Intel           | Ethernet Connection X722 | 100%   |          | FE32C2BD18 |

### Net/wireless (PCI)

322 out of 1266 (25.43%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 104c:8400 | 1186:3b01 | Texas Instru... | ACX 100 22Mbps Wirele... | 100%   |          | 902F92D261 |
| 104c:9066 | 1086:3b04 | Texas Instru... | ACX 111 54Mbps Wirele... | 100%   |          | DBFFE622A8 |
| 104c:9066 | 1186:3b04 | Texas Instru... | ACX 111 54Mbps Wirele... | 77.8%  | 4.18.16  | CA6E89DE47 |
| 104c:9066 | 13d1:ab90 | Texas Instru... | ACX 111 54Mbps Wirele... | 100%   |          | 6FF7C7478E |
| 104c:9066 | 17cf:0032 | Texas Instru... | ACX 111 54Mbps Wirele... | 100%   |          | 9B37C1E94F |
| 1050:0033 | 1050:0033 | Winbond Elec... | W89C33D 802.11 a/b/g ... | 100%   |          | 9B37C1E94F |
| 105b:e0ab | 105b:e0ab | Foxconn Inte... | Wireless controller      | 100%   |          | 49AAD4B320 |
| 10ec:8176 | 103c:1629 | Realtek Semi... | RTL8188CE 802.11b/g/n... | 0.8%   | 3.10.19  | 031B9CF2AF |
| 10ec:8176 | 10ec:8181 | Realtek Semi... | RTL8188CE 802.11b/g/n... | 1.6%   | 3.10.46  | 046BFED81F |
| 10ec:8176 | 1a3b:1139 | Realtek Semi... | RTL8188CE 802.11b/g/n... | 1.3%   | 3.14.33  | 51273F53DF |
| 10ec:8178 | 1043:84b6 | Realtek Semi... | RTL8192CE PCIe Wirele... | 4.5%   | 4.9.20   | BE8312BB93 |
| 10ec:8179 | 103c:197d | Realtek Semi... | RTL8188EE Wireless Ne... | 8%     | 3.14.25  | 220BF859F8 |
| 10ec:8179 | 10ec:8197 | Realtek Semi... | RTL8188EE Wireless Ne... | 8.7%   | 4.9.60   | D4FDC9B47A |
| 10ec:8179 | 17aa:0179 | Realtek Semi... | RTL8188EE Wireless Ne... | 4.8%   | 3.14.44  | 08BB09B100 |
| 10ec:8179 | 1a3b:1f38 | Realtek Semi... | RTL8188EE Wireless Ne... | 4.3%   | 4.1.13   | 5A2A5A23F7 |
| 10ec:8185 | 10ec:8225 | Realtek Semi... | RTL-8185 IEEE 802.11a... | 2%     | 3.14.44  | E44354FF81 |
| 10ec:818b | 10ec:818b | Realtek Semi... | RTL8192EE PCIe Wirele... | 25%    | 4.18.16  | 26018540A4 |
| 10ec:818b | 10ec:8196 | Realtek Semi... | RTL8192EE PCIe Wirele... | 3.7%   | 4.15.0   | 52D70A47DA |
| 10ec:8190 | 10ec:8190 | Realtek Semi... | RTL8190 802.11n PCI W... | 100%   |          | A93721363C |
| 10ec:8723 | 10ec:0726 | Realtek Semi... | RTL8723AE PCIe Wirele... | 0.8%   | 3.18.10  | 598F621727 |
| 10ec:8723 | 10ec:0733 | Realtek Semi... | RTL8723AE PCIe Wirele... | 100%   |          | 2F246CACD8 |
| 10ec:8812 | 10ec:8203 | Realtek Semi... | RTL8812AE 802.11ac PC... | 50%    | 4.15.0   | D8226DE108 |
| 10ec:8813 | 10ec:8813 | Realtek Semi... | RTL8813AE 802.11ac PC... | 100%   |          | 60389B7FFA |
| 10ec:8821 | 1043:207f | Realtek Semi... | RTL8821AE 802.11ac PC... | 100%   |          | A226259559 |
| 10ec:8821 | 17aa:a803 | Realtek Semi... | RTL8821AE 802.11ac PC... | 20%    | 4.18.16  | 762E9BD18E |
| 10ec:8821 | 1a3b:2161 | Realtek Semi... | RTL8821AE 802.11ac PC... | 7.4%   | 3.14.44  | 5EEDC9CEE8 |
| 10ec:b723 | 1025:b734 | Realtek Semi... | RTL8723BE PCIe Wirele... | 9.1%   | 4.1.10   | DE10405623 |
| 10ec:b723 | 103c:2231 | Realtek Semi... | RTL8723BE PCIe Wirele... | 25.6%  | 3.18.11  | 9CFD1D3FF6 |
| 10ec:b723 | 103c:804c | Realtek Semi... | RTL8723BE PCIe Wirele... | 3.9%   | 4.1.15   | C3ACAEB030 |
| 10ec:b723 | 103c:8167 | Realtek Semi... | RTL8723BE PCIe Wirele... | 50%    | 4.9.60   | A17480222D |
| 10ec:b723 | 10ec:b729 | Realtek Semi... | RTL8723BE PCIe Wirele... | 26.1%  | 3.17.4   | FD5BC52C49 |
| 10ec:b723 | 10ec:b733 | Realtek Semi... | RTL8723BE PCIe Wirele... | 10%    | 4.1.38   | BDAF59B6EB |
| 10ec:b723 | 11ad:1723 | Realtek Semi... | RTL8723BE PCIe Wirele... | 1.6%   | 4.9.9    | E6285FD8C3 |
| 10ec:b723 | 17aa:b728 | Realtek Semi... | RTL8723BE PCIe Wirele... | 20%    | 3.18.14  | 02D1977887 |
| 10ec:b723 | 17aa:b736 | Realtek Semi... | RTL8723BE PCIe Wirele... | 10.5%  | 3.18.16  | 39A9917502 |
| 10ec:b723 | 1a3b:2159 | Realtek Semi... | RTL8723BE PCIe Wirele... | 3.6%   | 4.1.15   | DDF48A7B95 |
| 10ec:b723 | 1b9a:2485 | Realtek Semi... | RTL8723BE PCIe Wirele... | 3.4%   | 4.3.3    | D57B5C86E0 |
| 10ec:b822 | 103c:831b | Realtek Semi... | RTL8822BE 802.11a/b/g... | 1.3%   | 3.10.0   | 9C6AD0A8DB |
| 10ec:b822 | 1043:8746 | Realtek Semi... | RTL8822BE 802.11a/b/g... | 2.1%   | 4.15.0   | 9FBBF0498F |
| 10ec:b822 | 17aa:b023 | Realtek Semi... | RTL8822BE 802.11a/b/g... | 3.3%   | 4.15.0   | F1C277189F |
| 10ec:b822 | 1a3b:2950 | Realtek Semi... | RTL8822BE 802.11a/b/g... | 2.4%   | 4.15.0   | F3E110826B |
| 10ec:c821 | 103c:831a | Realtek Semi... | RTL8821CE 802.11ac PC... | 87.6%  | 4.15.0   | 49834FC974 |
| 10ec:c821 | 103c:884d | Realtek Semi... | RTL8821CE 802.11ac PC... | 71.4%  | 5.10.10  | 918E09E044 |
| 10ec:c821 | 1043:87ae | Realtek Semi... | RTL8821CE 802.11ac PC... | 75%    | 5.10.14  | 801DCDD873 |
| 10ec:c821 | 1043:87b0 | Realtek Semi... | RTL8821CE 802.11ac PC... | 100%   |          | 440961AE4A |
| 10ec:c821 | 10ec:c821 | Realtek Semi... | RTL8821CE 802.11ac PC... | 84.6%  | 5.6.14   | CEE847C753 |
| 10ec:c821 | 10ec:c827 | Realtek Semi... | RTL8821CE 802.11ac PC... | 75%    | 4.15.0   | 0D3A90E1DE |
| 10ec:c821 | 17aa:c024 | Realtek Semi... | RTL8821CE 802.11ac PC... | 74.9%  | 4.9.124  | 80F0E0228B |
| 10ec:c821 | 1a3b:3040 | Realtek Semi... | RTL8821CE 802.11ac PC... | 82.8%  | 4.18.16  | 1779BD65F6 |
| 10ec:c821 | 1a3b:3041 | Realtek Semi... | RTL8821CE 802.11ac PC... | 59.6%  | 4.18.16  | 6BCA7E05DB |
| 10ec:c822 | 103c:85f7 | Realtek Semi... | RTL8822CE 802.11ac PC... | 11.1%  | 5.4.8    | 25F309DA06 |
| 10ec:c822 | 1058:1e25 | Realtek Semi... | RTL8822CE 802.11ac PC... | 9.1%   | 5.4.40   | 7F2A537A33 |
| 10ec:c822 | 11ad:0810 | Realtek Semi... | RTL8822CE 802.11ac PC... | 3.1%   | 4.18.16  | 3A1B31970C |
| 10ec:c822 | 17aa:c123 | Realtek Semi... | RTL8822CE 802.11ac PC... | 20%    | 5.4.32   | 166932E73B |
| 10ec:c822 | 1a3b:3750 | Realtek Semi... | RTL8822CE 802.11ac PC... | 44.4%  | 5.4.32   | 9C797156F9 |
| 10ec:c82f | 17aa:c02f | Realtek Semi... | RTL8822CE 802.11ac PC... | 89.3%  | 5.10.7   | 5C170164B4 |
| 10ec:d723 | 103c:8319 | Realtek Semi... | RTL8723DE Wireless Ne... | 90.7%  | 4.9.41   | 6436F82675 |
| 11ab:1fa6 | 1043:138f | Marvell Tech... | Marvell W8300 802.11 ... | 100%   |          | E75F4538BC |
| 11ab:1fa6 | 1186:3b09 | Marvell Tech... | Marvell W8300 802.11 ... | 100%   |          | 4BDC000ABE |
| 11ab:1fa7 | 1043:138f | Marvell Tech... | 88W8310 and 88W8000G ... | 100%   |          | 436FC401D1 |
| 11ab:1faa | 1186:3b22 | Marvell Tech... | 88w8335 [Libertas] 80... | 100%   |          | E3C769130D |
| 11ab:1faa | 11ab:1faa | Marvell Tech... | 88w8335 [Libertas] 80... | 100%   |          | E639B08710 |
| 11ab:1faa | 1385:6b00 | Marvell Tech... | 88w8335 [Libertas] 80... | 100%   |          | 9E34ADFE39 |
| 11ab:2a02 | 1385:7e00 | Marvell Tech... | 88W8361 [TopDog] 802.... | 100%   |          | 51F69F1430 |
| 11ab:2a08 | 11ab:2a08 | Marvell Tech... | 88W8362e [TopDog] 802... | 100%   |          | 73A456C9AA |
| 1260:3890 | 1385:4800 | Intersil        | ISL3890 [Prism GT/Pri... | 100%   |          | D6154D7955 |
| 1260:3890 | 17cf:0014 | Intersil        | ISL3890 [Prism GT/Pri... | 75%    | 4.15.0   | 289D2B0685 |
| 14c3:7630 | 103c:197c | MEDIATEK        | MT7630e 802.11bgn Wir... | 100%   |          | E27420B2EA |
| 14c3:7630 | 105b:e074 | MEDIATEK        | MT7630e 802.11bgn Wir... | 100%   |          | F5A173D797 |
| 14c3:7630 | 105b:e084 | MEDIATEK        | MT7630e 802.11bgn Wir... | 100%   |          | DF4413AF58 |
| 14e4:0576 | 14e4:0576 | Broadcom        | BCM43224 802.11a/b/g/n   | 11.1%  | 4.15.0   | FAD005747E |
| 14e4:4311 | 1028:0007 | Broadcom        | BCM4311 802.11b/g WLAN   | 1.7%   | 3.10.34  | 7B12363B97 |
| 14e4:4311 | 103c:1363 | Broadcom        | BCM4311 802.11b/g WLAN   | 8.8%   | 3.10.34  | 56702DE7D4 |
| 14e4:4311 | 103c:1364 | Broadcom        | BCM4311 802.11b/g WLAN   | 6.2%   | 3.14.33  | A422A9DE40 |
| 14e4:4311 | 1468:0316 | Broadcom        | BCM4311 802.11b/g WLAN   | 100%   |          | 7F0BB0CC92 |
| 14e4:4311 | 1468:0422 | Broadcom        | BCM4311 802.11b/g WLAN   | 8.1%   | 3.10.34  | 1606FA1431 |
| 14e4:4311 | 14e4:0465 | Broadcom        | BCM4311 802.11b/g WLAN   | 7.1%   | 4.1.25   | 2E87CB3413 |
| 14e4:4312 | 1028:0007 | Broadcom Lim... | BCM4311 802.11a/b/g      | 14%    | 3.14.44  | AD2104F7C9 |
| 14e4:4312 | 103c:1361 | Broadcom Lim... | BCM4311 802.11a/b/g      | 37.5%  | 3.14.44  | 14CC279C8C |
| 14e4:4312 | 106b:0089 | Broadcom        | BCM4311 802.11a/b/g      | 14.3%  | 4.15.0   | 376EF8BAEC |
| 14e4:4315 | 1028:000b | Broadcom        | BCM4312 802.11b/g LP-PHY | 0.9%   | 3.10.34  | CC25AD321C |
| 14e4:4315 | 1028:000c | Broadcom Lim... | BCM4312 802.11b/g LP-PHY | 2.1%   | 3.10.34  | C55F3CA871 |
| 14e4:4315 | 103c:137d | Broadcom        | BCM4312 802.11b/g LP-PHY | 0.6%   | 3.14.33  | A5594A75D1 |
| 14e4:4315 | 103c:1508 | Broadcom        | BCM4312 802.11b/g LP-PHY | 0.8%   | 3.14.44  | D0F06C8499 |
| 14e4:4315 | 14e4:04b5 | Broadcom        | BCM4312 802.11b/g LP-PHY | 7.5%   | 3.14.25  | B9CE65486B |
| 14e4:4318 | 103c:1356 | Broadcom        | BCM4318 [AirForce One... | 3%     | 4.1.19   | 306E665622 |
| 14e4:4318 | 1043:100f | Broadcom        | BCM4318 [AirForce One... | 4.1%   | 3.14.44  | 61A278E2B6 |
| 14e4:4318 | 1468:0312 | Broadcom Lim... | BCM4318 [AirForce One... | 9.1%   | 3.10.34  | A28F7B2623 |
| 14e4:4320 | 103c:12f8 | Broadcom        | BCM4306 802.11b/g Wir... | 28.6%  | 3.10.34  | FE61304CD4 |
| 14e4:4320 | 103c:12fa | Broadcom        | BCM4306 802.11b/g Wir... | 20%    | 4.15.0   | 0FE7032974 |
| 14e4:4324 | 1028:0003 | Broadcom        | BCM4309 802.11abg Wir... | 50%    | 4.15.0   | 0077E52877 |
| 14e4:4328 | 1028:000a | Broadcom Lim... | BCM4321 802.11a/b/g/n    | 1.4%   | 3.10.34  | C63D7A491D |
| 14e4:4328 | 106b:0087 | Broadcom Lim... | BCM4321 802.11a/b/g/n    | 3.7%   | 4.9.20   | 394EF62F20 |
| 14e4:4328 | 106b:0088 | Broadcom        | BCM4321 802.11a/b/g/n    | 2.7%   | 4.1.15   | 0F9CBE4B62 |
| 14e4:4328 | 106b:008c | Broadcom        | BCM4321 802.11a/b/g/n    | 3.8%   | 4.1.38   | 6BCA23F21C |
| 14e4:4328 | 106b:0090 | Broadcom Lim... | BCM4321 802.11a/b/g/n    | 2.2%   | 4.1.22   | 030A81E657 |
| 14e4:432b | 1028:000d | Broadcom        | BCM4322 802.11a/b/g/n... | 2.4%   | 3.10.0   | 103788F3AC |
| 14e4:432b | 103c:1510 | Broadcom        | BCM4322 802.11a/b/g/n... | 100%   |          | 23C8DE7582 |
| 14e4:432b | 106b:008d | Broadcom        | BCM4322 802.11a/b/g/n... | 1.3%   | 4.1.38   | 8B736DA7F7 |
| 14e4:432b | 106b:008e | Broadcom        | BCM4322 802.11a/b/g/n... | 3.6%   | 4.9.20   | 0CD93A5F3A |
| 14e4:4331 | 106b:00d6 | Broadcom        | BCM4331 802.11a/b/g/n    | 3.7%   | 4.1.25   | C551F2BDFF |
| 14e4:4331 | 106b:00f5 | Broadcom        | BCM4331 802.11a/b/g/n    | 1.8%   | 4.9.20   | 437B3EB74D |
| 14e4:4331 | 106b:010e | Broadcom        | BCM4331 802.11a/b/g/n    | 2%     | 3.14.44  | C7640973E7 |
| 14e4:4331 | 14e4:4331 | Broadcom        | BCM4331 802.11a/b/g/n    | 5.1%   | 4.1.25   | 19C76A69A3 |
| 14e4:4353 | 1028:000e | Broadcom        | BCM43224 802.11a/b/g/n   | 3.1%   | 4.1.15   | 1F602B4A6B |
| 14e4:4353 | 103c:1509 | Broadcom Lim... | BCM43224 802.11a/b/g/n   | 3.6%   | 4.9.9    | EF84151F18 |
| 14e4:4353 | 103c:1510 | Broadcom        | BCM43224 802.11a/b/g/n   | 1.7%   | 4.1.25   | 55752483EF |
| 14e4:4353 | 106b:0093 | Broadcom        | BCM43224 802.11a/b/g/n   | 3.9%   | 4.1.15   | 75DC2B77CE |
| 14e4:4353 | 106b:00d1 | Broadcom        | BCM43224 802.11a/b/g/n   | 4%     | 3.14.25  | A3168C57EA |
| 14e4:4357 | 105b:e021 | Broadcom        | BCM43225 802.11b/g/n     | 3.3%   | 3.14.25  | DA8880B543 |
| 14e4:4357 | 144f:7181 | Broadcom        | BCM43225 802.11b/g/n     | 33.3%  | 4.15.0   | 9D9E59F8A7 |
| 14e4:4357 | 14e4:04da | Broadcom Lim... | BCM43225 802.11b/g/n     | 4.8%   | 4.1.13   | E4BBFE0245 |
| 14e4:4357 | 14e4:0570 | Broadcom        | BCM43225 802.11b/g/n     | 3.6%   | 4.15.0   | 902963AE8F |
| 14e4:4358 | 105b:e040 | Broadcom        | BCM43227 802.11b/g/n     | 2%     | 3.14.33  | 1790F79449 |
| 14e4:4359 | 1028:0011 | Broadcom        | BCM43228 802.11a/b/g/n   | 1.4%   | 3.14.44  | 49AC9F2B94 |
| 14e4:4359 | 1028:0014 | Broadcom        | BCM43228 802.11a/b/g/n   | 1.9%   | 3.14.44  | 71510169F8 |
| 14e4:4359 | 103c:182c | Broadcom        | BCM43228 802.11a/b/g/n   | 5.3%   | 4.1.25   | A2536BD6FE |
| 14e4:4359 | 103c:2135 | Broadcom        | BCM43228 802.11a/b/g/n   | 14.3%  | 4.1.25   | 3E13F8A157 |
| 14e4:4359 | 1043:850c | Broadcom        | BCM43228 802.11a/b/g/n   | 11.3%  | 3.14.44  | 925EC1C4FD |
| 14e4:4359 | 105b:e04b | Broadcom        | BCM43228 802.11a/b/g/n   | 3.9%   | 3.14.44  | BABECD66A1 |
| 14e4:4359 | 105b:e08b | Broadcom Lim... | BCM43228 802.11a/b/g/n   | 7.1%   | 4.1.34   | 0D43FC94FE |
| 14e4:4359 | 11ad:6603 | Broadcom        | BCM43228 802.11a/b/g/n   | 6.2%   | 4.1.15   | C6F99AC92E |
| 14e4:4359 | 14e4:05e2 | Broadcom        | BCM43228 802.11a/b/g/n   | 3.7%   | 3.10.42  | 2C52151F77 |
| 14e4:4359 | 14e4:0607 | Broadcom Lim... | BCM43228 802.11a/b/g/n   | 1.8%   | 3.14.44  | A30712CD7D |
| 14e4:4365 | 1028:0016 | Broadcom        | BCM43142 802.11b/g/n     | 6.6%   | 3.14.33  | 2E65A0F466 |
| 14e4:4365 | 1028:0018 | Broadcom        | BCM43142 802.11b/g/n     | 28.6%  | 4.1.25   | F9EC6964BB |
| 14e4:4365 | 103c:2230 | Broadcom        | BCM43142 802.11b/g/n     | 40.3%  | 3.14.44  | CC7F828773 |
| 14e4:4365 | 103c:2232 | Broadcom        | BCM43142 802.11b/g/n     | 28.6%  | 4.19.0   | AC98ADAF56 |
| 14e4:4365 | 103c:804a | Broadcom        | BCM43142 802.11b/g/n     | 22.2%  | 4.1.15   | 2D0FB807ED |
| 14e4:4365 | 105b:e071 | Broadcom        | BCM43142 802.11b/g/n     | 38.2%  | 3.14.44  | 77DF70A98A |
| 14e4:4365 | 105b:e07e | Broadcom        | BCM43142 802.11b/g/n     | 49%    | 3.14.44  | E9004A67E9 |
| 14e4:4365 | 11ad:6605 | Broadcom        | BCM43142 802.11b/g/n     | 11%    | 3.14.33  | 4DB9710D78 |
| 14e4:4365 | 11ad:6645 | Broadcom        | BCM43142 802.11b/g/n     | 34%    | 3.14.33  | 6E75E7C288 |
| 14e4:4365 | 11ad:6655 | Broadcom        | BCM43142 802.11b/g/n     | 49.1%  | 4.9.9    | AB3B576BD1 |
| 14e4:4365 | 11ad:6675 | Broadcom Lim... | BCM43142 802.11b/g/n     | 33.7%  | 3.14.44  | 90646A2169 |
| 14e4:4365 | 11ad:66a5 | Broadcom        | BCM43142 802.11b/g/n     | 33.3%  | 4.1.15   | CA3628282A |
| 14e4:4365 | 17aa:0611 | Broadcom        | BCM43142 802.11b/g/n     | 10.8%  | 3.14.25  | 410EC3D411 |
| 14e4:4365 | 17aa:0621 | Broadcom        | BCM43142 802.11b/g/n     | 21%    | 3.14.25  | 93033F85C6 |
| 14e4:4365 | 1a3b:2155 | Broadcom        | BCM43142 802.11b/g/n     | 41.2%  | 4.15.0   | 4B47248331 |
| 14e4:4365 | 1b9a:3002 | Broadcom        | BCM43142 802.11b/g/n     | 62.2%  | 4.1.25   | 503D9DACF6 |
| 14e4:43a0 | 1043:85df | Broadcom        | BCM4360 802.11ac Wire... | 27.8%  | 4.15.0   | 57895DF9DF |
| 14e4:43a0 | 1043:8659 | Broadcom        | BCM4360 802.11ac Wire... | 14.3%  | 3.10.0   | 7A813C93B0 |
| 14e4:43a0 | 106b:0111 | Broadcom        | BCM4360 802.11ac Wire... | 19.4%  | 4.15.0   | 0AC71FBEBA |
| 14e4:43a0 | 106b:0117 | Broadcom Lim... | BCM4360 802.11ac Wire... | 17.1%  | 4.18.0   | 9D1694385F |
| 14e4:43a0 | 106b:0134 | Broadcom        | BCM4360 802.11ac Wire... | 11.1%  | 4.18.0   | C7FFF34E01 |
| 14e4:43a0 | 106b:0135 | Broadcom        | BCM4360 802.11ac Wire... | 62.5%  | 5.0.0    | 4AAF32A9FC |
| 14e4:43a0 | 106b:013b | Broadcom Lim... | BCM4360 802.11ac Wire... | 26.7%  | 4.18.0   | 42B0868834 |
| 14e4:43a0 | 14e4:0619 | Broadcom        | BCM4360 802.11ac Wire... | 7.5%   | 4.15.0   | AC6B5ED34E |
| 14e4:43ae | 17aa:0622 | Broadcom        | BCM43162 802.11ac Wir... | 72.4%  | 4.18.16  | F995163FF4 |
| 14e4:43b1 | 1028:0017 | Broadcom Lim... | BCM4352 802.11ac Wire... | 14.3%  | 4.1.13   | 95FA029C09 |
| 14e4:43b1 | 1028:0019 | Broadcom Lim... | BCM4352 802.11ac Wire... | 38.5%  | 4.18.0   | 4C6F76D2E4 |
| 14e4:43b1 | 103c:2154 | Broadcom Lim... | BCM4352 802.11ac Wire... | 80.8%  | 4.18.0   | 12460D9CF7 |
| 14e4:43b1 | 1043:855c | Broadcom        | BCM4352 802.11ac Wire... | 26.7%  | 4.15.0   | 32805E80B1 |
| 14e4:43b1 | 1043:85ba | Broadcom        | BCM4352 802.11ac Wire... | 40%    | 4.18.0   | 35365BE0E8 |
| 14e4:43b1 | 17aa:0623 | Broadcom Lim... | BCM4352 802.11ac Wire... | 11.1%  | 4.15.0   | FDB99E4DB2 |
| 14e4:43b1 | 1a3b:2123 | Broadcom        | BCM4352 802.11ac Wire... | 6.2%   | 4.15.0   | 9CACD1608E |
| 14e4:43b1 | 1a3b:2b23 | Broadcom        | BCM4352 802.11ac Wire... | 12.5%  | 4.15.0   | 14ABE97F88 |
| 14e4:43ba | 106b:0133 | Broadcom        | BCM43602 802.11ac Wir... | 2.3%   | 4.9.9    | D766064036 |
| 14e4:43ba | 106b:014a | Broadcom        | BCM43602 802.11ac Wir... | 6.7%   | 4.18.16  | 5984E1BBAC |
| 14e4:43ba | 106b:0157 | Broadcom        | BCM43602 802.11ac Wir... | 37.5%  | 4.15.0   | 0388E1560C |
| 14e4:43ba | 106b:0173 | Broadcom        | BCM43602 802.11ac Wir... | 11.1%  | 5.3.0    | 6F3816ABBD |
| 14e4:43c3 | 1043:86fb | Broadcom        | Network controller       | 2.3%   | 4.15.0   | 530CC43BE2 |
| 14e4:4464 | 106b:07bf | Broadcom        | BCM4364 802.11ac Wire... | 54.7%  | 5.6.0    | 2140D3DF59 |
| 14e4:4488 | 106b:0870 | Broadcom        | BCM4377b Wireless Net... | 100%   |          | CB7AAC8083 |
| 14e4:4727 | 1028:0010 | Broadcom        | BCM4313 802.11bgn Wir... | 4.5%   | 4.9.0    | 213509A58E |
| 14e4:4727 | 1028:0012 | Broadcom Lim... | BCM4313 802.11bgn Wir... | 15.4%  | 4.15.0   | CB18C38BD3 |
| 14e4:4727 | 1028:0015 | Broadcom        | BCM4313 802.11bgn Wir... | 12.5%  | 4.15.0   | 94A78C36AF |
| 14e4:4727 | 103c:145c | Broadcom        | BCM4313 802.11bgn Wir... | 4.5%   | 3.10.42  | D1CAD27E6F |
| 14e4:4727 | 103c:1483 | Broadcom        | BCM4313 802.11bgn Wir... | 2.6%   | 4.1.34   | 4DB85F6450 |
| 14e4:4727 | 103c:1795 | Broadcom        | BCM4313 802.11bgn Wir... | 13.8%  | 3.10.42  | 6CF581A2C9 |
| 14e4:4727 | 105b:e042 | Broadcom        | BCM4313 802.11bgn Wir... | 4.9%   | 4.15.0   | 3938D2C1BC |
| 14e4:4727 | 144f:7175 | Broadcom        | BCM4313 802.11bgn Wir... | 10%    | 4.15.0   | CF01B0DC10 |
| 14e4:4727 | 144f:7179 | Broadcom        | BCM4313 802.11bgn Wir... | 10.8%  | 3.10.34  | 28B6B15E59 |
| 14e4:4727 | 14e4:0510 | Broadcom        | BCM4313 802.11bgn Wir... | 12.7%  | 4.2.6    | 635A9139E1 |
| 14e4:4727 | 14e4:051b | Broadcom        | BCM4313 802.11bgn Wir... | 3.1%   | 2.6.32   | 0DB2A8DFAD |
| 14e4:4727 | 14e4:0587 | Broadcom Lim... | BCM4313 802.11bgn Wir... | 6.8%   | 4.15.0   | A48E280881 |
| 14e4:4727 | 14e4:0608 | Broadcom        | BCM4313 802.11bgn Wir... | 14.3%  | 4.1.38   | E7EF3A9E86 |
| 14e4:4727 | 185f:051a | Broadcom        | BCM4313 802.11bgn Wir... | 7.4%   | 4.9.0    | B379B29AED |
| 14e4:4727 | 1a3b:2a47 | Broadcom Lim... | BCM4313 802.11bgn Wir... | 25%    | 3.10.34  | 79326DA8CA |
| 167b:2116 | 340f:187e | ZyDAS Techno... | ZD1212B Wireless Adapter | 100%   |          | C399CBB5F3 |
| 168c:0013 | 1186:3a13 | Qualcomm Ath... | AR5212/5213/2414 Wire... | 2.4%   | 3.14.44  | EEB27108B2 |
| 168c:001c | 103c:137b | Qualcomm Ath... | AR242x / AR542x Wirel... | 0.5%   | 3.14.33  | 93C0EF7223 |
| 168c:001c | 144f:7106 | Qualcomm Ath... | AR242x / AR542x Wirel... | 4.8%   | 3.14.33  | 310DDB721F |
| 168c:002a | 106b:008f | Qualcomm Ath... | AR928X Wireless Netwo... | 1%     | 3.14.44  | ECB4D0EF2A |
| 168c:002a | 1a3b:1067 | Qualcomm Ath... | AR928X Wireless Netwo... | 0.5%   | 3.0.28   | A13580724B |
| 168c:002b | 103c:1461 | Qualcomm Ath... | AR9285 Wireless Netwo... | 0.4%   | 3.14.33  | F4DE983D96 |
| 168c:002b | 144f:7173 | Qualcomm Ath... | AR9285 Wireless Netwo... | 1%     | 3.14.44  | 211A9802DB |
| 168c:002d | 168c:0300 | Qualcomm Ath... | AR9227 Wireless Netwo... | 1.2%   | 3.14.33  | AA24EEDD97 |
| 168c:002e | 105b:e034 | Qualcomm Ath... | AR9287 Wireless Netwo... | 0.2%   | 3.10.0   | 8FE3AF49FB |
| 168c:002e | 10cf:158f | Qualcomm Ath... | AR9287 Wireless Netwo... | 2.7%   | 4.1.25   | 958D094890 |
| 168c:0032 | 11ad:6608 | Qualcomm Ath... | AR9485 Wireless Netwo... | 1.6%   | 3.14.33  | 67009EFFAA |
| 168c:0032 | 11ad:6617 | Qualcomm Ath... | AR9485 Wireless Netwo... | 0.3%   | 3.14.25  | 86D2D3B0E1 |
| 168c:0032 | 11ad:6628 | Qualcomm Ath... | AR9485 Wireless Netwo... | 0.8%   | 3.14.44  | 469E04E0D5 |
| 168c:0032 | 144d:4105 | Qualcomm Ath... | AR9485 Wireless Netwo... | 0.3%   | 3.10.0   | 5BD6CA5ABA |
| 168c:0034 | 1028:020b | Qualcomm Ath... | AR9462 Wireless Netwo... | 14.3%  | 5.4.0    | F674F91052 |
| 168c:0034 | 103c:1864 | Qualcomm Ath... | AR9462 Wireless Netwo... | 4%     | 3.10.0   | CF3ED91B8A |
| 168c:0034 | 105b:e052 | Qualcomm Ath... | AR9462 Wireless Netwo... | 0.4%   | 3.10.34  | 23E2162B8E |
| 168c:0036 | 1028:020c | Qualcomm Ath... | QCA9565 / AR9565 Wire... | 0.2%   | 3.10.0   | 517406F8B6 |
| 168c:0036 | 1028:020e | Qualcomm Ath... | QCA9565 / AR9565 Wire... | 1%     | 4.4.0    | 87C36A9322 |
| 168c:0036 | 11ad:0642 | Qualcomm Ath... | QCA9565 / AR9565 Wire... | 0.6%   | 3.10.51  | 384DEF70B1 |
| 168c:0036 | 11ad:0803 | Qualcomm Ath... | QCA9565 / AR9565 Wire... | 1%     | 3.14.44  | 401BBED185 |
| 168c:0036 | 17aa:4026 | Qualcomm Ath... | QCA9565 / AR9565 Wire... | 0.5%   | 3.10.51  | EEFC7C92B2 |
| 168c:0036 | 1a3b:2130 | Qualcomm Ath... | QCA9565 / AR9565 Wire... | 0.7%   | 3.14.44  | E3E9F32F6D |
| 168c:0037 | 1a3b:1195 | Qualcomm Ath... | AR9485 Wireless Netwo... | 11.1%  | 4.9.20   | CE8124E5F4 |
| 168c:0037 | 1a3b:2100 | Qualcomm Ath... | AR9485 Wireless Netwo... | 2.6%   | 3.14.25  | 0F8E9B7955 |
| 168c:003e | 1028:0310 | Qualcomm Ath... | QCA6174 802.11ac Wire... | 0.2%   | 4.4.0    | EBA5E925B8 |
| 168c:003e | 1a56:1535 | Qualcomm Ath... | QCA6174 802.11ac Wire... | 0.2%   | 4.15.0   | 6695D2A05E |
| 168c:0042 | 1028:1810 | Qualcomm Ath... | QCA9377 802.11ac Wire... | 0.1%   | 4.4.0    | F591FD6F3D |
| 168c:0042 | 11ad:0806 | Qualcomm Ath... | QCA9377 802.11ac Wire... | 3.3%   | 4.4.0    | ECB6A89DFC |
| 168c:0042 | 11ad:08a6 | Qualcomm Ath... | QCA9377 802.11ac Wire... | 0.1%   | 3.10.0   | E7395D0EE2 |
| 168c:0042 | 17aa:0901 | Qualcomm Ath... | QCA9377 802.11ac Wire... | 0.5%   | 4.4.0    | 4CCF4659D4 |
| 168c:0042 | 17aa:4035 | Qualcomm Ath... | QCA9377 802.11ac Wire... | 0.4%   | 4.8.0    | C3352134E9 |
| 17cb:0001 | 1737:0045 | Qualcomm        | AGN100 802.11 a/b/g T... | 100%   |          | 7D17E6E1A3 |
| 17cb:1101 | 1a56:a501 | Qualcomm        | QCA6390 Wireless Netw... | 17.6%  | 5.10.0   | 1819DE4A98 |
| 17fe:2220 | 1468:0305 | InProComm       | IPN 2220 802.11g         | 100%   |          | 76920BC1B7 |
| 17fe:2220 | 1468:0310 | InProComm       | IPN 2220 802.11g         | 100%   |          | E9BD04F647 |
| 1814:0201 | 1432:0c54 | Ralink          | RT2500 Wireless 802.11bg | 100%   |          | 310DDB721F |
| 1814:0300 | 1186:3c09 | Ralink          | Wireless Adapter Cany... | 100%   |          | 24F60E51DE |
| 1814:0301 | 1814:2561 | Ralink          | RT2561/RT61 802.11g PCI  | 4.7%   | 3.14.33  | C74C010C1B |
| 1814:3062 | 1814:3062 | Ralink          | RT3062 Wireless 802.1... | 1.6%   | 3.14.44  | 9D9E2DB550 |
| 1814:3090 | 1462:6894 | Ralink          | RT3090 Wireless 802.1... | 10%    | 4.18.16  | E40B76E473 |
| 1814:3090 | 1814:3090 | Ralink          | RT3090 Wireless 802.1... | 0.9%   | 3.14.33  | E15B3DCFA3 |
| 1814:3290 | 103c:18ec | Ralink          | RT3290 Wireless 802.1... | 0.7%   | 3.14.15  | 387BBD9C5B |
| 1814:5390 | 105b:e054 | Ralink          | RT5390 Wireless 802.1... | 0.7%   | 3.14.33  | 11B77977B4 |
| 1814:5392 | 1186:3c0b | Ralink          | RT5392 PCIe Wireless ... | 3.3%   | 3.14.33  | D3F4DEFFA5 |
| 1814:5392 | 1814:5392 | Ralink          | RT5392 PCIe Wireless ... | 16.7%  | 4.18.0   | 57643353CE |
| 1814:539a | 103c:1839 | Ralink          | WLAN controller          | 6.7%   | 4.1.15   | 2E60620A98 |
| 1814:539f | 103c:1637 | Ralink          | RT5390 [802.11 b/g/n ... | 1.4%   | 3.14.44  | ED2FBC90A0 |
| 1814:5592 | 1043:851a | Ralink          | RT5592 PCIe Wireless ... | 92.6%  | 5.8.0    | 9CE5EAB595 |
| 1814:5592 | 1814:5592 | Ralink          | RT5592 PCIe Wireless ... | 100%   |          | 760C31A638 |
| 1a47:0003 | 0000:0300 | 3DSP            | WLAN and Bluetooth Card  | 100%   |          | 25DB9022C9 |
| 1ae9:0301 | 1ae9:0000 | Wilocity        | Wil6200 802.11ad Wire... | 100%   |          | E769A18F8A |
| 8086:0082 | 8086:1321 | Intel           | Centrino Advanced-N 6... | 0.9%   | 3.14.33  | 7DBD1D34B7 |
| 8086:0085 | 8086:1311 | Intel           | Centrino Advanced-N 6... | 0.2%   | 3.10.0   | 0BD1499DB9 |
| 8086:0085 | 8086:c220 | Intel           | Centrino Advanced-N 6... | 5.9%   | 3.14.15  | 578D1BADCA |
| 8086:008a | 8086:0000 | Intel           | Centrino Wireless-N 1... | 100%   |          | 28086B6CA8 |
| 8086:02f0 | 8086:0034 | Intel           | Comet Lake PCH-LP CNV... | 1.5%   | 4.15.0   | FCD9F8DF27 |
| 8086:02f0 | 8086:0074 | Intel           | Comet Lake PCH-LP CNV... | 2.2%   | 3.10.0   | A161A19F04 |
| 8086:02f0 | 8086:0234 | Intel           | Comet Lake PCH-LP CNV... | 4.2%   | 4.15.0   | 324F862858 |
| 8086:02f0 | 8086:4070 | Intel           | Comet Lake PCH-LP CNV... | 4.1%   | 5.3.0    | C308A5A20B |
| 8086:06f0 | 8086:0074 | Intel           | Comet Lake PCH CNVi WiFi | 1.7%   | 3.10.0   | 66DE8410B3 |
| 8086:06f0 | 8086:4070 | Intel           | Comet Lake PCH CNVi WiFi | 2.4%   | 4.18.0   | 3A565370DE |
| 8086:06f0 | 8086:42a4 | Intel           | Comet Lake PCH CNVi WiFi | 8.3%   | 4.15.0   | 3510F864F1 |
| 8086:088e | 8086:4060 | Intel           | Centrino Advanced-N 6235 | 0.2%   | 3.10.34  | AC608E1D37 |
| 8086:088e | 8086:4460 | Intel           | Centrino Advanced-N 6235 | 0.7%   | 3.10.0   | 9ABF14D168 |
| 8086:0891 | 8086:4222 | Intel           | Centrino Wireless-N 2200 | 0.9%   | 3.10.42  | 44F6A1F73B |
| 8086:0893 | 8086:0262 | Intel           | Centrino Wireless-N 135  | 2.8%   | 3.10.0   | 2DD89E3983 |
| 8086:0896 | 8086:5005 | Intel           | Centrino Wireless-N 130  | 0.2%   | 3.10.34  | 69C8FA5FEE |
| 8086:08ae | 8086:1005 | Intel           | Centrino Wireless-N 100  | 1.1%   | 3.10.42  | CF401BD3E4 |
| 8086:08b1 | 8086:4070 | Intel           | Wireless 7260            | 0.5%   | 3.10.0   | 1A67EAFE01 |
| 8086:08b1 | 8086:4470 | Intel           | Wireless 7260            | 0.4%   | 3.14.44  | DB19B78EB8 |
| 8086:08b1 | 8086:c070 | Intel           | Wireless 7260            | 2%     | 4.1.15   | 22D4B9FB7B |
| 8086:08b2 | 8086:c260 | Intel           | Wireless 7260            | 0.6%   | 4.1.16   | 819B048062 |
| 8086:08b3 | 8086:0070 | Intel           | Wireless 3160            | 0.3%   | 3.14.44  | 9D967E969D |
| 8086:08b3 | 8086:8070 | Intel           | Wireless 3160            | 2.6%   | 3.16.0   | 6A0C5E5BDA |
| 8086:08b3 | 8086:8470 | Intel           | Wireless 3160            | 0.3%   | 3.16.0   | 7E3EEBA3CA |
| 8086:08b4 | 8086:8270 | Intel           | Wireless 3160            | 0.7%   | 3.14.44  | AB6BD693BE |
| 8086:093c | 8086:0181 | Intel           | Wireless Gigabit 17265   | 100%   |          | 4382F7F583 |
| 8086:093c | 8086:0190 | Intel           | Wireless Gigabit 17265   | 100%   |          | F9A5B44211 |
| 8086:093c | 8086:2181 | Intel           | Wireless Gigabit 17265   | 100%   |          | FFDB13EDA0 |
| 8086:093c | 8086:2191 | Intel           | Wireless Gigabit 17265   | 100%   |          | 00FB0F909E |
| 8086:093c | 8086:5181 | Intel           | Wireless Gigabit 17265   | 100%   |          | 8DA437BE1F |
| 8086:093c | 8086:7001 | Intel           | Wireless Gigabit 17265   | 100%   |          | C05C701EBC |
| 8086:095a | 8086:5010 | Intel           | Wireless 7265            | 0.1%   | 4.18.0   | C60FCEAEE4 |
| 8086:095a | 8086:5400 | Intel           | Wireless 7265            | 5.6%   | 4.1.25   | 9CAA1B1F2B |
| 8086:095a | 8086:5410 | Intel           | Wireless 7265            | 0.3%   | 3.10.0   | 62308C2EBC |
| 8086:095b | 8086:5210 | Intel           | Wireless 7265            | 1%     | 4.1.34   | 6BCE8819C3 |
| 8086:24f3 | 8086:0010 | Intel           | Wireless 8260            | 0.6%   | 3.10.0   | 6158B04856 |
| 8086:24f3 | 8086:0130 | Intel           | Wireless 8260            | 0.7%   | 3.10.0   | B612D89D47 |
| 8086:24f3 | 8086:0150 | Intel           | Wireless 8260            | 2.9%   | 4.18.0   | FD44B61DAF |
| 8086:24f3 | 8086:1010 | Intel           | Wireless 8260            | 0.9%   | 4.1.15   | 5195396549 |
| 8086:24f3 | 8086:1130 | Intel           | Wireless 8260            | 0.5%   | 4.4.0    | 3A43711362 |
| 8086:24f3 | 8086:9010 | Intel           | Wireless 8260            | 1.2%   | 3.10.0   | 0A01176CBE |
| 8086:24fb | 8086:2110 | Intel           | Dual Band Wireless-AC... | 0.8%   | 4.19.0   | 4080E1B43F |
| 8086:24fd | 8086:0010 | Intel           | Wireless 8265 / 8275     | 0.2%   | 3.10.0   | 53BA44732D |
| 8086:24fd | 8086:0050 | Intel           | Wireless 8265 / 8275     | 0.7%   | 3.10.0   | 54E871CA5D |
| 8086:24fd | 8086:0110 | Intel           | Wireless 8265 / 8275     | 1.5%   | 4.12.14  | F03901ADED |
| 8086:24fd | 8086:1010 | Intel           | Wireless 8265 / 8275     | 0.3%   | 4.8.15   | 6C5EE38371 |
| 8086:24fd | 8086:9010 | Intel           | Wireless 8265 / 8275     | 0.8%   | 4.9.0    | 77B139696D |
| 8086:2526 | 1a56:1550 | Intel           | Wireless-AC 9260         | 1.1%   | 4.15.0   | EA77C657C0 |
| 8086:2526 | 8086:0014 | Intel           | Wireless-AC 9260         | 1.6%   | 4.15.0   | 55CDAF18A6 |
| 8086:2723 | 1a56:1654 | Intel           | Wi-Fi 6 AX200            | 4.5%   | 4.15.0   | 5964A40D34 |
| 8086:2723 | 8086:0080 | Intel           | Wi-Fi 6 AX200            | 2.4%   | 4.18.0   | 8C056E4751 |
| 8086:2723 | 8086:0084 | Intel           | Wi-Fi 6 AX200            | 3.3%   | 4.15.0   | 5A99A3A590 |
| 8086:2723 | 8086:008c | Intel           | Wi-Fi 6 AX200            | 3.6%   | 4.18.0   | A838427772 |
| 8086:2723 | 8086:4080 | Intel           | Wi-Fi 6 AX200            | 6.3%   | 4.15.0   | 405638D41C |
| 8086:2725 | 8086:0024 | Intel           | Wi-Fi 6 AX210/AX211/A... | 13.8%  | 5.8.0    | 8F45F37B98 |
| 8086:3165 | 8086:4010 | Intel           | Wireless 3165            | 0.2%   | 4.1.15   | 54574B77F2 |
| 8086:3165 | 8086:8010 | Intel           | Wireless 3165            | 0.3%   | 4.4.0    | AD10DD6BE0 |
| 8086:3165 | 8086:8110 | Intel           | Wireless 3165            | 0.6%   | 4.9.20   | 48E3CC8030 |
| 8086:3166 | 8086:4210 | Intel           | Dual Band Wireless-AC... | 0.3%   | 4.1.15   | FC2E5D7E80 |
| 8086:31dc | 8086:0034 | Intel           | Gemini Lake PCH CNVi ... | 2.6%   | 4.13.0   | 4D0AAEFEF6 |
| 8086:31dc | 8086:02a4 | Intel           | Gemini Lake PCH CNVi ... | 1.1%   | 4.14.71  | C364BD9F45 |
| 8086:34f0 | 8086:0000 | Intel           | Ice Lake-LP PCH CNVi ... | 50%    | 5.11.15  | 86927CE44D |
| 8086:34f0 | 8086:0034 | Intel           | Ice Lake-LP PCH CNVi ... | 9.1%   | 5.3.0    | 4019B6C1FF |
| 8086:34f0 | 8086:0074 | Intel           | Ice Lake-LP PCH CNVi ... | 0.9%   | 5.3.0    | 63ED12357B |
| 8086:4222 | 103c:135c | Intel           | PRO/Wireless 3945ABG ... | 1%     | 3.14.25  | 9EDB73DD0E |
| 8086:4223 | 8086:1040 | Intel           | PRO/Wireless 2915ABG ... | 16.7%  | 4.15.0   | 8488B3D0B9 |
| 8086:4227 | 8086:1010 | Intel           | PRO/Wireless 3945ABG ... | 1.8%   | 3.14.39  | 73B406FF03 |
| 8086:4229 | 8086:1001 | Intel           | PRO/Wireless 4965 AG ... | 3.7%   | 3.14.44  | 13824A2872 |
| 8086:4229 | 8086:1101 | Intel           | PRO/Wireless 4965 AG ... | 0.5%   | 3.14.44  | 2DCD0E4E69 |
| 8086:422c | 8086:1321 | Intel           | Centrino Advanced-N 6200 | 0.9%   | 4.1.15   | 2ED429A812 |
| 8086:4232 | 8086:1201 | Intel           | WiFi Link 5100           | 0.6%   | 3.10.34  | 6D1385653B |
| 8086:4232 | 8086:1301 | Intel           | WiFi Link 5100           | 0.5%   | 3.10.46  | 4ED6CCC4E4 |
| 8086:4237 | 8086:1311 | Intel           | PRO/Wireless 5100 AGN... | 3.7%   | 3.10.34  | 10708BAA81 |
| 8086:4238 | 8086:1111 | Intel           | Centrino Ultimate-N 6300 | 0.2%   | 3.10.34  | 4CAE7DC78D |
| 8086:4239 | 8086:1311 | Intel           | Centrino Advanced-N 6200 | 0.3%   | 3.0.28   | 5DD7A5FCE1 |
| 8086:7360 |           | Intel           | XMM7360 LTE Advanced ... | 100%   |          | 2B27DC30AC |
| 8086:7360 | 1028:5820 | Intel           | XMM7360 LTE Advanced ... | 100%   |          | 7448B10EFA |
| 8086:7360 | 103c:8337 | Intel           | XMM7360 LTE Advanced ... | 98.4%  | 5.3.18   | 50B75A0212 |
| 8086:7360 | 1cf8:8521 | Intel           | XMM7360 LTE Advanced ... | 100%   |          | A035BE3EA2 |
| 8086:7360 | 8086:0020 | Intel           | XMM7360 LTE Advanced ... | 98%    | 5.7.0    | C0EE92C218 |
| 8086:7560 | 103c:8507 | Intel           | Wireless controller      | 100%   |          | 11BBC16301 |
| 8086:7560 | 1cf8:8601 | Intel           | Wireless controller      | 100%   |          | 868DF33C64 |
| 8086:9df0 | 8086:0034 | Intel           | Cannon Point-LP CNVi ... | 0.3%   | 3.10.0   | 2928437EAC |
| 8086:9df0 | 8086:2034 | Intel           | Cannon Point-LP CNVi ... | 3.4%   | 4.18.0   | D60073EAD5 |
| 8086:9df0 | 8086:4030 | Intel           | Cannon Point-LP CNVi ... | 0.6%   | 4.15.0   | 241B649AD1 |
| 8086:9df0 | 8086:42a4 | Intel           | Cannon Point-LP CNVi ... | 1.7%   | 4.15.0   | 906A07309D |
| 8086:a370 | 1a56:1552 | Intel           | Cannon Lake PCH CNVi ... | 2.9%   | 4.18.0   | 7CB20A8170 |
| 8086:a370 | 8086:0030 | Intel           | Cannon Lake PCH CNVi ... | 1.2%   | 3.10.0   | FFDEE2C6E0 |
| 8086:a370 | 8086:0034 | Intel           | Cannon Lake PCH CNVi ... | 0.8%   | 3.10.0   | 9E4B82FB49 |
| 8086:a370 | 8086:02a4 | Intel           | Cannon Lake PCH CNVi ... | 0.9%   | 4.15.0   | 105C3ABAEB |

### Network (PCI)

68 out of 963 (7.06%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 0000:0002 | 002c:0000 |                 | Network controller       | 100%   |          | 3859A12973 |
| 0000:0210 | 002c:0000 |                 | Network controller       | 100%   |          | 3859A12973 |
| 0000:0210 | 1105:8300 |                 |                          | 100%   |          | 3859A12973 |
| 001c:0008 | 001c:0005 | PEAK-System ... | Network controller       | 100%   |          | B364724E53 |
| 03d0:2103 | 03d0:2103 |                 | Network controller       | 100%   |          | AD6A707B6C |
| 1006:3106 | 1086:1405 | Reply Group     | Reply Ethernet contro... | 100%   |          | F597A38FF5 |
| 1011:0009 | 1011:500a | Digital Equi... | DECchip 21140 [Faster... | 100%   |          | 7D749B3ECC |
| 1014:0201 | 002c:0002 | IBM             | Network controller       | 100%   |          | D2B25B94EF |
| 10b7:9055 | 10b7:9055 | 3Com            | 3c905B 100BaseTX [Cyc... | 2.6%   | 4.1.15   | 7B55587C5A |
| 10de:03ef | 1849:03ef | Nvidia          | MCP61 Ethernet           | 0.1%   | 3.14.15  | 5CA838575D |
| 10ec:8125 | 1043:87d7 | Realtek Semi... | RTL8125 2.5GbE Contro... | 10%    | 5.4.0    | 323C65CC17 |
| 10ec:8125 | 10ec:0123 | Realtek Semi... | RTL8125 2.5GbE Contro... | 4.3%   | 4.14.24  | C8A9642B81 |
| 10ec:8125 | 1458:e000 | Realtek Semi... | RTL8125 2.5GbE Contro... | 14%    | 4.19.0   | 48AB0D2ACD |
| 10ec:8125 | 1462:7c06 | Realtek Semi... | RTL8125 2.5GbE Contro... | 33.3%  | 5.8.0    | 8112942B50 |
| 10ec:8125 | 1462:7c35 | Realtek Semi... | RTL8125 2.5GbE Contro... | 6.8%   | 5.0.0    | DC7E369D45 |
| 10ec:8125 | 1462:7c75 | Realtek Semi... | RTL8125 2.5GbE Contro... | 28.6%  | 4.15.0   | 3C3D7B7AA1 |
| 10ec:8125 | 1462:7c79 | Realtek Semi... | RTL8125 2.5GbE Contro... | 33.3%  | 5.4.0    | D47B6C6CDB |
| 10ec:8125 | 1462:7c80 | Realtek Semi... | RTL8125 2.5GbE Contro... | 25%    | 5.4.0    | FFD532C8D8 |
| 10ec:8125 | 1462:7c82 | Realtek Semi... | RTL8125 2.5GbE Contro... | 12.5%  | 5.4.0    | F7341FD5B2 |
| 10ec:8125 | 1462:7c84 | Realtek Semi... | RTL8125 2.5GbE Contro... | 20.9%  | 5.4.0    | 6B7033F43D |
| 10ec:8125 | 1462:7c86 | Realtek Semi... | RTL8125 2.5GbE Contro... | 66.7%  | 5.4.0    | F43C35F402 |
| 10ec:8125 | 1462:7c91 | Realtek Semi... | RTL8125 2.5GbE Contro... | 6.8%   | 5.4.0    | 8ED70A9094 |
| 10ec:8125 | 1462:7c94 | Realtek Semi... | RTL8125 2.5GbE Contro... | 12.5%  | 4.18.0   | 1DA678C883 |
| 10ec:8125 | 1849:8125 | Realtek Semi... | RTL8125 2.5GbE Contro... | 7.4%   | 5.0.0    | 643C0A4F4D |
| 10ec:8125 | 1849:8168 | Realtek Semi... | RTL8125 2.5GbE Contro... | 4.3%   | 5.4.0    | 62201590BF |
| 10ee:2014 | 10ee:0009 | Xilinx          | Network controller       | 100%   |          | 8A2B6750B9 |
| 1106:1106 | 1186:1405 | VIA Technolo... | VT82C570MV               | 100%   |          | 5CA838575D |
| 1106:3065 | 1849:3065 | VIA Technolo... | VT6102/VT6103 [Rhine-II] | 5.1%   | 3.10.0   | 6FAC734286 |
| 1106:3102 | 1186:1401 | VIA Technolo... | VT8662 Host Bridge       | 100%   |          | EAD04A61E4 |
| 1106:3106 | 1106:0105 | VIA Technolo... | VT6105/VT6106S [Rhine... | 29.4%  | 4.1.16   | A6659EE127 |
| 1106:a409 | 1106:a409 | VIA Technolo... | VX855/VX875/VX900 Ser... | 100%   |          | 528A1449B7 |
| 1260:3886 | 16be:2004 | Intersil        | ISL3886 [Prism Javeli... | 20%    | 5.0.0    | ACACF55F1F |
| 12d0:2103 | 12d0:2103 | GDE Systems     | GDE Network controller   | 100%   |          | 8C5E6472B2 |
| 148c:002d | 148c:0301 | Tul Corporat... | Network controller       | 100%   |          | 15959C0828 |
| 14c3:7961 | 1a3b:4680 | MEDIATEK        | Network controller       | 100%   |          | 32546ECAA0 |
| 14e4:170c | 1028:01af | Broadcom        | BCM4401-B0 100Base-TX    | 2.3%   | 3.14.44  | A6BB0BFD0B |
| 14e4:170c | 1028:01f1 | Broadcom        | BCM4401-B0 100Base-TX    | 11.5%  | 3.14.53  | B5A30E2784 |
| 14e4:170c | 1028:01fc | Broadcom Lim... | BCM4401-B0 100Base-TX    | 10%    | 4.1.25   | 8C9EBDAF0F |
| 14e4:5fa0 | 106b:0870 | Broadcom        | Network controller       | 87.5%  | 5.4.0    | CB7AAC8083 |
| 14f3:2030 | 14f3:2001 | BroadLogic      | 2030 DVB-S Satellite ... | 100%   |          | 4648006D19 |
| 15b3:673c | 15b3:0036 | Mellanox Tec... | MT25408A0-FCC-QI Conn... | 100%   |          | CC8791AAA6 |
| 168c:0028 | 168c:2092 | Qualcomm Ath... | 11n AR9160 Anwi Diagn... | 100%   |          | 90E2E642CF |
| 168c:004a | 15aa:4035 | Qualcomm Ath... | Network controller       | 100%   |          | 04F6BB6978 |
| 168c:0063 | 168c:3071 | Qualcomm Ath... | Network controller       | 100%   |          | 8F99628F42 |
| 1810:3060 | 8001:0000 | HCL Technolo... | Network controller       | 100%   |          | CFD57C3B89 |
| 1923:0040 | a111:3913 | Sangoma Tech... | A200/Remora FXO/FXS A... | 100%   |          | 264F928670 |
| 19a2:0710 | 103c:3340 | Emulex          | OneConnect 10Gb NIC (... | 100%   |          | C40BB90F77 |
| 8086:0436 | 8086:0000 | Intel           | DH8900CC Null Device     | 100%   |          | 14C76E0C83 |
| 8086:10bd | 1019:2636 | Intel           | 82566DM-2 Gigabit Net... | 25%    | 5.4.0    | 6F1D219377 |
| 8086:10ca | 8086:a02c | Intel           | 82576 Virtual Function   | 100%   |          | 103A67B98A |
| 8086:10d3 | 8086:0000 | Intel           | 82574L Gigabit Networ... | 7%     | 2.6.32   | ADB076ED03 |
| 8086:10d3 | 8086:a01f | Intel           | 82574L Gigabit Networ... | 0.5%   | 3.10.0   | 9B75A42A1E |
| 8086:10de | 103c:3034 | Intel           | 82567LM-3 Gigabit Net... | 2.1%   | 3.14.44  | 5DC57BDE0C |
| 8086:10eb | 8086:0000 | Intel           | 82577LC Gigabit Netwo... | 88.9%  | 5.3.0    | CAB38C04CB |
| 8086:10f0 | 1019:1324 | Intel           | 82578DC Gigabit Netwo... | 50%    | 5.4.0    | 50B445BA68 |
| 8086:10f5 | 17aa:20ee | Intel           | 82567LM Gigabit Netwo... | 0.3%   | 3.10.0   | 349F58CAE3 |
| 8086:1502 | 1028:047e | Intel           | 82579LM Gigabit Netwo... | 0.6%   | 4.1.25   | 19795140C8 |
| 8086:1502 | 1028:0493 | Intel           | 82579LM Gigabit Netwo... | 1.3%   | 3.14.33  | 901B94B26D |
| 8086:1502 | 103c:179b | Intel           | 82579LM Gigabit Netwo... | 1.1%   | 3.14.44  | 18835A8B6C |
| 8086:1502 | 1043:849c | Intel           | 82579LM Gigabit Netwo... | 100%   |          | 44AA7CC920 |
| 8086:1503 | 8086:2017 | Intel           | 82579V Gigabit Networ... | 2%     | 2.6.32   | CF6242CACA |
| 8086:1531 | 8086:0000 | Intel           | I210 Gigabit Unprogra... | 80%    | 4.9.140  | F70E13FDBA |
| 8086:1533 | 1ab6:0214 | Intel           | I210 Gigabit Network ... | 5%     | 5.3.0    | 4312C9878E |
| 8086:1539 | 1043:85f0 | Intel           | I211 Gigabit Network ... | 0.2%   | 3.10.0   | 1F560968AB |
| 8086:1539 | 1458:e000 | Intel           | I211 Gigabit Network ... | 0.5%   | 4.9.0    | 60B6348B70 |
| 8086:1539 | 1849:1539 | Intel           | I211 Gigabit Network ... | 0.1%   | 3.10.0   | AC6DF0A8C0 |
| d161:8002 | d161:8002 | Digium          | Wildcard AEX800 8-por... | 100%   |          | FE3D758C20 |
| d161:8005 | d161:8005 | Digium          | Wildcard TDM410 4-por... | 100%   |          | 8C44DA7365 |

### Sd host controller (PCI)

121 out of 938 (12.90%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1022:7813 | 17aa:3801 | AMD             | FCH SD Flash Controller  | 0.4%   | 3.14.25  | EEFC7C92B2 |
| 104c:8034 | 103c:3085 | Texas Instru... | PCIxx21/PCIxx11 SD Ho... | 4.3%   | 4.19.66  | E643DE7D13 |
| 104c:803c | 17aa:207d | Texas Instru... | PCIxx12 SDA Standard ... | 11.1%  | 3.14.44  | E5C5CE1445 |
| 10ec:5209 | 103c:1659 | Realtek Semi... | RTS5209 PCI Express C... | 3.8%   | 4.1.15   | 119A35F980 |
| 1180:0822 | 1028:0263 | Ricoh           | R5C822 SD/SDIO/MMC/MS... | 2.6%   | 4.4.202  | 079101F502 |
| 1180:0822 | 103c:7008 | Ricoh           | R5C822 SD/SDIO/MMC/MS... | 1.3%   | 3.10.34  | 5DD7A5FCE1 |
| 1180:0822 | 1043:1827 | Ricoh           | R5C822 SD/SDIO/MMC/MS... | 33.3%  | 5.4.0    | 5B8E446BE1 |
| 1217:8221 | 1028:0493 | O2 Micro        | OZ600FJ0/OZ900FJ0/OZ6... | 0.4%   | 3.14.33  | F33530C32A |
| 1217:8321 | 1028:053e | O2 Micro        | OZ600RJ0/OZ900RJ0/OZ6... | 3.4%   | 4.9.124  | F674F91052 |
| 1217:8520 | 1028:05cb | O2 Micro        | SD/MMC Card Reader Co... | 0.9%   | 4.9.60   | 037A28C347 |
| 1217:8520 | 1028:05cd | O2 Micro        | SD/MMC Card Reader Co... | 5%     | 4.15.0   | 95FA029C09 |
| 1217:8520 | 1028:05e0 | O2 Micro        | SD/MMC Card Reader Co... | 1.9%   | 4.9.9    | 8EA71BA2AE |
| 1217:8520 | 1217:0002 | O2 Micro        | SD/MMC Card Reader Co... | 100%   |          | D125ABF69E |
| 1217:8621 | 17aa:3824 | O2 Micro        | SD/MMC Card Reader Co... | 1.8%   | 4.15.0   | 80F496EACD |
| 1217:8621 | 17aa:507e | O2 Micro        | SD/MMC Card Reader Co... | 6.9%   | 5.4.0    | 418D6EE98E |
| 1217:8621 | 8086:2064 | O2 Micro        | SD/MMC Card Reader Co... | 3.2%   | 3.10.0   | 4D423F3865 |
| 14e4:16bc | 1025:0647 | Broadcom        | BCM57765/57785 SDXC/M... | 0.1%   | 3.10.34  | 86D2D3B0E1 |
| 14e4:16bc | 1025:0775 | Broadcom        | BCM57765/57785 SDXC/M... | 0.4%   | 3.14.22  | 81B19839F7 |
| 14e4:16bc | 14e4:96bc | Broadcom Lim... | BCM57765/57785 SDXC/M... | 1.3%   | 4.1.34   | 2961E0C973 |
| 17a0:9750 | 17aa:2279 | Genesys Logic   | GL9750 SD Host Contro... | 3.9%   | 3.10.0   | B6F9682F0B |
| 17a0:9750 | 17aa:2286 | Genesys Logic   | GL9750 SD Host Contro... | 3.6%   | 4.18.0   | D4FA985843 |
| 197b:2381 | 1025:013d | JMicron Tech... | Standard SD Host Cont... | 16.7%  | 4.15.0   | DB999A95A6 |
| 197b:2381 | 1025:0140 | JMicron Tech... | Standard SD Host Cont... | 14.3%  | 5.3.0    | C85107D1C1 |
| 197b:2381 | 1025:0142 | JMicron Tech... | Standard SD Host Cont... | 11.8%  | 4.1.25   | 6780FC2A44 |
| 197b:2381 | 1025:0145 | JMicron Tech... | Standard SD Host Cont... | 36.4%  | 4.1.15   | 3C60271275 |
| 197b:2381 | 1025:015b | JMicron Tech... | Standard SD Host Cont... | 7.1%   | 3.14.44  | F88D38A138 |
| 197b:2381 | 1025:022c | JMicron Tech... | Standard SD Host Cont... | 16.7%  | 3.14.44  | 20A691C8E3 |
| 197b:2381 | 1025:0260 | JMicron Tech... | Standard SD Host Cont... | 10%    | 4.15.0   | ABC5736623 |
| 197b:2381 | 1025:0275 | JMicron Tech... | Standard SD Host Cont... | 53.8%  | 4.15.0   | 09734ADC68 |
| 197b:2381 | 103c:2a97 | JMicron Tech... | Standard SD Host Cont... | 50%    | 5.8.0    | F2DC6038F3 |
| 197b:2381 | 103c:2aa2 | JMicron Tech... | Standard SD Host Cont... | 36.4%  | 4.1.15   | 3D5AB5199F |
| 197b:2381 | 103c:30f4 | JMicron Tech... | Standard SD Host Cont... | 38.5%  | 3.14.53  | 17B1DC07BF |
| 197b:2381 | 103c:30f7 | JMicron Tech... | Standard SD Host Cont... | 24.4%  | 4.1.25   | E15FD6726E |
| 197b:2381 | 103c:30fb | JMicron Tech... | Standard SD Host Cont... | 4.5%   | 3.14.44  | 229CCDA963 |
| 197b:2381 | 103c:30fc | JMicron Tech... | Standard SD Host Cont... | 35.7%  | 4.18.0   | 1CAAC71B77 |
| 197b:2381 | 103c:30fe | JMicron Tech... | Standard SD Host Cont... | 50%    | 5.3.0    | F2648EDD87 |
| 197b:2381 | 103c:3600 | JMicron Tech... | Standard SD Host Cont... | 7.1%   | 4.1.25   | CD2EF33093 |
| 197b:2381 | 103c:3603 | JMicron Tech... | Standard SD Host Cont... | 15.9%  | 3.14.44  | 5BB8EF6423 |
| 197b:2381 | 103c:3610 | JMicron Tech... | Standard SD Host Cont... | 27.3%  | 4.15.0   | 47374D1B5F |
| 197b:2381 | 103c:361b | JMicron Tech... | Standard SD Host Cont... | 40%    | 4.15.0   | C3E0C828A1 |
| 197b:2381 | 103c:3624 | JMicron Tech... | Standard SD Host Cont... | 5.9%   | 4.1.16   | CDF6CCEAA1 |
| 197b:2381 | 103c:3628 | JMicron Tech... | Standard SD Host Cont... | 19.7%  | 3.14.44  | 8B9CD8BAC1 |
| 197b:2381 | 103c:363c | JMicron Tech... | Standard SD Host Cont... | 66.7%  | 5.6.7    | 662A781C83 |
| 197b:2381 | 103c:3659 | JMicron Tech... | Standard SD Host Cont... | 7.9%   | 3.14.53  | 827D185513 |
| 197b:2381 | 103c:365c | JMicron Tech... | Standard SD Host Cont... | 37.5%  | 5.3.0    | 727672085E |
| 197b:2381 | 103c:7001 | JMicron Tech... | Standard SD Host Cont... | 15%    | 3.0.28   | 298015ECAC |
| 197b:2381 | 1043:1a07 | JMicron Tech... | Standard SD Host Cont... | 7.9%   | 3.10.34  | 8D83CA7912 |
| 197b:2381 | 1043:84af | JMicron Tech... | Standard SD Host Cont... | 100%   |          | DF82BB0E17 |
| 197b:2381 | 1071:9525 | JMicron Tech... | Standard SD Host Cont... | 60%    | 5.3.0    | EC12AF8F5D |
| 197b:2381 | 1179:fd30 | JMicron Tech... | Standard SD Host Cont... | 43.4%  | 3.14.33  | 23143AD7AE |
| 197b:2381 | 1179:ff02 | JMicron Tech... | Standard SD Host Cont... | 4.5%   | 4.1.15   | 0F1EC4CE4E |
| 197b:2381 | 1297:2000 | JMicron Tech... | Standard SD Host Cont... | 27.6%  | 4.4.0    | A82B81CD57 |
| 197b:2381 | 1297:2001 | JMicron Tech... | Standard SD Host Cont... | 20%    | 4.15.0   | 537B80CF25 |
| 197b:2381 | 1297:2008 | JMicron Tech... | Standard SD Host Cont... | 50%    | 5.4.0    | 8F6ED609DD |
| 197b:2381 | 1297:2012 | JMicron Tech... | Standard SD Host Cont... | 33.3%  | 5.0.0    | 126E42AA03 |
| 197b:2381 | 1297:2020 | JMicron Tech... | Standard SD Host Cont... | 21.4%  | 4.15.0   | DFE23BF8AF |
| 197b:2381 | 1297:2023 | JMicron Tech... | Standard SD Host Cont... | 14.3%  | 4.15.0   | C9ACF37E3D |
| 197b:2381 | 1297:2027 | JMicron Tech... | Standard SD Host Cont... | 53.1%  | 4.15.0   | E396067726 |
| 197b:2381 | 1297:2028 | JMicron Tech... | Standard SD Host Cont... | 22.2%  | 4.9.0    | 941A82D659 |
| 197b:2381 | 14c0:0031 | JMicron Tech... | Standard SD Host Cont... | 100%   |          | 56B05900A0 |
| 197b:2381 | 14c0:003e | JMicron Tech... | Standard SD Host Cont... | 50%    | 5.0.0    | E702E7ABAC |
| 197b:2381 | 1558:0801 | JMicron Tech... | Standard SD Host Cont... | 29.6%  | 4.9.20   | 93B0E6EBE1 |
| 197b:2381 | 1558:0803 | JMicron Tech... | Standard SD Host Cont... | 21.7%  | 4.15.0   | 0E33922AF7 |
| 197b:2381 | 1558:1110 | JMicron Tech... | Standard SD Host Cont... | 33.3%  | 4.1.15   | C545781337 |
| 197b:2381 | 1558:4120 | JMicron Tech... | Standard SD Host Cont... | 58.3%  | 4.20.17  | 307FCF8F37 |
| 197b:2381 | 1558:7465 | JMicron Tech... | Standard SD Host Cont... | 35.7%  | 4.9.20   | 72F9AD676B |
| 197b:2381 | 1734:113f | JMicron Tech... | Standard SD Host Cont... | 13.6%  | 4.15.0   | E6848FB30E |
| 197b:2381 | 17aa:212d | JMicron Tech... | Standard SD Host Cont... | 19.4%  | 3.14.44  | 66346C1594 |
| 197b:2381 | 17aa:3602 | JMicron Tech... | Standard SD Host Cont... | 25%    | 3.14.44  | C25FDFE643 |
| 197b:2381 | 17aa:387f | JMicron Tech... | Standard SD Host Cont... | 15.4%  | 3.14.25  | A5EC379304 |
| 197b:2381 | 17aa:3d9a | JMicron Tech... | Standard SD Host Cont... | 15.4%  | 4.1.3    | 34E6D98329 |
| 197b:2391 | 1028:0446 | JMicron Tech... | Standard SD Host Cont... | 33.3%  | 4.15.0   | 5BCD793D64 |
| 197b:2391 | 1028:050e | JMicron Tech... | Standard SD Host Cont... | 80%    | 5.4.0    | 0FEA972B34 |
| 197b:2391 | 103c:1618 | JMicron Tech... | Standard SD Host Cont... | 11.7%  | 4.1.15   | 231E31E9F0 |
| 197b:2391 | 103c:1619 | JMicron Tech... | Standard SD Host Cont... | 8.3%   | 3.10.0   | 21DFC28BFC |
| 197b:2391 | 103c:161c | JMicron Tech... | Standard SD Host Cont... | 27.2%  | 4.1.15   | 6F3D7A9D3F |
| 197b:2391 | 103c:161d | JMicron Tech... | Standard SD Host Cont... | 32.7%  | 4.15.0   | 939B480C49 |
| 197b:2391 | 103c:1620 | JMicron Tech... | Standard SD Host Cont... | 83.3%  | 5.4.0    | DF179D59AF |
| 197b:2391 | 103c:1621 | JMicron Tech... | Standard SD Host Cont... | 53.3%  | 4.4.0    | 877E10CCD2 |
| 197b:2391 | 103c:162a | JMicron Tech... | Standard SD Host Cont... | 36.7%  | 4.15.0   | 16A9F3CDE3 |
| 197b:2391 | 103c:162b | JMicron Tech... | Standard SD Host Cont... | 5.3%   | 3.14.44  | ECDECF72EC |
| 197b:2391 | 103c:1630 | JMicron Tech... | Standard SD Host Cont... | 19%    | 4.9.155  | 654AD66096 |
| 197b:2391 | 103c:1631 | JMicron Tech... | Standard SD Host Cont... | 20.6%  | 4.1.19   | ADA2C0663B |
| 197b:2391 | 103c:1633 | JMicron Tech... | Standard SD Host Cont... | 18.2%  | 3.10.42  | 7B4814EAA8 |
| 197b:2391 | 103c:1635 | JMicron Tech... | Standard SD Host Cont... | 83.3%  | 5.3.0    | 517E898344 |
| 197b:2391 | 103c:164f | JMicron Tech... | Standard SD Host Cont... | 8.3%   | 4.15.0   | 4A66A57A41 |
| 197b:2391 | 103c:167c | JMicron Tech... | Standard SD Host Cont... | 9.6%   | 4.1.4    | 5FF33D4354 |
| 197b:2391 | 103c:167e | JMicron Tech... | Standard SD Host Cont... | 41%    | 3.14.44  | 16CFC17219 |
| 197b:2391 | 103c:168b | JMicron Tech... | Standard SD Host Cont... | 23.8%  | 3.14.44  | E6AC959C5E |
| 197b:2391 | 103c:176b | JMicron Tech... | Standard SD Host Cont... | 6.1%   | 4.9.76   | BD697A03F8 |
| 197b:2391 | 103c:176c | JMicron Tech... | Standard SD Host Cont... | 50%    | 4.15.0   | 9B49622881 |
| 197b:2391 | 103c:179b | JMicron Tech... | Standard SD Host Cont... | 21.4%  | 3.14.44  | 40D2D85153 |
| 197b:2391 | 103c:179c | JMicron Tech... | Standard SD Host Cont... | 6.5%   | 4.9.20   | 18F5FAB938 |
| 197b:2391 | 103c:17a7 | JMicron Tech... | Standard SD Host Cont... | 26.8%  | 3.14.44  | B7A001665E |
| 197b:2391 | 103c:17ab | JMicron Tech... | Standard SD Host Cont... | 17.6%  | 4.1.25   | 7621EB165A |
| 197b:2391 | 103c:17df | JMicron Tech... | Standard SD Host Cont... | 12.1%  | 4.1.25   | 3BF2664982 |
| 197b:2391 | 103c:17ed | JMicron Tech... | Standard SD Host Cont... | 27.3%  | 3.14.44  | 6AE3EB396F |
| 197b:2391 | 103c:17f3 | JMicron Tech... | Standard SD Host Cont... | 33.3%  | 4.9.193  | 8E6C01F203 |
| 197b:2391 | 103c:17f6 | JMicron Tech... | Standard SD Host Cont... | 16.5%  | 3.14.39  | 3EEBEDC4C6 |
| 197b:2391 | 103c:180f | JMicron Tech... | Standard SD Host Cont... | 10%    | 4.4.195  | 06DA2207CD |
| 197b:2391 | 103c:1815 | JMicron Tech... | Standard SD Host Cont... | 55.6%  | 4.15.0   | 6E4A5F9C76 |
| 197b:2391 | 103c:18df | JMicron Tech... | Standard SD Host Cont... | 19.2%  | 3.14.44  | B9CFAAC7A6 |
| 197b:2391 | 103c:18f8 | JMicron Tech... | Standard SD Host Cont... | 40%    | 4.18.0   | B6B29C8237 |
| 197b:2391 | 103c:2af2 | JMicron Tech... | Standard SD Host Cont... | 100%   |          | F94C9AF809 |
| 197b:2391 | 103c:3561 | JMicron Tech... | Standard SD Host Cont... | 100%   |          | 90E0F93E8D |
| 197b:2391 | 103c:3596 | JMicron Tech... | Standard SD Host Cont... | 100%   |          | 265CDC3301 |
| 197b:2391 | 1179:fc30 | JMicron Tech... | Standard SD Host Cont... | 21.7%  | 4.15.0   | 65DB006D0A |
| 197b:2391 | 1462:107f | JMicron Tech... | Standard SD Host Cont... | 80%    | 3.14.44  | 7EBAF712E3 |
| 197b:2391 | 14c0:006b | JMicron Tech... | Standard SD Host Cont... | 100%   |          | C97368216B |
| 197b:2391 | 1558:1500 | JMicron Tech... | Standard SD Host Cont... | 18.2%  | 4.9.20   | 504B81E5A0 |
| 197b:2391 | 1558:2100 | JMicron Tech... | Standard SD Host Cont... | 6.2%   | 3.14.39  | CA8ECE28F8 |
| 197b:2391 | 1558:2431 | JMicron Tech... | Standard SD Host Cont... | 100%   |          | F395EB44CF |
| 197b:2391 | 1558:2432 | JMicron Tech... | Standard SD Host Cont... | 100%   |          | 16EFC2E75F |
| 197b:2391 | 1558:2450 | JMicron Tech... | Standard SD Host Cont... | 100%   |          | 450ED4C040 |
| 197b:2391 | 1558:2700 | JMicron Tech... | Standard SD Host Cont... | 85.7%  | 4.15.0   | 1A3040469A |
| 197b:2391 | 1558:3500 | JMicron Tech... | Standard SD Host Cont... | 16.7%  | 4.15.0   | 7434BE9250 |
| 197b:2391 | 1558:4140 | JMicron Tech... | Standard SD Host Cont... | 6.2%   | 4.4.0    | EAEB27C7F2 |
| 197b:2391 | 1558:4510 | JMicron Tech... | Standard SD Host Cont... | 25%    | 4.15.0   | 7886F96B81 |
| 197b:2391 | 1558:5102 | JMicron Tech... | Standard SD Host Cont... | 16.7%  | 4.9.20   | AD5FC91174 |
| 197b:2391 | 17aa:3976 | JMicron Tech... | Standard SD Host Cont... | 13.8%  | 3.14.44  | 94D22E7673 |
| 197b:2391 | 17aa:3977 | JMicron Tech... | Standard SD Host Cont... | 41.7%  | 4.1.34   | F088672FD6 |

### Sound (PCI)

463 out of 14759 (3.14%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 0045:c061 | 0045:c061 |                 | Audio device             | 100%   |          | 8D884B92FA |
| 1002:1308 | 1025:0864 | AMD             | Kaveri HDMI/DP Audio ... | 2.8%   | 3.14.44  | 8D6D195DA2 |
| 1002:1314 | 1025:0520 | AMD             | Wrestler HDMI Audio      | 1.6%   | 3.14.44  | BF118AA31C |
| 1002:1314 | 103c:188b | AMD             | Wrestler HDMI Audio      | 1.1%   | 4.1.15   | 48946EFC8F |
| 1002:1314 | 1043:84e7 | AMD             | Wrestler HDMI Audio      | 11.1%  | 4.15.0   | 58F57667EE |
| 1002:15b3 | 103c:84ac | AMD             | High Definition Audio... | 0.7%   | 4.15.0   | 4F1105BCA0 |
| 1002:15b3 | 103c:84e5 | AMD             | High Definition Audio... | 33.3%  | 4.15.0   | 9087960124 |
| 1002:15de | 1043:876b | AMD             | Raven/Raven2/Fenghuan... | 0.3%   | 4.4.0    | 6AF7F81CA3 |
| 1002:1637 | 1043:16cf | AMD             | Renoir Radeon High De... | 2.4%   | 4.18.16  | 3A1B31970C |
| 1002:1637 | 17aa:5082 | AMD             | Renoir Radeon High De... | 2.3%   | 5.4.0    | DE9EA1422C |
| 1002:4383 | 1025:0520 | AMD             | SBx00 Azalia (Intel HDA) | 1.6%   | 3.14.44  | BF118AA31C |
| 1002:4383 | 1043:836c | AMD             | SBx00 Azalia (Intel HDA) | 0.9%   | 3.10.0   | 189BABB8BE |
| 1002:4383 | 1043:8444 | AMD             | SBx00 Azalia (Intel HDA) | 1.4%   | 3.14.33  | 8388FBE3B4 |
| 1002:4383 | 1043:8445 | AMD             | SBx00 Azalia (Intel HDA) | 0.1%   | 3.10.0   | 8A4E34A210 |
| 1002:4383 | 1043:84fb | AMD             | SBx00 Azalia (Intel HDA) | 0.3%   | 3.14.44  | D3AEFE0601 |
| 1002:4383 | 1043:8576 | AMD             | SBx00 Azalia (Intel HDA) | 0.4%   | 3.10.0   | 35D0F345A4 |
| 1002:4383 | 1458:a182 | AMD             | SBx00 Azalia (Intel HDA) | 0.2%   | 3.10.0   | C3443E0857 |
| 1002:4383 | 1462:d693 | AMD             | SBx00 Azalia (Intel HDA) | 0.4%   | 3.14.15  | F71DD78128 |
| 1002:960f | 1002:960f | AMD             | RS780 HDMI Audio [Rad... | 0.5%   | 3.10.0   | C3443E0857 |
| 1002:970f | 1458:960f | AMD             | RS880 HDMI Audio [Rad... | 1.1%   | 3.14.44  | 911703286C |
| 1002:9840 | 1025:0800 | AMD             | Kabini HDMI/DP Audio     | 8.1%   | 3.14.53  | 370BD439D7 |
| 1002:9840 | 103c:8245 | AMD             | Kabini HDMI/DP Audio     | 6.2%   | 4.9.20   | B348BC9186 |
| 1002:9840 | 17aa:2219 | AMD             | Kabini HDMI/DP Audio     | 2.4%   | 4.9.60   | 94058A82CA |
| 1002:9840 | 17aa:3801 | AMD             | Kabini HDMI/DP Audio     | 0.4%   | 3.14.25  | EEFC7C92B2 |
| 1002:9902 | 103c:1992 | AMD             | Trinity HDMI Audio Co... | 4.2%   | 4.1.25   | 2C52151F77 |
| 1002:9902 | 1462:7721 | AMD             | Trinity HDMI Audio Co... | 1.6%   | 3.14.44  | 4587AB8EDD |
| 1002:aa08 | 1043:aa08 | AMD             | RV630 HDMI Audio [Rad... | 5%     | 4.1.15   | D2E947F1AD |
| 1002:aa18 | 1787:aa18 | AMD             | RV670/680 HDMI Audio ... | 16.7%  | 3.14.44  | 26D33EB0DE |
| 1002:aa28 | 1043:aa28 | AMD             | RV620 HDMI Audio [Rad... | 1.9%   | 3.14.44  | 119AD3E83D |
| 1002:aa30 | 1682:aa30 | AMD             | RV770 HDMI Audio [Rad... | 14.3%  | 4.9.9    | 335083A19F |
| 1002:aa38 | 1002:aa38 | AMD             | RV710/730 HDMI Audio ... | 2.2%   | 3.14.25  | 6D1385653B |
| 1002:aa38 | 1043:aa38 | AMD             | RV710/730 HDMI Audio ... | 0.7%   | 3.13.0   | 3A2604A18A |
| 1002:aa38 | 1462:aa38 | AMD             | RV710/730 HDMI Audio ... | 1.3%   | 3.10.0   | 51837DE98F |
| 1002:aa38 | 174b:aa38 | AMD             | RV710/730 HDMI Audio ... | 1.8%   | 3.14.25  | B701C37D96 |
| 1002:aa50 | 1002:aa50 | AMD             | Cypress HDMI Audio [R... | 1.6%   | 4.1.15   | C6C1C28B2D |
| 1002:aa58 | 1787:aa58 | AMD             | Juniper HDMI Audio [R... | 0.8%   | 3.14.25  | C8888818C9 |
| 1002:aa68 | 1025:0487 | AMD             | Cedar HDMI Audio [Rad... | 2.5%   | 3.14.44  | 68F61986F8 |
| 1002:aa68 | 1545:aa68 | AMD             | Cedar HDMI Audio [Rad... | 10%    | 4.15.0   | 51D516FF60 |
| 1002:aa90 | 1179:fb41 | AMD             | Turks HDMI Audio [Rad... | 4.5%   | 3.14.44  | 67009EFFAA |
| 1002:aa98 | 103c:161e | AMD             | Caicos HDMI Audio [Ra... | 4.4%   | 4.1.15   | 71029063A4 |
| 1002:aa98 | 1043:aa98 | AMD             | Caicos HDMI Audio [Ra... | 0.8%   | 3.0.38   | 2A34C16AB3 |
| 1002:aa98 | 174b:aa98 | AMD             | Caicos HDMI Audio [Ra... | 0.5%   | 3.14.22  | 24BF705591 |
| 1002:aab0 | 1028:aab0 | AMD             | Oland/Hainan/Cape Ver... | 0.8%   | 4.3.0    | 0C434691D6 |
| 1002:aab0 | 103c:1990 | AMD             | Oland/Hainan/Cape Ver... | 4%     | 4.18.0   | DCE9CDAF8E |
| 1002:aab0 | 1043:aab0 | AMD             | Oland/Hainan/Cape Ver... | 0.5%   | 3.14.22  | 66219C1D36 |
| 1002:aab0 | 1682:aab0 | AMD             | Oland/Hainan/Cape Ver... | 1%     | 3.14.22  | 189BABB8BE |
| 1002:aab0 | 174b:aab0 | AMD             | Oland/Hainan/Cape Ver... | 0.1%   | 3.13.0   | 9B9C670167 |
| 1002:aac0 | 103c:aac0 | AMD             | Tobago HDMI Audio [Ra... | 33.3%  | 4.15.0   | B9EB4A5652 |
| 1002:aac0 | 1458:aac0 | AMD             | Tobago HDMI Audio [Ra... | 1.7%   | 3.14.44  | 62E0E97099 |
| 1002:aae0 | 1043:aae0 | AMD             | Baffin HDMI/DP Audio ... | 0.5%   | 4.1.25   | 9D3FE31D76 |
| 1002:aae0 | 1682:aae0 | AMD             | Baffin HDMI/DP Audio ... | 0.6%   | 4.9.60   | 8212CC8601 |
| 1002:aaf0 | 1462:aaf0 | AMD             | Ellesmere HDMI Audio ... | 0.4%   | 3.10.0   | 761ECD0A1C |
| 1002:aaf0 | 148c:aaf0 | AMD             | Ellesmere HDMI Audio ... | 0.5%   | 4.10.16  | F61EE20F03 |
| 1002:aaf0 | 1682:aaf0 | AMD             | Ellesmere HDMI Audio ... | 0.7%   | 4.13.0   | 3A69ABB947 |
| 1002:aaf0 | 1da2:aaf0 | AMD             | Ellesmere HDMI Audio ... | 0.3%   | 4.8.0    | 94B280C39D |
| 1002:ab28 | 1002:ab28 | AMD             | Navi 21 HDMI Audio [R... | 2%     | 5.4.0    | 9FA9842EC9 |
| 1002:ab38 | 1002:ab38 | AMD             | Navi 10 HDMI Audio       | 0.3%   | 4.9.0    | A011C9B38F |
| 1002:ab38 | 1462:12b5 | AMD             | Navi 10 HDMI Audio       | 9.1%   | 5.4.0    | 08ED0821EF |
| 1013:6003 |           | Cirrus Logic    | CS 4614/22/24/30 [Cry... | 3.7%   | 4.4.0    | 169428CB9E |
| 1022:1457 | 1043:86c7 | AMD             | Family 17h (Models 00... | 0.2%   | 3.10.0   | F1C95A10CC |
| 1022:1457 | 1043:8733 | AMD             | Family 17h (Models 00... | 0.4%   | 4.9.0    | BF6FD8E5AC |
| 1022:1457 | 1043:8735 | AMD             | Family 17h (Models 00... | 1.1%   | 4.9.60   | FC3F785613 |
| 1022:1457 | 1462:9b84 | AMD             | Family 17h (Models 00... | 4.3%   | 4.15.0   | A011A6EF0E |
| 1022:1457 | 1462:cb09 | AMD             | Family 17h (Models 00... | 28.6%  | 4.15.0   | 3B92D6CC85 |
| 1022:1457 | 1462:cb79 | AMD             | Family 17h (Models 00... | 1.3%   | 4.9.60   | C818EB5CB4 |
| 1022:1457 | 1462:fa39 | AMD             | Family 17h (Models 00... | 2.6%   | 4.9.0    | 84ED791AF7 |
| 1022:1457 | 1849:2220 | AMD             | Family 17h (Models 00... | 1.9%   | 4.18.0   | 707960B3EC |
| 1022:1487 | 1022:c950 | AMD             | Starship/Matisse HD A... | 25%    | 5.6.4    | 09640A1376 |
| 1022:1487 | 1043:874f | AMD             | Starship/Matisse HD A... | 29.7%  | 5.4.0    | 1F560968AB |
| 1022:1487 | 1043:8797 | AMD             | Starship/Matisse HD A... | 0.4%   | 4.15.0   | 82A9A037CB |
| 1022:1487 | 1043:87c5 | AMD             | Starship/Matisse HD A... | 0.6%   | 4.18.0   | B1F5EAC9A6 |
| 1022:1487 | 1458:a0c3 | AMD             | Starship/Matisse HD A... | 1.3%   | 4.15.0   | 4080E1B43F |
| 1022:1487 | 1458:a0cd | AMD             | Starship/Matisse HD A... | 1.4%   | 4.20.16  | 97217688BF |
| 1022:1487 | 1458:a0cf | AMD             | Starship/Matisse HD A... | 2%     | 5.3.0    | 57B918A36E |
| 1022:1487 | 1458:a182 | AMD             | Starship/Matisse HD A... | 0.7%   | 3.10.0   | 62A8A899ED |
| 1022:1487 | 1462:9c37 | AMD             | Starship/Matisse HD A... | 1.7%   | 4.15.0   | 07BD3ED250 |
| 1022:1487 | 1462:cb60 | AMD             | Starship/Matisse HD A... | 25%    | 5.4.0    | 4748E04A66 |
| 1022:1487 | 1462:cb86 | AMD             | Starship/Matisse HD A... | 2.7%   | 4.15.0   | 761ECD0A1C |
| 1022:1487 | 1462:cb93 | AMD             | Starship/Matisse HD A... | 2.9%   | 4.15.0   | D88BFB96F9 |
| 1022:1487 | 1849:2221 | AMD             | Starship/Matisse HD A... | 2.8%   | 4.18.16  | DA311C1D96 |
| 1022:1487 | 1849:6893 | AMD             | Starship/Matisse HD A... | 1.1%   | 4.19.0   | D13F15D786 |
| 1022:1487 | 1849:d887 | AMD             | Starship/Matisse HD A... | 4%     | 4.15.0   | F61EE20F03 |
| 1022:157a | 103c:84ac | AMD             | Family 15h (Models 60... | 0.8%   | 4.15.0   | 4F1105BCA0 |
| 1022:157a | 103c:84e5 | AMD             | Family 15h (Models 60... | 33.3%  | 4.15.0   | 9087960124 |
| 1022:15e3 | 103c:87b1 | AMD             | Family 17h (Models 10... | 4.2%   | 5.7.8    | 2C929E66BC |
| 1022:15e3 | 1043:1e21 | AMD             | Family 17h (Models 10... | 1.2%   | 4.18.16  | 3A1B31970C |
| 1022:15e3 | 1043:86c7 | AMD             | Family 17h (Models 10... | 0.3%   | 4.4.0    | 6AF7F81CA3 |
| 1022:15e3 | 1462:12b5 | AMD             | Family 17h (Models 10... | 9.1%   | 5.4.0    | 08ED0821EF |
| 1022:15e3 | 17aa:5082 | AMD             | Family 17h (Models 10... | 2.3%   | 5.4.0    | DE9EA1422C |
| 1022:2093 | 1022:2093 | AMD             | CS5536 [Geode compani... | 100%   |          | 6D9551F87E |
| 1022:780d | 1025:0800 | AMD             | FCH Azalia Controller    | 7%     | 3.14.53  | 370BD439D7 |
| 1022:780d | 1025:0864 | AMD             | FCH Azalia Controller    | 2.8%   | 3.14.44  | 8D6D195DA2 |
| 1022:780d | 103c:1992 | AMD             | FCH Azalia Controller    | 4.2%   | 4.1.25   | 2C52151F77 |
| 1022:780d | 103c:8245 | AMD             | FCH Azalia Controller    | 6.2%   | 4.9.20   | B348BC9186 |
| 1022:780d | 1043:8576 | AMD             | FCH Azalia Controller    | 0.2%   | 3.14.25  | 7E0AF76200 |
| 1022:780d | 1043:85cd | AMD             | FCH Azalia Controller    | 3.1%   | 3.14.44  | CDC3F83CDB |
| 1022:780d | 1043:86c7 | AMD             | FCH Azalia Controller    | 12.5%  | 4.9.14   | 71ABA86389 |
| 1022:780d | 1462:d721 | AMD             | FCH Azalia Controller    | 0.4%   | 3.14.33  | 4587AB8EDD |
| 1022:780d | 17aa:3801 | AMD             | FCH Azalia Controller    | 0.4%   | 3.14.25  | EEFC7C92B2 |
| 1039:7502 | 1043:1783 | Silicon Inte... | Azalia Audio Controller  | 1.7%   | 4.1.34   | A13580724B |
| 106b:1803 | 106b:1803 | Apple           | Audio Device             | 100%   |          | 43CB3AF3A5 |
| 106b:1803 | 106b:1880 | Apple           | Audio Device             | 83.3%  | 5.6.19   | 935B673683 |
| 106b:1803 | 106b:1881 | Apple           | Audio Device             | 97.9%  | 5.8.0    | 9D73FAB087 |
| 106b:1803 | 106b:1884 | Apple           | Audio Device             | 100%   |          | D09823163E |
| 106b:1803 | 106b:1885 | Apple           | Audio Device             | 100%   |          | 2352614158 |
| 106b:1803 | 106b:1887 | Apple           | Audio Device             | 16.7%  | 5.4.0    | C3D1F2F1E7 |
| 106b:1803 | 106b:1888 | Apple           | Audio Device             | 100%   |          | CB7AAC8083 |
| 106b:1803 | 106b:1889 | Apple           | Audio Device             | 83.3%  | 5.7.0    | E3790FD911 |
| 106b:1803 | 106b:188b | Apple           | Audio Device             | 100%   |          | 0E4DAA1DE2 |
| 106b:1803 | 106b:188c | Apple           | Audio Device             | 100%   |          | EC2AF584B3 |
| 1073:0010 | 1073:0010 | Yamaha          | YMF-744B [DS-1S Audio... | 20%    | 4.9.9    | D2E947F1AD |
| 1073:1000 | 1073:1000 | Yamaha          | SW1000XG [XG Factory]    | 100%   |          | 4DCC71B299 |
| 10de:0059 | 1043:81ae | Nvidia          | CK804 AC'97 Audio Con... | 50%    | 3.14.25  | A6659EE127 |
| 10de:006b | 1043:0c11 | Nvidia          | nForce Audio Processi... | 100%   |          | 543960170E |
| 10de:006b | 147b:1c00 | Nvidia          | nForce Audio Processi... | 100%   |          | CB892B4614 |
| 10de:03f0 | 103c:2a6c | Nvidia          | MCP61 High Definition... | 1.5%   | 4.1.15   | 52991F9A5A |
| 10de:03f0 | 1458:a002 | Nvidia          | MCP61 High Definition... | 0.9%   | 3.14.15  | 119AD3E83D |
| 10de:03f0 | 1849:0397 | Nvidia          | MCP61 High Definition... | 0.2%   | 3.14.15  | C8888818C9 |
| 10de:03f0 | 1849:0888 | Nvidia          | MCP61 High Definition... | 17.4%  | 3.14.53  | B701C37D96 |
| 10de:0774 | 1043:836c | Nvidia          | MCP72XE/MCP72P/MCP78U... | 4%     | 3.10.19  | E1B7D175A1 |
| 10de:0774 | 1462:7578 | Nvidia          | MCP72XE/MCP72P/MCP78U... | 14.3%  | 4.9.20   | 8F804041A2 |
| 10de:0ac0 | 103c:2aa1 | Nvidia          | MCP79 High Definition... | 50%    | 4.18.0   | C2FD4F3C01 |
| 10de:0be2 | 174b:2160 | Nvidia          | GT216 HDMI Audio Cont... | 4.8%   | 4.15.0   | 60F738965A |
| 10de:0be3 | 103c:0862 | Nvidia          | High Definition Audio... | 5.6%   | 4.4.0    | 4B1F2221EE |
| 10de:0be3 | 1043:8354 | Nvidia          | High Definition Audio... | 0.9%   | 3.14.44  | 67BFE1B221 |
| 10de:0be3 | 1043:8490 | Nvidia          | High Definition Audio... | 15.2%  | 4.1.38   | A6659EE127 |
| 10de:0be3 | 10de:0862 | Nvidia          | High Definition Audio... | 10%    | 4.9.0    | F47CB1587E |
| 10de:0be3 | 1462:8094 | Nvidia          | High Definition Audio... | 0.6%   | 3.14.44  | 895D8612B4 |
| 10de:0be3 | 3842:1215 | Nvidia          | High Definition Audio... | 66.7%  | 5.3.0    | 08F4C825CC |
| 10de:0be3 | 3842:1310 | Nvidia          | High Definition Audio... | 62.5%  | 4.9.124  | 8388FBE3B4 |
| 10de:0be5 | 19da:1153 | Nvidia          | GF100 High Definition... | 25%    | 4.1.15   | FD37A435F8 |
| 10de:0be9 | 10de:084a | Nvidia          | GF106 High Definition... | 1.3%   | 3.14.44  | D92809A26A |
| 10de:0bea | 1025:064a | Nvidia          | GF108 High Definition... | 25%    | 4.15.0   | 344148537E |
| 10de:0bea | 1462:2304 | Nvidia          | GF108 High Definition... | 9.1%   | 3.14.44  | ED9D8A148D |
| 10de:0bea | 17aa:21cf | Nvidia          | GF108 High Definition... | 14.3%  | 3.10.34  | 4CAE7DC78D |
| 10de:0bea | 1991:5584 | Nvidia          | GF108 High Definition... | 50%    | 4.1.34   | CE8124E5F4 |
| 10de:0bee |           | Nvidia          | GF116 High Definition... | 0.9%   | 3.14.39  | 77909796EC |
| 10de:0e08 |           | Nvidia          | GF119 HDMI Audio Cont... | 2%     | 3.14.33  | 8F9504F263 |
| 10de:0e08 | 174b:0620 | Nvidia          | GF119 HDMI Audio Cont... | 40%    | 4.9.60   | 6566319F04 |
| 10de:0e08 | 174b:1222 | Nvidia          | GF119 HDMI Audio Cont... | 25%    | 5.4.0    | C0A7DFF96D |
| 10de:0e0a |           | Nvidia          | GK104 HDMI Audio Cont... | 7.1%   | 4.15.0   | 2961E0C973 |
| 10de:0e0a | 1558:0371 | Nvidia          | GK104 HDMI Audio Cont... | 50%    | 5.4.0    | 712D4A0730 |
| 10de:0e0f | 1043:84d6 | Nvidia          | GK208 HDMI/DP Audio C... | 7.7%   | 4.1.15   | 072483C895 |
| 10de:0e0f | 1043:84f5 | Nvidia          | GK208 HDMI/DP Audio C... | 9.5%   | 3.14.44  | 57B918A36E |
| 10de:0e0f | 10de:118b | Nvidia          | GK208 HDMI/DP Audio C... | 2.2%   | 4.9.0    | C40A63CD12 |
| 10de:0e0f | 1462:8c93 | Nvidia          | GK208 HDMI/DP Audio C... | 0.3%   | 3.19.0   | EE56035E75 |
| 10de:0e0f | 19da:5360 | Nvidia          | GK208 HDMI/DP Audio C... | 7.1%   | 4.15.0   | 7A813C93B0 |
| 10de:0e0f | 19da:7326 | Nvidia          | GK208 HDMI/DP Audio C... | 1.1%   | 4.9.60   | 84ED791AF7 |
| 10de:0e0f | 3842:1731 | Nvidia          | GK208 HDMI/DP Audio C... | 100%   |          | 04BFACB4A7 |
| 10de:0e1a | 103c:1036 | Nvidia          | GK110 High Definition... | 50%    | 5.4.17   | 83DFC4B9D8 |
| 10de:0e1a | 1043:8451 | Nvidia          | GK110 High Definition... | 12.5%  | 3.14.44  | 626DB9E244 |
| 10de:0e1b | 1028:053e | Nvidia          | GK107 HDMI Audio Cont... | 7.7%   | 4.15.0   | F674F91052 |
| 10de:0e1b | 103c:094c | Nvidia          | GK107 HDMI Audio Cont... | 2.4%   | 4.12.14  | 449A9223A3 |
| 10de:0e1b | 10de:094b | Nvidia          | GK107 HDMI Audio Cont... | 3.8%   | 4.1.15   | 949DD823D7 |
| 10de:0e1b | 1462:8a96 | Nvidia          | GK107 HDMI Audio Cont... | 5.8%   | 3.10.0   | 8E26B54DE5 |
| 10de:0e1b | 1462:8a9e | Nvidia          | GK107 HDMI Audio Cont... | 3.2%   | 3.14.44  | 05258AEA35 |
| 10de:0e1b | 1569:0fc6 | Nvidia          | GK107 HDMI Audio Cont... | 0.9%   | 3.14.33  | 8F804041A2 |
| 10de:0fb0 | 1462:3232 | Nvidia          | GM200 High Definition... | 6.7%   | 5.0.0    | AF58D23265 |
| 10de:0fb0 | 1462:3233 | Nvidia          | GM200 High Definition... | 10%    | 4.15.0   | 6054B96BC5 |
| 10de:0fb8 | 1462:8c98 | Nvidia          | GP108 High Definition... | 0.5%   | 4.4.0    | 8260769B47 |
| 10de:0fb9 |           | Nvidia          | GP107GL High Definiti... | 0.3%   | 3.10.0   | FFDEE2C6E0 |
| 10de:0fb9 | 1025:1265 | Nvidia          | GP107GL High Definiti... | 1.7%   | 4.15.0   | 077D639C2D |
| 10de:0fb9 | 1043:85c7 | Nvidia          | GP107GL High Definiti... | 25%    | 4.15.0   | 6A9C548EF5 |
| 10de:0fb9 | 1043:85d3 | Nvidia          | GP107GL High Definiti... | 13.3%  | 4.1.25   | E1E2F84AB5 |
| 10de:0fb9 | 10de:12af | Nvidia          | GP107GL High Definiti... | 100%   |          | C11BA25134 |
| 10de:0fb9 | 1458:3729 | Nvidia          | GP107GL High Definiti... | 4.8%   | 4.9.9    | F71DD78128 |
| 10de:0fb9 | 1458:3733 | Nvidia          | GP107GL High Definiti... | 2.5%   | 4.9.60   | DADA6C90F4 |
| 10de:0fb9 | 1458:3763 | Nvidia          | GP107GL High Definiti... | 4%     | 4.15.0   | F1C95A10CC |
| 10de:0fb9 | 1462:8c96 | Nvidia          | GP107GL High Definiti... | 1.4%   | 4.1.38   | 9578024712 |
| 10de:0fb9 | 3842:6253 | Nvidia          | GP107GL High Definiti... | 1.8%   | 4.9.0    | FC6C12EB1D |
| 10de:0fb9 | ffff:ffff | Nvidia          | GP107GL High Definiti... | 1.4%   | 5.0.0    | BB46F7172F |
| 10de:0fba | 1043:8520 | Nvidia          | GM206 High Definition... | 1.2%   | 3.14.53  | 8D2A73DD23 |
| 10de:0fba | 1458:36be | Nvidia          | GM206 High Definition... | 3.4%   | 4.9.60   | 919A0EA816 |
| 10de:0fba | 3842:2962 | Nvidia          | GM206 High Definition... | 25%    | 5.7.2    | 707960B3EC |
| 10de:0fbb | 1458:3672 | Nvidia          | GM204 High Definition... | 18.2%  | 4.15.0   | 57643353CE |
| 10de:0fbb | 1458:367c | Nvidia          | GM204 High Definition... | 28.6%  | 4.19.0   | 57643353CE |
| 10de:0fbb | 1462:3170 | Nvidia          | GM204 High Definition... | 4.3%   | 4.9.60   | 07BD3ED250 |
| 10de:0fbb | 19da:b282 | Nvidia          | GM204 High Definition... | 50%    | 5.4.80   | 2EB3FFC86C |
| 10de:0fbc | 10de:105f | Nvidia          | GM107 High Definition... | 9.1%   | 4.1.16   | 627983AA9A |
| 10de:0fbc | 10de:1140 | Nvidia          | GM107 High Definition... | 12.5%  | 4.15.0   | 375D6B6557 |
| 10de:0fbc | 1462:3102 | Nvidia          | GM107 High Definition... | 2.4%   | 3.14.44  | 071F922873 |
| 10de:0fbc | 196e:1381 | Nvidia          | GM107 High Definition... | 8.3%   | 3.14.44  | 5ACBE289AA |
| 10de:0fbc | 3842:3753 | Nvidia          | GM107 High Definition... | 2.4%   | 4.9.60   | 541846E7D7 |
| 10de:10ef | 10de:120f | Nvidia          | GP102 HDMI Audio Cont... | 6.7%   | 4.4.0    | 60B6348B70 |
| 10de:10ef | 1458:374c | Nvidia          | GP102 HDMI Audio Cont... | 5.3%   | 4.18.16  | DDA56057CF |
| 10de:10ef | 1462:3602 | Nvidia          | GP102 HDMI Audio Cont... | 7.7%   | 4.12.14  | E7B3AD7E11 |
| 10de:10ef | 1462:3607 | Nvidia          | GP102 HDMI Audio Cont... | 14.3%  | 4.15.0   | 877BEE4B1A |
| 10de:10ef | 1462:360c | Nvidia          | GP102 HDMI Audio Cont... | 42.9%  | 5.4.0    | F7A48733A6 |
| 10de:10f0 | 1043:8597 | Nvidia          | GP104 High Definition... | 10.5%  | 4.15.0   | 32166A5865 |
| 10de:10f0 | 1043:8599 | Nvidia          | GP104 High Definition... | 2.3%   | 4.9.9    | 2E49A21374 |
| 10de:10f0 | 1043:85aa | Nvidia          | GP104 High Definition... | 2.6%   | 4.9.9    | D2E5D9AE8E |
| 10de:10f0 | 1558:0879 | Nvidia          | GP104 High Definition... | 50%    | 4.19.0   | A7DB7C544F |
| 10de:10f0 | 19da:2435 | Nvidia          | GP104 High Definition... | 3%     | 5.1.6    | C818EB5CB4 |
| 10de:10f0 | 3842:6183 | Nvidia          | GP104 High Definition... | 9.1%   | 4.18.16  | D88BFB96F9 |
| 10de:10f0 | 3842:6288 | Nvidia          | GP104 High Definition... | 50%    | 5.8.0    | FC3F785613 |
| 10de:10f1 | 103c:8581 | Nvidia          | GP106 High Definition... | 20%    | 4.15.0   | 85885ECEF9 |
| 10de:10f1 | 10de:1c03 | Nvidia          | GP106 High Definition... | 1.1%   | 4.9.20   | E996F15E3E |
| 10de:10f1 | 1458:3724 | Nvidia          | GP106 High Definition... | 3.6%   | 4.1.34   | C74C010C1B |
| 10de:10f1 | 1462:3281 | Nvidia          | GP106 High Definition... | 0.8%   | 4.1.25   | A4BDAC2CEA |
| 10de:10f1 | 1462:3490 | Nvidia          | GP106 High Definition... | 16.7%  | 4.15.0   | 1B722DF896 |
| 10de:10f1 | 1462:8c94 | Nvidia          | GP106 High Definition... | 5.6%   | 4.9.87   | D864C8519E |
| 10de:10f7 | 1462:3717 | Nvidia          | TU102 High Definition... | 50%    | 5.9.1    | 97217688BF |
| 10de:10f8 | 1043:8797 | Nvidia          | TU104 HD Audio Contro... | 100%   |          | 82A9A037CB |
| 10de:10f9 | 1028:0990 | Nvidia          | TU106 High Definition... | 12.5%  | 5.4.0    | F6D1EB0921 |
| 10de:10f9 | 1043:8698 | Nvidia          | TU106 High Definition... | 7.7%   | 4.15.0   | BF6FD8E5AC |
| 10de:10f9 | 10de:12fb | Nvidia          | TU106 High Definition... | 33.3%  | 5.9.16   | 3B92D6CC85 |
| 10de:10f9 | 10de:12fe | Nvidia          | TU106 High Definition... | 10%    | 5.4.0    | 0FA979BBFB |
| 10de:10f9 | 1458:37ad | Nvidia          | TU106 High Definition... | 25%    | 5.4.0    | B1F5EAC9A6 |
| 10de:10f9 | 1458:3fda | Nvidia          | TU106 High Definition... | 25%    | 4.15.0   | F0D57310C5 |
| 10de:10fa | 1025:142f | Nvidia          | TU107 GeForce GTX 165... | 4.2%   | 4.15.0   | F7A69F2819 |
| 10de:10fa | 103c:8611 | Nvidia          | TU107 GeForce GTX 165... | 11.1%  | 4.18.0   | BDD15B19B1 |
| 10de:10fa | 103c:87b1 | Nvidia          | TU107 GeForce GTX 165... | 4.3%   | 5.7.8    | 2C929E66BC |
| 10de:10fa | 10de:1320 | Nvidia          | TU107 GeForce GTX 165... | 3.7%   | 4.15.0   | DA311C1D96 |
| 10de:1aeb | 1028:0949 | Nvidia          | TU116 High Definition... | 1.7%   | 5.0.0    | E0FB0728BB |
| 10de:1aeb | 1043:16cf | Nvidia          | TU116 High Definition... | 2.4%   | 4.18.16  | 3A1B31970C |
| 10de:1aeb | 10de:2184 | Nvidia          | TU116 High Definition... | 14.3%  | 4.15.0   | A011A6EF0E |
| 10de:1aeb | 1458:4013 | Nvidia          | TU116 High Definition... | 4%     | 4.18.19  | 4080E1B43F |
| 10de:1aeb | 1458:4014 | Nvidia          | TU116 High Definition... | 5.3%   | 5.3.0    | 03EEF2B7D3 |
| 10de:1aef | 1043:87b3 | Nvidia          | GA102 High Definition... | 100%   |          | EC3E24BBCC |
| 10de:1aef | 1462:3881 | Nvidia          | GA102 High Definition... | 50%    | 5.8.0    | EC3E24BBCC |
| 10de:1aef | 19da:1613 | Nvidia          | GA102 High Definition... | 33.3%  | 5.4.0    | EC3E24BBCC |
| 10de:1aef | 3842:3987 | Nvidia          | GA102 High Definition... | 33.3%  | 5.9.13   | 0D787440F2 |
| 10de:228b | 1043:87ba | Nvidia          | GA104 High Definition... | 100%   |          | FA5AAEE132 |
| 10de:228b | 1458:404d | Nvidia          | GA104 High Definition... | 50%    | 5.10.10  | FA5AAEE132 |
| 1102:0004 | 1102:1003 | Creative Labs   | EMU10k2/CA0100/CA0102... | 5.6%   | 4.1.15   | D74C162548 |
| 1102:0004 | 1102:2002 | Creative Labs   | EMU10k2/CA0100/CA0102... | 1%     | 3.14.44  | 2B0A36F85F |
| 1102:0007 | 1102:100a | Creative Labs   | CA0106/CA0111 [SB Liv... | 1.2%   | 3.14.25  | BCEA5A9B37 |
| 1102:000b | 1102:0041 | Creative Labs   | EMU20k2 [Sound Blaste... | 3.3%   | 4.1.16   | 947267E711 |
| 1102:0010 | 1102:0073 | Creative Labs   | Creative Audio device    | 50%    | 5.9.1    | 97217688BF |
| 1102:0012 | 1102:0010 | Creative Labs   | Sound Core3D [Sound B... | 0.6%   | 3.14.44  | 57643353CE |
| 1274:1371 | 1274:1371 | Ensoniq         | ES1371/ES1373 / Creat... | 6%     | 3.14.44  | CB5FCEB934 |
| 1274:5880 | 1274:2000 | Ensoniq         | 5880B / Creative Labs... | 3.2%   | 3.14.44  | 7A874B3AA5 |
| 137a:0001 |           | Mark of the ... | PCI-324 Audiowire Int... | 100%   |          | 5A23275111 |
| 13e6:0111 | 13e6:1802 | Argosy research | Argosy Multimedia aud... | 100%   |          | 6C9D42B55D |
| 13f2:0111 |           | Ford Microel... |                          | 100%   |          | 95162A226D |
| 13f2:0111 | ffff:ffff | Ford Microel... | Multimedia audio cont... | 100%   |          | 95162A226D |
| 13f6:0111 | 13f6:0111 | C-Media Elec... | CMI8738/CMI8768 PCI A... | 0.9%   | 3.14.22  | 1E2CC675FA |
| 13f6:0111 | 153b:1144 | C-Media Elec... | CMI8738/CMI8768 PCI A... | 3.3%   | 4.1.25   | 86F297ED58 |
| 13f6:8788 | 1043:8427 | C-Media Elec... | CMI8788 [Oxygen HD Au... | 100%   |          | BFB822D98C |
| 13f6:8788 | 1043:8463 | C-Media Elec... | CMI8788 [Oxygen HD Au... | 100%   |          | 9E13784BB3 |
| 13f6:8788 | 1043:8521 | C-Media Elec... | CMI8788 [Oxygen HD Au... | 0.9%   | 3.14.44  | 45FCBC8B9A |
| 13f6:8788 | 1043:855e | C-Media Elec... | CMI8788 [Oxygen HD Au... | 100%   |          | C9AF16A580 |
| 13f6:8788 | 7284:9783 | C-Media Elec... | CMI8788 [Oxygen HD Au... | 100%   |          | 40EA4505B9 |
| 1412:1624 | 1412:2403 | VIA Technolo... | Multimedia audio cont... | 100%   |          | 2AF6424751 |
| 1412:1712 | 153b:1115 | VIA Technolo... | ICE1712 [Envy24] PCI ... | 33.3%  | 5.8.0    | 95F4B4A653 |
| 19fe:7000 | 0e51:0002 | ESI             | MAYA44e Controller       | 100%   |          | D91E94A951 |
| 1c67:0101 | 1c67:0101 |                 | Multimedia audio cont... | 100%   |          | 589F688E41 |
| 8086:02c8 | 1028:0954 | Intel           | Comet Lake PCH-LP cAVS   | 50%    | 5.8.0    | 8740133E10 |
| 8086:02c8 | 1028:0969 | Intel           | Comet Lake PCH-LP cAVS   | 100%   |          | 7ABAC766F3 |
| 8086:02c8 | 1028:09a0 | Intel           | Comet Lake PCH-LP cAVS   | 5.3%   | 5.4.0    | 916DB21F7F |
| 8086:02c8 | 103c:85f1 | Intel           | Comet Lake PCH-LP cAVS   | 7.1%   | 5.3.0    | 733DA06DF4 |
| 8086:02c8 | 1043:1a61 | Intel           | Comet Lake PCH-LP cAVS   | 26.7%  | 5.3.0    | 2C64A52714 |
| 8086:02c8 | 17aa:3185 | Intel           | Comet Lake PCH-LP cAVS   | 100%   |          | 324F862858 |
| 8086:02c8 | 17aa:5079 | Intel           | Comet Lake PCH-LP cAVS   | 0.6%   | 4.15.0   | 8DAEEEE12F |
| 8086:06c8 | 1025:142f | Intel           | Comet Lake PCH cAVS      | 20%    | 4.15.0   | F7A69F2819 |
| 8086:06c8 | 1028:0984 | Intel           | Comet Lake PCH cAVS      | 50%    | 5.0.0    | 3A565370DE |
| 8086:06c8 | 1458:a184 | Intel           | Comet Lake PCH cAVS      | 16.7%  | 5.4.0    | EC3E24BBCC |
| 8086:06c8 | 17aa:380e | Intel           | Comet Lake PCH cAVS      | 9.1%   | 5.4.0    | 66DE8410B3 |
| 8086:0a0c | 1025:0775 | Intel           | Haswell-ULT HD Audio ... | 0.6%   | 3.14.25  | 81B19839F7 |
| 8086:0a0c | 103c:2249 | Intel           | Haswell-ULT HD Audio ... | 9.1%   | 4.1.25   | 8DCBD3C2B1 |
| 8086:0a0c | 17aa:3978 | Intel           | Haswell-ULT HD Audio ... | 0.2%   | 3.14.25  | B3B3794709 |
| 8086:0c0c | 1028:0612 | Intel           | Xeon E3-1200 v3/4th G... | 0.9%   | 4.15.0   | D2ECCACD0C |
| 8086:0c0c | 103c:18e6 | Intel           | Xeon E3-1200 v3/4th G... | 12.5%  | 3.14.44  | CF3ED91B8A |
| 8086:0c0c | 103c:18e7 | Intel           | Xeon E3-1200 v3/4th G... | 2.3%   | 4.1.25   | 627983AA9A |
| 8086:0c0c | 8086:0c0c | Intel           | Xeon E3-1200 v3/4th G... | 12.5%  | 4.9.60   | B364724E53 |
| 8086:0c0c | 8086:2010 | Intel           | Xeon E3-1200 v3/4th G... | 0.4%   | 2.6.32   | DE3D4B192E |
| 8086:0f04 | 1043:14dd | Intel           | Atom Processor Z36xxx... | 1.3%   | 3.14.33  | 106830C1CC |
| 8086:0f04 | 17aa:3695 | Intel           | Atom Processor Z36xxx... | 16.7%  | 4.15.0   | 08BB09B100 |
| 8086:0f04 | 1849:c892 | Intel           | Atom Processor Z36xxx... | 7.7%   | 4.13.7   | 78F7E1012F |
| 8086:0f28 | 17aa:3907 | Intel           | Atom Processor Z36xxx... | 100%   |          | 6D960BD235 |
| 8086:0f28 | 8086:0f28 | Intel           | Atom Processor Z36xxx... | 100%   |          | AD5481A5BC |
| 8086:0f28 | 8086:7270 | Intel           | Atom Processor Z36xxx... | 100%   |          | 44359D461E |
| 8086:160c | 1025:098a | Intel           | Broadwell-U Audio Con... | 0.7%   | 3.14.44  | 4F849E1E80 |
| 8086:160c | 1025:1019 | Intel           | Broadwell-U Audio Con... | 100%   |          | 5DBE9649A7 |
| 8086:160c | 17aa:390b | Intel           | Broadwell-U Audio Con... | 2.6%   | 4.9.60   | AB6BD693BE |
| 8086:1c20 | 1025:0492 | Intel           | 6 Series/C200 Series ... | 1.4%   | 3.10.34  | C0A7DFF96D |
| 8086:1c20 | 1025:0504 | Intel           | 6 Series/C200 Series ... | 0.3%   | 3.10.0   | 8FE3AF49FB |
| 8086:1c20 | 1028:0492 | Intel           | 6 Series/C200 Series ... | 3%     | 4.9.60   | EAFEF7DB79 |
| 8086:1c20 | 1028:0493 | Intel           | 6 Series/C200 Series ... | 2.1%   | 3.14.33  | EFD71FBD61 |
| 8086:1c20 | 1028:04ad | Intel           | 6 Series/C200 Series ... | 1.1%   | 4.1.25   | ACF06E07B8 |
| 8086:1c20 | 103c:1495 | Intel           | 6 Series/C200 Series ... | 0.8%   | 3.10.0   | FFB9D2F433 |
| 8086:1c20 | 103c:1587 | Intel           | 6 Series/C200 Series ... | 16.7%  | 4.15.0   | 4B1F2221EE |
| 8086:1c20 | 103c:161c | Intel           | 6 Series/C200 Series ... | 1.1%   | 4.1.15   | 71029063A4 |
| 8086:1c20 | 103c:2ada | Intel           | 6 Series/C200 Series ... | 2.6%   | 4.4.14   | 6A9C548EF5 |
| 8086:1c20 | 1043:841b | Intel           | 6 Series/C200 Series ... | 6.5%   | 3.10.34  | 95722413A6 |
| 8086:1c20 | 1043:8444 | Intel           | 6 Series/C200 Series ... | 0.5%   | 3.10.0   | 47DBD40DAE |
| 8086:1c20 | 1043:8445 | Intel           | 6 Series/C200 Series ... | 0.5%   | 3.10.0   | DDC4A811C7 |
| 8086:1c20 | 10cf:15dc | Intel           | 6 Series/C200 Series ... | 1%     | 4.1.34   | 958D094890 |
| 8086:1c20 | 1179:fc50 | Intel           | 6 Series/C200 Series ... | 1.1%   | 3.14.44  | 046BFED81F |
| 8086:1c20 | 1462:7673 | Intel           | 6 Series/C200 Series ... | 5.9%   | 3.14.33  | 15193EDA95 |
| 8086:1c20 | 17aa:21cf | Intel           | 6 Series/C200 Series ... | 0.7%   | 3.10.0   | 4CAE7DC78D |
| 8086:1c20 | 1849:1892 | Intel           | 6 Series/C200 Series ... | 2%     | 3.10.0   | 895D8612B4 |
| 8086:1c20 | 1849:3662 | Intel           | 6 Series/C200 Series ... | 2.2%   | 3.14.25  | 0139CCFE4A |
| 8086:1c20 | 1849:a662 | Intel           | 6 Series/C200 Series ... | 0.9%   | 3.14.44  | 7F5766D5DA |
| 8086:1c20 | 1b0a:20b2 | Intel           | 6 Series/C200 Series ... | 12.5%  | 4.15.0   | 62F72208D5 |
| 8086:1d20 | 1028:05d2 | Intel           | C600/X79 series chips... | 2.8%   | 4.12.14  | 949DD823D7 |
| 8086:1d20 | 1043:84fd | Intel           | C600/X79 series chips... | 12.5%  | 4.1.25   | 626DB9E244 |
| 8086:1d20 | 17aa:1027 | Intel           | C600/X79 series chips... | 16.7%  | 4.1.25   | 8D7A62CE1A |
| 8086:1d20 | 8086:1d20 | Intel           | C600/X79 series chips... | 1.4%   | 4.4.0    | BBFC99D048 |
| 8086:1e20 | 1025:0649 | Intel           | 7 Series/C216 Chipset... | 0.4%   | 3.14.25  | 344148537E |
| 8086:1e20 | 1025:067d | Intel           | 7 Series/C216 Chipset... | 10%    | 3.14.44  | 8ABC23484B |
| 8086:1e20 | 1025:074f | Intel           | 7 Series/C216 Chipset... | 28.6%  | 5.4.0    | 6566319F04 |
| 8086:1e20 | 1028:052c | Intel           | 7 Series/C216 Chipset... | 1.5%   | 4.15.0   | 29A0FC6CE0 |
| 8086:1e20 | 1028:053e | Intel           | 7 Series/C216 Chipset... | 3.4%   | 4.9.124  | F674F91052 |
| 8086:1e20 | 103c:1845 | Intel           | 7 Series/C216 Chipset... | 14.3%  | 3.14.44  | 2E60620A98 |
| 8086:1e20 | 1043:841a | Intel           | 7 Series/C216 Chipset... | 10%    | 4.1.15   | 3A69ABB947 |
| 8086:1e20 | 1043:8436 | Intel           | 7 Series/C216 Chipset... | 2.4%   | 3.14.44  | AF3425A2EC |
| 8086:1e20 | 1043:851f | Intel           | 7 Series/C216 Chipset... | 11.1%  | 4.13.0   | 0201C4C0FD |
| 8086:1e20 | 1179:fb40 | Intel           | 7 Series/C216 Chipset... | 12.5%  | 4.1.15   | 67009EFFAA |
| 8086:1e20 | 1297:2033 | Intel           | 7 Series/C216 Chipset... | 6.5%   | 4.9.20   | 9137B29AFE |
| 8086:1e20 | 1458:a002 | Intel           | 7 Series/C216 Chipset... | 0.4%   | 4.9.0    | 740BF21A40 |
| 8086:1e20 | 1462:d751 | Intel           | 7 Series/C216 Chipset... | 5%     | 4.15.0   | 7A756F5970 |
| 8086:1e20 | 1558:0371 | Intel           | 7 Series/C216 Chipset... | 50%    | 5.4.0    | 712D4A0730 |
| 8086:1e20 | 17aa:21f3 | Intel           | 7 Series/C216 Chipset... | 0.8%   | 3.14.44  | 5904CA74C2 |
| 8086:1e20 | 17aa:21fa | Intel           | 7 Series/C216 Chipset... | 0.4%   | 3.10.42  | 4E98739F72 |
| 8086:1e20 | 17aa:21fb | Intel           | 7 Series/C216 Chipset... | 3.2%   | 4.9.20   | 55427995B5 |
| 8086:1e20 | 17aa:3083 | Intel           | 7 Series/C216 Chipset... | 3%     | 4.9.111  | E3BF127788 |
| 8086:1e20 | 17aa:3977 | Intel           | 7 Series/C216 Chipset... | 0.2%   | 3.10.0   | 2DD89E3983 |
| 8086:1e20 | 8086:1e20 | Intel           | 7 Series/C216 Chipset... | 0.9%   | 4.1.34   | CE8124E5F4 |
| 8086:2284 | 1025:1009 | Intel           | Atom/Celeron/Pentium ... | 9.1%   | 4.9.20   | 401BBED185 |
| 8086:2284 | 1028:06ac | Intel           | Atom/Celeron/Pentium ... | 1.1%   | 4.4.0    | B5721FA9D5 |
| 8086:2284 | 1043:1cbd | Intel           | Atom/Celeron/Pentium ... | 10.7%  | 4.4.0    | 71CCEBC0C1 |
| 8086:2284 | 1458:fa20 | Intel           | Atom/Celeron/Pentium ... | 50%    | 4.15.0   | 2FD537312F |
| 8086:2284 | 8086:7270 | Intel           | Atom/Celeron/Pentium ... | 1.7%   | 4.9.20   | FE38A788E3 |
| 8086:22a8 | 8086:7270 | Intel           | Atom/Celeron/Pentium ... | 100%   |          | EF051B442A |
| 8086:24d5 | 105b:0c07 | Intel           | 82801EB/ER (ICH5/ICH5... | 100%   |          | A3DF896B35 |
| 8086:266e | 103c:3006 | Intel           | 82801FB/FBM/FR/FW/FRW... | 25%    | 4.9.20   | 51837DE98F |
| 8086:266e | 1179:ff00 | Intel           | 82801FB/FBM/FR/FW/FRW... | 3.6%   | 4.15.0   | 8488B3D0B9 |
| 8086:266e | 1458:ae01 | Intel           | 82801FB/FBM/FR/FW/FRW... | 7.7%   | 3.14.44  | FD291EB728 |
| 8086:269a | 103c:1307 | Intel           | 631xESB/632xESB High ... | 13.6%  | 4.1.15   | 51D516FF60 |
| 8086:27d8 | 1019:2683 | Intel           | NM10/ICH7 Family High... | 1.3%   | 3.14.44  | EAA25586D2 |
| 8086:27d8 | 1025:0349 | Intel           | NM10/ICH7 Family High... | 0.7%   | 3.14.44  | F556D9CE96 |
| 8086:27d8 | 1028:01de | Intel           | NM10/ICH7 Family High... | 6.2%   | 3.14.44  | 60F738965A |
| 8086:27d8 | 1028:0220 | Intel           | NM10/ICH7 Family High... | 2.1%   | 3.14.44  | BBA0FE2672 |
| 8086:27d8 | 1043:8290 | Intel           | NM10/ICH7 Family High... | 0.3%   | 3.14.25  | 45FCBC8B9A |
| 8086:27d8 | 1043:83d4 | Intel           | NM10/ICH7 Family High... | 0.8%   | 3.14.44  | 8807184E95 |
| 8086:27d8 | 104d:81fc | Intel           | NM10/ICH7 Family High... | 100%   |          | 7F0BB0CC92 |
| 8086:27d8 | 1458:a002 | Intel           | NM10/ICH7 Family High... | 0.4%   | 3.10.0   | 8D2893FCFB |
| 8086:27d8 | 1462:104e | Intel           | NM10/ICH7 Family High... | 20%    | 4.1.15   | 5F15F028A8 |
| 8086:27d8 | 1462:7592 | Intel           | NM10/ICH7 Family High... | 1.5%   | 3.10.19  | FD37A435F8 |
| 8086:27d8 | 1631:c027 | Intel           | NM10/ICH7 Family High... | 20%    | 4.9.60   | 83204D550C |
| 8086:27d8 | 17aa:2010 | Intel           | NM10/ICH7 Family High... | 1%     | 3.10.0   | 73B406FF03 |
| 8086:27d8 | 1854:005f | Intel           | NM10/ICH7 Family High... | 11.1%  | 4.15.0   | F60C56AC42 |
| 8086:27d8 | 1b0a:0001 | Intel           | NM10/ICH7 Family High... | 1.6%   | 3.14.44  | 396BE2A324 |
| 8086:27d8 | 8086:27d8 | Intel           | NM10/ICH7 Family High... | 1.9%   | 3.14.44  | 37B1114873 |
| 8086:284b | 103c:3618 | Intel           | 82801H (ICH8 Family) ... | 6.1%   | 3.14.44  | 13824A2872 |
| 8086:284b | 1734:1083 | Intel           | 82801H (ICH8 Family) ... | 14.3%  | 3.14.44  | F626D15B06 |
| 8086:293e | 1025:017e | Intel           | 82801I (ICH9 Family) ... | 33.3%  | 4.1.25   | 6D1385653B |
| 8086:293e | 1028:0211 | Intel           | 82801I (ICH9 Family) ... | 0.6%   | 3.14.44  | 95F4B4A653 |
| 8086:293e | 103c:281e | Intel           | 82801I (ICH9 Family) ... | 1.1%   | 3.14.44  | 61D1ED752A |
| 8086:293e | 103c:2a6f | Intel           | 82801I (ICH9 Family) ... | 0.9%   | 3.14.15  | EEE4525E5F |
| 8086:293e | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 5.6%   | 3.14.44  | 93C0EF7223 |
| 8086:293e | 103c:3676 | Intel           | 82801I (ICH9 Family) ... | 16.7%  | 4.1.25   | 031B9CF2AF |
| 8086:293e | 1043:8277 | Intel           | 82801I (ICH9 Family) ... | 0.5%   | 3.14.44  | 39270C836F |
| 8086:293e | 1458:a002 | Intel           | 82801I (ICH9 Family) ... | 0.3%   | 3.14.33  | F47CB1587E |
| 8086:293e | 1458:a022 | Intel           | 82801I (ICH9 Family) ... | 4.4%   | 3.14.44  | 071F922873 |
| 8086:293e | 17aa:20f2 | Intel           | 82801I (ICH9 Family) ... | 0.2%   | 3.10.0   | 9B9F58A14D |
| 8086:34c8 | 1028:0979 | Intel           | Ice Lake-LP Smart Sou... | 2.9%   | 5.0.0    | 7F4CE08DF9 |
| 8086:34c8 | 1028:097a | Intel           | Ice Lake-LP Smart Sou... | 11.5%  | 5.0.0    | 17D09024B3 |
| 8086:34c8 | 103c:868a | Intel           | Ice Lake-LP Smart Sou... | 25%    | 5.4.0    | 9F4F9A0186 |
| 8086:34c8 | 103c:86ab | Intel           | Ice Lake-LP Smart Sou... | 10%    | 5.4.0    | 4019B6C1FF |
| 8086:34c8 | 17aa:3810 | Intel           | Ice Lake-LP Smart Sou... | 6.2%   | 5.0.0    | F8B39E4272 |
| 8086:3a3e | 1025:0251 | Intel           | 82801JI (ICH10 Family... | 10%    | 4.18.0   | DFD78F1056 |
| 8086:3a3e | 1028:026d | Intel           | 82801JI (ICH10 Family... | 6.2%   | 4.15.0   | 08F4C825CC |
| 8086:3a3e | 1028:0293 | Intel           | 82801JI (ICH10 Family... | 3.5%   | 3.10.0   | D92809A26A |
| 8086:3a3e | 1028:02ac | Intel           | 82801JI (ICH10 Family... | 5.9%   | 4.1.25   | 8563E0FB2C |
| 8086:3a3e | 1028:0439 | Intel           | 82801JI (ICH10 Family... | 2.3%   | 4.4.0    | 486BCF83D7 |
| 8086:3a3e | 1043:82fe | Intel           | 82801JI (ICH10 Family... | 0.6%   | 3.14.44  | 072483C895 |
| 8086:3a3e | 1043:8357 | Intel           | 82801JI (ICH10 Family... | 0.5%   | 3.14.25  | C6C1C28B2D |
| 8086:3a3e | 1043:837b | Intel           | 82801JI (ICH10 Family... | 1.5%   | 3.14.15  | 3A2604A18A |
| 8086:3a3e | 1462:7522 | Intel           | 82801JI (ICH10 Family... | 3.2%   | 4.1.16   | 335083A19F |
| 8086:3a6e | 1028:0420 | Intel           | 82801JD/DO (ICH10 Fam... | 0.5%   | 3.10.0   | 2B2AA48899 |
| 8086:3b56 | 1025:0487 | Intel           | 5 Series/3400 Series ... | 0.4%   | 3.14.25  | 68F61986F8 |
| 8086:3b56 | 103c:3674 | Intel           | 5 Series/3400 Series ... | 3.1%   | 3.16.0   | F4DE983D96 |
| 8086:3b56 | 103c:7008 | Intel           | 5 Series/3400 Series ... | 1.3%   | 3.10.34  | 5DD7A5FCE1 |
| 8086:3b56 | 1043:8375 | Intel           | 5 Series/3400 Series ... | 2.4%   | 3.14.44  | C74C010C1B |
| 8086:3b56 | 104d:9071 | Intel           | 5 Series/3400 Series ... | 0.4%   | 3.14.44  | 0EA9B1F8A9 |
| 8086:3b56 | 1458:a002 | Intel           | 5 Series/3400 Series ... | 0.4%   | 3.10.42  | 66219C1D36 |
| 8086:3b56 | 1849:6718 | Intel           | 5 Series/3400 Series ... | 6.7%   | 3.14.25  | 1D9934126C |
| 8086:5a98 | 8086:7270 | Intel           | Celeron N3350/Pentium... | 5.5%   | 4.4.0    | 622CED4019 |
| 8086:8c20 | 1028:05a4 | Intel           | 8 Series/C220 Series ... | 0.6%   | 3.10.0   | 541846E7D7 |
| 8086:8c20 | 1028:0612 | Intel           | 8 Series/C220 Series ... | 0.7%   | 4.15.0   | D2ECCACD0C |
| 8086:8c20 | 103c:18e6 | Intel           | 8 Series/C220 Series ... | 12.5%  | 3.14.44  | CF3ED91B8A |
| 8086:8c20 | 103c:18e7 | Intel           | 8 Series/C220 Series ... | 2.2%   | 4.1.25   | 627983AA9A |
| 8086:8c20 | 1043:129d | Intel           | 8 Series/C220 Series ... | 1.4%   | 3.14.25  | DE3D4B192E |
| 8086:8c20 | 1043:143f | Intel           | 8 Series/C220 Series ... | 6.7%   | 4.9.41   | A268D267B1 |
| 8086:8c20 | 1458:a002 | Intel           | 8 Series/C220 Series ... | 0.6%   | 3.10.0   | E996F15E3E |
| 8086:8c20 | 1849:1151 | Intel           | 8 Series/C220 Series ... | 5.4%   | 3.10.0   | 8E26B54DE5 |
| 8086:8c20 | 8086:7270 | Intel           | 8 Series/C220 Series ... | 0.6%   | 4.1.25   | 2961E0C973 |
| 8086:8c20 | 8086:8c20 | Intel           | 8 Series/C220 Series ... | 13.2%  | 4.9.124  | B364724E53 |
| 8086:8ca0 | 1462:d917 | Intel           | 9 Series Chipset Fami... | 2%     | 4.1.15   | 8D2A73DD23 |
| 8086:8ca0 | 1849:1151 | Intel           | 9 Series Chipset Fami... | 2.7%   | 3.14.44  | 5ACBE289AA |
| 8086:8d20 | 1028:0617 | Intel           | C610/X99 series chips... | 2.8%   | 3.10.0   | 375D6B6557 |
| 8086:8d20 | 103c:2129 | Intel           | C610/X99 series chips... | 22.2%  | 5.4.0    | 83DFC4B9D8 |
| 8086:8d20 | 1043:8637 | Intel           | C610/X99 series chips... | 1.1%   | 3.10.0   | 6054B96BC5 |
| 8086:8d20 | 1043:8699 | Intel           | C610/X99 series chips... | 14.3%  | 4.1.25   | 8212CC8601 |
| 8086:8d20 | 1458:a182 | Intel           | C610/X99 series chips... | 3.4%   | 4.1.15   | 6AFD8A5657 |
| 8086:98c8 | 144d:c18b | Intel           | HD Graphics SGPC         | 100%   |          | 6D40FDC958 |
| 8086:9c20 | 1025:086b | Intel           | 8 Series HD Audio Con... | 10%    | 4.1.34   | 81B19839F7 |
| 8086:9c20 | 103c:2249 | Intel           | 8 Series HD Audio Con... | 9.1%   | 4.1.25   | 8DCBD3C2B1 |
| 8086:9c20 | 17aa:3978 | Intel           | 8 Series HD Audio Con... | 0.2%   | 3.14.25  | B3B3794709 |
| 8086:9ca0 | 1025:098a | Intel           | Wildcat Point-LP High... | 0.7%   | 3.14.44  | 4F849E1E80 |
| 8086:9ca0 | 1025:1019 | Intel           | Wildcat Point-LP High... | 100%   |          | 5DBE9649A7 |
| 8086:9ca0 | 17aa:390b | Intel           | Wildcat Point-LP High... | 2.6%   | 4.9.60   | AB6BD693BE |
| 8086:9ca0 | 19da:b282 | Intel           | Wildcat Point-LP High... | 50%    | 5.4.80   | 2EB3FFC86C |
| 8086:9d70 |           | Intel           | Sunrise Point-LP HD A... | 10%    | 4.8.17   | D2F13246B1 |
| 8086:9d70 | 17aa:3815 | Intel           | Sunrise Point-LP HD A... | 1.1%   | 4.1.25   | C1778EA9B9 |
| 8086:9d70 | 17aa:3827 | Intel           | Sunrise Point-LP HD A... | 100%   |          | 588AC16C28 |
| 8086:9d70 | 8086:7270 | Intel           | Sunrise Point-LP HD A... | 1%     | 4.9.20   | 2CBA94FE45 |
| 8086:9d71 |           | Intel           | Sunrise Point-LP HD A... | 8.3%   | 4.4.232  | 4F9AEAAD47 |
| 8086:9d71 | 1025:1273 | Intel           | Sunrise Point-LP HD A... | 12.5%  | 4.15.0   | 8F64E7F2FF |
| 8086:9d71 | 1028:075b | Intel           | Sunrise Point-LP HD A... | 1.1%   | 4.4.0    | 6695D2A05E |
| 8086:9d71 | 1028:07a8 | Intel           | Sunrise Point-LP HD A... | 8.3%   | 5.3.0    | EBA5E925B8 |
| 8086:9d71 | 1028:081c | Intel           | Sunrise Point-LP HD A... | 2.2%   | 4.12.14  | 54E871CA5D |
| 8086:9d71 | 17aa:2249 | Intel           | Sunrise Point-LP HD A... | 33.3%  | 4.13.12  | 7B04D129D6 |
| 8086:9d71 | 17aa:225d | Intel           | Sunrise Point-LP HD A... | 0.9%   | 4.12.14  | 7D7E6AD5D5 |
| 8086:9d71 | 1ae0:006b | Intel           | Sunrise Point-LP HD A... | 25%    | 5.1.15   | 5918F8787E |
| 8086:9d71 | 1ae0:006c | Intel           | Sunrise Point-LP HD A... | 57.1%  | 5.4.0    | 215EFDCFF2 |
| 8086:9d71 | 8086:7270 | Intel           | Sunrise Point-LP HD A... | 0.8%   | 4.1.25   | 11068700F7 |
| 8086:9d72 | 1028:06e6 | Intel           | 300 Series Chipset Sm... | 100%   |          | B7465A5AE4 |
| 8086:9dc8 | 1025:129a | Intel           | Cannon Point-LP High ... | 5.9%   | 5.0.0    | 6E9BFB3B01 |
| 8086:9dc8 | 1028:089d | Intel           | Cannon Point-LP High ... | 7.7%   | 4.15.0   | DAF389F21B |
| 8086:9dc8 | 1028:08a8 | Intel           | Cannon Point-LP High ... | 6.2%   | 4.15.0   | B6DF9FEC5F |
| 8086:9dc8 | 1028:08b8 | Intel           | Cannon Point-LP High ... | 2.5%   | 4.19.0   | 241B649AD1 |
| 8086:9dc8 | 1028:08bc | Intel           | Cannon Point-LP High ... | 3%     | 4.15.0   | 5ED5F692A4 |
| 8086:9dc8 | 1028:08ca | Intel           | Cannon Point-LP High ... | 1.1%   | 4.15.0   | 906A07309D |
| 8086:9dc8 | 103c:856e | Intel           | Cannon Point-LP High ... | 7.1%   | 4.19.0   | 2928437EAC |
| 8086:9dc8 | 103c:857f | Intel           | Cannon Point-LP High ... | 16.7%  | 5.3.0    | A838427772 |
| 8086:9dc8 | 17aa:2279 | Intel           | Cannon Point-LP High ... | 0.7%   | 3.10.0   | B6F9682F0B |
| 8086:9dc8 | 17aa:3816 | Intel           | Cannon Point-LP High ... | 2.5%   | 5.0.0    | 64AF4308B0 |
| 8086:9dc8 | 8086:2074 | Intel           | Cannon Point-LP High ... | 0.6%   | 3.10.0   | 7AB72B120C |
| 8086:a0c8 | 1028:0a25 | Intel           | Tiger Lake-LP Smart S... | 20%    | 5.4.0    | DCC3B1005E |
| 8086:a0c8 | 17aa:3804 | Intel           | Tiger Lake-LP Smart S... | 50%    | 5.10.29  | 89AE55D07E |
| 8086:a0c8 | 17aa:5087 | Intel           | Tiger Lake-LP Smart S... | 3.6%   | 5.4.0    | DA96B2EC5B |
| 8086:a170 | 103c:8257 | Intel           | 100 Series/C230 Serie... | 9.1%   | 4.15.0   | D079BA6F90 |
| 8086:a170 | 1043:86ae | Intel           | 100 Series/C230 Serie... | 1.8%   | 4.1.38   | 57643353CE |
| 8086:a170 | 1043:86c7 | Intel           | 100 Series/C230 Serie... | 0.3%   | 3.14.53  | FFA7928110 |
| 8086:a170 | 1458:a0a2 | Intel           | 100 Series/C230 Serie... | 100%   |          | 9D1C5DC708 |
| 8086:a170 | 1462:d970 | Intel           | 100 Series/C230 Serie... | 16.7%  | 4.1.25   | 0FA979BBFB |
| 8086:a170 | 1462:d977 | Intel           | 100 Series/C230 Serie... | 4%     | 4.9.60   | 877BEE4B1A |
| 8086:a170 | 1462:f996 | Intel           | 100 Series/C230 Serie... | 0.9%   | 4.1.15   | 9B9C670167 |
| 8086:a170 | 1462:f998 | Intel           | 100 Series/C230 Serie... | 7.7%   | 4.15.0   | 2E49A21374 |
| 8086:a170 | 1462:fa15 | Intel           | 100 Series/C230 Serie... | 2%     | 4.9.60   | CD74218E72 |
| 8086:a171 | 1028:07d0 | Intel           | CM238 HD Audio Contro... | 3.1%   | 4.9.9    | D4927A9F76 |
| 8086:a171 | 144d:c790 | Intel           | CM238 HD Audio Contro... | 12.5%  | 4.15.0   | F8A5C21D24 |
| 8086:a1f0 | 103c:81c7 | Intel           | Lewisburg MROM 0         | 9.1%   | 3.10.0   | 0C434691D6 |
| 8086:a2f0 | 103c:82f2 | Intel           | 200 Series PCH HD Audio  | 3.2%   | 4.9.60   | 49D42CD641 |
| 8086:a2f0 | 1043:8735 | Intel           | 200 Series PCH HD Audio  | 5.4%   | 4.9.95   | 816A1797C5 |
| 8086:a2f0 | 1458:a182 | Intel           | 200 Series PCH HD Audio  | 1.3%   | 3.10.0   | FC6C12EB1D |
| 8086:a2f0 | 1558:0879 | Intel           | 200 Series PCH HD Audio  | 22.2%  | 4.18.0   | A7DB7C544F |
| 8086:a348 | 1025:126c | Intel           | Cannon Lake PCH cAVS     | 100%   |          | C1339E884A |
| 8086:a348 | 1028:0851 | Intel           | Cannon Lake PCH cAVS     | 100%   |          | 05D6B79D2F |
| 8086:a348 | 1028:0949 | Intel           | Cannon Lake PCH cAVS     | 1%     | 4.19.0   | E0FB0728BB |
| 8086:a348 | 103c:8581 | Intel           | Cannon Lake PCH cAVS     | 20%    | 4.15.0   | 85885ECEF9 |
| 8086:a348 | 103c:860f | Intel           | Cannon Lake PCH cAVS     | 6.2%   | 4.18.0   | BDD15B19B1 |
| 8086:a348 | 1043:86c7 | Intel           | Cannon Lake PCH cAVS     | 0.5%   | 2.6.32   | 9578024712 |
| 8086:a348 | 1043:8723 | Intel           | Cannon Lake PCH cAVS     | 0.8%   | 4.15.0   | 8260769B47 |
| 8086:a348 | 1458:a182 | Intel           | Cannon Lake PCH cAVS     | 1.7%   | 4.9.20   | F0D57310C5 |
| 8086:a348 | 1462:122f | Intel           | Cannon Lake PCH cAVS     | 7.7%   | 4.15.0   | 105C3ABAEB |
| 8086:a348 | 17aa:225f | Intel           | Cannon Lake PCH cAVS     | 2.8%   | 3.10.0   | FFDEE2C6E0 |
| 8086:a348 | 17aa:36e7 | Intel           | Cannon Lake PCH cAVS     | 25%    | 4.15.0   | 1B722DF896 |
| 8086:a348 | 17aa:3812 | Intel           | Cannon Lake PCH cAVS     | 1.3%   | 4.15.0   | BB46F7172F |
| 8086:a348 | 1849:5892 | Intel           | Cannon Lake PCH cAVS     | 2.1%   | 4.9.124  | 06EB8AFDBC |

### Storage (PCI)

80 out of 219 (36.53%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 104c:8033 | 1179:ff05 | Texas Instru... | PCIxx21/PCIxx11 Flash... | 5.6%   | 4.15.0   | 8488B3D0B9 |
| 104c:803b | 1025:011f | Texas Instru... | PCIxx12 Flash Media C... | 0.5%   | 3.14.33  | 2EE51E8201 |
| 104c:803b | 104d:81fc | Texas Instru... | PCIxx12 Flash Media C... | 100%   |          | 7F0BB0CC92 |
| 104c:803b | 17aa:207c | Texas Instru... | PCIxx12 Flash Media C... | 11.1%  | 3.14.44  | E5C5CE1445 |
| 1106:401a | 1028:02f5 | VIA Technolo... | VIA Card Reader Host ... | 100%   |          | 8EF532D4EC |
| 1106:401a | 1028:0408 | VIA Technolo... | VIA Card Reader Host ... | 100%   |          | B55E0BA8CB |
| 1106:401a | 1071:9515 | VIA Technolo... | VIA Card Reader Host ... | 100%   |          | E028F277D4 |
| 1106:401a | 1106:401a | VIA Technolo... | VIA Card Reader Host ... | 100%   |          | FF6AA83006 |
| 1106:401a | 17aa:3608 | VIA Technolo... | VIA Card Reader Host ... | 100%   |          | 69574214D7 |
| 117c:0064 | 117c:0064 | ATTO Technology | Celerity FC 16Gb/s Ge... | 100%   |          | 43EE2001E1 |
| 11f8:8032 | 117c:003b | PMC-Sierra      | PM8032 Tachyon QE8       | 66.7%  | 4.15.0   | 48E71CC737 |
| 1217:7130 | 1019:300e | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 3C221F81A4 |
| 1217:7130 | 1025:010d | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 287952FB68 |
| 1217:7130 | 1025:011a | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 9B2C049705 |
| 1217:7130 | 1025:0123 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | B127BEAD10 |
| 1217:7130 | 1025:0124 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 5AAFE28787 |
| 1217:7130 | 1025:012b | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | A01F7549B8 |
| 1217:7130 | 1025:0138 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 9EEE1E10B8 |
| 1217:7130 | 1025:013a | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | E3C4E48E57 |
| 1217:7130 | 1025:013c | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | F3C2EB74E0 |
| 1217:7130 | 1025:0148 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 6B6DF6431C |
| 1217:7130 | 1028:026f | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 79951D3FA6 |
| 1217:7130 | 1028:0273 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 186F1ABCFA |
| 1217:7130 | 1028:0275 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | A359187C45 |
| 1217:7130 | 1071:8258 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 98006DB3BD |
| 1217:7130 | 107b:0390 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 716346340E |
| 1217:7130 | 107b:0696 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | E9F51C8451 |
| 1217:7130 | 107b:0704 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 713D68894F |
| 1217:7130 | 10cf:13c6 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 8648B42278 |
| 1217:7130 | 10cf:143d | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | F72CB25216 |
| 1217:7130 | 10cf:14d6 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 79DC3442B5 |
| 1217:7130 | 1179:ff50 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 62AC427393 |
| 1217:7130 | 1462:3fbb | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | FDCEAF9E02 |
| 1217:7130 | 1462:3fc1 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 800B19FF2D |
| 1217:7130 | 1462:3fe9 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | DA33747D00 |
| 1217:7130 | 1462:3ff3 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 483C20774A |
| 1217:7130 | 1462:4327 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 0DCF53C3D6 |
| 1217:7130 | 1462:63f6 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | BA35BAD99E |
| 1217:7130 | 1462:6440 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 43D96E36AB |
| 1217:7130 | 1462:7190 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | AB28AB5B76 |
| 1217:7130 | 1462:7220 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | B6DB68C949 |
| 1217:7130 | 14ff:a003 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 7EE061C41D |
| 1217:7130 | 1631:0188 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 7E9A381494 |
| 1217:7130 | 1631:018c | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 3FCA6C42B5 |
| 1217:7130 | 1631:c218 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 7817BF7259 |
| 1217:7130 | 1734:10b8 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 6D68CE16BD |
| 1217:7130 | 1734:10c7 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | 8B444CC339 |
| 1217:7130 | 17aa:3a21 | O2 Micro        | Integrated MS/xD Cont... | 100%   |          | BF3EE678DA |
| 1217:8130 | 1025:019f | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | 806ABC807D |
| 1217:8130 | 1025:038b | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | 18D1FC7788 |
| 1217:8130 | 1028:02bb | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | 95DC1639D3 |
| 1217:8130 | 1028:02bc | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | F2747CCCC2 |
| 1217:8130 | 1028:02c0 | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | 9A7F9AAED3 |
| 1217:8130 | 1028:02ea | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | 5857AFEA78 |
| 1217:8130 | 1028:02eb | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | 31C1B6A828 |
| 1217:8130 | 1028:041b | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | 3AAE3F0B4B |
| 1217:8130 | 10cf:1568 | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | 9B2FC1E55F |
| 1217:8130 | 1179:ff50 | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | 721A4DF615 |
| 1217:8130 | 17aa:3068 | O2 Micro        | Integrated MS/MSPRO/x... | 100%   |          | 27E7D42D53 |
| 1217:8231 | 1028:0493 | O2 Micro        | O2Micro Integrated MS... | 100%   |          | 3627E6BB56 |
| 1217:8231 | 1028:04a9 | O2 Micro        | O2Micro Integrated MS... | 100%   |          | 41E38AE50A |
| 1217:8231 | 1028:04e4 | O2 Micro        | O2Micro Integrated MS... | 100%   |          | 0BDB8E28F5 |
| 1217:8231 | 1bcf:a012 | O2 Micro        | O2Micro Integrated MS... | 100%   |          | 2708BA9972 |
| 1217:8330 | 1028:04a3 | O2 Micro        | OZ600 MS/xD Controller   | 100%   |          | 9F1F5B7EF7 |
| 1217:8330 | 1028:04a4 | O2 Micro        | OZ600 MS/xD Controller   | 100%   |          | 117E981EF3 |
| 1217:8330 | 10cf:16ae | O2 Micro        | OZ600 MS/xD Controller   | 100%   |          | CB4C0AC9A9 |
| 1217:8331 | 1028:0494 | O2 Micro        | O2 Flash Memory Card     | 100%   |          | EEAE263935 |
| 1217:8331 | 1028:049a | O2 Micro        | O2 Flash Memory Card     | 100%   |          | 33B9916878 |
| 1217:8331 | 1028:049b | O2 Micro        | O2 Flash Memory Card     | 100%   |          | 989DD7D36F |
| 1217:8331 | 1bcf:a013 | O2 Micro        | O2 Flash Memory Card     | 100%   |          | 1494683BB9 |
| 1261:3001 | 1261:3001 | Matsushita-K... | Storage controller       | 100%   |          | BC1A12A76F |
| 1aed:2001 | 1028:1f70 | SanDisk         | ioDrive2                 | 100%   |          | 1AFA47E662 |
| 1aed:2001 | 1590:006d | SanDisk         | ioDrive2                 | 100%   |          | 4A5147AC07 |
| 1aed:2001 | 1590:006f | SanDisk         | ioDrive2                 | 100%   |          | CD543E37E2 |
| 1aed:2001 | 1aed:2001 | SanDisk         | ioDrive2                 | 50%    | 4.15.0   | CD543E37E2 |
| 1aed:3002 | 1014:04d3 | SanDisk         | ioMemory HHHL            | 100%   |          | FB0D0A1860 |
| 1aed:3002 | 1137:013d | SanDisk         | ioMemory HHHL            | 100%   |          | 775B21277B |
| 8086:98fa | 8086:7270 | Intel           | Universal Flash Stora... | 100%   |          | 6D40FDC958 |
| ace1:0005 | ace1:0005 |                 | Storage controller       | 100%   |          | 22F215C605 |
| ace1:0006 | ace1:0006 |                 | Storage controller       | 100%   |          | EF20304D33 |

### Storage/ata (PCI)

17 out of 6438 (0.26%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1022:43b6 | 1b21:1062 | AMD             | X399 Series Chipset S... | 0.5%   | 3.10.0   | F29791E5C7 |
| 1022:43c8 | 1b21:1062 | AMD             | 400 Series Chipset SA... | 0%     | 3.10.0   | 21D76CDE28 |
| 1022:7801 | 103c:1992 | AMD             | FCH SATA Controller [... | 4.5%   | 4.1.25   | 2C52151F77 |
| 1022:7901 | 1022:7901 | AMD             | FCH SATA Controller [... | 0.2%   | 4.2.8    | 3C11A0856C |
| 1022:7901 | 1043:87c0 | AMD             | FCH SATA Controller [... | 0.2%   | 4.9.155  | 21D76CDE28 |
| 1022:7901 | 1462:7b92 | AMD             | FCH SATA Controller [... | 14.3%  | 5.4.0    | F29791E5C7 |
| 11ab:6141 | 1043:81d6 | Marvell Tech... | 88SE614x SATA II PCI-... | 100%   |          | 9EA64D6592 |
| 1b4b:9130 | 1043:8438 | Marvell Tech... | 88SE9128 PCIe SATA 6 ... | 0.6%   | 3.14.22  | 513772FEBC |
| 1b4b:9183 | 1b4b:9183 | Marvell Tech... | 88SS9183 PCIe SSD Con... | 1.4%   | 4.1.33   | 5E07806B7E |
| 8086:02d3 | 17aa:3802 | Intel           | Comet Lake SATA AHCI ... | 2%     | 5.3.0    | 78ECA17C40 |
| 8086:1c03 | 1179:fc50 | Intel           | 6 Series/C200 Series ... | 1.2%   | 3.14.44  | 046BFED81F |
| 8086:2929 | 103c:306b | Intel           | 82801IBM/IEM (ICH9M/I... | 5.6%   | 3.14.44  | 93C0EF7223 |
| 8086:9c03 | 17aa:3978 | Intel           | 8 Series SATA Control... | 0.2%   | 3.14.25  | B3B3794709 |
| 8086:9d03 | 1028:0816 | Intel           | Sunrise Point-LP SATA... | 5.9%   | 4.15.0   | 894BD38B38 |
| 8086:a103 | 103c:83bb | Intel           | HM170/QM170 Chipset S... | 4.3%   | 5.0.0    | 20EA46B0CE |
| 8086:a353 | 1028:087c | Intel           | Cannon Lake Mobile PC... | 1.5%   | 4.15.0   | 7B17868903 |
| 8086:a353 | 1028:0905 | Intel           | Cannon Lake Mobile PC... | 1.3%   | 4.15.0   | 293A792A22 |

### Storage/ide (PCI)

41 out of 4527 (0.91%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1002:439c | 1043:82ef | AMD             | SB7x0/SB8x0/SB9x0 IDE... | 0.6%   | 3.14.15  | 32AD3B2344 |
| 1002:439c | 1043:8389 | AMD             | SB7x0/SB8x0/SB9x0 IDE... | 0.1%   | 3.10.0   | AF37124D62 |
| 1002:439c | 1458:5002 | AMD             | SB7x0/SB8x0/SB9x0 IDE... | 0.1%   | 3.10.0   | 9FF481D661 |
| 1002:439c | 1462:7640 | AMD             | SB7x0/SB8x0/SB9x0 IDE... | 3.6%   | 4.1.15   | CC4B365068 |
| 1002:439c | 1849:439c | AMD             | SB7x0/SB8x0/SB9x0 IDE... | 0.1%   | 3.14.25  | 9FCF5D6433 |
| 1022:780c | 103c:22c8 | AMD             | FCH IDE Controller       | 11.1%  | 4.1.15   | EDC8ED595B |
| 1022:780c | 103c:3593 | AMD             | FCH IDE Controller       | 2.1%   | 3.10.42  | 65917EBD9D |
| 1022:780c | 1458:5002 | AMD             | FCH IDE Controller       | 0.6%   | 3.14.25  | 1013DC1D5F |
| 1022:780c | 1458:b002 | AMD             | FCH IDE Controller       | 10%    | 4.1.38   | FA543553EC |
| 10de:0053 | 1043:815a | Nvidia          | CK804 IDE                | 3%     | 3.10.19  | A6659EE127 |
| 10de:03ec | 1849:03ec | Nvidia          | MCP61 IDE                | 0.1%   | 3.14.15  | C8888818C9 |
| 10de:03f6 | 1849:03f6 | Nvidia          | MCP61 SATA Controller    | 0.1%   | 3.14.15  | C8888818C9 |
| 10de:056c | 1631:e038 | Nvidia          | MCP73 IDE Controller     | 12.5%  | 4.15.0   | 8CBA2E7FA8 |
| 11ab:6101 | 11ab:6101 | Marvell Tech... | 88SE6101/6102 single-... | 0.4%   | 3.13.0   | CCA71067AA |
| 1283:8213 | 1458:b000 | Integrated T... | IT8213 IDE Controller    | 1.2%   | 3.10.42  | 13ACEC4985 |
| 197b:0368 | 197b:1368 | JMicron Tech... | JMB368 IDE controller    | 1.1%   | 3.14.44  | DA311C1D96 |
| 197b:2363 | 1458:b000 | JMicron Tech... | JMB363 SATA/IDE Contr... | 0.1%   | 3.10.0   | C1CD5017A5 |
| 197b:2363 | 1462:7522 | JMicron Tech... | JMB363 SATA/IDE Contr... | 5%     | 4.1.16   | 335083A19F |
| 197b:2368 | 1458:b000 | JMicron Tech... | JMB368 IDE controller    | 0.2%   | 3.14.33  | CFAD3DA667 |
| 197b:2368 | 1462:7636 | JMicron Tech... | JMB368 IDE controller    | 10%    | 4.1.19   | 48D4121155 |
| 1b21:0611 | 1b21:1060 | ASMedia Tech... | ASM1061 SATA IDE Cont... | 6.7%   | 3.14.25  | 98BA9E428E |
| 1b4b:914d | 1043:8400 | Marvell Tech... | 88SE914D SATA-600 Con... | 5.1%   | 4.1.16   | 2655172FC1 |
| 8086:1d3c | 1028:05d4 | Intel           | C600/X79 series chips... | 12.5%  | 5.4.0    | 19FB02CA4E |
| 8086:1d3c | 103c:158b | Intel           | C600/X79 series chips... | 4.3%   | 4.15.0   | 6BC73950DD |
| 8086:27c0 | 8086:27c0 | Intel           | NM10/ICH7 Family SATA... | 0.8%   | 3.14.39  | 37B1114873 |
| 8086:27df | 17aa:200c | Intel           | 82801G (ICH7 Family) ... | 1.7%   | 3.14.44  | E5C5CE1445 |
| 8086:27df | 8086:27df | Intel           | 82801G (ICH7 Family) ... | 1%     | 3.14.44  | 37B1114873 |
| 8086:2850 | 106b:00a3 | Intel           | 82801HM/HEM (ICH8M/IC... | 25%    | 4.10.0   | 64593DD4A6 |
| 8086:2996 | 1734:10b5 | Intel           | 82Q963/Q965 PT IDER C... | 25%    | 4.9.60   | D66BC8959A |
| 8086:29b6 | 1734:10fc | Intel           | 82Q35 Express PT IDER... | 4.8%   | 4.9.20   | BDC2121D7E |
| 8086:29b6 | 17aa:3038 | Intel           | 82Q35 Express PT IDER... | 14.3%  | 4.1.15   | 04D11E7B8C |
| 8086:2a06 | 17aa:20d3 | Intel           | Mobile PM965/GM965 PT... | 18.8%  | 3.14.53  | E672D3211C |
| 8086:2a46 | 103c:30e1 | Intel           | Mobile 4 Series Chips... | 15.4%  | 3.14.25  | D54424038E |
| 8086:2a46 | 103c:30eb | Intel           | Mobile 4 Series Chips... | 16.7%  | 3.14.15  | E416FA2A3B |
| 8086:2a46 | 103c:30ec | Intel           | Mobile 4 Series Chips... | 16.7%  | 5.4.0    | 9650848634 |
| 8086:2a46 | 10cf:1466 | Intel           | Mobile 4 Series Chips... | 100%   |          | CD2222973B |
| 8086:2e16 | 17aa:3047 | Intel           | 4 Series Chipset PT I... | 2.8%   | 4.9.60   | 1A9DE278E0 |
| 8086:2e16 | 17aa:3048 | Intel           | 4 Series Chipset PT I... | 11.5%  | 4.1.15   | 2EBC1306C7 |
| 8086:2e16 | 17aa:3049 | Intel           | 4 Series Chipset PT I... | 23.5%  | 4.4.0    | 0784AFDDE4 |
| 8086:3b66 | 10cf:152e | Intel           | 5 Series/3400 Series ... | 3%     | 4.4.0    | 48FC4FF4DB |
| 8086:8d3c | 8086:7270 | Intel           | C610/X99 series chips... | 100%   |          | B2AD449201 |

### Storage/nvme (PCI)

11 out of 168 (6.55%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 106b:2001 | 106b:2001 | Apple           | S1X NVMe Controller      | 15.4%  | 4.9.20   | 3B124353D9 |
| 106b:2005 | 106b:1800 | Apple           | ANS2 NVMe Controller     | 8.8%   | 5.4.0    | 935B673683 |
| 10ec:5760 | 5760:10ec | Realtek Semi... | Realtek Non-Volatile ... | 3.6%   | 4.12.14  | 53EA23119E |
| 10ec:5762 | 10ec:5762 | Realtek Semi... | RTS5763DL NVMe SSD Co... | 1.1%   | 4.15.0   | 9ED3CA1095 |
| 144d:a802 | 144d:a801 | Samsung Elec... | NVMe SSD Controller S... | 0.4%   | 4.1.15   | A23E1AB6F7 |
| 144d:a808 | 144d:a801 | Samsung Elec... | NVMe SSD Controller S... | 0%     | 3.10.0   | D03C207BF2 |
| 1987:5008 | 1987:5008 | Phison Elect... | NVMe Storage Controller  | 0.9%   | 4.4.0    | 002D0884A9 |
| 1987:5012 | 1987:5012 | Phison Elect... | E12 NVMe Controller      | 0.2%   | 4.9.0    | EA6F3DC938 |
| 8086:2522 | 8086:0000 | Intel           | NVMe Optane Memory Se... | 100%   |          | 77B2CCC8F7 |
| 8086:2522 | 8086:3806 | Intel           | NVMe Optane Memory Se... | 2.9%   | 4.15.0   | 13353E2037 |
| 8086:f1a6 | 8086:390b | Intel           | SSD Pro 7600p/760p/E ... | 0.4%   | 3.10.0   | 1E7ADBE67A |

### Storage/raid (PCI)

38 out of 1287 (2.95%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1000:0010 | 0e11:4040 | Broadcom / LSI  | 53C1510                  | 100%   |          | 0B5D843F10 |
| 1000:0073 | 1000:9240 | Broadcom / LSI  | MegaRAID SAS 2008 [Fa... | 20%    | 5.3.0    | 38E4B2547A |
| 1000:0411 | 8086:1003 | Broadcom / LSI  | MegaRAID SAS 1068        | 100%   |          | 0E19261B88 |
| 1022:43bd | 1028:098e | AMD             | FCH RAID Controller      | 100%   |          | E1BC8D1CDD |
| 1022:43bd | 1849:43c8 | AMD             | FCH RAID Controller      | 100%   |          | 7E1BCF3383 |
| 1022:43bd | 1b21:1062 | AMD             | FCH RAID Controller      | 88.4%  | 5.3.0    | 220E356F41 |
| 1028:0016 | 1028:1f24 | Dell            | PowerEdge Expandable ... | 100%   |          | 650772B11D |
| 103c:193f | 103c:3381 | Hewlett-Packard | Dynamic Smart Array B... | 100%   |          | 3C08E6393F |
| 1095:1114 | 1095:5114 | Silicon Image   | RAID bus controller      | 100%   |          | 126A2B0E4F |
| 1095:3132 | 1043:819f | Silicon Image   | SiI 3132 Serial ATA R... | 2.2%   | 3.0.28   | 193ECC62CF |
| 1103:0611 | 1103:0611 | HighPoint Te... | RAID bus controller      | 100%   |          | E8AECFE123 |
| 1103:0622 | 1103:0001 | HighPoint Te... | RocketRAID 622 2 Port... | 100%   |          | 64A313C9E3 |
| 1103:0622 | 1103:0100 | HighPoint Te... | RocketRAID 622 2 Port... | 100%   |          | 24D6E7E1CE |
| 1103:0640 | 1103:0001 | HighPoint Te... | RocketRAID 640 4 Port... | 100%   |          | C1648A7961 |
| 1103:2840 | 1103:0000 | HighPoint Te... | RAID bus controller      | 100%   |          | 7653740066 |
| 1103:7103 | 1103:0001 | HighPoint Te... | RAID bus controller      | 100%   |          | DF1A8A847C |
| 1103:7110 | 1103:0000 | HighPoint Te... | RAID bus controller      | 100%   |          | EA6F3DC938 |
| 1106:1241 | 1106:1241 | VIA Technolo... | RAID bus controller      | 100%   |          | 921BC861D9 |
| 117c:002c | 117c:002c | ATTO Technology | ExpressSAS R380          | 100%   |          | F233ABA040 |
| 1590:0045 | 1590:0045 | Hewlett-Packard | RAID bus controller      | 100%   |          | 3FAC52AF81 |
| 19e5:a25a |           | Huawei Techn... | HiSilicon RDE Engine     | 100%   |          | BD05C84564 |
| 6883:0dd4 | 6883:0dd4 |                 | RAID bus controller      | 100%   |          | 7211932892 |
| 8086:02d7 | 1028:0951 | Intel           | Comet Lake PCH-LP SAT... | 100%   |          | 1C83B9C63C |
| 8086:02d7 | 1043:1c51 | Intel           | Comet Lake PCH-LP SAT... | 100%   |          | C5079022A9 |
| 8086:02d7 | 1043:1db1 | Intel           | Comet Lake PCH-LP SAT... | 100%   |          | F38D5CCA67 |
| 8086:06d6 | 1028:09a4 | Intel           | 400 Series Chipset Fa... | 50%    | 5.9.0    | 34E1267A80 |
| 8086:06d6 | 1043:8694 | Intel           | 400 Series Chipset Fa... | 33.3%  | 5.8.0    | 925A360F1F |
| 8086:06d6 | 1462:7c99 | Intel           | 400 Series Chipset Fa... | 100%   |          | B2DE3AF507 |
| 8086:2822 | 1043:8694 | Intel           | SATA Controller [RAID... | 0.5%   | 4.4.0    | 9578024712 |
| 8086:43d6 | 1043:8694 | Intel           | 500 Series Chipset Fa... | 66.7%  | 5.10.0   | C73E7C5DA9 |
| 8086:9a0b | 1028:0a25 | Intel           | Volume Management Dev... | 20%    | 5.4.0    | DCC3B1005E |
| 8086:9a0b | 14c0:012d | Intel           | Volume Management Dev... | 20%    | 5.8.0    | 89AE55D07E |
| 8086:a386 | 1028:09b6 | Intel           | 300 Series Chipset Fa... | 50%    | 5.12.2   | C798A114F2 |
| 8086:a386 | 1043:8694 | Intel           | 300 Series Chipset Fa... | 50%    | 5.8.0    | 503BF43E35 |
| 8086:a386 | 1462:7c88 | Intel           | 300 Series Chipset Fa... | 100%   |          | 972C8BFC2F |
| 8086:a386 | 1849:a382 | Intel           | 300 Series Chipset Fa... | 100%   |          | B83DE8C4AF |
| 9005:0285 | 9005:0290 | Adaptec         | AAC-RAID                 | 100%   |          | 591107EC98 |
| 9005:0285 | 9005:02d1 | Adaptec         | AAC-RAID                 | 7.7%   | 4.15.0   | 591107EC98 |

### System peripheral (PCI)

192 out of 889 (21.60%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 0014:7a0b |           | Loongson Tec... | SPI Controller           | 100%   |          | DD319B8387 |
| 0180:0592 | 003c:30d6 |                 | System peripheral        | 100%   |          | 4BDD603282 |
| 0180:0843 | 003c:30d6 |                 | System peripheral        | 100%   |          | 4BDD603282 |
| 0180:0852 | 003c:30d6 |                 | System peripheral        | 100%   |          | 4BDD603282 |
| 0e11:a0f0 | 0e11:b0f3 | Compaq Computer | Advanced System Manag... | 100%   |          | 0B5D843F10 |
| 0e11:b203 | 0e11:b206 | Compaq Computer | Integrated Lights Out... | 100%   |          | BF8AB3D150 |
| 0e11:b203 | 103c:3305 | Compaq Computer | Integrated Lights Out... | 87.7%  | 4.9.60   | 2ED58CCD22 |
| 103c:3306 | 103c:3309 | Hewlett-Packard | Integrated Lights-Out... | 84.4%  | 2.6.32   | C56840DF98 |
| 103c:3306 | 103c:330e | Hewlett-Packard | Integrated Lights-Out... | 60%    | 5.9.16   | BB50BB3A46 |
| 103c:3306 | 103c:3381 | Hewlett-Packard | Integrated Lights-Out... | 68.8%  | 2.6.32   | A4B9BC232A |
| 103c:3306 | 1590:00e4 | Hewlett-Packard | Integrated Lights-Out... | 33.3%  | 3.10.0   | AB3C1BEE64 |
| 104c:8201 | 103c:006b | Texas Instru... | PCI1620 Firmware Load... | 100%   |          | 5171D8BC33 |
| 104c:8201 | 103c:006d | Texas Instru... | PCI1620 Firmware Load... | 100%   |          | 564B583FED |
| 104c:8201 | 103c:08b0 | Texas Instru... | PCI1620 Firmware Load... | 100%   |          | 316E375A5C |
| 104c:8204 | 1028:0139 | Texas Instru... | PCI7410/7510/7610 PCI... | 100%   |          | 1629FF31A1 |
| 104c:8204 | 1028:014e | Texas Instru... | PCI7410/7510/7610 PCI... | 100%   |          | 0493B906A1 |
| 10b5:2065 | 10b5:9030 | PLX Technology  | System peripheral        | 100%   |          | BF5B58520E |
| 10b5:8609 | 10b5:8609 | PLX Technology  | PEX 8609 8-lane, 8-Po... | 50%    | 5.3.0    | E8AECFE123 |
| 1179:0805 | 1179:0001 | Toshiba Amer... | SD TypA Controller       | 40%    | 4.1.34   | 6ED70A9B46 |
| 1180:0576 | 10cf:1256 | Ricoh           | R5C576 SD Bus Host Ad... | 100%   |          | 4DCFB332DF |
| 1180:0576 | ffff:ffff | Ricoh           | R5C576 SD Bus Host Ad... | 100%   |          | 116C24A4D7 |
| 1180:0592 | 1028:02a0 | Ricoh           | R5C592 Memory Stick B... | 3.3%   | 3.14.53  | C5E6461593 |
| 1180:0592 | 103c:30b5 | Ricoh           | R5C592 Memory Stick B... | 40%    | 4.1.38   | EFFFE561DA |
| 1180:0592 | 1043:1127 | Ricoh           | R5C592 Memory Stick B... | 100%   |          | 79A40B4127 |
| 1180:0592 | 1043:1827 | Ricoh           | R5C592 Memory Stick B... | 33.3%  | 5.4.0    | 5B8E446BE1 |
| 1180:0592 | 17aa:20ca | Ricoh           | R5C592 Memory Stick B... | 1.5%   | 3.14.25  | FE8FFB1FC3 |
| 1180:0592 | 17aa:210c | Ricoh           | R5C592 Memory Stick B... | 6.5%   | 4.1.13   | A53BF69F31 |
| 1180:0843 | 1028:0263 | Ricoh           | R5C843 MMC Host Contr... | 100%   |          | 079101F502 |
| 1180:0843 | 1043:1827 | Ricoh           | R5C843 MMC Host Contr... | 100%   |          | 5B8E446BE1 |
| 1180:0852 | 1025:0121 | Ricoh           | xD-Picture Card Contr... | 1.5%   | 3.14.44  | 7CF5D7B04A |
| 1180:0852 | 1025:0126 | Ricoh           | xD-Picture Card Contr... | 2.2%   | 3.14.39  | D878DBB71E |
| 1180:0852 | 1028:0272 | Ricoh           | xD-Picture Card Contr... | 7.7%   | 4.15.0   | 2A2617D846 |
| 1180:0852 | 1028:029f | Ricoh           | xD-Picture Card Contr... | 7.7%   | 4.1.15   | 44C743E996 |
| 1180:0852 | 1028:02a0 | Ricoh           | xD-Picture Card Contr... | 3.3%   | 3.14.53  | C5E6461593 |
| 1180:0852 | 103c:1520 | Ricoh           | xD-Picture Card Contr... | 3.6%   | 3.10.42  | E7152C06C4 |
| 1180:0852 | 103c:1521 | Ricoh           | xD-Picture Card Contr... | 14.1%  | 4.1.15   | FFC46C9472 |
| 1180:0852 | 103c:30b5 | Ricoh           | xD-Picture Card Contr... | 40%    | 4.1.38   | EFFFE561DA |
| 1180:0852 | 103c:30c3 | Ricoh           | xD-Picture Card Contr... | 14.3%  | 4.1.34   | B65B21F334 |
| 1180:0852 | 103c:30cd | Ricoh           | xD-Picture Card Contr... | 3%     | 3.2.0    | 19CDA851D2 |
| 1180:0852 | 1043:1127 | Ricoh           | xD-Picture Card Contr... | 100%   |          | 79A40B4127 |
| 1180:0852 | 1043:1567 | Ricoh           | xD-Picture Card Contr... | 11.1%  | 3.14.44  | 31DD762F09 |
| 1180:0852 | 1043:1827 | Ricoh           | xD-Picture Card Contr... | 33.3%  | 5.4.0    | 5B8E446BE1 |
| 1180:0852 | 1043:1877 | Ricoh           | xD-Picture Card Contr... | 2.7%   | 3.0.28   | 70CC866946 |
| 1180:0852 | 1043:1897 | Ricoh           | xD-Picture Card Contr... | 6.4%   | 3.14.44  | 8ABF85E052 |
| 1180:0852 | 1631:c213 | Ricoh           | xD-Picture Card Contr... | 33.3%  | 5.4.0    | 5A6ABBD8F4 |
| 1180:0852 | 1734:10ad | Ricoh           | xD-Picture Card Contr... | 10%    | 4.1.33   | D6BC4ADE36 |
| 1180:0852 | 17aa:20cb | Ricoh           | xD-Picture Card Contr... | 7.6%   | 3.14.25  | 85DEF78A94 |
| 1180:0852 | 17aa:210d | Ricoh           | xD-Picture Card Contr... | 12.9%  | 4.1.13   | E6E9C572A0 |
| 1180:e230 | 1028:02bd | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | BF361A7ED3 |
| 1180:e230 | 1028:02fe | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 3664956B06 |
| 1180:e230 | 1028:0401 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 3D8F2E2B96 |
| 1180:e230 | 1028:0402 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | C55F3CA871 |
| 1180:e230 | 1028:0413 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 8AF25501BB |
| 1180:e230 | 1028:0442 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | D1ECE8006F |
| 1180:e230 | 103c:1455 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 3A32FA9C5A |
| 1180:e230 | 103c:146d | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 47BCDF1BC3 |
| 1180:e230 | 103c:146e | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 74C2B345B8 |
| 1180:e230 | 103c:1471 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | B192718656 |
| 1180:e230 | 103c:1722 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 638A36ACC8 |
| 1180:e230 | 103c:1726 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 759D141031 |
| 1180:e230 | 103c:307e | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 7AB10A9CE6 |
| 1180:e230 | 1043:1b97 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 5977217568 |
| 1180:e230 | 1043:1f47 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 1543283EC3 |
| 1180:e230 | 104d:905a | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 537D05799C |
| 1180:e230 | 104d:905e | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 92C2DD4C5F |
| 1180:e230 | 104d:9060 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 90A75A8826 |
| 1180:e230 | 104d:9066 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | D2527D279C |
| 1180:e230 | 104d:9067 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 6DE1770865 |
| 1180:e230 | 104d:9069 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 188765C8F8 |
| 1180:e230 | 104d:9071 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | E79E0F2021 |
| 1180:e230 | 104d:9072 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 4398B323B3 |
| 1180:e230 | 104d:9074 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 68937CF6BB |
| 1180:e230 | 104d:907a | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 76B08BA6D3 |
| 1180:e230 | 1179:0001 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | BD61CCC317 |
| 1180:e230 | 1179:ff1e | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 04F947FD57 |
| 1180:e230 | 1179:ff40 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 50BAA8508F |
| 1180:e230 | 1179:ffc0 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 42449081BB |
| 1180:e230 | 1179:ffc7 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 2711AE5ECA |
| 1180:e230 | 17aa:2134 | Ricoh           | R5U2xx (R5U230 / R5U2... | 100%   |          | 29BCDE9934 |
| 1180:e232 | 104d:907e | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 626BFE0484 |
| 1180:e232 | 104d:9081 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 2DEA50C3B6 |
| 1180:e232 | 104d:9083 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 005AEEF791 |
| 1180:e232 | 104d:9086 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | C1F9CF2BE3 |
| 1180:e232 | 104d:9089 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 22921FB0B7 |
| 1180:e232 | 104d:908e | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 59BB8EC907 |
| 1180:e232 | 104d:9095 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | E61B623334 |
| 1180:e232 | 104d:9097 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 4657C4112A |
| 1180:e232 | 1179:0001 | Ricoh           | PCIe Memory Stick Hos... | 100%   |          | 0A547BA59A |
| 1180:e822 | 17aa:21cf | Ricoh           | MMC/SD Host Controller   | 1.8%   | 3.14.15  | 4CAE7DC78D |
| 1180:e822 | 17aa:21fb | Ricoh           | MMC/SD Host Controller   | 6.2%   | 4.9.20   | 657F2A7F37 |
| 1180:e823 | 17aa:21da | Ricoh           | PCIe SDXC/MMC Host Co... | 0.9%   | 4.1.22   | F9CF2CED7E |
| 1180:e823 | 17aa:21fb | Ricoh           | PCIe SDXC/MMC Host Co... | 2.5%   | 4.15.0   | 55427995B5 |
| 1217:7110 | 103c:0890 | O2 Micro        | OZ711Mx 4-in-1 Memory... | 100%   |          | 44DF53B183 |
| 1217:7110 | 10cf:11c4 | O2 Micro        | OZ711Mx 4-in-1 Memory... | 100%   |          | EA732BEA27 |
| 1217:7110 | 1584:3008 | O2 Micro        | OZ711Mx 4-in-1 Memory... | 100%   |          | E9BC9B3C8A |
| 1217:7110 | 1734:106c | O2 Micro        | OZ711Mx 4-in-1 Memory... | 100%   |          | BFFEEEDE0D |
| 14e4:16be | 1025:0500 | Broadcom        | BCM57765/57785 MS Car... | 100%   |          | B26958098C |
| 14e4:16be | 1025:0504 | Broadcom        | BCM57765/57785 MS Car... | 100%   |          | 500756649B |
| 14e4:16be | 1025:0599 | Broadcom Lim... | BCM57765/57785 MS Car... | 100%   |          | 6372F79BC4 |
| 14e4:16be | 1025:0605 | Broadcom Lim... | BCM57765/57785 MS Car... | 100%   |          | 853337664F |
| 14e4:16be | 1025:0647 | Broadcom        | BCM57765/57785 MS Car... | 100%   |          | 8770317D57 |
| 14e4:16bf | 1025:0500 | Broadcom        | BCM57765/57785 xD-Pic... | 100%   |          | B26958098C |
| 14e4:16bf | 1025:0504 | Broadcom        | BCM57765/57785 xD-Pic... | 100%   |          | 500756649B |
| 14e4:16bf | 1025:0599 | Broadcom Lim... | BCM57765/57785 xD-Pic... | 100%   |          | 6372F79BC4 |
| 14e4:16bf | 1025:0605 | Broadcom Lim... | BCM57765/57785 xD-Pic... | 100%   |          | 853337664F |
| 14e4:16bf | 1025:0647 | Broadcom        | BCM57765/57785 xD-Pic... | 100%   |          | 8770317D57 |
| 197b:2382 | 1297:2020 | JMicron Tech... | SD/MMC Host Controller   | 3.6%   | 4.15.0   | D826611187 |
| 197b:2384 | 1019:2238 | JMicron Tech... | xD Host Controller       | 100%   |          | 7E782321C8 |
| 197b:2384 | 1019:2689 | JMicron Tech... | xD Host Controller       | 100%   |          | 7CF090FB8F |
| 197b:2384 | 1025:0128 | JMicron Tech... | xD Host Controller       | 100%   |          | EA94093CD5 |
| 197b:2384 | 1025:013b | JMicron Tech... | xD Host Controller       | 100%   |          | AB3A38954A |
| 197b:2384 | 1025:013d | JMicron Tech... | xD Host Controller       | 100%   |          | DB999A95A6 |
| 197b:2384 | 1025:013e | JMicron Tech... | xD Host Controller       | 100%   |          | B563FF6430 |
| 197b:2384 | 1025:0140 | JMicron Tech... | xD Host Controller       | 100%   |          | 7157A6069B |
| 197b:2384 | 1025:0142 | JMicron Tech... | xD Host Controller       | 100%   |          | 6780FC2A44 |
| 197b:2384 | 1025:0143 | JMicron Tech... | xD Host Controller       | 100%   |          | 310A169187 |
| 197b:2384 | 1025:0144 | JMicron Tech... | xD Host Controller       | 100%   |          | 8EC4FA1849 |
| 197b:2384 | 1025:0145 | JMicron Tech... | xD Host Controller       | 100%   |          | 147AA532D6 |
| 197b:2384 | 1025:0146 | JMicron Tech... | xD Host Controller       | 100%   |          | 649CB24583 |
| 197b:2384 | 1025:014b | JMicron Tech... | xD Host Controller       | 100%   |          | EBB35F1079 |
| 197b:2384 | 1025:015b | JMicron Tech... | xD Host Controller       | 100%   |          | F88D38A138 |
| 197b:2384 | 1025:0160 | JMicron Tech... | xD Host Controller       | 100%   |          | BBCDDB4D27 |
| 197b:2384 | 1025:0167 | JMicron Tech... | xD Host Controller       | 100%   |          | CBE6A288F1 |
| 197b:2384 | 1025:0200 | JMicron Tech... | xD Host Controller       | 100%   |          | EB8F15B14D |
| 197b:2384 | 1025:0259 | JMicron Tech... | xD Host Controller       | 100%   |          | 432C7B7B63 |
| 197b:2384 | 1025:0260 | JMicron Tech... | xD Host Controller       | 100%   |          | AFEFC6A739 |
| 197b:2384 | 1025:0311 | JMicron Tech... | xD Host Controller       | 100%   |          | 57FFADB7C2 |
| 197b:2384 | 1025:042f | JMicron Tech... | xD Host Controller       | 100%   |          | 1395FA2E0F |
| 197b:2384 | 103c:1489 | JMicron Tech... | xD Host Controller       | 100%   |          | 603E26F80F |
| 197b:2384 | 103c:2a97 | JMicron Tech... | xD Host Controller       | 100%   |          | EDEACD39C6 |
| 197b:2384 | 103c:2aa2 | JMicron Tech... | xD Host Controller       | 100%   |          | CEEBC6A90B |
| 197b:2384 | 103c:2aa6 | JMicron Tech... | xD Host Controller       | 100%   |          | 3EE3ED2E83 |
| 197b:2384 | 103c:30f4 | JMicron Tech... | xD Host Controller       | 100%   |          | A87C66370A |
| 197b:2384 | 103c:30f7 | JMicron Tech... | xD Host Controller       | 100%   |          | E15FD6726E |
| 197b:2384 | 103c:30fb | JMicron Tech... | xD Host Controller       | 100%   |          | 229CCDA963 |
| 197b:2384 | 103c:30fc | JMicron Tech... | xD Host Controller       | 100%   |          | 47E6366EB5 |
| 197b:2384 | 103c:30fe | JMicron Tech... | xD Host Controller       | 100%   |          | F2648EDD87 |
| 197b:2384 | 103c:3600 | JMicron Tech... | xD Host Controller       | 100%   |          | 2DF1512442 |
| 197b:2384 | 103c:3603 | JMicron Tech... | xD Host Controller       | 100%   |          | 14F176409D |
| 197b:2384 | 103c:3610 | JMicron Tech... | xD Host Controller       | 100%   |          | DEAD2B5B56 |
| 197b:2384 | 103c:361b | JMicron Tech... | xD Host Controller       | 100%   |          | C3E0C828A1 |
| 197b:2384 | 103c:3624 | JMicron Tech... | xD Host Controller       | 100%   |          | 17DCAC4931 |
| 197b:2384 | 103c:3628 | JMicron Tech... | xD Host Controller       | 100%   |          | DCE60F14E1 |
| 197b:2384 | 103c:3629 | JMicron Tech... | xD Host Controller       | 100%   |          | F1CC639EDF |
| 197b:2384 | 103c:3636 | JMicron Tech... | xD Host Controller       | 100%   |          | FF31E18FB9 |
| 197b:2384 | 103c:363c | JMicron Tech... | xD Host Controller       | 100%   |          | 662A781C83 |
| 197b:2384 | 103c:363e | JMicron Tech... | xD Host Controller       | 100%   |          | A9E05596D5 |
| 197b:2384 | 103c:3659 | JMicron Tech... | xD Host Controller       | 100%   |          | 827D185513 |
| 197b:2384 | 103c:365c | JMicron Tech... | xD Host Controller       | 100%   |          | 727672085E |
| 197b:2384 | 103c:7001 | JMicron Tech... | xD Host Controller       | 100%   |          | 298015ECAC |
| 197b:2384 | 103c:7010 | JMicron Tech... | xD Host Controller       | 100%   |          | 6E70B36184 |
| 197b:2384 | 1043:1a07 | JMicron Tech... | xD Host Controller       | 100%   |          | F34139992A |
| 197b:2384 | 1071:9525 | JMicron Tech... | xD Host Controller       | 100%   |          | 4B29F60F4E |
| 197b:2384 | 1179:fd30 | JMicron Tech... | xD Host Controller       | 100%   |          | 0946B14D18 |
| 197b:2384 | 1179:fdb0 | JMicron Tech... | xD Host Controller       | 100%   |          | 084F254E1F |
| 197b:2384 | 1179:ff02 | JMicron Tech... | xD Host Controller       | 100%   |          | 5DA06FD6B1 |
| 197b:2384 | 1179:ff08 | JMicron Tech... | xD Host Controller       | 100%   |          | 0173C2AFDA |
| 197b:2384 | 1462:100f | JMicron Tech... | xD Host Controller       | 100%   |          | CB6654E18B |
| 197b:2384 | 1462:6510 | JMicron Tech... | xD Host Controller       | 100%   |          | 93F0D8D3F2 |
| 197b:2384 | 1462:6520 | JMicron Tech... | xD Host Controller       | 100%   |          | 12132D4EBD |
| 197b:2384 | 14c0:0031 | JMicron Tech... | xD Host Controller       | 100%   |          | 56B05900A0 |
| 197b:2384 | 152d:0834 | JMicron Tech... | xD Host Controller       | 100%   |          | C6D0242C42 |
| 197b:2384 | 1558:0803 | JMicron Tech... | xD Host Controller       | 100%   |          | 0E33922AF7 |
| 197b:2384 | 1558:0806 | JMicron Tech... | xD Host Controller       | 100%   |          | F3BF4D62C0 |
| 197b:2384 | 1734:113b | JMicron Tech... | xD Host Controller       | 100%   |          | 68F95EA08D |
| 197b:2384 | 1734:113d | JMicron Tech... | xD Host Controller       | 100%   |          | BD5D293529 |
| 197b:2384 | 1734:113f | JMicron Tech... | xD Host Controller       | 100%   |          | E6848FB30E |
| 197b:2384 | 17aa:2130 | JMicron Tech... | xD Host Controller       | 100%   |          | A687D09DE6 |
| 197b:2384 | 17aa:3051 | JMicron Tech... | xD Host Controller       | 100%   |          | 0812A4EFC1 |
| 197b:2384 | 17aa:3602 | JMicron Tech... | xD Host Controller       | 100%   |          | C25FDFE643 |
| 197b:2384 | 17aa:3881 | JMicron Tech... | xD Host Controller       | 100%   |          | F1C5A43472 |
| 197b:2384 | 17c0:10da | JMicron Tech... | xD Host Controller       | 100%   |          | 74D6F0A5E2 |
| 197b:2384 | 17c0:408c | JMicron Tech... | xD Host Controller       | 100%   |          | 4A528AFFEB |
| 197b:2387 | 17aa:3921 | JMicron Tech... | SD/MMC Host Controller   | 100%   |          | A51ABD79CE |
| 197b:2389 | 17aa:3924 | JMicron Tech... | xD Host Controller       | 100%   |          | A51ABD79CE |
| 197b:2394 | 1025:050a | JMicron Tech... | xD Host Controller       | 100%   |          | 63D11EBB5A |
| 197b:2394 | 1028:0446 | JMicron Tech... | xD Host Controller       | 100%   |          | 5BCD793D64 |
| 197b:2394 | 1028:0468 | JMicron Tech... | xD Host Controller       | 100%   |          | 291B1C0A01 |
| 197b:2394 | 1028:050e | JMicron Tech... | xD Host Controller       | 100%   |          | 0FEA972B34 |
| 197b:2394 | 103c:2ac6 | JMicron Tech... | xD Host Controller       | 100%   |          | 90725B3C8A |
| 197b:2394 | 103c:2ae5 | JMicron Tech... | xD Host Controller       | 100%   |          | 025934D12A |
| 197b:2394 | 103c:2af2 | JMicron Tech... | xD Host Controller       | 100%   |          | F94C9AF809 |
| 197b:2394 | 103c:2b00 | JMicron Tech... | xD Host Controller       | 100%   |          | 048555EFF7 |
| 197b:2394 | 103c:3561 | JMicron Tech... | xD Host Controller       | 100%   |          | 90E0F93E8D |
| 197b:2394 | 1179:fc30 | JMicron Tech... | xD Host Controller       | 100%   |          | AABBAA4370 |
| 197b:2394 | 1462:107f | JMicron Tech... | xD Host Controller       | 100%   |          | 7EBAF712E3 |
| 197b:2394 | 14c0:006b | JMicron Tech... | xD Host Controller       | 100%   |          | C97368216B |
| 197b:2394 | 17aa:3976 | JMicron Tech... | xD Host Controller       | 100%   |          | 94D22E7673 |
| 197b:2394 | 17aa:3977 | JMicron Tech... | xD Host Controller       | 100%   |          | F088672FD6 |
| 197b:2394 | ffff:ffff | JMicron Tech... | xD Host Controller       | 100%   |          | 6F346C88EC |
| 19e5:a122 |           | Huawei Techn... | HiSilicon Embedded DM... | 12.5%  | 5.4.0    | 63BDABB5A4 |
| 1ac1:089a | 1ac1:089a | Global Unichip  | Coral Edge TPU           | 25%    | 5.4.0    | 0A01176CBE |

### Tv card (PCI)

10 out of 351 (2.85%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1131:7130 | 5ace:5050 | Philips Semi... | SAA7130 Video Broadca... | 3%     | 3.14.44  | D82F0A25EA |
| 1131:7133 | 16be:0007 | Philips Semi... | SAA7131/SAA7133/SAA71... | 25%    | 4.18.16  | 24A0914BA3 |
| 1131:7133 | 16be:0008 | Philips Semi... | SAA7131/SAA7133/SAA71... | 25%    | 4.18.16  | 24A0914BA3 |
| 1131:7134 | 16be:5000 | Philips Semi... | SAA7134/SAA7135HL Vid... | 20%    | 4.9.60   | D506D4320D |
| 11de:6057 | 1031:7efe | Zoran           | ZR36057PQC Video cutt... | 16.7%  | 3.14.44  | 9D96782463 |
| 11de:6057 | 1031:d801 | Zoran           | ZR36057PQC Video cutt... | 100%   |          | F700FF20C6 |
| 14f1:8800 | 8922:8888 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 70%    | 4.1.25   | 7011550263 |
| 14f1:8802 | 8922:8888 | Conexant Sys... | CX23880/1/2/3 PCI Vid... | 70%    | 4.1.25   | 7011550263 |
| 14f1:8880 | 1461:d439 | Conexant Sys... | CX23887/8 PCIe Broadc... | 11.1%  | 4.15.0   | D8325626F2 |
| 4444:0016 | 0070:8801 | Internext Co... | iTVC16 (CX23416) Vide... | 3%     | 4.1.15   | 8854FD6644 |

### Usb controller (PCI)

140 out of 22623 (0.62%)

| ID        | Subsystem | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------|-----------------|--------------------------|--------|----------|------------|
| 1002:4396 | 1002:4396 | AMD             | SB7x0/SB8x0/SB9x0 USB... | 0%     | 3.10.0   | 012357C526 |
| 1002:4397 | 1002:4397 | AMD             | SB7x0/SB8x0/SB9x0 USB... | 0.1%   | 3.10.0   | 012357C526 |
| 1002:4397 | 1458:5004 | AMD             | SB7x0/SB8x0/SB9x0 USB... | 0%     | 3.10.0   | 0533339E4E |
| 1002:4399 | 1002:4399 | AMD             | SB7x0/SB8x0/SB9x0 USB... | 0.1%   | 3.10.0   | 012357C526 |
| 1002:4399 | 1458:5004 | AMD             | SB7x0/SB8x0/SB9x0 USB... | 0%     | 3.10.0   | 0533339E4E |
| 1022:7807 | 103c:1992 | AMD             | FCH USB OHCI Controller  | 4.2%   | 4.1.25   | 2C52151F77 |
| 1022:7807 | 103c:216f | AMD             | FCH USB OHCI Controller  | 5.3%   | 4.9.20   | E190391A64 |
| 1022:7807 | 1458:5004 | AMD             | FCH USB OHCI Controller  | 0.1%   | 3.14.25  | FA543553EC |
| 1022:7808 | 103c:1992 | AMD             | FCH USB EHCI Controller  | 4.2%   | 4.1.25   | 2C52151F77 |
| 1022:7808 | 103c:216f | AMD             | FCH USB EHCI Controller  | 5.3%   | 4.9.20   | E190391A64 |
| 1022:7809 | 103c:1992 | AMD             | FCH USB OHCI Controller  | 4.2%   | 4.1.25   | 2C52151F77 |
| 1022:7809 | 1458:5004 | AMD             | FCH USB OHCI Controller  | 0.1%   | 3.14.25  | FA543553EC |
| 1022:7814 | 103c:1992 | AMD             | FCH USB XHCI Controller  | 4.3%   | 4.1.25   | 2C52151F77 |
| 1022:7814 | 103c:216f | AMD             | FCH USB XHCI Controller  | 5.3%   | 4.9.20   | E190391A64 |
| 1022:7914 | 103c:8331 | AMD             | FCH USB XHCI Controller  | 1.7%   | 4.9.20   | 30C73729A4 |
| 1033:0035 | 14c2:0105 | NEC Computers   | OHCI USB Controller      | 3.1%   | 3.14.25  | 65E45D0208 |
| 1033:0035 | 1631:0035 | NEC Computers   | OHCI USB Controller      | 100%   |          | CF4F87AEFD |
| 1033:0035 | ffff:ffff | NEC Computers   | OHCI USB Controller      | 66.7%  | 5.4.0    | ACE0E3FED5 |
| 1033:00e0 | 14c2:0205 | NEC Computers   | uPD72010x USB 2.0 Con... | 3.1%   | 3.14.25  | 65E45D0208 |
| 1033:00e0 | 1631:1600 | NEC Computers   | uPD72010x USB 2.0 Con... | 100%   |          | CF4F87AEFD |
| 1033:00e0 | 1799:0002 | NEC Computers   | uPD72010x USB 2.0 Con... | 3.8%   | 4.15.0   | A715A916F9 |
| 1033:00e0 | ffff:ffff | NEC Computers   | uPD72010x USB 2.0 Con... | 100%   |          | ACE0E3FED5 |
| 1033:0194 | 1033:0194 | NEC Computers   | uPD720200 USB 3.0 Hos... | 6.8%   | 4.13.0   | 1250C7DFBE |
| 1033:0194 | 1179:fc50 | NEC Computers   | uPD720200 USB 3.0 Hos... | 2%     | 3.14.44  | 046BFED81F |
| 1033:0194 | ffff:ffff | NEC Computers   | uPD720200 USB 3.0 Hos... | 1%     | 2.6.32   | C4006430A8 |
| 104c:8241 | 103c:17e2 | Texas Instru... | TUSB73x0 SuperSpeed U... | 23.5%  | 4.9.0    | E96EEBB6D7 |
| 104c:8241 | 103c:2ada | Texas Instru... | TUSB73x0 SuperSpeed U... | 2.6%   | 4.4.14   | 3BB5A2AB3E |
| 104c:8241 | 1854:0159 | Texas Instru... | TUSB73x0 SuperSpeed U... | 100%   |          | 41DFC50F20 |
| 106b:003f |           | Apple           | KeyLargo/Intrepid USB    | 100%   |          | 47DE429737 |
| 10b9:5239 | 1071:8351 | ULi Electronics | USB 2.0 Controller       | 75%    | 5.4.0    | 1088093ABA |
| 10de:005a | 1043:815a | Nvidia          | CK804 USB Controller     | 3%     | 3.10.19  | A6659EE127 |
| 10de:005b | 1043:815a | Nvidia          | CK804 USB Controller     | 3%     | 3.10.19  | A6659EE127 |
| 10de:03f1 | 1849:03f1 | Nvidia          | MCP61 USB 1.1 Controller | 0.1%   | 3.14.15  | C8888818C9 |
| 10de:03f2 | 1849:03f2 | Nvidia          | MCP61 USB 2.0 Controller | 0.1%   | 3.14.15  | C8888818C9 |
| 10de:1ad8 |           | Nvidia          | TU104 USB 3.1 Host Co... | 100%   |          | EEFA8BB9FA |
| 10de:1ada | 1028:098f | Nvidia          | TU106 USB 3.1 Host Co... | 3.1%   | 5.4.0    | 84387A75F7 |
| 10de:1ada | 1458:3fc1 | Nvidia          | TU106 USB 3.1 Host Co... | 15.4%  | 5.3.0    | 014FE23FC5 |
| 10de:1ada | 3842:2067 | Nvidia          | TU106 USB 3.1 Host Co... | 50%    | 4.12.14  | 5A5C05E953 |
| 10ec:816d | 1043:85b5 | Realtek Semi... | RTL811x EHCI host con... | 18.8%  | 4.18.0   | C6A901E853 |
| 1106:1104 | 1106:1104 | VIA Technolo... | USB Controller           | 100%   |          | 6B4E0A3965 |
| 1106:3038 | 1106:3038 | VIA Technolo... | VT82xx/62xx/VX700/8x0... | 0.5%   | 4.1.38   | 433FDCFFCA |
| 1106:3104 | 1106:3104 | VIA Technolo... | USB 2.0 EHCI-Complian... | 1.3%   | 4.1.38   | 69EBCB63DE |
| 1106:3104 | 1106:318a | VIA Technolo... | USB 2.0 EHCI-Complian... | 8.3%   | 4.1.25   | E56DD30CA2 |
| 1106:3432 | 1458:5007 | VIA Technolo... | VL800/801 xHCI USB 3.... | 1.5%   | 4.1.15   | 30536633CF |
| 1106:3483 | 1106:3483 | VIA Technolo... | VL805/806 xHCI USB 3.... | 0.5%   | 3.14.44  | A895BE79C6 |
| 1106:3483 | 1458:5007 | VIA Technolo... | VL805/806 xHCI USB 3.... | 12.7%  | 3.10.0   | 25AD87E22B |
| 1233:00e0 | 1233:00e0 | Bus-Tech        | USB Controller           | 100%   |          | FF71C3BFE9 |
| 1306:3104 | 1306:3038 | Duet Technol... | USB Controller           | 100%   |          | 84FEB3D2F6 |
| 1912:0014 |           | Renesas Tech... | uPD720201 USB 3.0 Hos... | 1.4%   | 4.1.25   | 5F0BF94D1C |
| 1912:0014 | 103c:1996 | Renesas Tech... | uPD720201 USB 3.0 Hos... | 3%     | 4.4.4    | 7CF6D970EC |
| 1912:0014 | 1912:0014 | Renesas Tech... | uPD720201 USB 3.0 Hos... | 1.2%   | 3.10.0   | E3CF1A821F |
| 1912:0014 | ffff:ffff | Renesas Tech... | uPD720201 USB 3.0 Hos... | 0.4%   | 3.10.0   | 6E75D68FEA |
| 1912:0015 |           | Renesas Tech... | uPD720202 USB 3.0 Hos... | 0.6%   | 3.14.25  | 740FC92339 |
| 1912:0015 | 1462:7866 | Renesas Tech... | uPD720202 USB 3.0 Hos... | 50%    | 5.7.17   | BBBF80A444 |
| 1912:0015 | ffff:ffff | Renesas Tech... | uPD720202 USB 3.0 Hos... | 2.3%   | 3.14.44  | 2C7A11667A |
| 1b21:1042 | 1043:1059 | ASMedia Tech... | ASM1042 SuperSpeed US... | 0.2%   | 3.10.34  | 6C9107BCAD |
| 1b21:1042 | 1043:8488 | ASMedia Tech... | ASM1042 SuperSpeed US... | 0.1%   | 3.10.0   | 254277B249 |
| 1b21:1042 | 1234:5678 | ASMedia Tech... | ASM1042 SuperSpeed US... | 100%   |          | AE8835794B |
| 1b21:1042 | 1297:6007 | ASMedia Tech... | ASM1042 SuperSpeed US... | 100%   |          | E32AB899C0 |
| 1b21:1042 | 1462:7693 | ASMedia Tech... | ASM1042 SuperSpeed US... | 3.1%   | 3.14.15  | FC5F1E6327 |
| 1b21:1042 | 1849:1042 | ASMedia Tech... | ASM1042 SuperSpeed US... | 1.5%   | 3.10.0   | 101E707D3C |
| 1b21:1343 | 1b21:1343 | ASMedia Tech... | ASM1143 USB 3.1 Host ... | 2%     | 4.9.60   | C76564A1E5 |
| 1b6f:7023 | 1458:5007 | Etron Techno... | EJ168 USB 3.0 Host Co... | 0.1%   | 3.10.0   | 746ED0F095 |
| 1b6f:7052 | 1849:7052 | Etron Techno... | EJ188/EJ198 USB 3.0 H... | 0.3%   | 3.14.33  | C76564A1E5 |
| 1b73:1000 | 1043:1039 | Fresco Logic    | FL1000G USB 3.0 Host ... | 0.5%   | 3.0.28   | 0EAEBD5FCA |
| 1b73:1100 | 1b73:1100 | Fresco Logic    | FL1100 USB 3.0 Host C... | 1.5%   | 3.14.44  | 409C6BF61C |
| 8086:06ed | 1028:098f | Intel           | Comet Lake USB 3.1 xH... | 2.6%   | 5.4.0    | 84387A75F7 |
| 8086:0f34 | 1043:8534 | Intel           | Atom Processor Z36xxx... | 50%    | 4.1.19   | D77C773BC7 |
| 8086:0f34 | 17aa:3986 | Intel           | Atom Processor Z36xxx... | 9.1%   | 3.14.44  | EC4481EC60 |
| 8086:0f37 | 8086:0f37 | Intel           | Atom Processor Z36xxx... | 9.7%   | 3.14.44  | 71CEC0648D |
| 8086:0f37 | 8086:7270 | Intel           | Atom Processor Z36xxx... | 7.1%   | 4.1.16   | C3623326F4 |
| 8086:1137 | 8086:0000 | Intel           | Thunderbolt 4 NHI [Ma... | 50%    | 5.8.0    | 6969C309D4 |
| 8086:15db | 2222:1111 | Intel           | JHL6340 Thunderbolt 3... | 1.1%   | 4.4.0    | 4D17CC2498 |
| 8086:15ec | 1028:098f | Intel           | JHL7540 Thunderbolt 3... | 2.6%   | 5.4.0    | 84387A75F7 |
| 8086:1c26 | 1179:fc50 | Intel           | 6 Series/C200 Series ... | 1.1%   | 3.14.44  | 046BFED81F |
| 8086:1c2d | 1179:fc50 | Intel           | 6 Series/C200 Series ... | 1.1%   | 3.14.44  | 046BFED81F |
| 8086:1d26 | 8086:3582 | Intel           | C600/X79 series chips... | 100%   |          | 9F6D925B73 |
| 8086:1d2d | 8086:3582 | Intel           | C600/X79 series chips... | 100%   |          | 9F6D925B73 |
| 8086:1e26 | 1043:201f | Intel           | 7 Series/C216 Chipset... | 0.8%   | 3.10.34  | 3C52D09634 |
| 8086:1e26 | 1043:84ca | Intel           | 7 Series/C216 Chipset... | 0.1%   | 3.10.34  | 44E0CE8FC8 |
| 8086:1e2d | 1043:201f | Intel           | 7 Series/C216 Chipset... | 0.8%   | 3.10.34  | 3C52D09634 |
| 8086:1e2d | 1043:84ca | Intel           | 7 Series/C216 Chipset... | 0.1%   | 3.10.34  | 44E0CE8FC8 |
| 8086:1e31 | 1028:0533 | Intel           | 7 Series/C210 Series ... | 1.4%   | 4.9.20   | 8255A6BF31 |
| 8086:1e31 | 1028:0534 | Intel           | 7 Series/C210 Series ... | 1.9%   | 4.1.19   | 4FBBA78CD4 |
| 8086:1e31 | 103c:1970 | Intel           | 7 Series/C210 Series ... | 4%     | 3.14.44  | E2F0FC675A |
| 8086:1e31 | 1043:1447 | Intel           | 7 Series/C210 Series ... | 4.8%   | 3.14.44  | F23B5BF0DA |
| 8086:1e31 | 1043:84ca | Intel           | 7 Series/C210 Series ... | 0.1%   | 3.10.34  | 44E0CE8FC8 |
| 8086:1e31 | 104d:9095 | Intel           | 7 Series/C210 Series ... | 2.4%   | 3.14.25  | 2A2BD0A648 |
| 8086:1e31 | 1179:fb30 | Intel           | 7 Series/C210 Series ... | 12.5%  | 3.14.44  | C9DF2252FA |
| 8086:1e31 | 1458:5007 | Intel           | 7 Series/C210 Series ... | 0.3%   | 3.10.0   | 837D994165 |
| 8086:1e31 | 17aa:21f3 | Intel           | 7 Series/C210 Series ... | 0.4%   | 3.14.44  | 3085B68179 |
| 8086:1e31 | 17aa:21fa | Intel           | 7 Series/C210 Series ... | 0.4%   | 3.10.42  | 689257C05A |
| 8086:1e31 | 8086:7270 | Intel           | 7 Series/C210 Series ... | 0.3%   | 3.14.44  | E1CD5BD1F3 |
| 8086:22b7 | 17aa:380a | Intel           | USB Synopsys Controller  | 40%    | 5.3.11   | 9B1C3D7AC7 |
| 8086:22b7 | 8086:7270 | Intel           | USB Synopsys Controller  | 9.2%   | 4.9.9    | 129D1BDA9E |
| 8086:27c8 | 8086:27c8 | Intel           | NM10/ICH7 Family USB ... | 0.7%   | 3.14.25  | 37B1114873 |
| 8086:27c9 | 8086:27c9 | Intel           | NM10/ICH7 Family USB ... | 0.7%   | 3.14.25  | 37B1114873 |
| 8086:27ca | 8086:27ca | Intel           | NM10/ICH7 Family USB ... | 0.7%   | 3.14.25  | 37B1114873 |
| 8086:27cb | 8086:27cb | Intel           | NM10/ICH7 Family USB ... | 0.7%   | 3.14.25  | 37B1114873 |
| 8086:27cc | 8086:27cc | Intel           | NM10/ICH7 Family USB2... | 0.8%   | 3.14.39  | 37B1114873 |
| 8086:2934 | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 5.6%   | 3.14.44  | 93C0EF7223 |
| 8086:2935 | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 5.6%   | 3.14.44  | 93C0EF7223 |
| 8086:2936 | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 5.6%   | 3.14.44  | 93C0EF7223 |
| 8086:2937 | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 5.6%   | 3.14.44  | 93C0EF7223 |
| 8086:2938 | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 5.6%   | 3.14.44  | 93C0EF7223 |
| 8086:2939 | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 5.6%   | 3.14.44  | 93C0EF7223 |
| 8086:293a | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 5.6%   | 3.14.44  | 93C0EF7223 |
| 8086:293c | 103c:306b | Intel           | 82801I (ICH9 Family) ... | 5.6%   | 3.14.44  | 93C0EF7223 |
| 8086:34ee | 1854:0361 | Intel           | USB Controller           | 100%   |          | BEA6A28EB1 |
| 8086:3b36 | 8086:7270 | Intel           | 5 Series/3400 Series ... | 76.9%  | 3.14.44  | C5621D630D |
| 8086:3b3b | 8086:7270 | Intel           | 5 Series/3400 Series ... | 76.9%  | 3.14.44  | C5621D630D |
| 8086:5aaa | 8086:7270 | Intel           | USB Controller           | 43.5%  | 4.10.0   | 867223F2CF |
| 8086:8a15 |           | Intel           | USB xDCI                 | 100%   |          | BEA6A28EB1 |
| 8086:8c26 | 103c:1909 | Intel           | 8 Series/C220 Series ... | 2.4%   | 4.9.0    | 196DFE92A3 |
| 8086:8c2d | 103c:1909 | Intel           | 8 Series/C220 Series ... | 2.4%   | 4.9.0    | 196DFE92A3 |
| 8086:8c31 | 8086:204a | Intel           | 8 Series/C220 Series ... | 3.1%   | 4.1.25   | 8C48173C7B |
| 8086:8d26 | 1043:8600 | Intel           | C610/X99 series chips... | 2.1%   | 3.10.0   | 89ABF0DB25 |
| 8086:8d2d | 1043:8600 | Intel           | C610/X99 series chips... | 2.1%   | 3.10.0   | 89ABF0DB25 |
| 8086:9a1b |           | Intel           | Tiger Lake-LP Thunder... | 9.6%   | 5.6.0    | 9A7CCA485D |
| 8086:9a1b | 2222:1111 | Intel           | Tiger Lake-LP Thunder... | 12.3%  | 5.6.0    | 241B13488E |
| 8086:9a1d |           | Intel           | Tiger Lake-LP Thunder... | 1.4%   | 5.6.0    | 5A7035D3AC |
| 8086:9a1d | 2222:1111 | Intel           | Tiger Lake-LP Thunder... | 7.5%   | 5.6.0    | 49AAD4B320 |
| 8086:9c26 | 1025:0a11 | Intel           | 8 Series USB EHCI #1     | 42.9%  | 4.9.60   | 9DC2B77BCD |
| 8086:9c26 | 103c:21ed | Intel           | 8 Series USB EHCI #1     | 16.7%  | 3.10.0   | 8A99B7CDDD |
| 8086:9c26 | 17aa:3978 | Intel           | 8 Series USB EHCI #1     | 0.2%   | 3.14.25  | B3B3794709 |
| 8086:9c31 | 1028:05e0 | Intel           | 8 Series USB xHCI HC     | 1.9%   | 4.9.9    | 8EA71BA2AE |
| 8086:9c31 | 17aa:3978 | Intel           | 8 Series USB xHCI HC     | 0.2%   | 3.14.25  | B3B3794709 |
| 8086:9ca6 | 1025:098a | Intel           | Wildcat Point-LP USB ... | 0.7%   | 3.14.44  | DE4737FCF1 |
| 8086:9ca6 | 1028:06be | Intel           | Wildcat Point-LP USB ... | 10%    | 4.15.0   | 1FBEE12FFE |
| 8086:9cb1 | 103c:806c | Intel           | Wildcat Point-LP USB ... | 100%   |          | 462F2D5347 |
| 8086:9d2f | 103c:807c | Intel           | Sunrise Point-LP USB ... | 2.9%   | 4.9.0    | 791A2EA6F5 |
| 8086:9d2f | 1043:201f | Intel           | Sunrise Point-LP USB ... | 0.1%   | 4.1.15   | 910087F48C |
| 8086:9d30 | 8086:7270 | Intel           | Skylake-U/Y USB Devic... | 58.3%  | 5.4.0    | B713CD21D1 |
| 8086:9d30 | 8086:9d30 | Intel           | Skylake-U/Y USB Devic... | 20%    | 4.15.0   | 3E70A8DFF1 |
| 8086:a12f | 1558:8587 | Intel           | 100 Series/C230 Serie... | 66.7%  | 4.15.0   | 69AEB1F90D |
| 8086:a12f | 1734:121d | Intel           | 100 Series/C230 Serie... | 6%     | 3.10.0   | 7152566435 |
| 8086:a12f | 1849:a12f | Intel           | 100 Series/C230 Serie... | 0.4%   | 3.19.0   | 314B078748 |
| 8086:a130 | 1458:5000 | Intel           | 100 Series/C230 Serie... | 66.7%  | 5.9.10   | 413E235718 |
| 8086:a2af | 1043:872f | Intel           | 200 Series/Z370 Chips... | 1%     | 4.9.9    | 4027AAA720 |
| 8086:a36d | 1043:8694 | Intel           | Cannon Lake PCH USB 3... | 0.2%   | 2.6.32   | 9578024712 |

USB Devices
-----------

Non-100% value in the 'Missed' column indicates that the driver for a device is available
in the latest kernel versions. You can find corresponding hwinfo reports for listed devices
by a probe ID.

Missed — percentage of probes with missed driver for the device,
Linux  — the minimum Linux kernel version in which the driver was found,
Probe  — latest probe ID with missed driver for the device.

### Audio (USB)

11 out of 202 (5.45%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 041e:3257 | Creative Tec... | Sound Blaster K3+        | 50%    | 5.4.0    | FBA2E4B49B |
| 046d:0a0b | Logitech        | ClearChat Pro USB        | 9.1%   | 4.15.0   | 56D5984A14 |
| 046d:0a87 | Logitech        | G935 Gaming Headset      | 4.5%   | 5.0.0    | 58C9748044 |
| 047f:c055 | Plantronics     |                          | 100%   |          | 885207B563 |
| 04d2:ff05 | Altec Lansin... | ADA-305 Speakers         | 100%   |          | 9DA28A4AEC |
| 0644:8030 | TEAC            | US-1800                  | 100%   |          | 75C7FE6B69 |
| 0763:201a | M-Audio         | M-Audio Micro            | 100%   |          | 37F36A2183 |
| 0955:7002 | Nvidia          | stereo controller        | 100%   |          | 024ABE4666 |
| 0b0e:0850 | GN Netcom       | Jabra LINK 850           | 100%   |          | 87F345B258 |
| 1235:8016 | Focusrite-No... | Focusrite Scarlett 2i2   | 2.9%   | 4.9.20   | F16ADBF7F3 |
| b58e:0005 | Blue Microph... | Yeti Nano                | 5%     | 5.0.0    | A588768A6C |

### Bluetooth (USB)

91 out of 420 (21.67%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 03f0:171d | Hewlett-Packard | Bluetooth 2.0 Interfa... | 0.6%   | 3.2.0    | B5FBFCF0A5 |
| 044e:300c | Alps Electric   | Bluetooth Controller ... | 4%     | 4.1.15   | 7F0BB0CC92 |
| 0489:e027 | Foxconn / Ho... | Bluetooth Device         | 21.1%  | 3.14.44  | 6D895891B9 |
| 0489:e031 | Foxconn / Ho... | BCM20702A0               | 3.1%   | 4.15.0   | 958D094890 |
| 0489:e036 | Foxconn / Ho... | Bluetooth USB Host Co... | 0.4%   | 3.0.28   | 69F933DD8C |
| 0489:e04e | Foxconn / Ho... | Bluetooth Device         | 0.5%   | 3.14.15  | BC54B9763A |
| 0489:e069 | Foxconn / Ho... | BT                       | 98.7%  | 4.9.41   | F5A173D797 |
| 0489:e080 | Foxconn / Ho... | BT                       | 100%   |          | EB9637AE4A |
| 04ca:2006 | Lite-On Tech... | Broadcom BCM43142A0 B... | 4.8%   | 4.0.8    | E649CC1304 |
| 04ca:2007 | Lite-On Tech... | Broadcom BCM43142A0 B... | 7.7%   | 4.1.7    | BAA62D56E7 |
| 04ca:2009 | Lite-On Tech... | BCM43142A0               | 4.5%   | 4.0.2    | 14539CFCC1 |
| 04ca:300b | Lite-On Tech... | Atheros AR3012 Bluetooth | 0.5%   | 3.10.51  | 166921ADE6 |
| 04ca:300d | Lite-On Tech... | Atheros AR3012 Bluetooth | 5.7%   | 4.1.19   | D9F38D66C3 |
| 04ca:3014 | Lite-On Tech... | Qualcomm Atheros Blue... | 3.3%   | 4.1.25   | 401BBED185 |
| 04ca:3015 | Lite-On Tech... | Qualcomm Atheros QCA9... | 0.1%   | 3.10.0   | DF6E0A3FF3 |
| 04ca:4005 | Lite-On Tech... | Bluetooth Radio          | 4.5%   | 4.18.16  | B10D744C6C |
| 050d:065a | Belkin Compo... | F8T065BF Mini Bluetoo... | 5.3%   | 4.1.15   | 1BEC700189 |
| 05ac:8204 | Apple           | Built-in Bluetooth 2.... | 100%   |          | 978FCB3A51 |
| 05ac:8215 | Apple           | Built-in Bluetooth 2.... | 0.3%   | 3.14.44  | D5C9D589F2 |
| 05ac:8289 | Apple           | Bluetooth Host Contro... | 1.4%   | 4.1.15   | 109E02E0F2 |
| 05ac:828d | Apple           | Bluetooth USB Host Co... | 0.7%   | 4.1.34   | 2961E0C973 |
| 05ac:8290 | Apple           | Bluetooth Host Contro... | 1.6%   | 4.9.9    | 5884A106A0 |
| 05e1:0100 | Syntek          | 802.11g + Bluetooth W... | 100%   |          | 59D2069D40 |
| 0930:0200 | Toshiba         | Integrated Bluetooth ... | 15.6%  | 4.1.16   | 9540E0D0D5 |
| 0930:0215 | Toshiba         | Bluetooth Device         | 21.4%  | 3.14.44  | 01A4EAFBB6 |
| 0930:0219 | Toshiba         | Bluetooth USB Host Co... | 1.2%   | 3.14.33  | 67009EFFAA |
| 0930:0220 | Toshiba         | Bluetooth Device         | 1.8%   | 3.14.15  | D7B4BF2642 |
| 0a12:0001 | Cambridge Si... | Bluetooth Dongle (HCI... | 0.3%   | 2.6.32   | C2B1B16459 |
| 0a5c:216c | Broadcom        | BCM43142A0 Bluetooth ... | 0.6%   | 3.14.44  | 2F3CB20593 |
| 0a5c:216d | Broadcom        | BCM43142A0 Bluetooth 4.0 | 0.3%   | 4.1.15   | 0374CA0B61 |
| 0a5c:217f | Broadcom        | BCM2045B (BDC-2.1)       | 0.1%   | 3.10.0   | 4CAE7DC78D |
| 0a5c:21b4 | Broadcom        | BCM2070 Bluetooth 2.1... | 0.2%   | 3.14.22  | 65917EBD9D |
| 0a5c:21d7 | Broadcom        | BCM43142 Bluetooth 4.0   | 0.4%   | 3.14.33  | 854DAA05D0 |
| 0a5c:21e6 | Broadcom        | BCM20702 Bluetooth 4.... | 0.6%   | 3.14.15  | 676F1B8DCE |
| 0a5c:21e8 | Broadcom        | BCM20702A0 Bluetooth 4.0 | 0.3%   | 4.1.15   | DC806CCAB7 |
| 0b05:1712 | ASUSTek Comp... | BT-183 Bluetooth 2.0+... | 0.4%   | 3.14.33  | 5B8E446BE1 |
| 0b05:17b5 | ASUSTek Comp... | BCM20702A0               | 1.8%   | 4.1.15   | 0201C4C0FD |
| 0b05:17cb | ASUSTek Comp... | Broadcom BCM20702A0 B... | 1.3%   | 2.6.32   | 13961E12A8 |
| 0bda:8771 | Realtek Semi... | Bluetooth Radio          | 2.3%   | 4.15.0   | 06B30E0725 |
| 0bda:b001 | Realtek Semi... | Bluetooth Radio          | 0.3%   | 3.14.15  | 8DCBD3C2B1 |
| 0bda:b006 | Realtek Semi... | Bluetooth Radio          | 8.4%   | 4.1.15   | 7E483F822D |
| 0bda:b009 | Realtek Semi... | Realtek Bluetooth 4.2... | 0.2%   | 3.10.0   | 603D2AC0FA |
| 0bda:b00a | Realtek Semi... | Realtek Bluetooth 4.2... | 0.2%   | 3.10.0   | 0B4A5C33EF |
| 0bda:b00c | Realtek Semi... | Bluetooth Radio          | 0.7%   | 4.14.219 | 5EAE12F393 |
| 0bda:b023 | Realtek Semi... | RTL8822BE Bluetooth 4... | 0.7%   | 4.15.0   | 2C9E565B99 |
| 0bda:b728 | Realtek Semi... | RTL8723B Bluetooth       | 1.2%   | 3.14.25  | 9A767F85C2 |
| 0bda:c024 | Realtek Semi... | Bluetooth Radio          | 0.2%   | 4.9.60   | 105B239349 |
| 0bda:c123 | Realtek Semi... | Bluetooth Radio          | 0.4%   | 4.15.0   | 38C41D5178 |
| 0bda:c821 | Realtek Semi... | Bluetooth Radio          | 7.7%   | 4.15.0   | FEE86BED02 |
| 0cf3:0036 | Qualcomm Ath... | AR9462 Bluetooth         | 0.5%   | 3.10.0   | 9BCFCED245 |
| 0cf3:3002 | Qualcomm Ath... | AR3011 Bluetooth         | 10%    | 3.14.44  | 7243A2DF4F |
| 0cf3:3004 | Qualcomm Ath... | AR3012 Bluetooth 4.0     | 0.5%   | 3.10.0   | 15DBF9FAD6 |
| 0cf3:3005 | Qualcomm Ath... | AR3011 Bluetooth         | 0.1%   | 3.10.0   | F4DE983D96 |
| 0cf3:3008 | Qualcomm Ath... | Bluetooth (AR3011)       | 1.6%   | 3.14.25  | F430167968 |
| 0cf3:311e | Qualcomm Ath... | Qualcomm Atheros Blue... | 4.2%   | 3.10.0   | CF3ED91B8A |
| 0cf3:3121 | Qualcomm Ath... | Qualcomm Atheros Blue... | 1%     | 3.14.44  | 6801725BAE |
| 0cf3:817a | Qualcomm Ath... | Qualcomm Atheros Blue... | 14.3%  | 5.4.0    | F674F91052 |
| 0cf3:e004 | Qualcomm Ath... | Bluetooth USB Host Co... | 0.8%   | 3.14.25  | 7617104233 |
| 0cf3:e005 | Qualcomm Ath... | Qualcomm Atheros Blue... | 1.7%   | 4.4.0    | B04793329D |
| 0cf3:e007 | Qualcomm Ath... | Qualcomm Atheros Blue... | 0.2%   | 4.4.0    | EBA5E925B8 |
| 0cf3:e300 | Qualcomm Ath... | Qualcomm Atheros Blue... | 0.1%   | 4.15.0   | 96374442C4 |
| 0cf3:e500 | Qualcomm Ath... | Qualcomm Atheros Blue... | 0.1%   | 3.14.44  | D6346FBB4B |
| 0e8d:763e | MediaTek        | MT7630e Bluetooth Ada... | 97.1%  | 5.11.7   | 9F0E83422C |
| 0e8d:763f | MediaTek        | BT                       | 3%     | 3.14.44  | E0F7826601 |
| 105b:e065 | Foxconn Inte... | BCM43142A0 Bluetooth ... | 7.9%   | 4.0.1    | F39685A972 |
| 1131:1001 | Integrated S... | KY-BT100 Bluetooth Ad... | 1.2%   | 3.14.15  | 132E2B687C |
| 1131:1004 | Integrated S... | Bluetooth Device         | 0.9%   | 3.14.44  | 8F5F5ABA10 |
| 1358:c123 | Realtek         | Bluetooth Radio          | 0.8%   | 4.15.0   | 763C1A213C |
| 13d3:3304 | IMC Networks    | Asus Integrated Bluet... | 2.2%   | 3.10.34  | 1787C065C7 |
| 13d3:3362 | IMC Networks    | Atheros AR3012 Blueto... | 0.5%   | 3.10.34  | D5866F9F0F |
| 13d3:3392 | IMC Networks    | Azurewave 43228+20702    | 33.3%  | 4.18.0   | 337156D639 |
| 13d3:3402 | IMC Networks    | Bluetooth USB Host Co... | 0.7%   | 3.14.15  | BBE5800595 |
| 13d3:3408 | IMC Networks    | Bluetooth Device         | 0.8%   | 3.14.44  | E3E9F32F6D |
| 13d3:3414 | IMC Networks    | Bluetooth Radio          | 2%     | 3.14.44  | 13961E12A8 |
| 13d3:3491 | IMC Networks    | Bluetooth Device         | 0.6%   | 4.4.0    | 94D2C67B3F |
| 13d3:3530 | IMC Networks    | Bluetooth Radio          | 0.8%   | 4.18.0   | C57627A5E0 |
| 413c:8143 | Dell            | Broadcom BCM20702A0 B... | 41.4%  | 4.15.0   | AE4C0F8B6B |
| 413c:8187 | Dell            | DW375 Bluetooth Module   | 0.2%   | 3.10.0   | F33530C32A |
| 413c:8197 | Dell            | BCM20702A0 Bluetooth ... | 0.8%   | 3.14.25  | 4E38982788 |
| 7392:c611 | Edimax Techn... | Bluetooth Adapter        | 40%    | 5.10.13  | 75BA67766B |
| 8086:0189 | Intel           | Centrino Advanced-N 6... | 0.1%   | 5.4.0    | 69C8FA5FEE |
| 8087:0025 | Intel           | Wireless-AC 9260 Blue... | 0.2%   | 4.9.60   | 9F55C5ECE0 |
| 8087:0026 | Intel           | Bluetooth Device         | 0.4%   | 3.10.0   | B3217892ED |
| 8087:0029 | Intel           | AX200 Bluetooth          | 1%     | 3.10.0   | AC7BF54F19 |
| 8087:0032 | Intel           | Bluetooth Device         | 14.3%  | 5.4.32   | 3D5116EC46 |
| 8087:07da | Intel           | Centrino Bluetooth Wi... | 0.2%   | 3.10.0   | DC66CB5CAF |
| 8087:07dc | Intel           | Bluetooth wireless in... | 0.4%   | 3.10.0   | 634C63D316 |
| 8087:0a2a | Intel           | Bluetooth wireless in... | 0.2%   | 3.10.0   | 063BBDBBAA |
| 8087:0a2b | Intel           | Bluetooth wireless in... | 0.5%   | 3.10.0   | 6F9D0F45BB |
| 8087:0aa7 | Intel           | Wireless-AC 3168 Blue... | 0.3%   | 4.19.0   | 4080E1B43F |
| 8087:0aaa | Intel           | Bluetooth 9460/9560 J... | 0.5%   | 3.10.0   | 241B649AD1 |

### Camera (USB)

284 out of 2993 (9.49%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0402:5603 | ALi             | M5603 Video Camera Co... | 100%   |          | 775945A948 |
| 0402:9665 | ALi             | Gateway Webcam           | 0.3%   | 3.14.25  | 68F61986F8 |
| 0408:2fb1 | Quanta          | Laptop_Integrated_Web... | 0.8%   | 3.10.0   | A993CB7099 |
| 0408:51e9 | Quanta          | HP Wide Vision HD Camera | 7.1%   | 4.9.9    | 2C576FB8A9 |
| 0408:5300 | Quanta          | HP Wide Vision HD Camera | 2.5%   | 4.15.0   | 3396357637 |
| 0408:5362 | Quanta          | HP TrueVision HD Camera  | 1.4%   | 4.13.0   | B5E9340D85 |
| 0408:5365 | Quanta          | HP TrueVision HD Camera  | 0.4%   | 4.15.0   | 88CF2BC0F5 |
| 0408:a031 | Quanta          | VGA WebCam               | 0.4%   | 4.9.0    | DF6E0A3FF3 |
| 0408:a060 | Quanta          | HD Webcam                | 0.2%   | 4.1.25   | 85BF9E9450 |
| 0408:a061 | Quanta          | HD User Facing           | 0.4%   | 4.15.0   | 009A95412F |
| 041e:400d | Creative Tec... | Webcam PD1001            | 100%   |          | 1892C5C88C |
| 041e:4039 | Creative Tec... | Webcam Live! Effects     | 100%   |          | D42D07BEBB |
| 041e:4080 | Creative Tec... | VF0610 Live! Cam Soci... | 4.8%   | 4.15.0   | C0A7DFF96D |
| 0458:702a | KYE Systems ... | WebCAM USB2.0            | 100%   |          | 3D86369A82 |
| 0458:7089 | KYE Systems ... | Genius FaceCam 320       | 2.8%   | 3.14.44  | 37D2955943 |
| 045e:0294 | Microsoft       | Video Camera             | 25%    | 4.9.20   | C8F6D28F76 |
| 045e:02ae | Microsoft       | Xbox NUI Camera          | 25%    | 4.1.25   | F2C8EC14C7 |
| 045e:0779 | Microsoft       | LifeCam HD-3000          | 0.8%   | 3.14.33  | 2F71E9B242 |
| 045e:097c | Microsoft       | Azure Kinect Depth Ca... | 100%   |          | 09AE9C9787 |
| 045e:097d | Microsoft       | Azure Kinect 4K Camera   | 100%   |          | 09AE9C9787 |
| 045e:0a00 | Microsoft       | Lumia 950 Dual SIM (R... | 80%    | 5.0.0    | 5A4E6DF962 |
| 046d:0801 | Logitech        | QuickCam Home            | 100%   |          | 605FE21A48 |
| 046d:081b | Logitech        | Webcam C310              | 0.2%   | 3.14.22  | 66219C1D36 |
| 046d:0821 | Logitech        | HD Webcam C910           | 0.7%   | 3.0.38   | F47CB1587E |
| 046d:0825 | Logitech        | Webcam C270              | 0.3%   | 4.9.60   | 6054B96BC5 |
| 046d:082c | Logitech        | HD Webcam C615           | 0.5%   | 3.14.44  | F61EE20F03 |
| 046d:082d | Logitech        | HD Pro Webcam C920       | 0.1%   | 4.15.0   | 26B5C18ABA |
| 046d:085c | Logitech        | C922 Pro Stream Webcam   | 1.4%   | 4.9.0    | 781F2CDA04 |
| 046d:0994 | Logitech        | QuickCam Orbit/Sphere AF | 5%     | 4.1.16   | DA311C1D96 |
| 046d:09a4 | Logitech        | QuickCam E 3500          | 2.4%   | 3.14.39  | 74709A1A7B |
| 046d:beef | Logitech        |                          | 50%    | 5.4.0    | A83AEEA4C8 |
| 04ca:7017 | Lite-On Tech... | TOSHIBA Web Camera - HD  | 2.1%   | 3.14.15  | F776B2E5C6 |
| 04ca:7025 | Lite-On Tech... | HP HD Webcam             | 8.3%   | 5.4.0    | 3B37587B81 |
| 04ca:7034 | Lite-On Tech... | HP HD Webcam             | 2%     | 4.9.0    | 858431DD69 |
| 04ca:7036 | Lite-On Tech... | Integrated Camera        | 3.2%   | 4.9.60   | 5FAA8E4CA3 |
| 04ca:7070 | Lite-On Tech... | Integrated Camera        | 0.4%   | 4.15.0   | D082B8D834 |
| 04ca:707f | Lite-On Tech... | HP Wide Vision HD Camera | 0.8%   | 4.4.0    | 06EE78EE4D |
| 04ca:7086 | Lite-On Tech... | HP Wide Vision FHD Ca... | 8.9%   | 4.15.0   | 04D98C9A75 |
| 04ca:709d | Lite-On Tech... | HP Wide Vision HD Camera | 2.2%   | 4.15.0   | ACFBF614C0 |
| 04f2:b012 | Chicony Elec... | 1.3 MPixel UVC Webcam    | 1.6%   | 3.14.44  | 2DCD0E4E69 |
| 04f2:b163 | Chicony Elec... | HP Webcam [2 MP Macro]   | 2%     | 4.1.22   | 5DD7A5FCE1 |
| 04f2:b185 | Chicony Elec... | HD Video WebCam          | 18.2%  | 4.4.0    | 4D4A33CDAF |
| 04f2:b1b4 | Chicony Elec... | Lenovo Integrated Camera | 4.5%   | 3.14.44  | 6DCCB35FCB |
| 04f2:b217 | Chicony Elec... | Lenovo Integrated Cam... | 0.4%   | 3.10.0   | 4CAE7DC78D |
| 04f2:b240 | Chicony Elec... | FJ Camera                | 2.9%   | 4.15.0   | 958D094890 |
| 04f2:b270 | Chicony Elec... | HP HD Webcam [Fixed]     | 3.2%   | 3.14.44  | AD6B18F63A |
| 04f2:b272 | Chicony Elec... | Lenovo EasyCamera        | 0.3%   | 2.6.32   | AF1E15F9D1 |
| 04f2:b28f | Chicony Elec... | USB 2.0 Camera           | 22.2%  | 4.15.0   | C1BEFDDDD7 |
| 04f2:b293 | Chicony Elec... | HP Webcam-101            | 2.1%   | 3.14.44  | 30478F743C |
| 04f2:b2da | Chicony Elec... | thinkpad t430s camera    | 1.6%   | 4.9.9    | E78B76FCF3 |
| 04f2:b2e1 | Chicony Elec... | Lenovo EasyCamera        | 0.5%   | 3.10.42  | F424D17C63 |
| 04f2:b2eb | Chicony Elec... | Integrated Camera        | 1.8%   | 3.14.44  | 8A22CE4B29 |
| 04f2:b307 | Chicony Elec... | TOSHIBA Web Camera - HD  | 0.7%   | 3.14.44  | 67009EFFAA |
| 04f2:b315 | Chicony Elec... | Integrated Camera        | 4.8%   | 3.14.53  | B7014678B5 |
| 04f2:b335 | Chicony Elec... | HD WebCam                | 1.1%   | 3.14.44  | 6A087DD575 |
| 04f2:b374 | Chicony Elec... | HD WebCam                | 1.7%   | 3.14.44  | 344148537E |
| 04f2:b3b2 | Chicony Elec... | TOSHIBA Web Camera - FHD | 5.9%   | 4.15.0   | 550460AAAC |
| 04f2:b40e | Chicony Elec... | HP Truevision HD camera  | 1.2%   | 3.14.25  | B5C4F3E278 |
| 04f2:b40f | Chicony Elec... | Lenovo EasyCamera        | 25%    | 4.1.25   | 43B95135E2 |
| 04f2:b43c | Chicony Elec... | Integrated Camera        | 100%   |          | 5152D7EEFA |
| 04f2:b452 | Chicony Elec... | HD WebCam                | 0.8%   | 3.14.25  | AF59A812BC |
| 04f2:b45a | Chicony Elec... | USB2.0 FHD Camera        | 7.7%   | 3.14.44  | 78D39E18EF |
| 04f2:b469 | Chicony Elec... | HD WebCam                | 1.1%   | 3.10.51  | 84429B1758 |
| 04f2:b47f | Chicony Elec... | VGA Webcam               | 0.3%   | 3.14.44  | 401BBED185 |
| 04f2:b50d | Chicony Elec... | HP Truevision HD         | 2.5%   | 4.1.15   | CE1A55614C |
| 04f2:b51c | Chicony Elec... | HP HD Camera             | 2.9%   | 4.1.15   | E9E3B904A9 |
| 04f2:b52b | Chicony Elec... | USB2.0 VGA UVC WebCam    | 0.9%   | 3.14.44  | A376ADDBEB |
| 04f2:b52c | Chicony Elec... | Integrated Camera        | 5.9%   | 4.9.9    | B2649601D3 |
| 04f2:b56c | Chicony Elec... | HP TrueVision HD         | 1%     | 4.1.38   | 45AEF7A11F |
| 04f2:b573 | Chicony Elec... | HD WebCam                | 1.1%   | 4.1.15   | C3486F6056 |
| 04f2:b59a | Chicony Elec... | XiaoMi USB 2.0 Webcam    | 3.4%   | 4.9.60   | B1B825395C |
| 04f2:b59e | Chicony Elec... | USB2.0 Camera            | 1.5%   | 4.9.124  | 2920E04DB9 |
| 04f2:b5a3 | Chicony Elec... | XiaoMi USB 2.0 Webcam    | 5.9%   | 4.8.14   | 1F8DE2B55C |
| 04f2:b5bb | Chicony Elec... | Integrated Camera        | 14.3%  | 5.2.18   | 7408A95129 |
| 04f2:b5d7 | Chicony Elec... | EasyCamera               | 0.6%   | 3.14.44  | 94A8A3E5B3 |
| 04f2:b5ed | Chicony Elec... | HP Wide Vision HD Camera | 10%    | 4.15.0   | 063BBDBBAA |
| 04f2:b5f7 | Chicony Elec... | HD WebCam                | 0.9%   | 4.9.20   | E703CB72E3 |
| 04f2:b604 | Chicony Elec... | Integrated Camera (12... | 0.5%   | 3.10.0   | FFDEE2C6E0 |
| 04f2:b614 | Chicony Elec... | Integrated Camera        | 1.8%   | 3.10.0   | 4438A85B31 |
| 04f2:b615 | Chicony Elec... | Integrated IR Camera     | 3.9%   | 4.15.0   | 4547E0D6FE |
| 04f2:b61e | Chicony Elec... | Integrated Camera        | 0.5%   | 4.15.0   | 8E74730A87 |
| 04f2:b648 | Chicony Elec... | USB 2.0 Webcam Device    | 22.2%  | 5.3.0    | 08ED0821EF |
| 04f2:b649 | Chicony Elec... | USB2.0 Camera            | 2.6%   | 4.18.0   | 38CC94083D |
| 04f2:b64f | Chicony Elec... | HD User Facing           | 1.1%   | 4.15.0   | 89497C0F27 |
| 04f2:b652 | Chicony Elec... | VGA WebCam               | 50%    | 5.9.16   | 03BCD5F0CC |
| 04f2:b664 | Chicony Elec... | USB 2.0 Webcam Device    | 100%   |          | C521DF4D98 |
| 04f2:b669 | Chicony Elec... | HP HD Camera             | 1.7%   | 4.15.0   | BDD15B19B1 |
| 04f2:b66a | Chicony Elec... | HP HD Camera             | 1.5%   | 3.10.0   | 6C504FBDF0 |
| 04f2:b671 | Chicony Elec... | HP Full-HD Camera        | 7.7%   | 4.18.0   | A838427772 |
| 04f2:b678 | Chicony Elec... | LG Camera                | 4.5%   | 4.15.0   | BF08AA9738 |
| 04f2:b67c | Chicony Elec... | Integrated Camera        | 0.5%   | 4.15.0   | CA529580D5 |
| 04f2:b67f | Chicony Elec... | HP TrueVision HD Camera  | 2.1%   | 4.15.0   | 4F1105BCA0 |
| 04f2:b684 | Chicony Elec... | USB2.0 Camera            | 3.1%   | 4.18.0   | 5CD28E369C |
| 04f2:b6b6 | Chicony Elec... | HP Wide Vision HD Camera | 4%     | 4.15.0   | 05E61F6A9D |
| 04f2:b6c2 | Chicony Elec... | Integrated Camera        | 1.3%   | 5.4.0    | 96374442C4 |
| 04f2:b6cb | Chicony Elec... | Integrated Camera        | 1.6%   | 4.18.0   | 1FDC0E17D4 |
| 04f2:b6d9 | Chicony Elec... | Integrated Camera        | 2.4%   | 4.15.0   | 1A6E48B6A6 |
| 0547:6512 | Anchor Chips    | UCMOS05100KPA            | 100%   |          | 93BF2F1F49 |
| 054c:0954 | Sony            | ILCE-7S                  | 100%   |          | 68979EBA8F |
| 0572:0040 | Conexant Sys... | Wondereye CP-115 Webcam  | 100%   |          | 6B3D175AF8 |
| 058f:3820 | Alcor Micro     | USB 2.0 PC Camera        | 25%    | 4.18.0   | FC6C12EB1D |
| 058f:5608 | Alcor Micro     | USB 2.0 Web Camera       | 0.2%   | 3.14.44  | E1C0563D70 |
| 058f:a001 | Alcor Micro     | HP Webcam-101            | 2.6%   | 3.14.44  | 031B9CF2AF |
| 058f:a014 | Alcor Micro     | Asus Integrated Webcam   | 0.5%   | 3.10.34  | 11547CB913 |
| 05ac:1293 | Apple           | iPod Touch 2.Gen         | 100%   |          | 454CDC1CD3 |
| 05ac:12a8 | Apple           | iPhone5/5C/5S/6          | 4.1%   | 3.10.0   | 50704A4B1B |
| 05ac:12aa | Apple           | iPod Touch 5.Gen [A1421] | 66.7%  | 5.8.0    | 409A76B0F1 |
| 05ac:8501 | Apple           | Built-in iSight [Micron] | 11.1%  | 4.15.0   | 6A774ADE41 |
| 05ac:8509 | Apple           | FaceTime HD Camera       | 0.9%   | 4.1.25   | 89174DDA21 |
| 05ac:8511 | Apple           | FaceTime HD Camera (B... | 0.5%   | 4.1.15   | 2961E0C973 |
| 05ac:8514 | Apple           | FaceTime HD Camera (B... | 30.8%  | 5.6.10   | 1E39B8A641 |
| 05ac:8600 | Apple           | iBridge                  | 25%    | 4.15.0   | 53977AB29B |
| 05c8:021e | Cheng Uei Pr... | HP Webcam-101            | 0.4%   | 3.14.33  | 585D199B71 |
| 05c8:0223 | Cheng Uei Pr... | HP Webcam-50             | 3.7%   | 3.14.44  | 2E60620A98 |
| 05c8:0359 | Cheng Uei Pr... | HP HD Webcam             | 1.6%   | 3.14.15  | 8DCBD3C2B1 |
| 05c8:0369 | Cheng Uei Pr... | HP HD Webcam             | 0.8%   | 4.1.25   | B0C4FE1761 |
| 05c8:036e | Cheng Uei Pr... | Webcam                   | 0.5%   | 3.10.0   | 2857EF3B7B |
| 05c8:0374 | Cheng Uei Pr... | HP EliteBook integrat... | 0.9%   | 4.9.0    | 82579034FE |
| 05c8:038f | Cheng Uei Pr... | HP TrueVision HD         | 0.6%   | 4.9.41   | 5F80EB8AB2 |
| 05c8:03a2 | Cheng Uei Pr... | XiaoMi USB 2.0 Webcam    | 4.5%   | 4.9.60   | 1B7596A646 |
| 05c8:03ab | Cheng Uei Pr... | HP Wide Vision HD Camera | 5.9%   | 4.9.60   | 142D7492C2 |
| 05c8:03b7 | Cheng Uei Pr... | XiaoMi USB 2.0 Webcam    | 2.4%   | 4.10.0   | 04146F06E0 |
| 05c8:03bc | Cheng Uei Pr... | HP Wide Vision HD Int... | 1.2%   | 3.10.0   | D45FF60CD3 |
| 05c8:0815 | Cheng Uei Pr... | HP Wide Vision FHD Ca... | 8.7%   | 4.19.10  | 8AAAF9416E |
| 05ca:1810 | Ricoh           | Pavilion Webcam [R5U870] | 41.7%  | 4.1.15   | BAD7484C1A |
| 05ca:181a | Ricoh           | Laptop_Integrated_Web... | 18.8%  | 4.9.0    | 898AE3EA34 |
| 05ca:1830 | Ricoh           | Visual Communication ... | 100%   |          | BEDA953594 |
| 05ca:1834 | Ricoh           | Visual Communication ... | 100%   |          | 52E6107C87 |
| 05ca:1836 | Ricoh           | Visual Communication ... | 100%   |          | 82BD19C032 |
| 05ca:1837 | Ricoh           | Visual Communication ... | 13.6%  | 3.14.44  | B46E85CDB2 |
| 05ca:1839 | Ricoh           | Visual Communication ... | 7.4%   | 3.14.44  | E012C971C6 |
| 05ca:183a | Ricoh           | Visual Communication ... | 38.5%  | 3.14.44  | F538E64507 |
| 05ca:183b | Ricoh           | Visual Communication ... | 9.4%   | 4.1.16   | EF2216FC07 |
| 05ca:183f | Ricoh           | Sony Visual Communica... | 6.7%   | 4.9.76   | F9D3268ABE |
| 05ca:1870 | Ricoh           | Webcam 1000              | 100%   |          | F39A330574 |
| 05ca:18ba | Ricoh           | Sony Visual Communica... | 4.2%   | 4.9.155  | F7C7A3CA92 |
| 05ca:18c0 | Ricoh           | USB2.0 Camera            | 0.9%   | 3.14.22  | EC69106A89 |
| 05ca:18ff | Ricoh           | NoData                   | 57.1%  | 5.4.0    | E34430353C |
| 05e3:f12a | Genesys Logic   | Integrated Camera        | 16.7%  | 4.15.0   | 393DA2834D |
| 064e:8110 | Suyin           | Laptop_Integrated_Web... | 25%    | 5.4.0    | 4E9804E6ED |
| 064e:a103 | Suyin           | Acer/HP Integrated We... | 1.5%   | 3.14.33  | 6D1385653B |
| 064e:a111 | Suyin           | USB2.0 UVC 1.3M WebCam   | 1.1%   | 3.0.28   | A13580724B |
| 064e:a117 | Suyin           | Acer HD Crystal Eye w... | 0.9%   | 3.14.44  | E0BCC4DF92 |
| 064e:d213 | Suyin           | UVC HD Webcam            | 1.6%   | 3.14.15  | DF8F241425 |
| 064e:d281 | Suyin           | HP TrueVision HD         | 4.3%   | 3.14.44  | 65917EBD9D |
| 064e:e330 | Suyin           | HD WebCam                | 0.7%   | 3.14.33  | 8ABC23484B |
| 07ca:1311 | AVerMedia Te... | Live Gamer Mini          | 100%   |          | DADA6C90F4 |
| 093a:7011 | Pixart Imaging  | Digital Wireless Camera  | 100%   |          | F8FD891B32 |
| 09da:2690 | A4Tech          | HD 720P PC Camera        | 6.2%   | 5.4.0    | CC4B365068 |
| 0ac8:3420 | Z-Star Micro... | Venus USB2.0 Camera      | 0.1%   | 3.14.15  | CDC3F83CDB |
| 0ac8:3450 | Z-Star Micro... | Vimicro USB Camera (A... | 0.3%   | 3.14.22  | 3C44204AA0 |
| 0ac8:c326 | Z-Star Micro... | Namuga 1.3M Webcam       | 4.5%   | 4.1.15   | 3AD0FF0E13 |
| 0ac8:c40a | Z-Star Micro... | A4 TECH USB2.0 PC Cam... | 0.3%   | 3.10.34  | B2C845B843 |
| 0b05:200b | ASUSTek Comp... | ASUS_Z00VD               | 100%   |          | EDFAB941DF |
| 0b97:8381 | O2 Micro        | Mini S USB2.0 Camera     | 100%   |          | F1A2C19FEB |
| 0bda:5520 | Realtek Semi... | Integrated_Webcam_HD     | 1.1%   | 4.4.0    | 90B19AF55F |
| 0bda:5521 | Realtek Semi... | Integrated_Webcam_HD     | 3.4%   | 4.15.0   | 03AD0892DE |
| 0bda:5539 | Realtek Semi... | Integrated_Webcam_HD     | 10.4%  | 4.15.0   | 241B649AD1 |
| 0bda:564b | Realtek Semi... | WebCamera                | 8.3%   | 4.16.18  | 5EA0111CED |
| 0bda:5650 | Realtek Semi... | Integrated Webcam_HD     | 3.1%   | 4.4.0    | 54E871CA5D |
| 0bda:5652 | Realtek Semi... | Integrated_Webcam_HD     | 10%    | 4.15.0   | 50CB6D53EF |
| 0bda:5659 | Realtek Semi... | Integrated_Webcam_HD     | 6.7%   | 4.15.0   | DAF389F21B |
| 0bda:5689 | Realtek Semi... | Integrated Webcam        | 0.5%   | 4.4.0    | E1C330A900 |
| 0bda:568c | Realtek Semi... | Integrated Webcam HD     | 1.4%   | 4.9.76   | EBA5E925B8 |
| 0bda:56c1 | Realtek Semi... | USB Camera               | 11.1%  | 4.15.0   | 1A171E7553 |
| 0bda:5730 | Realtek Semi... | HP 2.0MP High Definit... | 33.3%  | 5.8.0    | CF3ED91B8A |
| 0bda:5760 | Realtek Semi... | Integrated_Webcam_FHD    | 16.7%  | 5.0.0    | 3A565370DE |
| 0bda:57b3 | Realtek Semi... | Acer 640 x 480 laptop... | 0.4%   | 3.8.0    | 4D3A6BBF1F |
| 0bda:57b4 | Realtek Semi... | USB Camera               | 1.3%   | 3.14.44  | E3E9F32F6D |
| 0bda:57cc | Realtek Semi... | HD Webcam - Realtek S... | 0.8%   | 4.1.25   | 5DBE9649A7 |
| 0bda:57ed | Realtek Semi... | USB2.0 VGA UVC WebCam    | 4.2%   | 4.9.9    | 551FF040B5 |
| 0bda:5841 | Realtek Semi... | USB Boot                 | 33.3%  | 4.19.0   | E63F4E6ED1 |
| 0bda:5846 | Realtek Semi... | USB Boot                 | 50%    | 5.4.0    | 2288F6D164 |
| 0bda:58bd | Realtek Semi... | USB2.0 HD UVC WebCam     | 6.2%   | 3.14.44  | B857F2B82D |
| 0bda:58be | Realtek Semi... | Laptop_Integrated_Web... | 3.1%   | 4.1.15   | A7211B4E35 |
| 0bda:58eb | Realtek Semi... | HP Wide Vision HD Camera | 1.9%   | 4.4.0    | D20F245092 |
| 0bda:58f4 | Realtek Semi... | Integrated_Webcam_HD     | 0.8%   | 4.14.65  | 60EC1448D4 |
| 0c45:62c0 | Microdia        | Sonix USB 2.0 Camera     | 1.5%   | 2.6.32   | 0F0153E2DB |
| 0c45:6310 | Microdia        | Sonix USB 2.0 Camera     | 4.8%   | 3.14.44  | 7C800A05D9 |
| 0c45:6350 | Microdia        | USB 2.0 Camera           | 100%   |          | 4A66A57A41 |
| 0c45:6362 | Microdia        | JOYACCESS JA-Webcam      | 50%    | 5.7.19   | E643F1337B |
| 0c45:6365 | Microdia        | USB 2.0 Camera           | 66.7%  | 5.4.0    | 344EC04FAF |
| 0c45:6369 | Microdia        | USB 2.0 Camera           | 54.5%  | 5.3.0    | 6B3CE5AC77 |
| 0c45:636d | Microdia        | USB 2.0 Camera           | 20%    | 5.4.0    | 57B918A36E |
| 0c45:63ee | Microdia        | Integrated_Webcam_1.3M   | 2.7%   | 4.4.16   | 536E9A34A7 |
| 0c45:6433 | Microdia        | Laptop Integrated Web... | 5.4%   | 4.9.60   | EAFEF7DB79 |
| 0c45:643f | Microdia        | Dell Integrated HD We... | 1.6%   | 4.1.15   | 4E38982788 |
| 0c45:648b | Microdia        | Integrated Webcam        | 0.4%   | 3.14.25  | F674F91052 |
| 0c45:649d | Microdia        | Laptop_Integrated_Web... | 1.1%   | 3.10.0   | 8EA71BA2AE |
| 0c45:64cb | Microdia        | Integrated_Webcam_HD     | 5.9%   | 3.14.44  | BFA1F898FB |
| 0c45:64d2 | Microdia        | Integrated Webcam        | 1.4%   | 4.9.60   | 037A28C347 |
| 0c45:6709 | Microdia        | Integrated_Webcam_HD     | 2.3%   | 4.1.18   | 173ECC36BA |
| 0c45:670c | Microdia        | Integrated Webcam HD     | 2.1%   | 4.1.25   | 7C815E9357 |
| 0c45:6718 | Microdia        | Integrated_Webcam_HD     | 2.3%   | 4.15.0   | DD4521B554 |
| 0c45:671d | Microdia        | Integrated_Webcam_HD     | 2.5%   | 4.15.0   | E31ABB4A0C |
| 0c45:671e | Microdia        | Integrated_Webcam_HD     | 0.4%   | 4.9.0    | 7ABAC766F3 |
| 0c45:6a04 | Microdia        | Integrated_Webcam_HD     | 3.5%   | 3.14.39  | 93CDABAFF0 |
| 0c45:6a05 | Microdia        | Integrated_Webcam_HD     | 1.6%   | 4.1.25   | D074E75C19 |
| 0c45:6a08 | Microdia        | Integrated_Webcam_HD     | 3.6%   | 4.15.0   | 6548681F70 |
| 0c45:8105 | Microdia        | USB camera               | 100%   |          | F16304CA03 |
| 0e8d:200b | MediaTek        | RAPID_10_LTE             | 75%    | 5.4.0    | 03EA0A12DC |
| 0f00:0050 | ndd Medizint... | EasyOne PictBridge Cr... | 100%   |          | 6C32F3272C |
| 0fce:0a07 | Sony Ericsso... | Xperia XA2               | 100%   |          | 20DB446598 |
| 13d3:5664 | IMC Networks    | Lenovo EasyCamera        | 27.3%  | 4.15.0   | E78A3CA624 |
| 13d3:56a2 | IMC Networks    | USB2.0 HD UVC WebCam     | 0.2%   | 4.15.0   | 3A1B31970C |
| 13d3:56a6 | IMC Networks    | Integrated Camera        | 0.9%   | 4.12.14  | CD929CAF4F |
| 13d3:56a8 | IMC Networks    | USB2.0 HD UVC WebCam     | 1.9%   | 4.15.0   | 723BA4E443 |
| 13d3:56b2 | IMC Networks    | Integrated Camera        | 0.3%   | 3.10.0   | BCCEC7C3D1 |
| 13d3:56dd | IMC Networks    | USB2.0 HD UVC WebCam     | 0.4%   | 4.15.0   | F856F4367C |
| 13d3:56e4 | IMC Networks    | USB2.0 HD IR UVC WebCam  | 20%    | 5.0.0    | 65529AFB99 |
| 13d3:56e5 | IMC Networks    | USB2.0 HD UVC WebCam     | 33.3%  | 5.8.0    | 9C797156F9 |
| 13d3:56ff | IMC Networks    | Integrated Camera        | 2.7%   | 4.18.16  | 38C41D5178 |
| 13d3:5727 | IMC Networks    | Lenovo EasyCamera        | 2.7%   | 4.1.15   | AB6BD693BE |
| 13d3:5744 | IMC Networks    | Lenovo EasyCamera        | 2.5%   | 3.19.0   | 9A767F85C2 |
| 13d3:5a01 | IMC Networks    | USB2.0 VGA UVC WebCam    | 0.6%   | 4.9.0    | 6E5F293574 |
| 13d3:5a07 | IMC Networks    | VGA UVC WebCam           | 1.4%   | 4.9.0    | 9F07F64EBF |
| 152d:0770 | JMicron Tech... | Alienware Integrated ... | 33.3%  | 5.0.0    | 7E166AFA9D |
| 174f:1122 | Syntek          | HP Webcam                | 18.2%  | 4.9.0    | 0230A47B05 |
| 174f:1134 | Syntek          | HP Webcam-101            | 12.5%  | 4.9.20   | DB518ED539 |
| 174f:114f | Syntek          | Lenovo EasyCamera        | 9.1%   | 3.14.44  | 2DD89E3983 |
| 174f:147b | Syntek          | Lenovo EasyCamera        | 1%     | 3.14.25  | AAB4F32C9F |
| 174f:14af | Syntek          | Lenovo EasyCamera        | 20%    | 4.15.0   | 08BB09B100 |
| 174f:14b8 | Syntek          | Lenovo EasyCamera        | 7.7%   | 4.1.15   | 39A9917502 |
| 174f:2408 | Syntek          | EasyCamera               | 6%     | 4.5.2    | C3D3D42413 |
| 174f:2426 | Syntek          | Integrated Camera        | 1.6%   | 4.18.0   | 2C9E565B99 |
| 174f:244c | Syntek          | Integrated Camera        | 0.6%   | 4.19.0   | 01C0AAC0E2 |
| 174f:5a35 | Syntek          | Sonix 1.3MPixel USB 2... | 1.5%   | 3.14.33  | 0A87DE5887 |
| 174f:6a33 | Syntek          | Web Cam - Asus F3SA, ... | 100%   |          | 0070B5EDA7 |
| 174f:6a51 | Syntek          | 2.0MPixel Web Cam - A... | 100%   |          | 224062149F |
| 174f:a821 | Syntek          | Web Cam - Packard Bel... | 100%   |          | 7D3E06E670 |
| 1782:4011 | Spreadtrum C... | Spreadtrum Phone         | 100%   |          | 78F12B69B1 |
| 17ef:4816 | Lenovo          | Integrated Webcam        | 1.2%   | 3.14.44  | 85AC90E935 |
| 1871:01b0 | Aveo Technology | Cheetah3 USB2.0 Device   | 100%   |          | 850E097AF9 |
| 18d1:4ee2 | Google          | Nexus Device (debug)     | 45%    | 4.15.0   | 11C4E43EEF |
| 18d1:4ee5 | Google          | Nexus 4 (PTP)            | 50%    | 5.4.28   | 383D5B106E |
| 18ec:3288 | Arkmicro Tec... | USB2.0 PC CAMERA         | 33.3%  | 4.1.22   | 9149BE671F |
| 18ec:3399 | Arkmicro Tec... | USB2.0 PC CAMERA         | 0.6%   | 3.14.25  | 9D9E2DB550 |
| 1908:2310 | GEMBIRD         | USB2.0 PC CAMERA         | 1.2%   | 4.1.15   | 0359993339 |
| 1908:2311 | GEMBIRD         | Generic UVC 1.00 came... | 2.1%   | 3.14.53  | CEAABF908D |
| 1b17:6111 | DarkHorse .     | USB2.0 Web Camera        | 100%   |          | 6E9BA31D2B |
| 1b3b:2938 | iPassion Tec... | PC Camera/Webcam cont... | 100%   |          | 87142BF4F1 |
| 1b3f:2002 | Generalplus ... | 808 Camera               | 2.3%   | 3.10.0   | 8F5CBE37DA |
| 1bbb:0170 | T & A Mobile... | VFD 529                  | 100%   |          | 875A197A28 |
| 1bcf:0b15 | Sunplus Inno... | Lihappe8 Webcam L0485... | 33.3%  | 5.4.0    | 38F7B776C9 |
| 1bcf:2802 | Sunplus Inno... | Laptop_Integrated_Web... | 1%     | 3.14.44  | F33530C32A |
| 1bcf:288a | Sunplus Inno... | 1.3M HD WebCam           | 1.2%   | 3.14.44  | 8FE3AF49FB |
| 1bcf:2b8a | Sunplus Inno... | Integrated_Webcam_HD     | 0.9%   | 3.14.44  | 7FE7F3FA13 |
| 1bcf:2b8b | Sunplus Inno... | Integrated_Webcam_HD     | 1.3%   | 3.14.44  | AA72A49A15 |
| 1bcf:2b90 | Sunplus Inno... | Integrated_Webcam_HD     | 2.7%   | 4.9.20   | 89D1209C2C |
| 1bcf:2b95 | Sunplus Inno... | Integrated_Webcam_HD     | 1.8%   | 4.9.0    | 26DBEC9F3A |
| 1bcf:2b96 | Sunplus Inno... | Integrated_Webcam_HD     | 1.1%   | 4.4.0    | D4927A9F76 |
| 1bcf:2c54 | Sunplus Inno... | HD WebCam                | 1.5%   | 3.14.39  | 81B19839F7 |
| 1bcf:2c6e | Sunplus Inno... | Laptop Integrated Web... | 1.2%   | 3.14.25  | 8D6D195DA2 |
| 1bcf:2c81 | Sunplus Inno... | HD WebCam                | 1%     | 4.1.15   | AA51C338B2 |
| 1bcf:2c87 | Sunplus Inno... | HP Wide Vision HD        | 2%     | 4.9.20   | 7BD53B3FFB |
| 1bcf:2c9b | Sunplus Inno... | HP TrueVision HD Camera  | 1.3%   | 4.9.60   | FB1A60597A |
| 1c4f:3000 | SiGma Micro     | Micro USB Web Camera     | 14.3%  | 5.0.0    | 7E7AD89D55 |
| 1d6c:1278 | HD WEBCAM       | NexiGo N60 FHD Webcam    | 33.3%  | 5.4.0    | EA5438D5FF |
| 2104:0124 | Tobii Techno... | EyeChip                  | 6.7%   | 4.9.60   | ACA7993158 |
| 22b8:2e83 | Motorola PCS    | Moto E (4) Plus          | 100%   |          | BC5ED8DEA4 |
| 22d9:2771 | MediaTek        | CPH1725                  | 50%    | 5.4.0    | 546A8D0043 |
| 2672:0049 | GoPro           | HERO8 BLACK              | 100%   |          | 08D6E7094F |
| 2717:ff10 | Xiaomi          | Mi/Redmi series (PTP)    | 66.7%  | 4.15.0   | D633DC9722 |
| 2970:4011 | Fly             | Life Jet                 | 100%   |          | 0C91AAB0FF |
| 2a70:904d | OnePlus         | GM1913                   | 100%   |          | D24E39C945 |
| 2a70:904e | OnePlus Tech... | A3000 phone (PTP mode... | 50%    | 5.9.16   | AA5B21E7DC |
| 30c9:0013 | Luxvisions I... | HP TrueVision HD Camera  | 1%     | 4.15.0   | 68C95D0921 |
| 5986:0143 | Acer            | HP Webcam                | 2.9%   | 4.1.16   | 0C8D7641B2 |
| 5986:014c | Acer            | BisonCam, NB Pro         | 1.6%   | 3.14.44  | F20EE95A8B |
| 5986:024b | Acer            | BisonCam, NB Pro         | 3%     | 3.14.44  | CD89DD62C8 |
| 5986:02d5 | Acer            | Integrated Camera        | 2%     | 3.14.44  | 55427995B5 |
| 5986:0652 | Acer            | Lenovo EasyCamera        | 0.3%   | 3.14.33  | EEFC7C92B2 |
| 5986:0683 | Acer            | BisonCam, NB Pro         | 2%     | 4.9.20   | 54574B77F2 |
| 5986:06b0 | Acer            | EasyCamera               | 3.7%   | 4.12.14  | 4869EA7144 |
| 5986:06b3 | Acer            | EasyCamera               | 2.3%   | 4.1.25   | D64B4A56E0 |
| 5986:0710 | Acer            | EasyCamera               | 20%    | 5.4.0    | 588AC16C28 |
| 5986:1127 | Acer            | EasyCamera               | 1.1%   | 4.9.60   | FE5BE9FB83 |
| 5986:1141 | Acer            | Integrated IR Camera     | 3.4%   | 4.15.0   | 6A667C9BA7 |
| 5986:210f | Acer            | EasyCamera               | 2.4%   | 4.4.0    | C3AA7A6297 |
| 5986:2113 | Acer            | Integrated Camera        | 0.3%   | 4.13.0   | 6A667C9BA7 |
| 5986:2130 | Acer            | Integrated Camera        | 1.1%   | 4.15.0   | 9C5D15BE62 |
| 5986:9102 | Acer            | BisonCam,NB Pro          | 1.5%   | 4.15.0   | 8E06C0291F |
| 6993:b019 | Yealink Netw... |                          | 100%   |          | 26DBEC9F3A |
| a16f:0304 | GenesysLogic... | USB2.0 UVC PC Camera     | 6.7%   | 4.9.111  | 50E7973730 |

### Card reader (USB)

21 out of 28 (75%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 04b4:5218 | Cypress Semi... | USB-Serial Bridge        | 100%   |          | 12CC462C7E |
| 04b4:521a | Cypress Semi... | USB-I2C Bridge           | 100%   |          | 12FFAAEFB1 |
| 04e6:512b | SCM Microsys... | SDI011 Contactless Re... | 100%   |          | 3810E77092 |
| 04e6:e003 | SCM Microsys... | SPR532 PinPad SmartCa... | 100%   |          | E035F59C6A |
| 062d:0001 | Taiwan Tai-H... | Smart Card Reader        | 100%   |          | 52D70A47DA |
| 072f:9000 | Advanced Car... | ACR38 AC1038-based Sm... | 24%    | 4.15.0   | 5A1B84993B |
| 0b0c:003f | Todos AB        | Todos C400 smartcard ... | 100%   |          | 03201EED9F |
| 0b97:7732 | O2 Micro        | Smart Card Reader        | 100%   |          | 16BEFD9DC3 |
| 0bda:0129 | Realtek Semi... | RTS5129 Card Reader C... | 0.3%   | 4.15.0   | 9A767F85C2 |
| 0bda:0139 | Realtek Semi... | RTS5139 Card Reader C... | 0.5%   | 3.10.34  | FC7DACB9EF |
| 0bda:0150 | Realtek Semi... | Realtek USB 2.0 Card ... | 20%    | 5.11.6   | 3C44204AA0 |
| 0c45:1018 | Microdia        | Compact Flash storage... | 100%   |          | 696C2127B6 |
| 0c4b:0500 | Reiner SCT K... | cyberJack RFID standa... | 90%    | 4.4.4    | 8A1C4909D6 |
| 0c4b:0501 | Reiner SCT K... | cyberJack RFID comfor... | 86.1%  | 4.19.0   | AC530E40AD |
| 0ca6:0010 | Castles Tech... | EZUSB PC/SC Smart Car... | 72.7%  | 5.8.0    | 72DB0D0125 |
| 0d8c:5200 | C-Media Elec... | Mass Storage Controll... | 100%   |          | 87456F207B |
| 11c5:0521 | Inmax           | IMT-0521 Smartcard Re... | 100%   |          | 6DCD3425DF |
| 17ef:3075 | Lenovo          | USB Billboard Device     | 100%   |          | 3C1D98DCE9 |
| 17ef:3078 | Lenovo          | USB Billboard            | 100%   |          | 13078A648E |
| 17ef:a38f | Lenovo          | 40AS                     | 3.6%   | 4.18.0   | 087EAF3A29 |
| 2ce3:9563 |                 | EMV Smartcard Reader     | 100%   |          | 6B0ED71AF5 |

### Chipcard (USB)

70 out of 87 (80.46%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0403:e3b4 | Future Techn... | Parsec Desktop Reader... | 100%   |          | 775160993D |
| 046a:002d | Cherry          | SmartTerminal XX44       | 100%   |          | C5B35954B5 |
| 046a:0070 | Cherry          | SmartTerminal XX1X       | 50%    | 5.4.0    | 181CA18DFB |
| 048d:1365 | Integrated T... | SmartCard Reader         | 100%   |          | DB4B891E15 |
| 04cc:5072 | ST-Ericsson     | Chipcard Reader          | 100%   |          | 65FD9B5315 |
| 04e6:5115 | SCM Microsys... | SCR335 SmartCard Reader  | 66.7%  | 5.3.0    | 89AB993C4A |
| 04e6:5116 | SCM Microsys... | SCR331-LC1 / SCR3310 ... | 80%    | 4.18.0   | A0E1E8DA67 |
| 04e6:5119 | SCM Microsys... | SCR3340 - ExpressCard... | 62.5%  | 3.10.0   | 81A0B5F406 |
| 04e6:5410 | SCM Microsys... | SCR35xx Smart Card Re... | 100%   |          | 3878A93172 |
| 04e6:e001 | SCM Microsys... | SCR331 SmartCard Reader  | 63.6%  | 3.10.0   | 7BDC2B1BB3 |
| 0529:0620 | Aladdin Know... | Token JC                 | 75%    | 2.6.32   | 57EDA985A5 |
| 058f:9520 | Alcor Micro     | Watchdata W 1981         | 86.5%  | 4.15.0   | 4F4FA6D3F6 |
| 058f:9522 | Alcor Micro     | EMV Smartcard Reader     | 100%   |          | 713028C9F2 |
| 058f:9540 | Alcor Micro     | AU9540 Smartcard Reader  | 89.3%  | 4.13.0   | 21BB7408E3 |
| 072f:2200 | Advanced Car... | ACR122U                  | 42.9%  | 4.15.0   | 9F4B9FFCAF |
| 072f:2224 | Advanced Car... | ACR1281 1S Dual Reader   | 33.3%  | 5.4.0    | 04E5B85D84 |
| 072f:90cc | Advanced Car... | ACR38 SmartCard Reader   | 42.6%  | 4.8.13   | D461E042A0 |
| 072f:90de | Advanced Car... | Token USB 64K            | 50%    | 4.1.25   | 02F1FBC843 |
| 072f:b000 | Advanced Car... | ACR3901U                 | 100%   |          | A44B651190 |
| 072f:b100 | Advanced Car... | ACR39U                   | 33.3%  | 5.4.0    | 32E899AFFD |
| 076b:1021 | OmniKey         | CardMan 1021             | 61.5%  | 4.15.0   | E1DC5A8EA7 |
| 076b:3021 | OmniKey         | CardMan 3021 / 3121      | 68.4%  | 3.14.33  | B3A1AE5051 |
| 076b:3031 | OmniKey         | 3x21 Smart Card Reader   | 25%    | 5.4.0    | 11EBF93798 |
| 076b:4321 | OmniKey         | CardMan 4321             | 100%   |          | DFC4564C84 |
| 076b:5421 | OmniKey         | Smart Card Reader USB    | 100%   |          | A72E3CC74F |
| 076b:a022 | OmniKey         | CardMan Smart@Link       | 100%   |          | 0138C33179 |
| 0783:0006 | C3PO            | LTC31v2                  | 100%   |          | AC8A218E93 |
| 0783:0036 | C3PO            | USB SMART CARD READER    | 50%    | 5.4.0    | 86286FAD9C |
| 08e6:3437 | Gemalto (was... | GemPC Twin SmartCard ... | 60%    | 4.10.0   | 23294D490E |
| 08e6:3438 | Gemalto (was... | GemPC Key SmartCard R... | 77.8%  | 5.9.1    | 2ADC81FAD9 |
| 08e6:34ec | Gemalto (was... | Compact Smart Card Re... | 94.4%  | 4.15.0   | 68610FE700 |
| 09c3:0013 | HID Global      | USB Reader V3            | 50%    | 5.8.10   | D53C2A8B0E |
| 0a5c:5800 | Broadcom        | BCM5880 Secure Applic... | 98.4%  | 3.10.36  | 1CF0DBBCB7 |
| 0a5c:5801 | Broadcom        | BCM5880 Secure Applic... | 95.1%  | 3.16.7   | 4A565EC7DE |
| 0a5c:5802 | Broadcom        | BCM5880 Secure Applic... | 96.9%  | 5.7.9    | 522D36A07E |
| 0a5c:5804 | Broadcom        | BCM5880 Secure Applic... | 96.2%  | 5.5.9    | F53A693225 |
| 0a5c:5805 | Broadcom        | 5880                     | 100%   |          | 4C46B3C18D |
| 0a5c:5832 | Broadcom        | 5880                     | 91.9%  | 3.10.0   | 9B726CE28D |
| 0a5c:5833 | Broadcom        | 5880                     | 100%   |          | 0CBB50CF63 |
| 0a5c:5834 | Broadcom        | 5880                     | 85.5%  | 3.10.0   | FFDB13EDA0 |
| 0a5c:5842 | Broadcom        | 58200                    | 84.8%  | 4.15.0   | 4A47F18D16 |
| 0a5c:5843 | Broadcom        | 58200                    | 89.7%  | 5.3.16   | A19F6677DB |
| 0a89:0025 | Aktiv           | Rutoken lite             | 66.7%  | 4.1.25   | 3728A3298E |
| 0b97:7762 | O2 Micro        | Oz776 SmartCard Reader   | 100%   |          | 116568909E |
| 0b97:7772 | O2 Micro        | OZ776 CCID Smartcard ... | 98.2%  | 4.15.0   | 71AA7CA9C7 |
| 0bda:0165 | Realtek Semi... | Smart Card Reader Int... | 75%    | 4.4.0    | A892A8230A |
| 0bf8:1006 | Fujitsu Siem... | SmartCard Reader 2A      | 83.3%  | 5.8.6    | B04F10E40A |
| 0bf8:1024 | Fujitsu Siem... | Smartcard Reader D323    | 100%   |          | 3BD076E0FA |
| 0c4b:0551 | Reiner SCT K... | tanJack USB              | 100%   |          | 5660749E4E |
| 0c4b:0580 | Reiner SCT K... | cyberJack one            | 100%   |          | 641E5EEB2A |
| 0c4b:9102 | Reiner SCT K... | cyberJack RFID basis ... | 100%   |          | DECA40F736 |
| 0ca6:00a0 | Castles Tech... | EZCCID Smart Card Reader | 100%   |          | 3DC7A36CB3 |
| 0d46:3010 | Kobil Systems   | KOBIL Class 3 Reader     | 100%   |          | CE2E3AD9AE |
| 0d46:3014 | Kobil Systems   | Smart Token              | 100%   |          | 5F126B3966 |
| 0dc3:1004 | Athena Smart... | ASEDrive V2C             | 91.7%  | 5.4.0    | C1FCE855C8 |
| 1059:0017 | Giesecke & D... | StarSign CUT             | 80%    | 5.8.0    | 518DC99F15 |
| 147e:2020 | Upek            | TouchChip Fingerprint... | 99.6%  | 5.4.0    | B79CAD571B |
| 15cf:0019 | Avtor           | SecureToken              | 100%   |          | 196CDBC09E |
| 17ef:1003 | Lenovo          | Integrated Smart Card... | 94.5%  | 3.10.0   | 68649A4EF8 |
| 1a44:0001 | VASCO Data S... | Digipass 905 SmartCar... | 43.8%  | 4.15.0   | 52E2D527CD |
| 1a44:0870 | VASCO Data S... | DIGIPASS 870             | 72.7%  | 5.4.0    | A011C9B38F |
| 1c34:91b1 | SpringCard      | Two                      | 100%   |          | F93D4537CB |
| 1fc9:010b | NXP Semicond... | PR533                    | 100%   |          | 2F9F2D0497 |
| 20a0:4108 | Clay Logic      | Nitrokey Pro             | 6.7%   | 4.19.0   | 9C7B7CDE1E |
| 20a0:4211 | Clay Logic      | Nitrokey Start           | 28.6%  | 4.19.0   | FF64809DC3 |
| 20a0:4230 | Clay Logic      | Nitrokey HSM             | 100%   |          | DEDECE32F6 |
| 23a0:0004 | BIFIT           | iBank2Key                | 100%   |          | A8A89AC09A |
| 24dc:0101 | ARDS            | JaCarta                  | 85.7%  | 4.15.0   | 4D5E452411 |
| 25dd:1101 | BIT4ID          | miniLector-S             | 100%   |          | D40236931F |
| 25dd:3111 | BIT4ID          | miniLector EVO           | 83.3%  | 5.4.0    | 93ACC58EFB |

### Converter (USB)

4 out of 7 (57.14%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0403:1237 | Future Techn... | Z397 GUARD Converter     | 100%   |          | 5F015278B6 |
| 0403:7a58 | Future Techn... | USB <-> Serial Cable     | 94.7%  | 4.15.0   | 0188249C12 |
| 0a12:0042 | Cambridge Si... | SPI Converter            | 100%   |          | E1C0C74CA6 |
| 110a:1110 | Moxa Technol... | UPort 1110               | 66.7%  | 4.9.124  | 3864E6C70F |

### Disk (USB)

58 out of 2562 (2.26%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0000:0000 |                 | UHCI Host Controller     | 4.8%   | 3.14.44  | B3175C4255 |
| 048d:1336 | Integrated T... | SD/MMC Cardreader        | 0.3%   | 3.14.22  | 2CA048A380 |
| 04e8:61b6 | Samsung Elec... | M3 Portable Hard Drive   | 0.7%   | 4.1.13   | 192F91ADA6 |
| 054c:05ba | Sony            | Storage Media            | 1.4%   | 3.14.44  | 23BBED2E16 |
| 058f:6362 | Alcor Micro     | Flash Card Reader/Writer | 0.1%   | 3.8.12   | 0D4B7AD71C |
| 058f:6366 | Alcor Micro     | Multi Flash Reader       | 0%     | 3.10.0   | 1EC8AF3962 |
| 05dc:a01a | Lexar Media     | Echo                     | 50%    | 5.4.0    | 15870EE6D4 |
| 05e3:0716 | Genesys Logic   | USB 2.0 Multislot Car... | 0.3%   | 3.14.25  | C2EDD5FBAF |
| 05e3:0723 | Genesys Logic   | GL827L SD/MMC/MS Flas... | 1.9%   | 3.10.0   | ACD23BB798 |
| 05e3:0743 | Genesys Logic   | SDXC and microSDXC Ca... | 2.2%   | 4.9.0    | 694EF3AE75 |
| 0624:0251 | Avocent         | Virtual Mass Storage     | 40%    | 4.15.0   | 98EA3E97E6 |
| 0624:0252 | Avocent         | XEN                      | 50%    | 5.4.0    | 98EA3E97E6 |
| 0718:069c | Imation         | TF35 USB 3.0             | 80%    | 5.8.0    | 92BF714334 |
| 0718:1905 | Imation         | M100 USB 3               | 25%    | 4.15.0   | 1F2C6BC8AF |
| 0781:5567 | SanDisk         | Cruzer Blade             | 0.2%   | 5.4.0    | 8CB76BB2F8 |
| 0781:5576 | SanDisk         | Cruzer Facet             | 2.6%   | 3.14.44  | 8A05529E0C |
| 0781:557e | SanDisk         | USB Flash Drive          | 12.5%  | 4.9.60   | E6F5C041EA |
| 0781:5581 | SanDisk         | Ultra                    | 0.2%   | 3.10.0   | F2FC35BC80 |
| 0781:5591 | SanDisk         | Ultra Flair              | 0.2%   | 4.1.15   | A39E2E7FA3 |
| 0781:55a5 | SanDisk         | Cruzer U                 | 1.5%   | 3.14.44  | 49EFA544EE |
| 090c:1000 | Silicon Motion  | Silicon-Power8G          | 0%     | 2.6.32   | 0C8D7641B2 |
| 0930:6545 | Toshiba         | Kingston DataTraveler... | 0.1%   | 3.14.25  | DA71739B25 |
| 0951:1603 | Kingston Tec... | DataTraveler 1GB/2GB ... | 1.2%   | 3.14.25  | FCD84BA9A1 |
| 0951:1666 | Kingston Tec... | DataTraveler 100 G3/G... | 0.2%   | 4.18.0   | 729161E56A |
| 0984:0301 | Apricorn        | SATAWire 6G              | 6.7%   | 4.4.0    | D20CC6E64D |
| 0a89:0030 | Aktiv           | Rutoken ECP              | 37.5%  | 4.1.25   | 1BB59DF9A7 |
| 0b05:5600 | ASUSTek Comp... | Android                  | 20%    | 4.1.22   | A1896B3549 |
| 0bda:0158 | Realtek Semi... | USB 2.0 multicard reader | 0.1%   | 2.6.32   | 7E32FFE51A |
| 0bda:0184 | Realtek Semi... | RTS5182 Card Reader      | 1%     | 3.14.44  | 6566319F04 |
| 0bda:0316 | Realtek Semi... | SD/MMC                   | 0.4%   | 3.14.44  | CB716FCDD9 |
| 0bda:0328 | Realtek Semi... | SD/MMC CRW               | 0.4%   | 3.10.0   | 4B9BEB25C2 |
| 0bda:1a2b | Realtek Semi... | Driver Storage           | 1.7%   | 4.15.0   | 582669A738 |
| 0e8d:0002 | MediaTek        | 1030D                    | 23.1%  | 4.9.60   | E4B342382F |
| 1004:631f | LG Electronics  | Optimus Android Phone... | 33.3%  | 4.15.0   | 38035357A1 |
| 1005:b113 | Apacer Techn... | Handy Steno 2.0/HT203    | 0.5%   | 3.0.28   | 9BFC9A8D7B |
| 1058:1130 | Western Digi... | My Book Essential (WD... | 9.1%   | 3.14.44  | DB141EF161 |
| 1058:25ee | Western Digi... | My Book 25EE             | 0.7%   | 4.4.0    | 911280F4FC |
| 12d1:2590 | Huawei Techn... | ORINOQUIA Auyantepui+... | 100%   |          | BEBC187DBD |
| 1307:0330 | Transcend       | 63-in-1 Multi-Card Re... | 0.4%   | 3.14.25  | 6752479144 |
| 1307:1171 | Transcend       | Fingerprint Reader       | 88.9%  | 4.12.14  | F38B4218AA |
| 13fd:1617 | Initio          | Flash Padlock            | 100%   |          | 0189BBB867 |
| 13fe:4300 | Kingston Tec... | USB DISK                 | 0.3%   | 4.1.38   | 704DE6C8EA |
| 13fe:5500 | Kingston Tec... | Patriot Memory           | 0.7%   | 3.14.44  | CE392DF9C0 |
| 14cd:125c | Super Top       | SD card reader           | 4.7%   | 3.14.44  | D461E042A0 |
| 152d:0578 | JMicron Tech... | JMS578 SATA 6Gb/s        | 0.3%   | 4.1.25   | 0A975A35B9 |
| 174c:55aa | ASMedia Tech... | ASM1051E SATA 6Gb/s b... | 0.1%   | 4.15.0   | BE1A115B55 |
| 19d2:2004 | ZTE WCDMA Te... | ZTE CDMA Technologies... | 33.3%  | 4.13.0   | 096216B249 |
| 1bcf:0c31 | Sunplus Inno... | SPIF30x Serial-ATA br... | 0.5%   | 3.10.34  | 650B03C57A |
| 1c6b:a222 | Philips & Li... | DVD Writer Slimtype e... | 6.7%   | 4.1.22   | 7A6327AB7B |
| 1d5c:2000 | Fresco Logic    | FL2000/FL2000DX VGA/D... | 51.4%  | 4.15.0   | B6812B6242 |
| 1f75:0611 | Innostor Tec... | IS611 SATA/PATA Bridg... | 1.7%   | 3.10.0   | EAF0F54B28 |
| 1f75:0817 | Innostor Tec... | innostor                 | 2.4%   | 4.1.25   | 06E385B318 |
| 2109:0711 | VIA Labs        | VL711 SATA 6Gb/s bridge  | 0.6%   | 4.1.38   | B246B730F4 |
| 5136:4678 | USB2.0          | Flash Disk 2.0           | 20%    | 4.1.38   | C1841B0A29 |
| 8564:1000 | Transcend       | JetFlash                 | 0.1%   | 3.10.19  | D49F64FC99 |
| 8644:8303 | Intenso GmbG    | USB Flash Disk           | 16.7%  | 4.9.20   | CE376CD0F4 |
| ffff:1201 | NAND            | USB2DISK                 | 2.5%   | 4.15.0   | A39E2E7FA3 |
| ffff:5678 | VendorCo        | Disk 2.0                 | 1.4%   | 3.10.0   | A9576F5520 |

### Dvb card (USB)

22 out of 80 (27.50%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 04ca:f01c | Lite-On Tech... | TT1280DA DVB-T TV Tuner  | 100%   |          | 646D7B3BFD |
| 07ca:0810 | AVerMedia Te... | H810 USB Hybrid DVB-T    | 100%   |          | B46F2FEE35 |
| 07ca:0830 | AVerMedia Te... | H830 USB Hybrid DVB-T    | 100%   |          | 79A097BF6F |
| 07ca:0831 | AVerMedia Te... | H831 USB Hybrid DVB-T/T2 | 100%   |          | D5A4F195AE |
| 07ca:1334 | AVerMedia Te... | H334 MiniCard Hybrid ... | 100%   |          | 54E6A4A4F7 |
| 07ca:1335 | AVerMedia Te... | H335C                    | 100%   |          | 81D55608B8 |
| 07ca:1336 | AVerMedia Te... | A336 MiniCard Hybrid ... | 100%   |          | A288705A4D |
| 07ca:1830 | AVerMedia Te... | AVerTV Volar Video Ca... | 100%   |          | A295A7FAC6 |
| 07ca:1831 | AVerMedia Te... | H831 USB Hybrid DVB-T/T2 | 100%   |          | 7DAAC9434C |
| 07ca:1871 | AVerMedia Te... | TD310 DVB-T/T2/C dongle  | 14.3%  | 5.3.8    | 26C41EBE1D |
| 07ca:3830 | AVerMedia Te... | H830 USB Hybrid DVB-T    | 100%   |          | BB4AEE1CE5 |
| 07ca:3867 | AVerMedia Te... | A867                     | 100%   |          | 159AB17857 |
| 07ca:4336 | AVerMedia Te... | A336 MiniCard Hybrid ... | 100%   |          | 0C3E26BCE7 |
| 07ca:a373 | AVerMedia Te... | A373                     | 100%   |          | 22317B4B49 |
| 0bda:2832 | Realtek Semi... | RTL2832U DVB-T           | 34.3%  | 4.1.19   | 6A8CCD44AA |
| 0bda:2838 | Realtek Semi... | RTL2838 DVB-T            | 13.2%  | 3.14.25  | BEB0D03960 |
| 1164:1f08 | YUAN High-Te... | STK7700D                 | 15.4%  | 3.14.44  | 2DCD0E4E69 |
| 1164:3edc | YUAN High-Te... | STK7700D                 | 100%   |          | DF82BB0E17 |
| 13d3:3282 | IMC Networks    | DVB-T + GPS Minicard ... | 100%   |          | 7F0F347502 |
| 1b80:c161 | Afatech         | DVB-T 2                  | 100%   |          | 2A8FB37B8C |
| 1b80:e39a | Afatech         | DVB-T395U [af9015]       | 100%   |          | 2A8FB37B8C |
| eb1a:5013 | eMPIA Techno... | USB 2883 Device          | 100%   |          | 5DD14F9164 |

### Fingerprint reader (USB)

90 out of 96 (93.75%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 045e:00bd | Microsoft       | Fingerprint Reader       | 100%   |          | 4F0031F39F |
| 0483:2016 | STMicroelect... | Fingerprint Reader       | 100%   |          | 8A05529E0C |
| 04e8:7301 | Samsung Elec... | Fingerprint Device       | 100%   |          | C2FAFA6C24 |
| 04e8:7309 | Samsung Elec... | Fingerprint Device       | 100%   |          | 739EE63E1D |
| 04e8:730a | Samsung Elec... | Fingerprint Device       | 100%   |          | 641AA732DA |
| 04e8:730b | Samsung Elec... | Fingerprint Sensor De... | 100%   |          | 662AF5B7D6 |
| 04f3:0903 | Elan Microel... | ELAN:Fingerprint         | 99.4%  | 5.4.0    | 72E52C0472 |
| 04f3:0c01 | Elan Microel... | ELAN:Fingerprint         | 100%   |          | EE3FF1A75D |
| 04f3:0c03 | Elan Microel... | ELAN:Fingerprint         | 100%   |          | 8697520F0A |
| 04f3:0c10 | Elan Microel... | ELAN:Fingerprint         | 100%   |          | 74C0BDD4EB |
| 04f3:0c1a | Elan Microel... | ELAN:Fingerprint         | 100%   |          | A8C47AD7F6 |
| 04f3:0c3a | Elan Microel... | Elan Security-WBF Fin... | 100%   |          | F3F60A5C06 |
| 05ba:0002 | DigitalPersona  | Fingerprint Scanner, ... | 100%   |          | AE361E5F23 |
| 05ba:000a | DigitalPersona  | Fingerprint Reader       | 78.6%  | 5.4.13   | 6CBCBA7414 |
| 06cb:0078 | Synaptics       | WBDI Device              | 100%   |          | 31CD72DB1B |
| 06cb:0081 | Synaptics       | Synaptics WBDI           | 100%   |          | A40F9103FA |
| 06cb:0082 | Synaptics       | Synaptics WBDI Finger... | 100%   |          | A48923935D |
| 06cb:009a | Synaptics       | Metallica MIS Touch F... | 95.4%  | 4.15.0   | E8E2BD3B06 |
| 06cb:009b | Synaptics       |                          | 100%   |          | 943D7DB9B3 |
| 06cb:00a2 | Synaptics       | Metallica MOH Touch F... | 100%   |          | 6D6D654A5A |
| 06cb:00a8 | Synaptics       |                          | 98.5%  | 5.8.0    | 98BE1903C4 |
| 06cb:00b7 | Synaptics       | Synaptics VFS7552 Tou... | 100%   |          | FA3E3FF217 |
| 06cb:00bb | Synaptics       |                          | 100%   |          | 638C4207CE |
| 06cb:00bd | Synaptics       | Prometheus MIS Touch ... | 99.5%  | 5.4.0    | 089C319771 |
| 06cb:00be | Synaptics       |                          | 100%   |          | C0EE92C218 |
| 06cb:00c7 | Synaptics       |                          | 100%   |          | B093A6F0EE |
| 06cb:00c9 | Synaptics       |                          | 98.9%  | 5.8.0    | FD2D87232F |
| 06cb:00df | Synaptics       | Synaptics FS7604 Touc... | 94.9%  | 5.6.0    | DEB906B69F |
| 06cb:00e7 | Synaptics       |                          | 100%   |          | E3BB17DEE5 |
| 06cb:00e9 | Synaptics       | Synaptics FS7604 Touc... | 100%   |          | 502CD63C0F |
| 08ff:1600 | AuthenTec       | AES1600                  | 100%   |          | 2494100ECB |
| 08ff:1660 | AuthenTec       | AES1660 Fingerprint S... | 100%   |          | A0E3328769 |
| 08ff:1680 | AuthenTec       | AES1660 Fingerprint S... | 100%   |          | 6C4DA274F4 |
| 08ff:1686 | AuthenTec       | Fingerprint Sensor       | 100%   |          | 3E43593D78 |
| 08ff:168a | AuthenTec       | Fingerprint Sensor       | 100%   |          | AF785987C5 |
| 08ff:168b | AuthenTec       | Fingerprint Sensor       | 100%   |          | BD61CCC317 |
| 08ff:168c | AuthenTec       | Fingerprint Sensor       | 100%   |          | 8D386EA5A9 |
| 08ff:168f | AuthenTec       | AES1660 Fingerprint S... | 98.8%  | 5.4.0    | 828A8AC75D |
| 08ff:2500 | AuthenTec       | AES2501                  | 100%   |          | 4DCFB332DF |
| 08ff:2550 | AuthenTec       | AES2550 Fingerprint S... | 98.7%  | 5.4.0    | 8E6CE923E0 |
| 08ff:2580 | AuthenTec       | AES2501 Fingerprint S... | 100%   |          | 8648B42278 |
| 08ff:2660 | AuthenTec       | AES2660 Fingerprint S... | 100%   |          | 0985E32752 |
| 08ff:2665 | AuthenTec       | Fingerprint Sensor       | 100%   |          | 12873CCE8E |
| 08ff:2683 | AuthenTec       | Fingerprint Sensor       | 100%   |          | 6AF6B1AA99 |
| 08ff:2691 | AuthenTec       | Fingerprint Sensor       | 100%   |          | 8395F7AEF5 |
| 08ff:2810 | AuthenTec       | AES2810                  | 100%   |          | C6B333E5E9 |
| 138a:0001 | Validity Sen... | VFS101 Fingerprint Re... | 100%   |          | 14F176409D |
| 138a:0005 | Validity Sen... | VFS301 Fingerprint Re... | 100%   |          | 662A781C83 |
| 138a:0007 | Validity Sen... | VFS451 Fingerprint Re... | 98.6%  | 4.15.0   | 86286FAD9C |
| 138a:0008 | Validity Sen... | VFS300 Fingerprint Re... | 100%   |          | E69A5A0142 |
| 138a:0010 | Validity Sen... | VFS Fingerprint sensor   | 100%   |          | 39DD5CA43B |
| 138a:0011 | Validity Sen... | VFS5011 Fingerprint R... | 99.4%  | 5.4.0    | D7921837F3 |
| 138a:0015 | Validity Sen... | VFS 5011 fingerprint ... | 100%   |          | 84DC871F65 |
| 138a:0017 | Validity Sen... | VFS 5011 fingerprint ... | 99.8%  | 4.18.0   | E12C82D1BE |
| 138a:0018 | Validity Sen... | Fingerprint scanner      | 100%   |          | FB309A7F37 |
| 138a:003c | Validity Sen... | VFS471 Fingerprint Re... | 99.3%  | 5.2.5    | 06BC21DB81 |
| 138a:003d | Validity Sen... | VFS491                   | 98.6%  | 5.4.0    | D1EDC3210E |
| 138a:003f | Validity Sen... | VFS495 Fingerprint Re... | 96.6%  | 4.9.0    | 136F81EF7F |
| 138a:0050 | Validity Sen... | Swipe Fingerprint Sensor | 100%   |          | 0F6A907976 |
| 138a:0090 | Validity Sen... | VFS7500 Touch Fingerp... | 99.6%  | 4.15.0   | 8347406C94 |
| 138a:0091 | Validity Sen... | VFS7552 Touch Fingerp... | 100%   |          | 4EA4747CBF |
| 138a:0092 | Validity Sen... | Synaptics VFS7552 Tou... | 100%   |          | 51178C1953 |
| 138a:0093 | Validity Sen... | Synaptics VFS7552 Tou... | 100%   |          | 579E1F3D79 |
| 138a:0094 | Validity Sen... | Synaptics WBDI           | 100%   |          | A4D6F3CCE4 |
| 138a:0097 | Validity Sen... | Synaptics WBDI           | 99.1%  | 5.8.0    | D3E1AE1C0C |
| 138a:009d | Validity Sen... | Synaptics WBDI           | 100%   |          | 847655CB40 |
| 138a:00a6 | Validity Sen... | Synaptics VFS7552 Tou... | 100%   |          | 466033EE28 |
| 138a:00ab | Validity Sen... | Synaptics VFS7552 Tou... | 100%   |          | 7454AF9190 |
| 147e:1000 | Upek            | Biometric Touchchip/T... | 100%   |          | DEF6307EBD |
| 147e:1001 | Upek            | TCS5B Fingerprint sensor | 100%   |          | 188765C8F8 |
| 147e:1002 | Upek            | Biometric Touchchip/T... | 100%   |          | 87EF82748D |
| 147e:2016 | Upek            | Biometric Touchchip/T... | 99.9%  | 5.4.0    | 1747F3D32A |
| 147e:3001 | Upek            | TCS1C EIM/STM32 Finge... | 100%   |          | 6D671DF349 |
| 147e:5002 | Upek            | TouchStrip Fingerprin... | 100%   |          | 335EF1CCCD |
| 1491:0020 | Futronic Tec... | FS81 Fingerprint Scan... | 33.3%  | 5.4.60   | F8BF9AFBE7 |
| 1c7a:0570 | LighTuning T... | EgisTec Touch Fingerp... | 100%   |          | 2B27DC30AC |
| 1c7a:0571 | LighTuning T... | EgisTec Touch Fingerp... | 100%   |          | 3BB19F53E9 |
| 1c7a:0577 | LighTuning T... | Fingerprint Sensor       | 100%   |          | F2D686D743 |
| 1c7a:0603 | LighTuning T... | ES603 Swipe Fingerpri... | 100%   |          | BF37A519FA |
| 1c7a:0801 | LighTuning T... | Fingerprint Reader       | 100%   |          | 7955F23581 |
| 27c6:5110 | Shenzhen Goo... | Goodix Fingerprint De... | 100%   |          | D9592EAD1E |
| 27c6:5117 | Shenzhen Goo... | Fingerprint Reader       | 100%   |          | 96C74BB052 |
| 27c6:530c | Shenzhen Goo... | Fingerprint Reader       | 100%   |          | 480FEF69F1 |
| 27c6:533c | Shenzhen Goo... | FingerPrint              | 100%   |          | B143ACDC5C |
| 27c6:538c | Shenzhen Goo... | Fingerprint Reader       | 100%   |          | C6F4D6DE84 |
| 27c6:5584 | Shenzhen Goo... | Fingerprint Reader       | 100%   |          | 348BE4B537 |
| 27c6:55a2 | Shenzhen Goo... | Goodix FingerPrint De... | 100%   |          | 28F6F5A90B |
| 27c6:55a4 | Shenzhen Goo... | Goodix FingerPrint De... | 100%   |          | 5632D74722 |
| 27c6:55b4 | Shenzhen Goo... | Fingerprint Reader       | 99.7%  | 5.3.0    | CD156B08D8 |
| 2808:9338 | Focal-system... | FT9201Fingerprint.       | 100%   |          | A4DB49A83F |

### Hardware key (USB)

4 out of 4 (100%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0471:485d | Philips (or ... | Senselock SenseIV v2.x   | 100%   |          | E4A6E39276 |
| 0a89:0003 | Aktiv           | Guardant Stealth 2       | 85.7%  | 5.4.60   | 5149320E81 |
| 0a89:0020 | Aktiv           | Rutoken S                | 75%    | 3.14.15  | B2FA33FC7E |
| 14a8:0001 | Soft protect... | Soft protection devic... | 100%   |          | 2CF2098617 |

### Hasp (USB)

1 out of 1 (100%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0529:0001 | Aladdin Know... | HASP copy protection ... | 98.3%  | 3.10.0   | 011928039E |

### Hub (USB)

28 out of 657 (4.26%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 03eb:3301 | Atmel           | at43301 4-Port Hub       | 1.6%   | 3.14.44  | 8CF625BE49 |
| 03eb:3325 | Atmel           | RDU_84_T7                | 100%   |          | 10DB69DD6C |
| 0424:2602 | Microchip Te... | USB 2.0 Hub              | 1.6%   | 4.1.19   | A8D52F4DF8 |
| 0451:1446 | Texas Instru... | TUSB2040/2070 Hub        | 2%     | 4.15.0   | 593A72A02B |
| 0451:4040 | Texas Instru... | Hub                      | 100%   |          | FCA58FF529 |
| 05e3:0606 | Genesys Logic   | USB 2.0 Hub / D-Link ... | 0.1%   | 3.14.39  | 9AB71624F9 |
| 05e3:0608 | Genesys Logic   | Hub                      | 0%     | 2.6.32   | DC387F9472 |
| 05e3:0610 | Genesys Logic   | Hub                      | 0%     | 3.10.0   | 1C3C4D9F98 |
| 05e3:0612 | Genesys Logic   | Hub                      | 0.1%   | 3.10.0   | 6F21980996 |
| 05e3:0616 | Genesys Logic   | hub                      | 0.3%   | 4.1.15   | 1C3C4D9F98 |
| 0a05:7211 | Unknown Manu... | hub                      | 2.5%   | 3.14.44  | E17CB89C8C |
| 0a5c:4500 | Broadcom        | BCM2046B1 USB 2.0 Hub... | 0%     | 3.0.28   | C64FCF2A5D |
| 0bda:5429 | Realtek Semi... | USB-C Computer Dockin... | 50%    | 5.6.19   | BCF22D328E |
| 1a40:0101 | Terminus Tec... | Hub                      | 0%     | 3.2.0    | 9596ECB170 |
| 1d6b:0002 | Linux Founda... | 2.0 root hub             | 0%     | 3.10.0   | FAF8BFF3BC |
| 1d6b:0003 | Linux Founda... | 3.0 root hub             | 0%     | 3.10.0   | FAF8BFF3BC |
| 2109:0810 | VIA Labs        | VL81x Hub                | 0.8%   | 3.14.33  | B1EFC2E064 |
| 2109:0813 | VIA Labs        | VL813 Hub                | 0.2%   | 3.10.0   | 1EC556E585 |
| 2109:2811 | VIA Labs        | Hub                      | 0.2%   | 3.10.0   | B16B2D9BD5 |
| 2109:2813 | VIA Labs        | VL813 Hub                | 0.2%   | 3.10.0   | 1EC556E585 |
| 2109:2817 | VIA Labs        | USB2.0 Hub               | 0.2%   | 4.4.154  | 5C7374311F |
| 2109:8817 | VIA Labs        | USB Billboard Device     | 95.5%  | 4.15.0   | C836825EA8 |
| 214b:7250 | Huasheng Ele... | USB2.0 HUB               | 0.3%   | 3.10.0   | DE7F4C6EE9 |
| 8087:0020 | Intel           | Integrated Rate Match... | 0%     | 3.0.28   | 57943279FE |
| 8087:0024 | Intel           | Integrated Rate Match... | 0%     | 3.10.0   | 7F0B8FB732 |
| 8087:8000 | Intel           | Integrated Rate Match... | 0%     | 3.10.0   | F5AC359422 |
| 8087:8001 | Intel           | Integrated Hub           | 0.1%   | 2.6.32   | BD6F7205F3 |
| 8087:8008 | Intel           | Integrated Rate Match... | 0%     | 3.10.0   | F5AC359422 |

### Human interface (USB)

32 out of 901 (3.55%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 03f0:150c | Hewlett-Packard | Mood Lighting (Microc... | 33.3%  | 5.4.0    | 0E1FA2C583 |
| 0424:274c | Microchip Te... | Hub Controller           | 0.7%   | 4.4.0    | D05C262E67 |
| 043e:9a39 | LG Electronics  | LG Monitor Controls      | 5.7%   | 4.15.0   | C8754F5971 |
| 044f:b106 | ThrustMaster    | T.Flight Stick X         | 20%    | 4.9.20   | 3B0BCF8DF9 |
| 044f:b10a | ThrustMaster    | T.16000M Joystick        | 2.2%   | 4.1.25   | 417453E269 |
| 045e:0659 | Microsoft       | HoloLens Sensors         | 8.3%   | 4.19.0   | A0BFCEB399 |
| 046d:c122 | Logitech        | Harmony 650/700 Remote   | 100%   |          | D7BCE39C2A |
| 0483:91d1 | STMicroelect... | Sensor Hub               | 0.5%   | 3.10.34  | BFA1F898FB |
| 048d:5702 | Integrated T... | ITE Device               | 2.5%   | 4.15.0   | EF3422DD2D |
| 04b4:fd13 | Cypress Semi... | Programmable power so... | 50%    | 4.18.0   | E7E5ACB3BB |
| 056d:4044 | EIZO            | EIZO USB HID Monitor     | 100%   |          | 5391547134 |
| 057e:0337 | Nintendo        | Wii U GameCube Contro... | 12.5%  | 5.4.0    | 50704A4B1B |
| 05ac:1393 | Apple           | AirPods case             | 25%    | 5.0.0    | CCED083509 |
| 096e:0201 | Feitian Tech... | USB DONGLE               | 66.7%  | 5.3.0    | ED3C250112 |
| 0971:2005 | Gretag-Macbeth  | Huey                     | 50%    | 4.1.13   | F456137399 |
| 0b05:1726 | ASUSTek Comp... | Laptop OLED Display      | 22.2%  | 3.14.44  | 2DCD0E4E69 |
| 0b05:175b | ASUSTek Comp... | Laptop OLED Display      | 12.5%  | 3.14.44  | 919044CAEC |
| 0b05:1867 | ASUSTek Comp... | AURA Custom Human int... | 1.2%   | 4.9.60   | 730F732CC8 |
| 11ff:3341 |                 | USB Joystick             | 20%    | 4.1.7    | CD7FA9B160 |
| 1462:7b93 | Micro Star I... | MYSTIC LIGHT             | 10.8%  | 4.15.0   | 5D99916419 |
| 1462:7c37 | Micro Star I... | MYSTIC LIGHT             | 0.5%   | 4.15.0   | 1DA5ED3876 |
| 1770:ff00 | MSI             | steel series rgb keyb... | 0.4%   | 3.10.0   | CF444064FC |
| 1781:0e57 | Multiple Ven... | GP Controller            | 50%    | 5.4.0    | E38AF664D6 |
| 187c:0520 | Alienware       | M17x                     | 3.3%   | 3.14.44  | 95838487AA |
| 187c:0550 | Alienware       | LED controller           | 1%     | 4.9.60   | 61D3FD5A59 |
| 1b1c:0a34 | Corsair         | ST100 LED Driver         | 8.3%   | 5.0.0    | F706762428 |
| 1b1c:0c04 | Corsair         | Link Cooling Node        | 1.4%   | 3.14.44  | A3C554166C |
| 1e71:170e | NZXT            | Kraken X                 | 1.4%   | 4.15.0   | 60038B2000 |
| 2386:3122 | Raydium         |                          | 100%   |          | 2E25D9AAFA |
| 2386:350e | Raydium         | Touch System             | 14.3%  | 4.15.0   | 0636C222DC |
| 2687:fb01 | Fitbit          | Base Station             | 3.3%   | 3.14.22  | 88110D5A78 |
| 2dc8:ab20 | SNES30          | Joy                      | 100%   |          | E6BB5EBB05 |

### Imaging (USB)

1 out of 2 (50%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 04a7:04d0 | Visioneer       | Xerox DocuMate 5460      | 100%   |          | 4ABAC242CC |

### Input/keyboard (USB)

21 out of 2448 (0.86%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 046d:c30e | Logitech        | UltraX Keyboard (Y-BL49) | 1.1%   | 3.14.44  | C0A9C9443B |
| 046d:c52b | Logitech        | Unifying Receiver        | 0%     | 3.10.0   | 8FC2C0633B |
| 046d:c534 | Logitech        | Unifying Receiver        | 0%     | 3.10.0   | AB3C4986E4 |
| 0483:5710 | STMicroelect... | Joystick in FS Mode      | 10%    | 4.9.60   | 9925C456E7 |
| 048d:8297 | Integrated T... | IT8297 RGB LED Contro... | 0.3%   | 4.12.14  | EFA77A90CB |
| 048d:ce00 | Integrated T... | ITE Device(8291)         | 2.9%   | 4.15.0   | 734DFCBE37 |
| 04d9:1505 | Holtek Semic... | Holtek Keyboard          | 25%    | 5.4.0    | 162B1C972A |
| 05ac:0236 | Apple           | Internal Keyboard/Tra... | 0.6%   | 4.1.16   | C6A5BE7D44 |
| 0624:0294 | Avocent         | Dell 03R874 KVM dongle   | 9.1%   | 3.10.0   | 97313ACF09 |
| 0a5c:4502 | Broadcom        | Keyboard (Boot Interf... | 0.2%   | 3.0.28   | 0C3E26BCE7 |
| 0b05:17fd | ASUSTek Comp... | ASUS ROG Macrokey        | 3.1%   | 3.14.44  | C5777BA928 |
| 0c45:7401 | Microdia        | TEMPer Temperature Se... | 74.1%  | 3.10.0   | 4F755869D0 |
| 0c45:7811 | Microdia        | USB FS Keyboard          | 25%    | 5.4.0    | 4F8794ED64 |
| 1050:0405 | Yubico.com      | Yubikey 4 OTP+CCID       | 33.3%  | 5.2.9    | B0543D9256 |
| 1050:0407 | Yubico.com      | Yubikey 4/5 OTP+U2F+CCID | 0.3%   | 3.10.0   | 454B6BB43A |
| 150a:1201 |                 | Keyboard                 | 50%    | 5.4.0    | 16C99D1061 |
| 1532:0228 | Razer USA       | BlackWidow Elite         | 1.4%   | 4.15.0   | 9127A5128E |
| 1a2c:4c5e | China Resour... | USB Keyboard             | 0.2%   | 4.1.38   | B3F2FAB399 |
| 258a:0001 | SINO WEALTH     | USB KEYBOARD             | 0.2%   | 3.10.0   | DE7F4C6EE9 |
| 25a7:fa11 | Areson Techn... | 2.4G Wireless Receiver   | 18.2%  | 5.4.0    | 1C3C4D9F98 |
| 28de:1142 | Valve Software  | Wireless Steam Contro... | 0.3%   | 4.18.16  | 36EAF717E9 |

### Input/mouse (USB)

28 out of 2675 (1.05%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 03eb:8a0c | Atmel           | maXTouch Digitizer       | 37.5%  | 4.15.0   | E994E96768 |
| 0458:003a | KYE Systems ... | NetScroll+ Mini Trave... | 0.1%   | 3.10.0   | 5599435B69 |
| 045e:0040 | Microsoft       | Wheel Mouse Optical      | 0.2%   | 3.10.0   | BFCD766C51 |
| 046d:c06c | Logitech        | Optical Mouse            | 0.4%   | 2.6.32   | C6690BB6D9 |
| 046d:c08e | Logitech        | MX518 Gaming Mouse       | 1.3%   | 4.15.0   | C0A9C9443B |
| 046d:c52f | Logitech        | Unifying Receiver        | 0%     | 3.10.0   | 0F6A89EF2C |
| 048d:8910 | Integrated T... | ITE Device(829x)         | 1.4%   | 4.13.0   | 2D91F64A77 |
| 04b4:0033 | Cypress Semi... | Mouse                    | 0.6%   | 3.14.25  | 4BCDE0B215 |
| 08ca:0010 | Aiptek Inter... | Tablet                   | 6.7%   | 3.14.44  | D295EC1834 |
| 0a5c:4503 | Broadcom        | Mouse (Boot Interface... | 0.2%   | 3.0.28   | A175422412 |
| 0b57:80b3 | Beijing Hanw... | Tablet                   | 100%   |          | 4B67EBD0C6 |
| 0b57:8501 | Beijing Hanw... | Tablet                   | 100%   |          | D77D4E79EB |
| 0b57:9016 | Beijing Hanw... | Beijing Hanwang Gener... | 100%   |          | EA3F987020 |
| 0bc7:0006 | X10 Wireless... | Wireless Transceiver ... | 10.7%  | 3.14.25  | 52C3157C62 |
| 0c45:5101 | Microdia        | 2.4G Wireless Device ... | 2.7%   | 4.15.0   | 1E15CE5E51 |
| 1038:1366 | SteelSeries ApS | Kinzu V2 Gaming Mouse    | 7.7%   | 4.1.15   | 50422D6C3F |
| 10c4:8108 | Silicon Labs    | USB OPTICAL MOUSE        | 0.4%   | 4.15.0   | CF1C2A4B27 |
| 1532:0037 | Razer USA       | DeathAdder 2013          | 0.9%   | 3.14.39  | D3BEA910CB |
| 1532:0042 | Razer USA       | Abyssus 2014             | 3.8%   | 4.9.76   | 31E99D9CEA |
| 18d1:4ee7 | Google          | Nexus/Pixel Device (c... | 80%    | 5.0.0    | 05F84C951F |
| 18f8:0f97 | [Maxxter]       | Optical Gaming Mouse ... | 0.1%   | 3.10.0   | BEADDBA484 |
| 1b1c:1b2e | Corsair         | Gaming M65 Pro RGB Mouse | 0.9%   | 4.8.0    | 4490A8D493 |
| 1b1c:1b51 | Corsair         | DARK CORE RGB SE Wire... | 4.8%   | 4.15.18  | E6AE7E8546 |
| 1c4f:0034 | SiGma Micro     | XM102K Optical Wheel ... | 0.1%   | 3.10.0   | 6834F4BC15 |
| 248a:8366 | Maxxter         | Wireless Optical Mous... | 0.2%   | 3.13.0   | BB566782BC |
| 256c:006e | TABLET          | Pen                      | 2.4%   | 4.1.16   | 1B290B3823 |
| 413c:8158 | Dell            | Integrated Touchpad /... | 86.2%  | 3.14.44  | 90762831E7 |
| 413c:8162 | Dell            | Integrated Touchpad [... | 83.3%  | 3.14.33  | B512B8997F |

### Modem (USB)

13 out of 197 (6.60%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0482:081f | Kyocera         | USB Device               | 100%   |          | 189475C3F5 |
| 04e8:6773 | Samsung Elec... | HSPA Modem               | 40%    | 4.15.0   | 3AD0FF0E13 |
| 0572:cb16 | Conexant Sys... | USB-ADSL Modem           | 100%   |          | 07217A2477 |
| 0baf:00ec | U.S. Robotics   | 56K Faxmodem             | 100%   |          | EF974030B3 |
| 0bdb:1900 | Ericsson Bus... | F3507g Mobile Broadba... | 1.4%   | 3.10.0   | 704DE6C8EA |
| 0bdb:1926 | Ericsson Bus... | H5321 gw Mobile Broad... | 2.1%   | 3.10.0   | 55427995B5 |
| 1209:1776 | InterBiometrics | Io                       | 15%    | 4.18.0   | AA8F2E17CA |
| 1965:0017 | Uniden          | BC125AT                  | 100%   |          | B636969767 |
| 22b8:40c0 | Motorola PCS    | W180 Mobile              | 100%   |          | 942ECE6E49 |
| 27c6:5301 | Shenzhen Goo... | Fingerprint Reader       | 0.3%   | 4.4.0    | 716CB93844 |
| 27c6:5381 | Shenzhen Goo... | Goodix Fingerprint De... | 2.8%   | 4.15.0   | C99B5F8C72 |
| 27c6:5395 | Shenzhen Goo... | Fingerprint Reader       | 5.3%   | 4.15.0   | 0FE92C8A70 |
| 2c99:0002 | Prusa           | Original Prusa i3 MK3    | 100%   |          | 0CF52B6B45 |

### Net/ethernet (USB)

1 out of 15 (6.67%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 03f0:0547 | Hewlett-Packard | L2311c LAN7500 Ethernet  | 100%   |          | EBB304F58E |

### Net/wimax (USB)

5 out of 7 (71.43%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 8086:0186 | Intel           | WiMAX Connection 2400m   | 12%    | 3.14.44  | E3B9A4233B |
| 8086:0187 | Intel           | Centrino Advanced-N +... | 8.3%   | 4.19.0   | 700DE148A7 |
| 8086:0188 | Intel           | WiMAX Connection 2400m   | 3.7%   | 4.9.9    | 6A0780CA42 |
| 8086:1406 | Intel           | WiMAX Connection 2400m   | 4.5%   | 3.10.19  | 3B6AB87F14 |
| 8087:07d6 | Intel           | Centrino Wireless-N +... | 11%    | 3.10.34  | 06C149DAB6 |

### Net/wireless (USB)

141 out of 420 (33.57%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 03f0:3b1d | Hewlett-Packard | Novatel Wireless 4G      | 100%   |          | FE7EE46763 |
| 03f0:581d | Hewlett-Packard | lt4112 Gobi 4G Module... | 6.2%   | 3.14.15  | E25F4ADB0B |
| 03f0:9d1d | Hewlett-Packard | HP lt4120 Snapdragon ... | 1.7%   | 4.4.1    | 2502C3D7E7 |
| 0411:0242 | BUFFALO         | 802.11ac WLAN Adapter    | 28.6%  | 4.15.0   | D92D4F0666 |
| 0457:0162 | Silicon Inte... | SiS162 usb Wireless L... | 100%   |          | 0A302BFAFD |
| 045e:028f | Microsoft       | Xbox360 Wireless Cont... | 100%   |          | 6977CB0073 |
| 045e:0292 | Microsoft       | Xbox360 Wireless Netw... | 100%   |          | 957117D4E3 |
| 045e:02e6 | Microsoft       | Wireless XBox Control... | 41.4%  | 4.19.0   | EFB44A46DD |
| 045e:02f9 | Microsoft       | Xbox Embedded Wireless   | 100%   |          | 1AED3EE552 |
| 045e:02fe | Microsoft       | XBOX ACC                 | 40%    | 5.4.0    | 98D52182A0 |
| 045e:0719 | Microsoft       | Xbox 360 Wireless Ada... | 0.8%   | 3.14.44  | 909FA88618 |
| 050d:1106 | Belkin Compo... | F9L1106v1 802.11a/b/g... | 100%   |          | EB677B25BF |
| 050d:1109 | Belkin Compo... | F9L1109v1 802.11a/b/g... | 100%   |          | E2265C3C14 |
| 050d:110a | Belkin Compo... | F9L1101v2 802.11abgn ... | 90%    | 5.8.0    | A502E8842E |
| 050d:615a | Belkin Compo... | F7D4101 / F9L1101v1 8... | 100%   |          | 04CE720011 |
| 050d:7050 | Belkin Compo... | F5D7050 Wireless G Ad... | 33.3%  | 5.4.0    | 7AC6824CEB |
| 056e:400a | Elecom          | 802.11ac WLAN            | 100%   |          | CFF1BAF251 |
| 057c:8502 | AVM             | FRITZ!WLAN AC 430        | 33.3%  | 5.1.9    | 7125E8AAA2 |
| 057c:8503 | AVM             | FRITZ!WLAN AC 860        | 5.7%   | 4.15.0   | A8D4B67DE8 |
| 057c:8602 | AVM             | FRITZ!WLAN USB Stick ... | 100%   |          | 6275993E94 |
| 0586:3425 | ZyXEL Commun... | NWD6505 802.11a/b/g/n... | 75%    | 5.4.0    | 26FD738844 |
| 0586:3426 | ZyXEL Commun... | ZyXEL Dual-Band Wirel... | 42.9%  | 4.15.0   | 8962D3E09B |
| 05c6:9001 | Qualcomm        | Gobi Wireless Modem      | 100%   |          | AACC9842E1 |
| 06b9:0121 | Alcatel Telecom | SpeedTouch 121g Wirel... | 100%   |          | D7C5E1D3E4 |
| 07d1:3a0d | D-Link System   | DWA-120 802.11g Wirel... | 100%   |          | 96DE7C819B |
| 07d1:3b01 | D-Link System   | AirPlus G DWL-G122 Wi... | 100%   |          | A55363D509 |
| 07d1:3b11 | D-Link System   | DWA-130 802.11n Wirel... | 100%   |          | 606522CEDA |
| 07d1:3c09 | D-Link System   | DWA-140 RangeBooster ... | 6.7%   | 4.1.16   | 211A9802DB |
| 083a:9a22 | Accton Techn... | WN7522BEP Wireless LA... | 100%   |          | 2BF53FC215 |
| 0846:4240 | NetGear         | WG111(v1) rev 2 54 Mb... | 100%   |          | 394B9426A3 |
| 0846:9011 | NetGear         | WNDA3100v2 802.11abgn... | 100%   |          | E4BFD31EF8 |
| 0846:9014 | NetGear         | WNDA3100v3 802.11abgn... | 90%    | 5.4.0    | 54DD671B29 |
| 0846:9020 | NetGear         | WNA3100(v1) Wireless-... | 100%   |          | B5C18575BF |
| 0846:9042 | NetGear         | On Networks N150MA 80... | 100%   |          | 0E5402CD3F |
| 0846:9050 | NetGear         | A6200 802.11a/b/g/n/a... | 100%   |          | 9730ABD01E |
| 0846:9052 | NetGear         | A6100 AC600 DB Wirele... | 57.7%  | 4.15.0   | 1CCB5B0600 |
| 0846:9053 | NetGear         | A6210                    | 10.5%  | 4.15.0   | 40AE5C532F |
| 0846:9054 | NetGear         | Nighthawk A7000 802.1... | 70%    | 5.0.0    | 3721F71FB0 |
| 0846:9055 | NetGear         | A6150                    | 66.7%  | 5.8.0    | DD53E0757E |
| 0951:16e7 | Kingston Tec... | HyperX CloudX Flight ... | 100%   |          | 12425CC77D |
| 0a5c:bd11 | Broadcom        | BCM4320 802.11bg Wire... | 100%   |          | CA66B01DF7 |
| 0a5c:bd13 | Broadcom        | BCM4323 802.11abgn Wi... | 100%   |          | 2B3378419F |
| 0a5c:bd16 | Broadcom        | BCM4319 802.11bgn Wir... | 100%   |          | AA0CA44BD4 |
| 0a93:0201 | C Technologi... | CLX.PayPen-Wireless      | 100%   |          | FEE1E401AD |
| 0b05:17c9 | ASUSTek Comp... | USB-AC53 802.11a/b/g/... | 100%   |          | C7951A3833 |
| 0b05:17d1 | ASUSTek Comp... | AC51 802.11a/b/g/n/ac... | 26%    | 4.19.0   | ADC4529AFF |
| 0b05:17d2 | ASUSTek Comp... | USB-AC56 802.11a/b/g/... | 29%    | 3.14.79  | 1CF830ACD9 |
| 0b05:17db | ASUSTek Comp... | WiFi                     | 100%   |          | 93C92CF446 |
| 0b05:1817 | ASUSTek Comp... | USB-AC68 802.11a/b/g/... | 84.2%  | 4.15.0   | E1EFA9FC86 |
| 0b05:1841 | ASUSTek Comp... | 802.11ac NIC             | 50%    | 4.15.0   | E8C4D5BC53 |
| 0b05:184c | ASUSTek Comp... | 802.11ac NIC             | 76.9%  | 4.15.0   | 3DC677388A |
| 0b05:1852 | ASUSTek Comp... | 802.11ac NIC             | 12.5%  | 5.4.0    | DA4C7A6493 |
| 0b05:1853 | ASUSTek Comp... | 802.11ac NIC             | 100%   |          | 78E05B078E |
| 0bda:0811 | Realtek Semi... | Realtek 8812AU/8821AU... | 71%    | 4.15.0   | 1B86C3E879 |
| 0bda:8172 | Realtek Semi... | RTL8191SU 802.11n WLA... | 0.4%   | 3.10.0   | 167CB26122 |
| 0bda:8176 | Realtek Semi... | RTL8188CUS 802.11n WL... | 0.7%   | 3.14.25  | 3635CADDD6 |
| 0bda:8179 | Realtek Semi... | RTL8188EUS 802.11n Wi... | 1.3%   | 3.14.25  | F0EE94E6C2 |
| 0bda:8187 | Realtek Semi... | RTL8187 Wireless Adapter | 1.4%   | 3.14.44  | F63AFE7E2A |
| 0bda:818b | Realtek Semi... | RTL8192EU 802.11b/g/n... | 6.7%   | 4.9.0    | 59B2905D0D |
| 0bda:8193 | Realtek Semi... | RTL8192DU 802.11an WL... | 100%   |          | 04346614FA |
| 0bda:8194 | Realtek Semi... | 802.11n NIC              | 50%    | 5.4.0    | 8B55873FBD |
| 0bda:8812 | Realtek Semi... | RTL8812AU 802.11a/b/g... | 41.1%  | 4.1.38   | C77A0AE517 |
| 0bda:8813 | Realtek Semi... | RTL8814AU 802.11a/b/g... | 55.6%  | 4.18.16  | 74FED2A2B8 |
| 0bda:881a | Realtek Semi... | 802.11n NIC              | 16.7%  | 5.4.0    | 2B311CE9E4 |
| 0bda:a811 | Realtek Semi... | RTL8811AU 802.11a/b/g... | 68.6%  | 4.4.0    | 4FEDA9BC8E |
| 0bda:b711 | Realtek Semi... | RTL8188GU 802.11n WLA... | 78.9%  | 5.4.0    | 8177EE7A36 |
| 0bda:b812 | Realtek Semi... | RTL88x2bu [AC1200 Tec... | 65.2%  | 4.4.0    | D9927FC022 |
| 0bda:c811 | Realtek Semi... | 802.11ac NIC             | 66.9%  | 4.4.0    | 4C98EF4248 |
| 0bda:f179 | Realtek Semi... | RTL8188FTV 802.11b/g/... | 78%    | 4.15.0   | 8110FAD44D |
| 0bda:f192 | Realtek Semi... | 802.11n WLAN Adapter     | 91.7%  | 5.4.85   | 041C426AE1 |
| 0bf8:100f | Fujitsu Siem... | miniCard D2301 802.11... | 100%   |          | 20512BBBE4 |
| 0cde:0015 | Z-Com           | XG-705A 802.11g Wirel... | 100%   |          | B4E374835E |
| 0cf3:1006 | Qualcomm Ath... | TP-Link TL-WN322G v3 ... | 1.5%   | 3.10.0   | 5D53E48607 |
| 0cf3:9271 | Qualcomm Ath... | AR9271 802.11n           | 0.9%   | 3.14.25  | E87B8FA941 |
| 0e8d:7603 | MediaTek        | 802.11 n WLAN            | 100%   |          | 7C3CADB886 |
| 0e8d:760c | MediaTek        | 802.11 n WLAN            | 100%   |          | DC64C81C35 |
| 0e8d:7610 | MediaTek        | WiFi                     | 26.2%  | 4.15.0   | 94CB5C6788 |
| 0e8d:7612 | MediaTek        | MT7612U 802.11a/b/g/n... | 19.2%  | 5.0.0    | 2373345C64 |
| 13b1:000a | Linksys         | WUSB54G v2 802.11g Ad... | 100%   |          | E6B8191910 |
| 13b1:0029 | Linksys         | WUSB300N 802.11bgn Wi... | 100%   |          | 18CF7C0503 |
| 13b1:0039 | Linksys         | AE1200 802.11bgn Wire... | 12.5%  | 4.15.0   | 7538D3A313 |
| 13b1:003a | Linksys         | AE2500 802.11abgn Wir... | 100%   |          | 29F9412B5B |
| 13b1:003e | Linksys         | AE6000 802.11a/b/g/n/... | 16.7%  | 5.3.0    | C27987482D |
| 13b1:003f | Linksys         | WUSB6300 802.11a/b/g/... | 66.1%  | 4.1.19   | F323B316A2 |
| 13b1:0042 | Linksys         | WUSB6100M 802.11a/b/g... | 5.9%   | 4.15.0   | 5155142A94 |
| 13b1:0043 | Linksys         | WUSB6400M                | 77.8%  | 5.4.0    | CD49ABE808 |
| 148f:3070 | Ralink Techn... | RT2870/RT3070 Wireles... | 0.1%   | 3.10.42  | DA645FE697 |
| 148f:5372 | Ralink Techn... | RT5372 Wireless Adapter  | 0.6%   | 3.10.0   | 6372F1B176 |
| 148f:7601 | Ralink Techn... | MT7601U Wireless Adapter | 7.2%   | 3.10.0   | 9D65301476 |
| 148f:760b | Ralink Techn... | MT7601U Wireless Adapter | 26.3%  | 3.14.33  | 165079588D |
| 148f:761a | Ralink Techn... | MT7610U ("Archer T2U"... | 31.2%  | 4.15.0   | DE264500C8 |
| 16f0:0003 | GN ReSound A/S  | Airlink Wireless Prog... | 100%   |          | 7EC6FBAC2B |
| 1799:8051 | Thales Norwa... | Belkin F5D8051 v2 802... | 100%   |          | 179E7C2689 |
| 1b75:8171 | Ovislink        | WN-370USB 802.11bgn W... | 100%   |          | 90FCEED1B5 |
| 1eda:2610 | AirTies Wire... | AirTies Wireless Adapter | 100%   |          | 591BDD6E15 |
| 2001:330f | D-Link          | DWA-125 11n Adapter      | 2.9%   | 3.14.44  | 01D21EA756 |
| 2001:3312 | D-Link          | Wireless N Nano USB A... | 100%   |          | 4629800E33 |
| 2001:3314 | D-Link          | DWA-171 AC600 DB Wire... | 53.5%  | 4.4.0    | 8406DEE7F4 |
| 2001:3315 | D-Link          | DWA-182 Wireless AC D... | 27.7%  | 3.14.39  | 19E3CFF2BE |
| 2001:3318 | D-Link          | 11ac adapter             | 66.7%  | 4.1.34   | BEFFD605B7 |
| 2001:3319 | D-Link          | Wireless N Nano USB A... | 17%    | 4.1.38   | C98634A421 |
| 2001:331a | D-Link          | 11ac Adapter             | 55.6%  | 5.3.0    | 8EBA4AAB16 |
| 2001:331b | D-Link          | WLAN controller          | 13%    | 4.15.0   | DEDD73D125 |
| 2001:331c | D-Link          | 802.11ac NIC             | 53.1%  | 4.15.0   | D248A5F049 |
| 2001:331d | D-Link          | DWA-171                  | 51.5%  | 5.4.0    | 0616FFAFA3 |
| 2001:331e | D-Link          | 802.11ac NIC             | 41.2%  | 5.8.16   | 9E8B256742 |
| 20f4:808a | TRENDnet        | 802.11ac NIC             | 100%   |          | F61A93BFBC |
| 226a:817b | Realtek         | 802.11n WLAN Adapter     | 100%   |          | 7ECF2BB4CB |
| 2357:0101 | TP-Link         | RTL8812AU Archer T4U ... | 48.6%  | 4.1.25   | 846D636ECA |
| 2357:0103 | TP-Link         | Archer T4UH wireless ... | 50%    | 3.14.44  | 66E54253FB |
| 2357:0105 | TP-Link         | Archer T1U 802.11a/n/... | 34.3%  | 5.0.0    | 116FFA29C6 |
| 2357:0106 | TP-Link         | Archer T9UH v1 [Realt... | 79.4%  | 4.15.0   | 332AE3E89F |
| 2357:0107 | TP-Link         | TL-WN821N v5/v6 [RTL8... | 8.3%   | 4.15.0   | 68A3D97EC6 |
| 2357:0108 | TP-Link         | TL-WN822N Version 4 R... | 4.4%   | 4.4.0    | A35DED4130 |
| 2357:0109 | TP-Link         | TL-WN823N v2/v3 [Real... | 6.1%   | 3.16.0   | 5452F92C7B |
| 2357:010b | TP-Link         | Archer T2UHP [MediaTe... | 100%   |          | 759A043B60 |
| 2357:010c | TP-Link         | TL-WN722N v2/v3 [Real... | 3.3%   | 4.9.41   | 046AA45464 |
| 2357:010d | TP-Link         | 802.11n NIC              | 60%    | 4.15.0   | 1CF6D1DAEA |
| 2357:010e | TP-Link         | TL-WN722N v2             | 75%    | 5.7.0    | CE020DD17D |
| 2357:0111 | TP-Link         | 802.11n NIC              | 27.3%  | 4.15.0   | CF6242CACA |
| 2357:0115 | TP-Link         | Archer T4U ver.3         | 67.3%  | 4.15.0   | EB5985FA85 |
| 2357:011e | TP-Link         | 802.11ac WLAN Adapter    | 69.5%  | 4.4.0    | 18CA89B617 |
| 2357:011f | TP-Link         | 802.11ac WLAN Adapter    | 67.1%  | 4.15.0   | EA920B884B |
| 2357:0120 | TP-Link         | 802.11ac WLAN Adapter    | 53.2%  | 4.15.0   | 9BC8B1B4E5 |
| 2357:0122 | TP-Link         | 802.11n NIC              | 50%    | 4.18.0   | 7F6510382A |
| 2357:0126 | TP-Link         | 802.11n NIC              | 52.4%  | 4.18.0   | B2276DA50D |
| 2357:012d | TP-Link         | Archer T3U [Realtek R... | 56.2%  | 4.4.0    | FB6A95C937 |
| 2357:0138 | TP-Link         | 802.11ac NIC             | 73.3%  | 5.4.0    | 2128085080 |
| 2604:0012 | Tenda           | U12                      | 50%    | 4.15.0   | 9C21C30887 |
| 2c4e:0100 | Mercucys        | MW300UM RTL8192EU wifi   | 78.9%  | 4.9.124  | 6CA29DAA21 |
| 2c4e:0102 | Mercucys        | 802.11n NIC              | 26.7%  | 5.4.0    | CBF18515B3 |
| 2c4e:0103 | MediaTek        | 802.11ac WLAN            | 50%    | 5.5.7    | 9946078BC6 |
| 413c:8102 | Dell            | TrueMobile 1300 802.1... | 100%   |          | 5776ED841E |
| 413c:81b6 | Dell            | DW5811e Snapdragon™... | 1.9%   | 4.1.25   | 568A079F29 |
| 4317:0720 | Broadcom        | Dynex DX-BUSB            | 100%   |          | 806CA649D7 |
| 7392:7811 | Edimax Techn... | EW-7811Un 802.11n Wir... | 0.6%   | 4.1.25   | FC3F785613 |
| 7392:a812 | Edimax Techn... | AC600 USB                | 45.2%  | 3.14.25  | C21AF112B2 |
| 7392:a822 | Edimax Techn... | 802.11n NIC              | 57.1%  | 5.4.0    | 5C28995118 |
| 7392:a833 | Edimax Techn... | AC1750 USB               | 40%    | 4.15.0   | EADEFAE73E |
| 7392:b822 | Edimax Techn... | EW-7822ULC 802.11ac W... | 77.3%  | 4.18.0   | 86AD9D1053 |
| a727:6893 | 3Com            | 3CRUSB20075 OfficeCon... | 100%   |          | 968045D52D |

### Network (USB)

16 out of 295 (5.42%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 03f0:411d | Hewlett-Packard | lt2522 Mobile Broadba... | 100%   |          | 8F0A119262 |
| 03f0:541d | Hewlett-Packard | hs3114 HSPA+ Mobile B... | 100%   |          | 4D8CCEE335 |
| 03f0:8e1d | Hewlett-Packard | hs3110 HSPA+ Mobile B... | 100%   |          | 310DD72B6A |
| 045e:091e | Microsoft       | XBOX ACC                 | 100%   |          | BAA04FAF58 |
| 04cc:226e | ST-Ericsson     |                          | 100%   |          | 0B958B270D |
| 05ac:12ab | Apple           | iPad 4/Mini1             | 8.3%   | 4.10.0   | 226AD1E0E2 |
| 0b95:7720 | ASIX Electro... | AX88772                  | 2.4%   | 4.4.0    | A41B1E7E12 |
| 0bda:8153 | Realtek Semi... | RTL8153 Gigabit Ether... | 0.6%   | 3.10.0   | F6BA1DA69A |
| 0bda:b720 | Realtek Semi... | 802.11n WLAN Adapter     | 1.4%   | 4.4.1    | 0F4722247C |
| 17e9:4324 | DisplayLink     | Plugable UGA-2KHDMI      | 33.3%  | 4.18.0   | DD1DF827C7 |
| 17ef:3082 | Lenovo          | ThinkPad TBT 3 Dock      | 1.5%   | 4.18.0   | B6F9682F0B |
| 1e7e:a4a1 | Linux 2.6.35... | Ethernet Gadget          | 100%   |          | 27E85EAA28 |
| 22b8:2e24 | Motorola PCS    | moto g power             | 1.6%   | 3.14.44  | 4BBF74E26D |
| 2cb7:0002 | Fibocom         | L831-EAU                 | 7.1%   | 4.9.155  | C0B7A3C300 |
| 2cb7:0210 | Fibocom         | L830-EB-00 LTE WWAN M... | 1%     | 4.15.0   | 12B5E06A49 |
| 413c:819a | Dell            | DW5802 4G (LTE-3G) Mo... | 100%   |          | 937EA2CB74 |

### Sound (USB)

11 out of 1171 (0.94%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 041e:3232 | Creative Tec... | Sound Blaster Premium... | 6.1%   | 4.1.25   | 4514D59538 |
| 046d:0a03 | Logitech        | Logitech USB Microphone  | 3.7%   | 4.12.14  | 250509DF15 |
| 046d:0a46 | Logitech        | Stereo H650e             | 14.3%  | 5.0.0    | 46B504A53C |
| 0763:2012 | M-Audio         | M-Audio Fast Track Pro   | 4.8%   | 4.15.0   | 1D9934126C |
| 09e8:0076 | AKAI Profess... | LPK25 MIDI Keyboard      | 14.3%  | 3.14.44  | F1C95A10CC |
| 0a12:1243 | Cambridge Si... | CSRA64110 USB Audio      | 12.5%  | 4.15.0   | D2A62B6AFB |
| 0d8c:0005 | C-Media Elec... | Blue Snowball            | 0.5%   | 4.15.0   | F2CC8FAE4D |
| 15e4:0025 | Numark          | iDJ3                     | 100%   |          | AE8CCF0298 |
| 194f:0302 | PreSonus Aud... | AudioBox USB             | 16.7%  | 4.15.0   | 03EEF2B7D3 |
| 1b1c:0a32 | Corsair         | ST100 Headset Output    | 8.3%   | 5.0.0    | F706762428 |
| 1b3f:2007 | Generalplus ... | USB Audio Device         | 20%    | 4.1.15   | CC62862FFE |

### Tv card (USB)

9 out of 161 (5.59%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0402:5602 | ALi             | M5602 Video Camera Co... | 1.4%   | 3.14.25  | 79A40B4127 |
| 046d:0892 | Logitech        | OrbiCam                  | 0.6%   | 3.10.0   | 6054B96BC5 |
| 046d:08a2 | Logitech        | Labtec Webcam Pro        | 14.3%  | 3.14.44  | 51837DE98F |
| 07ca:0889 | AVerMedia Te... | AVerTV Satellite 2       | 100%   |          | 174EC665C6 |
| 093a:2468 | Pixart Imaging  | SoC PC-Camera            | 8.5%   | 3.14.44  | B701C37D96 |
| 0ac8:c002 | Z-Star Micro... | Visual Communication ... | 10%    | 4.4.0    | 7F0BB0CC92 |
| 0c45:6030 | Microdia        | VideoCAM ExpressII       | 100%   |          | 6F28F56C47 |
| 0c45:6242 | Microdia        | PC Camera (SN9C201 + ... | 28.6%  | 4.9.20   | EF01565711 |
| 0c45:627b | Microdia        | PC Camera (SN9C201 + ... | 50%    | 5.10.0   | E5C5CE1445 |

### Ups (USB)

3 out of 22 (13.64%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0592:0002 | Powerware       | UPS (X-Slot)             | 5%     | 4.15.0   | 049C18DB44 |
| 06da:0002 | Phoenixtec P... | UPS                      | 100%   |          | 4F5E89A87E |
| 09ae:3016 | Tripp Lite      | UPS                      | 11.1%  | 5.3.0    | 76299BB9FF |

### Video (USB)

5 out of 12 (41.67%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 0fd9:0051 | Elgato Systems  | GameCapture HD           | 100%   |          | 3A3874784C |
| 1164:1ee9 | YUAN High-Te... | Polaris AV Capture       | 100%   |          | E1BB0618FD |
| 1b80:a41c | Afatech         | Polaris AV Capture       | 100%   |          | F20674C0B8 |
| 2304:0224 | Pinnacle Sys... | Pinnacle High Speed U... | 100%   |          | 97D31BFF69 |
| 5555:3382 | Epiphan Systems | VGA2USB Frame Grabber    | 100%   |          | 37A831391B |

### Wireless (USB)

1 out of 64 (1.56%)

| ID        | MFG             | Name                     | Missed | Linux    | Probe      |
|-----------|-----------------|--------------------------|--------|----------|------------|
| 15a9:003a | Gemtek          | Modem YOTA 4G LTE        | 50%    | 5.11.12  | 02E0DBC8D3 |

