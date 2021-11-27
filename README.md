# Jarkom-Modul-4-T12-2021

Nama Kelompok :  
- Ian Felix Jonathan Simanjuntak (nomor 1-6)
- Muhammad Zakky Ghufron (Nomor 7-10)
- Muhammad Naufal Imantyasto (Nomor 11 -13)

### Gambar Topologi
![image 54](https://user-images.githubusercontent.com/50267676/143535136-600b7185-1a5b-419b-b8ad-4166a920b214.png)

### Metode Subnetting dan Routing VLSM
Untuk mengerjakan dengan meotde VLSM, pertama sekali kami membagi gambar tersebut kedalam beberapa bagian kecil. Berikut adalah gambar pembagian yang telah kami buat.

![Group 81](https://user-images.githubusercontent.com/50267676/143535337-20af5dd2-8104-48c8-bc42-2e146fec0086.png)

Setelah kami melakukan pembagian tersebut, berikut nya kami menghitung berapa jumlah host pada setiap subnet dan netmask berapa yang akan digunakan. Berikut adalah perhitungan yang kami gunakan

<table>
    <tr>
        <td>Label</td>
        <td>Jumlah Host</td>
        <td>Netmask</td>
    </tr>
    <tr>
        <td>A1</td>
        <td>1001</td>
        <td>/22</td>
    </tr>
        <tr>
        <td>A2</td>
        <td>701</td>
        <td>/22</td>
    </tr>
        <tr>
        <td>A3</td>
        <td>2</td>
        <td>/30</td>
    </tr>
        <tr>
        <td>A4</td>
        <td>2</td>
        <td>/30</td>
    </tr>
        <tr>
        <td>A5</td>
        <td>2</td>
        <td>/30</td>
    </tr>
        <tr>
        <td>A6</td>
        <td>101</td>
        <td>/25</td>
    </tr>
        <tr>
        <td>A7</td>
        <td>2021</td>
        <td>/21</td>
    </tr>
        <tr>
        <td>A8</td>
        <td>521</td>
        <td>/22</td>
    </tr>
        <tr>
        <td>A9</td>
        <td>2</td>
        <td>/30</td>
    </tr>
        <tr>
        <td>A10</td>
        <td>502</td>
        <td>/23</td>
    </tr>
        <tr>
        <td>A11</td>
        <td>13</td>
        <td>/28</td>
    </tr>
        <tr>
        <td>A12</td>
        <td>2</td>
        <td>/30</td>
    </tr>
        <tr>
        <td>A13</td>
        <td>252</td>
        <td>/24</td>
    </tr>
        <tr>
        <td>A14</td>
        <td>721</td>
        <td>/22</td>
    </tr>
    <tr>
        <td>A15</td>
        <td>2</td>
        <td>/30</td>
    </tr>
        <tr>
        <td>Total</td>
        <td>5845</td>
        <td>/19</td>
    </tr>
</table>
Dapat dilihat bahwa major network nya berada pada netmask /19. Prefix IP kelompok kami adalah 192.217.X.X. Untuk melakukan perhitungan subnetting dengan metode VLSM, maka kami membuat pohon perhitungan VLSM sebagai berikut.

![JarkomVLSM](https://user-images.githubusercontent.com/50267676/143536121-ab760839-e089-4445-81e8-e8bb23315986.jpg)

Untuk table perhitungannya adalah sebagai berikut : 
<table cellspacing="0" border="0">
	<colgroup span="8" width="64"></colgroup>
	<tr>
		<td   height="60" align="center" valign=middle><b><font face="Arial" color="#000000">Nama Subnet</b></td>
		<td   align="center" valign=middle><b><font face="Arial" color="#000000">Size Diperlukan</b></td>
		<td   align="center" valign=middle><b><font face="Arial" color="#000000">Di Alokasikan</b></td>
		<td   align="center" valign=middle><b><font face="Arial" color="#000000">Address</b></td>
		<td   align="center" valign=middle><b><font face="Arial" color="#000000">Mask</b></td>
		<td   align="center" valign=middle><b><font face="Arial" color="#000000">Dec Mask</b></td>
		<td   align="center" valign=middle><b><font face="Arial" color="#000000">Assignable Range</b></td>
		<td   align="center" valign=middle><b><font face="Arial" color="#000000">Broadcast</b></td>
	</tr>
	<tr>
		<td   height="80" align="center" valign=middle><b>A7</b></td>
		<td   align="center" valign=middle sdval="2021" sdnum="1033;">2021</td>
		<td   align="center" valign=middle sdval="2046" sdnum="1033;">2046</td>
		<td   align="center" valign=middle>192.217.0.0</td>
		<td   align="center" valign=middle>/21</td>
		<td   align="center" valign=middle>255.255.248.0</td>
		<td   align="center" valign=middle>192.217.0.1 - 192.217.7.254</td>
		<td   align="center" valign=middle>192.217.7.255</td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b>A1</b></td>
		<td   align="center" valign=middle sdval="1001" sdnum="1033;">1001</td>
		<td   align="center" valign=middle sdval="1022" sdnum="1033;">1022</td>
		<td   align="center" valign=middle>192.217.8.0</td>
		<td   align="center" valign=middle>/22</td>
		<td   align="center" valign=middle>255.255.252.0</td>
		<td   align="center" valign=middle>192.217.8.1 - 192.217.11.254</td>
		<td   align="center" valign=middle>192.217.11.255</td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b>A14</b></td>
		<td   align="center" valign=middle sdval="721" sdnum="1033;">721</td>
		<td   align="center" valign=middle sdval="1022" sdnum="1033;">1022</td>
		<td   align="center" valign=middle>192.217.12.0</td>
		<td   align="center" valign=middle>/22</td>
		<td   align="center" valign=middle>255.255.252.0</td>
		<td   align="center" valign=middle>192.217.12.1 - 192.217.15.254</td>
		<td   align="center" valign=middle>192.217.15.255</td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b>A2</b></td>
		<td   align="center" valign=middle sdval="701" sdnum="1033;">701</td>
		<td   align="center" valign=middle sdval="1022" sdnum="1033;">1022</td>
		<td   align="center" valign=middle>192.217.16.0</td>
		<td   align="center" valign=middle>/22</td>
		<td   align="center" valign=middle>255.255.252.0</td>
		<td   align="center" valign=middle>192.217.16.1 - 192.217.19.254</td>
		<td   align="center" valign=middle>192.217.19.255</td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b>A8</b></td>
		<td   align="center" valign=middle sdval="521" sdnum="1033;">521</td>
		<td   align="center" valign=middle sdval="1022" sdnum="1033;">1022</td>
		<td   align="center" valign=middle>192.217.20.0</td>
		<td   align="center" valign=middle>/22</td>
		<td   align="center" valign=middle>255.255.252.0</td>
		<td   align="center" valign=middle>192.217.20.1 - 192.217.23.254</td>
		<td   align="center" valign=middle>192.217.23.255</td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b>A10</b></td>
		<td   align="center" valign=middle sdval="502" sdnum="1033;">502</td>
		<td   align="center" valign=middle sdval="510" sdnum="1033;">510</td>
		<td   align="center" valign=middle>192.217.24.0</td>
		<td   align="center" valign=middle>/23</td>
		<td   align="center" valign=middle>255.255.254.0</td>
		<td   align="center" valign=middle>192.217.24.1 - 192.217.25.254</td>
		<td   align="center" valign=middle>192.217.25.255</td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b>A13</b></td>
		<td   align="center" valign=middle sdval="251" sdnum="1033;">251</td>
		<td   align="center" valign=middle sdval="254" sdnum="1033;">254</td>
		<td   align="center" valign=middle>192.217.26.0</td>
		<td   align="center" valign=middle>/24</td>
		<td   align="center" valign=middle>255.255.255.0</td>
		<td   align="center" valign=middle>192.217.26.1 - 192.217.26.254</td>
		<td   align="center" valign=middle>192.217.26.255</td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b>A6</b></td>
		<td   align="center" valign=middle sdval="101" sdnum="1033;">101</td>
		<td   align="center" valign=middle sdval="126" sdnum="1033;">126</td>
		<td   align="center" valign=middle>192.217.27.0</td>
		<td   align="center" valign=middle>/25</td>
		<td   align="center" valign=middle sdval="255255255128" sdnum="1033;0;#,##0">255,255,255,128</td>
		<td   align="center" valign=middle>192.217.27.1 - 192.217.27.126</td>
		<td   align="center" valign=middle>192.217.27.127</td>
	</tr>
	<tr>
		<td   height="120" align="center" valign=middle><b>A11</b></td>
		<td   align="center" valign=middle sdval="13" sdnum="1033;">13</td>
		<td   align="center" valign=middle sdval="14" sdnum="1033;">14</td>
		<td   align="center" valign=middle>192.217.27.128</td>
		<td   align="center" valign=middle>/28</td>
		<td   align="center" valign=middle sdval="255255255240" sdnum="1033;0;#,##0">255,255,255,240</td>
		<td   align="center" valign=middle>192.217.27.129 - 192.217.27.142</td>
		<td   align="center" valign=middle>192.217.27.143</td>
	</tr>
	<tr>
		<td   height="120" align="center" valign=middle><b>A12</b></td>
		<td   align="center" valign=middle sdval="2" sdnum="1033;">2</td>
		<td   align="center" valign=middle sdval="2" sdnum="1033;">2</td>
		<td   align="center" valign=middle>192.217.27.144</td>
		<td   align="center" valign=middle>/30</td>
		<td   align="center" valign=middle sdval="255255255252" sdnum="1033;0;#,##0">255,255,255,252</td>
		<td   align="center" valign=middle>192.217.27.145 - 192.217.27.146</td>
		<td   align="center" valign=middle>192.217.27.147</td>
	</tr>
	<tr>
		<td   height="120" align="center" valign=middle><b>A15</b></td>
		<td   align="center" valign=middle sdval="2" sdnum="1033;">2</td>
		<td   align="center" valign=middle sdval="2" sdnum="1033;">2</td>
		<td   align="center" valign=middle>192.217.27.148</td>
		<td   align="center" valign=middle>/30</td>
		<td   align="center" valign=middle sdval="255255255252" sdnum="1033;0;#,##0">255,255,255,252</td>
		<td   align="center" valign=middle>192.217.27.149 - 192.217.27.150</td>
		<td   align="center" valign=middle>192.217.27.151</td>
	</tr>
	<tr>
		<td   height="120" align="center" valign=middle><b>A3</b></td>
		<td   align="center" valign=middle sdval="2" sdnum="1033;">2</td>
		<td   align="center" valign=middle sdval="2" sdnum="1033;">2</td>
		<td   align="center" valign=middle>192.217.27.152</td>
		<td   align="center" valign=middle>/30</td>
		<td   align="center" valign=middle sdval="255255255252" sdnum="1033;0;#,##0">255,255,255,252</td>
		<td   align="center" valign=middle>192.217.27.153 - 192.217.27.154</td>
		<td   align="center" valign=middle>192.217.27.155</td>
	</tr>
	<tr>
		<td   height="120" align="center" valign=middle><b>A4</b></td>
		<td   align="center" valign=middle sdval="2" sdnum="1033;">2</td>
		<td   align="center" valign=middle sdval="2" sdnum="1033;">2</td>
		<td   align="center" valign=middle>192.217.27.156</td>
		<td   align="center" valign=middle>/30</td>
		<td   align="center" valign=middle sdval="255255255252" sdnum="1033;0;#,##0">255,255,255,252</td>
		<td   align="center" valign=middle>192.217.27.157 - 192.217.27.158</td>
		<td   align="center" valign=middle>192.217.27.159</td>
	</tr>
	<tr>
		<td   height="120" align="center" valign=middle><b>A5</b></td>
		<td   align="center" valign=middle sdval="2" sdnum="1033;">2</td>
		<td   align="center" valign=middle sdval="2" sdnum="1033;">2</td>
		<td   align="center" valign=middle>192.217.27.160</td>
		<td   align="center" valign=middle>/30</td>
		<td   align="center" valign=middle sdval="255255255252" sdnum="1033;0;#,##0">255,255,255,252</td>
		<td   align="center" valign=middle>192.217.27.161 - 192.217.27.162</td>
		<td   align="center" valign=middle>192.217.27.163</td>
	</tr>
	<tr>
		<td   height="120" align="center" valign=middle><b>A9</b></td>
		<td   align="center" valign=middle sdval="2" sdnum="1033;">2</td>
		<td   align="center" valign=middle sdval="2" sdnum="1033;">2</td>
		<td   align="center" valign=middle>192.217.27.164</td>
		<td   align="center" valign=middle>/30</td>
		<td   align="center" valign=middle sdval="255255255252" sdnum="1033;0;#,##0">255,255,255,252</td>
		<td   align="center" valign=middle>192.217.27.165 - 192.217.27.166</td>
		<td   align="center" valign=middle>192.217.27.167</td>
	</tr>
</table>

Untuk VLSM kami mengerjakan nya pada Cisco Packet Tracert. Pada CPT kami membuat topologi jaringan terlebih dahulu sebagai berikut

![image](https://user-images.githubusercontent.com/50267676/143538029-e7b5e8e2-2649-4c24-80e9-41d6b300e795.png)

Untuk pengaturan IP, kami mengatur IP berdasarkan table perhitungan yang telah kami buat, lalu kami mengassign Ip tersebut kedalam setiap node. Sebagai Contoh kita ambil subnet A1.
```
Subnet A1 : 
    NID : 192.217.8.0
    Netmask : 255.255.252.0
    IP range : 192.217.8.1 - 192.217.11.254
```
berdasarkan data tersebut, maka kita dapat mengatur nya pada cisco packet tracer nya. Pada Foosha dapat kita lihat bahwa interface yang terhubung dengan subnet A1 adalah `Fa0/1`. maka ip pada `interface Fa0/1` yang kita atur dengan IP range yang tersedia sebagai berikut :

![image](https://user-images.githubusercontent.com/50267676/143538645-3eccdc2f-2e42-40b9-a78e-7740ca22a330.png)

Setelah mengatur IP pada foosha, selanjutnya kita mengatur IP pada `Blueno` dengan IP range yang telah tersedia sebagai berikut : 

![image](https://user-images.githubusercontent.com/50267676/143539035-86f3b6e8-1184-4325-9c04-fad83fbc623e.png)

Setelah kita berhasil mengatur IP pada subnet A1, kita lanjutkan terus mengatur IP setiap subnet sampai A15 sesuai dengan hasil perhitungan yang telah kita dapatkan sebelumnya. Karena terlalu banyak, kami hanya mencontohkan assign IP pada satu subnet saja. Untuk assign lengkap nya dapat di akses melalui <a href="https://github.com/Ianphantom/Jarkom-Modul-4-T12-2021/blob/main/Jarkom.pkt"><b style="color:red">link berikut ini</b></a> 

Setelah semua Node sudah diatur IP nya, selanjutnya kita akan melakukan routing agar semua node saling terhubung. Sebagai contoh penjelasan, kita ambil `Router Water7`. 
- Water 7 harus terhubung dengan subnet A6
- Water 7 harus terhubung dengan subnet A7
- Subnet A6 dan A7 terhubung ke `Pucci`
- Oleh karena itu, nexthop dari subnet A6 dan A7 adalah interface `Pucci` yang terhubung ke `Water7`

Maka Pengaturan routing nya adalah :
```
Subnet A6 :
    NID = 192.217.27.0
    Netmask = 255.255.255.128
    NextHop  = 192.217.27.154

Subnet A6 :
    NID = 192.217.0.0
    Netmask = 255.255.248.0
    NextHop  = 192.217.27.154

Dan kerena water7 berada di bawah Foosha, maka kita perlu menabmahkan routing
    NID : 0.0.0.0
    Netmask : 0.0.0.0
    Nexthop : 192.217.27.149
```
Berikut adalah contoh jika kita sudah melakukan routing pada `Water7`

![image](https://user-images.githubusercontent.com/50267676/143540760-969c9315-07d5-4516-97e8-fff26c9e16f3.png)

Berikut adalah routing untuk setiap router yang ada :
- Pucci
```
0.0.0.0/0 via 192.217.27.153
```
- Water7
```
192.217.27.0/25 via 192.217.27.154
192.217.0.0/21 via 192.217.27.154
0.0.0.0/0 via 192.217.27.149
```
- Foosha
```
192.217.16.0/22 via 192.217.27.150
192.217.27.152/30 via 192.217.27.150
192.217.27.0/25 via 192.217.27.150
192.217.0.0/21 via 192.217.27.150
192.217.20.0/22 via 192.217.27.158
192.217.24.0/23 via 192.217.27.158
192.217.27.128/28 via 192.217.27.158
192.217.27.160/30 via 192.217.27.158
192.217.27.164/30 via 192.217.27.158
192.217.12.0/22 via 192.217.27.158
192.217.26.0/24 via 192.217.27.158
```
- Guanhao
```
0.0.0.0/0 via 192.217.27.157
192.217.27.128/28 via 192.217.24.3
192.217.27.164/30 via 192.217.27.162
192.217.26.0/24 via 192.217.27.162
192.217.12.0/22 via 192.217.27.162
```
- Alabasta
```
0.0.0.0/0 via 192.217.24.1
```
- Oimo
```
0.0.0.0/0 via 192.217.27.161
192.217.12.0/22 via 192.217.26.3
```
- Seastone
```
0.0.0.0/0 via 192.217.26.1
```

Dengan melakukan routing seperti itu, kita sudah dapat memastikan bahwa semua node sudah terhubung. Sebagai contoh kita ambil `Jipangu - Elena`

![image](https://user-images.githubusercontent.com/50267676/143541669-20e79ea1-4f16-4c78-aaff-2c3b48e52dbc.png)

Hasil routing kami juga sudah berhasil melewati serangkaian tes yang telah diberikan oleh asisten saat demo. Sehingga dapat dipastikan bahwa subnetting dan routing dengan metode VLSM kami sudah benar dan tepat.

Untuk hasil lengkapnya dapat dilihat pada <a href="https://github.com/Ianphantom/Jarkom-Modul-4-T12-2021/blob/main/Jarkom.pkt"><b style="color:red">link berikut ini</b></a> 


### Metode Subnetting dan Routing CIDR
Untuk mengerjakan dengan metode CIDR, pertama sekali kami membagi gambar tersebut menjadi kelompok yang lebih besar dengan menggabungkan antara kelompok kelompok yang sudah dibuat menjadi satu kelompok besar. Berikut adalah gambar pembagian yang telah kami buat.

![Pengelompokkan CIDR](https://user-images.githubusercontent.com/63605397/143672891-c5ee3f8e-23bc-4a1d-9abe-4ab61c315bc0.png)

Setelah kami melakukan pembagian tersebut, berikutnya kami menentukan NID dari masing-masing subnet menyesuaikan kelompok besar yang sudah dibuat. Untuk melakukan perhitungan subnetting dengan metode CIDR, maka kami membuat pohon perhitungan CIDR sebagai berikut.

![CIDR TREE](https://user-images.githubusercontent.com/63605397/143673255-d0ca3c15-1180-4d15-91c8-c7368be632ad.jpg)

Berdasarkan perhitungan, maka didapatkan pembagian IP sebagai berikut : 
<table cellspacing="0" border="0">
	<colgroup span="8" width="64"></colgroup>
	<tr>
		<td   height="60" align="center" valign=middle><b><font face="Arial" color="#000000">Subnet</b></td>
		<td   align="center" valign=middle><b><font face="Arial" color="#000000">NID</b></td>
		<td   align="center" valign=middle><b><font face="Arial" color="#000000">Mask</b></td>
		<td   align="center" valign=middle><b><font face="Arial" color="#000000">Dec Mask</b></td>
	</tr>
	<tr>
		<td   height="80" align="center" valign=middle><b>A1</b></td>
		<td   align="center" valign=middle>192.217.128.0</td>
		<td   align="center" valign=middle>/30</td>
		<td   align="center" valign=middle>255.255.255.252</td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b>A2</b></td>
		<td   align="center" valign=middle>192.217.224.0</td>
		<td   align="center" valign=middle>/22</td>
		<td   align="center" valign=middle>255.255.252.0</td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b>A3</b></td>
		<td   align="center" valign=middle>192.217.128.0</td>
		<td   align="center" valign=middle>/30</td>
		<td   align="center" valign=middle>255.255.255.252</td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b>A4</b></td>
		<td   align="center" valign=middle>192.217.136.0</td>
		<td   align="center" valign=middle>/30</td>
		<td   align="center" valign=middle>255.255.255.252</td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b>A5</b></td>
		<td   align="center" valign=middle>192.217.208.0</td>
		<td   align="center" valign=middle>/30</td>
		<td   align="center" valign=middle>255.255.255.252</td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b>A6</b></td>
		<td   align="center" valign=middle>192.217.200.0</td>
		<td   align="center" valign=middle>/25</td>
		<td   align="center" valign=middle>255.255.255.128</td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b>A7</b></td>
		<td   align="center" valign=middle>192.217.192.0</td>
		<td   align="center" valign=middle>/21</td>
		<td   align="center" valign=middle>255.255.248.0</td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b>A8</b></td>
		<td   align="center" valign=middle>192.217.4.0</td>
		<td   align="center" valign=middle>/22</td>
		<td   align="center" valign=middle>255.255.252.0</td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b>A9</b></td>
		<td   align="center" valign=middle>192.217.64.0</td>
		<td   align="center" valign=middle>/30</td>
		<td   align="center" valign=middle>255.255.255.252</td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b>A10</b></td>
		<td   align="center" valign=middle>192.217.0.0</td>
		<td   align="center" valign=middle>/23</td>
		<td   align="center" valign=middle>255.255.254.0</td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b>A11</b></td>
		<td   align="center" valign=middle>192.217.2.0</td>
		<td   align="center" valign=middle>/28</td>
		<td   align="center" valign=middle>255.255.255.240</td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b>A12</b></td>
		<td   align="center" valign=middle>192.217.48.0</td>
		<td   align="center" valign=middle>/30</td>
		<td   align="center" valign=middle>255.255.255.252</td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b>A13</b></td>
		<td   align="center" valign=middle>192.217.36.0</td>
		<td   align="center" valign=middle>/24</td>
		<td   align="center" valign=middle>255.255.255.0</td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b>A14</b></td>
		<td   align="center" valign=middle>192.217.32.0</td>
		<td   align="center" valign=middle>/22</td>
		<td   align="center" valign=middle>255.255.252.0</td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b>A15</b></td>
		<td   align="center" valign=middle>192.217.40.0</td>
		<td   align="center" valign=middle>/30</td>
		<td   align="center" valign=middle>255.255.255.252</td>
	</tr>
</table>

Untuk CIDR kami mengerjakan nya pada GNS3. Pada GNS3 kami membuat topologi jaringan terlebih dahulu sebagai berikut

![Topologi GNS3](https://user-images.githubusercontent.com/63605397/143672770-1504eb70-fed1-4c18-9749-dcb5def194eb.png)

Berdasarkan perhitungan diatas, selanjutnya kami mengkonfigurasi IP kedalam setiap node. Kita ambil contoh pada subnet A2 dimana terdapat router `Water7` yang terhubung dengan `Cipher` melalui `eth1` sebagai berikut:
```
auto eth1
iface eth1 inet static
	address 192.217.224.1
	netmask 255.255.252.0
```

Sedangkan pada Cipher konfigurasinya sebagai berikut:
```
auto eth0
iface eth0 inet static
	address 192.217.224.2
	netmask 255.255.252.0
	gateway 192.217.224.1
```

Untuk versi lengkapnya dapat dilihat langsung di file <a href="https://github.com/Ianphantom/Jarkom-Modul-4-T12-2021/blob/main/Modul4.gns3project"><b style="color:blue">berikut</b></a> 

### Kendala
1. Untuk kendalanya sendiri, kami kebingungan dalam menentukan IP dari masing-masing subnet pada metode CIDR sehingga kami membutuhkan waktu yang agak lama dalam menentukannya dan teratasi dengan menyeimbangkan tree yang sebelumnya sudah kami buat dan setelah menyeimbangkan tree sebelumnya terbentuklah tree yang baru seperti pada gambar tree CIDR di atas.
