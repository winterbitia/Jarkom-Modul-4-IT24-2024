# Jarkom-Modul-4-IT24-2024

| Nama | NRP |
|---|---|
|Amoes Noland|5027231028|
|Radella Chesa Syaharani|5027231064|

## Daftar Isi

- [Jarkom-Modul-4-IT24-2024](#jarkom-modul-4-it24-2024)
  - [Daftar Isi](#daftar-isi)
  - [Pendahuluan](#pendahuluan)
  - [Topologi](#topologi)
      - [Topologi GNS3 CIDR](#topologi-gns3-cidr)
      - [Topologi CPT VLSM](#topologi-cpt-vlsm)
  - [Routing Table](#routing-table)
  - [Subnetting GNS - Metode CIDR](#subnetting-gns---metode-cidr)
    - [Penggabungan IP](#penggabungan-ip)
    - [Tree CIDR](#tree-cidr)
    - [Pembagian IP](#pembagian-ip)
    - [Routing](#routing)
    - [Testing](#testing)
  - [Subnetting Cisco Packet Tracer - Metode VLSM](#subnetting-cisco-packet-tracer---metode-vlsm)
    - [Tree VLSM](#tree-vlsm)
    - [Pembagian IP](#pembagian-ip-1)
    - [Konfigurasi](#konfigurasi)
    - [Routing](#routing-1)
    - [Testing](#testing-1)

## Pendahuluan

## Topologi
#### Topologi GNS3 CIDR
![GNS3](assets/topo-gns3.png)

#### Topologi CPT VLSM
![CPT](assets/topo-cpt.png)

## Routing Table

| Nama Subnet | Rute | Jumlah IP | Netmask |
|---|---|---|---|
| A1 | Hololive > HoloID | 2 | /30 |
| A2 | Hololive > HoloID > AREA-15 | 2 | /30 |
| A3 | Hololive > HoloID > AREA-15 > Switch6 > Moona + Risu + lofi | 661 | /22 |
| A4 | Hololive > HoloID > holoro | 2 | /30 |
| A5 | Hololive > HoloID > holoro > Switch7 > Ollie + Anya + Reine | 34 | /26 |
| A6 | Hololive > HoloID > holoh3ro | 2 | /30 |
| A7 | Hololive > HoloID > holoh3ro > Switch8 > Zeta + Kaela + Kobo | 299 | /23 |
| A8 | Hololive > HoloJP | 2 | /30 |
| A9 | Hololive > HoloJP > Switch1 > DEV_IS + GEN:0 | 3 | /29 |
| A10 | Hololive > HoloJP > Switch1 > DEV_IS > Re:Gloss > Ririka_Raden + Ao + Hajime_Kanade | 14 | /28 |
| A11 | Hololive > HoloJP > Switch1 > GEN:0 > Switch3 > MiComet + Sora_Robo_AZK + GEN:1 | 2045 | /21 |
| A12 | Hololive > HoloJP > Switch1 > GEN:0 > Switch3 > GEN:1 > Member > FBK_Matsuri + Aki_Hachama | 470 | /23 |
| A13 | Hololive > HoloJP > Switch1 > GEN:0 > Switch3 > GEN:1 > GAMERS | 2 | /30 |
| A14 | Hololive > HoloJP > Switch1 > GEN:0 > Switch3 > GEN:1 > GAMERS > Fubuki > Korone + Okayu + Mio | 120 | /25 |
| A15 | Hololive > HoloEN | 2 | /30 |
| A16 | Hololive > HoloEN > HoloAdvent | 2 | /30 |
| A17 | Hololive > HoloEN > HoloAdvent > Switch0 > FuwaMoco + Shiori_Nerissa + Biboo | 28 | /27 |
| A18 | Hololive > HoloEN > Holo-Myth | 2 | /30 |
| A19 | Hololive > HoloEN > Holo-Myth > Switch2 > Gura_Ame_Ina + Kiara_Calli | 503 | /23 |
| A20 | Hololive > HoloEN > Holo-Myth > HoloPromise > Project-Hope + Holo_Council | 3 | /29 |
| A21 | Hololive > HoloEN > Holo-Myth > HoloPromise > Project-Hope > Irys | 3 | /29 |
| A22 | Hololive > HoloEN > Holo-Myth > HoloPromise > Holo-Council > Switch4 > Kronii_Mumei + Bae_Fauna | 62 | /26 |
| Total | | 4263 | /19 |

## Subnetting GNS - Metode CIDR

### Penggabungan IP

### Tree CIDR

### Pembagian IP

### Routing

### Testing

## Subnetting Cisco Packet Tracer - Metode VLSM

### Tree VLSM

![VLSM Tree](assets/VLSM.drawio.png)

### Pembagian IP

**Info :**
* Used IPs : 4263 (52.05%)
* Unused IPs : 3927 (47.94%)

Subnet | Network ID | Netmask | Broadcast | Range IP
|---|---|---|---|---|
A1 | 192.245.19.72 | 255.255.255.252 | 192.245.19.75 | 192.245.19.73 - 192.245.19.74
A2 | 192.245.19.92 | 255.255.255.252 | 192.245.19.95 | 192.245.19.93 - 192.245.19.94
A3 | 192.245.8.0 | 255.255.252.0 | 192.245.11.255 | 192.245.8.1 - 192.245.11.254
A4 | 192.245.19.96 | 255.255.255.252 | 192.245.19.99 | 192.245.19.97 - 192.245.19.98
A5 | 192.245.18.192 | 255.255.255.192 | 192.245.18.255 | 192.245.18.193 - 192.245.18.254
A6 | 192.245.19.100 | 255.255.255.252 | 192.245.19.103 | 192.245.19.101 - 192.245.19.102
A7 | 192.245.16.0 | 255.255.254.0 | 192.245.17.255 | 192.245.16.1 - 192.245.17.254
A8 | 192.245.19.104 | 255.255.255.252 | 192.245.19.107 | 192.245.19.105 - 192.245.19.106
A9 | 192.245.19.64 | 255.255.255.248 | 192.245.19.71 | 192.245.19.65 - 192.245.19.70
A10 | 192.245.19.32 | 255.255.255.240 | 192.245.19.47 | 192.245.19.33 - 192.245.19.46
A11 | 192.245.0.0 | 255.255.248.0 | 192.245.7.255 | 192.245.0.1 - 192.245.7.254
A12 | 192.245.14.0 | 255.255.254.0 | 192.245.15.255 | 192.245.14.1 - 192.245.15.254
A13 | 192.245.19.76 | 255.255.255.252 | 192.245.19.79 | 192.245.19.77 - 192.245.19.78
A14 | 192.245.18.0 | 255.255.255.128 | 192.245.18.127 | 192.245.18.1 - 192.245.18.126
A15 | 192.245.19.80 | 255.255.255.252 | 192.245.19.83 | 192.245.19.81 - 192.245.19.82
A16 | 192.245.19.84 | 255.255.255.252 | 192.245.19.87 | 192.245.19.85 - 192.245.19.86
A17 | 192.245.19.0 | 255.255.255.224 | 192.245.19.31 | 192.245.19.1 - 192.245.19.30
A18 | 192.245.19.88 | 255.255.255.252 | 192.245.19.91 | 192.245.19.89 - 192.245.19.90
A19 | 192.245.12.0 | 255.255.254.0 | 192.245.13.255 | 192.245.12.1 - 192.245.13.254
A20 | 192.245.19.48 | 255.255.255.248 | 192.245.19.55 | 192.245.19.49 - 192.245.19.54
A21 | 192.245.19.56 | 255.255.255.248 | 192.245.19.63 | 192.245.19.57 - 192.245.19.62
A22 | 192.245.18.128 | 255.255.255.192 | 192.245.18.191 | 192.245.18.129 - 192.245.18.190

### Konfigurasi

### Routing

### Testing