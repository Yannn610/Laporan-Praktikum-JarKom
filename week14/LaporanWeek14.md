NAMA: RIYAN CHANDRA SAPUTRA

NIM: 103072400129

KELAS: IF-04-02

LAPORAN PRAKTIKUM WEEK 14

1. Host sudah diasosiasikan dengan 30 Munroe St AP saat pelacakan dimulai. Pada t = 24,82, host membuat permintaan HTTP ke http://gaia.cs.umass.edu/wiresharklabs/alice.txt. Alamat IP gaia.cs.umass.edu adalah 128.119.245.12.
2. Pada t=32.82, host membuat permintaan HTTP ke http://www.cs.umass.edu, dengan alamat IP 128.119.240.19. Pada t = 49,58, host memutuskan sambungan dari 30 Munroe St AP dan mencoba menyambung ke linksys_ses_24086. Ini bukan titik akses terbuka,dan host akhirnya tidak dapat terhubung ke AP ini.
3. Pada t=63.0 tuan rumah menyerah mencoba untuk mengasosiasikan dengan linksys_ses_24086 AP, dan mengasosiasikan lagi dengan titik akses 30 Munroe St.
![](../week14/image/image1.png)
![](../week14/image/image2.png)


## Beacon Frames

Fungsi : Mengumumkan keberadaan jaringan WiFi (SSID) dan memberikan informasi konfigurasi jaringan kepada perangkat di sekitar.
![](../week14/image/image3.png)
Analisis :
SSID = 30 Munroe St
BSSID = 00:16:b6:f7:1d:51
SOURCEADDRESS = 00:16:b6:f7:1d:51
DESTINATIONADDRESS = ff:ff:ff:ff:ff:ff
Beacon Interval = BI = 100 Beacon Interval = 100 TU (Time Unit)

## Data Transfer

Fungsi : Mengirimkan data pengguna seperti HTTP, TCP, DNS, dan aplikasi lainnya melalui jaringan WiFi.
![](../week14/image/image4.png)


## Association/Disassociation

Fungsi Assocation Request : Association Request adalah frame yang dikirim oleh client (station) kepada Access Point untuk meminta izin bergabung ke jaringan WiFi.
![](../week14/image/image5.png)
Fungsi Assocation Response : B alasan dari Access Point terhadap permintaan Association Request dari client.
![](../week14/image/image6.png)
Fungsi Disassociation : Disassociation digunakan untuk mengakhiri hubungan antara client (station) dan Access Point pada jaringan WiFi. Tidak ditemukan frame Disassociation pada file capture Wireshark_802_11.pcap yang digunakan dalam praktikum. Hal ini menunjukkan bahwa selama proses perekaman tidak terjadi pemutusan hubungan antara client dan Access Point, atau proses tersebut tidak ikut terekam dalam capture.