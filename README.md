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
		<td   height="60" align="center" valign=middle><b><font face="Arial" color="#000000">Nama Subnet</font></b></td>
		<td   align="center" valign=middle><b><font face="Arial" color="#000000">Size Diperlukan</font></b></td>
		<td   align="center" valign=middle><b><font face="Arial" color="#000000">Di Alokasikan</font></b></td>
		<td   align="center" valign=middle><b><font face="Arial" color="#000000">Address</font></b></td>
		<td   align="center" valign=middle><b><font face="Arial" color="#000000">Mask</font></b></td>
		<td   align="center" valign=middle><b><font face="Arial" color="#000000">Dec Mask</font></b></td>
		<td   align="center" valign=middle><b><font face="Arial" color="#000000">Assignable Range</font></b></td>
		<td   align="center" valign=middle><b><font face="Arial" color="#000000">Broadcast</font></b></td>
	</tr>
	<tr>
		<td   height="80" align="center" valign=middle><b><font face="Arial" size=3 color="#000000">A7</font></b></td>
		<td   align="center" valign=middle sdval="2021" sdnum="1033;"><font face="Arial" size=3 color="#000000">2021</font></td>
		<td   align="center" valign=middle sdval="2046" sdnum="1033;"><font face="Arial" size=3 color="#000000">2046</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.0.0</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">/21</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">255.255.248.0</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.0.1 - 192.217.7.254</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.7.255</font></td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b><font face="Arial" size=3 color="#000000">A1</font></b></td>
		<td   align="center" valign=middle sdval="1001" sdnum="1033;"><font face="Arial" size=3 color="#000000">1001</font></td>
		<td   align="center" valign=middle sdval="1022" sdnum="1033;"><font face="Arial" size=3 color="#000000">1022</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.8.0</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">/22</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">255.255.252.0</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.8.1 - 192.217.11.254</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.11.255</font></td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b><font face="Arial" size=3 color="#000000">A14</font></b></td>
		<td   align="center" valign=middle sdval="721" sdnum="1033;"><font face="Arial" size=3 color="#000000">721</font></td>
		<td   align="center" valign=middle sdval="1022" sdnum="1033;"><font face="Arial" size=3 color="#000000">1022</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.12.0</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">/22</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">255.255.252.0</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.12.1 - 192.217.15.254</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.15.255</font></td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b><font face="Arial" size=3 color="#000000">A2</font></b></td>
		<td   align="center" valign=middle sdval="701" sdnum="1033;"><font face="Arial" size=3 color="#000000">701</font></td>
		<td   align="center" valign=middle sdval="1022" sdnum="1033;"><font face="Arial" size=3 color="#000000">1022</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.16.0</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">/22</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">255.255.252.0</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.16.1 - 192.217.19.254</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.19.255</font></td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b><font face="Arial" size=3 color="#000000">A8</font></b></td>
		<td   align="center" valign=middle sdval="521" sdnum="1033;"><font face="Arial" size=3 color="#000000">521</font></td>
		<td   align="center" valign=middle sdval="1022" sdnum="1033;"><font face="Arial" size=3 color="#000000">1022</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.20.0</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">/22</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">255.255.252.0</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.20.1 - 192.217.23.254</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.23.255</font></td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b><font face="Arial" size=3 color="#000000">A10</font></b></td>
		<td   align="center" valign=middle sdval="502" sdnum="1033;"><font face="Arial" size=3 color="#000000">502</font></td>
		<td   align="center" valign=middle sdval="510" sdnum="1033;"><font face="Arial" size=3 color="#000000">510</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.24.0</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">/23</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">255.255.254.0</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.24.1 - 192.217.25.254</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.25.255</font></td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b><font face="Arial" size=3 color="#000000">A13</font></b></td>
		<td   align="center" valign=middle sdval="251" sdnum="1033;"><font face="Arial" size=3 color="#000000">251</font></td>
		<td   align="center" valign=middle sdval="254" sdnum="1033;"><font face="Arial" size=3 color="#000000">254</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.26.0</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">/24</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">255.255.255.0</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.26.1 - 192.217.26.254</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.26.255</font></td>
	</tr>
	<tr>
		<td   height="100" align="center" valign=middle><b><font face="Arial" size=3 color="#000000">A6</font></b></td>
		<td   align="center" valign=middle sdval="101" sdnum="1033;"><font face="Arial" size=3 color="#000000">101</font></td>
		<td   align="center" valign=middle sdval="126" sdnum="1033;"><font face="Arial" size=3 color="#000000">126</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.27.0</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">/25</font></td>
		<td   align="center" valign=middle sdval="255255255128" sdnum="1033;0;#,##0"><font face="Arial" size=3 color="#000000">255,255,255,128</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.27.1 - 192.217.27.126</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.27.127</font></td>
	</tr>
	<tr>
		<td   height="120" align="center" valign=middle><b><font face="Arial" size=3 color="#000000">A11</font></b></td>
		<td   align="center" valign=middle sdval="13" sdnum="1033;"><font face="Arial" size=3 color="#000000">13</font></td>
		<td   align="center" valign=middle sdval="14" sdnum="1033;"><font face="Arial" size=3 color="#000000">14</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.27.128</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">/28</font></td>
		<td   align="center" valign=middle sdval="255255255240" sdnum="1033;0;#,##0"><font face="Arial" size=3 color="#000000">255,255,255,240</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.27.129 - 192.217.27.142</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.27.143</font></td>
	</tr>
	<tr>
		<td   height="120" align="center" valign=middle><b><font face="Arial" size=3 color="#000000">A12</font></b></td>
		<td   align="center" valign=middle sdval="2" sdnum="1033;"><font face="Arial" size=3 color="#000000">2</font></td>
		<td   align="center" valign=middle sdval="2" sdnum="1033;"><font face="Arial" size=3 color="#000000">2</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.27.144</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">/30</font></td>
		<td   align="center" valign=middle sdval="255255255252" sdnum="1033;0;#,##0"><font face="Arial" size=3 color="#000000">255,255,255,252</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.27.145 - 192.217.27.146</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.27.147</font></td>
	</tr>
	<tr>
		<td   height="120" align="center" valign=middle><b><font face="Arial" size=3 color="#000000">A15</font></b></td>
		<td   align="center" valign=middle sdval="2" sdnum="1033;"><font face="Arial" size=3 color="#000000">2</font></td>
		<td   align="center" valign=middle sdval="2" sdnum="1033;"><font face="Arial" size=3 color="#000000">2</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.27.148</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">/30</font></td>
		<td   align="center" valign=middle sdval="255255255252" sdnum="1033;0;#,##0"><font face="Arial" size=3 color="#000000">255,255,255,252</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.27.149 - 192.217.27.150</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.27.151</font></td>
	</tr>
	<tr>
		<td   height="120" align="center" valign=middle><b><font face="Arial" size=3 color="#000000">A3</font></b></td>
		<td   align="center" valign=middle sdval="2" sdnum="1033;"><font face="Arial" size=3 color="#000000">2</font></td>
		<td   align="center" valign=middle sdval="2" sdnum="1033;"><font face="Arial" size=3 color="#000000">2</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.27.152</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">/30</font></td>
		<td   align="center" valign=middle sdval="255255255252" sdnum="1033;0;#,##0"><font face="Arial" size=3 color="#000000">255,255,255,252</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.27.153 - 192.217.27.154</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.27.155</font></td>
	</tr>
	<tr>
		<td   height="120" align="center" valign=middle><b><font face="Arial" size=3 color="#000000">A4</font></b></td>
		<td   align="center" valign=middle sdval="2" sdnum="1033;"><font face="Arial" size=3 color="#000000">2</font></td>
		<td   align="center" valign=middle sdval="2" sdnum="1033;"><font face="Arial" size=3 color="#000000">2</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.27.156</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">/30</font></td>
		<td   align="center" valign=middle sdval="255255255252" sdnum="1033;0;#,##0"><font face="Arial" size=3 color="#000000">255,255,255,252</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.27.157 - 192.217.27.158</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.27.159</font></td>
	</tr>
	<tr>
		<td   height="120" align="center" valign=middle><b><font face="Arial" size=3 color="#000000">A5</font></b></td>
		<td   align="center" valign=middle sdval="2" sdnum="1033;"><font face="Arial" size=3 color="#000000">2</font></td>
		<td   align="center" valign=middle sdval="2" sdnum="1033;"><font face="Arial" size=3 color="#000000">2</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.27.160</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">/30</font></td>
		<td   align="center" valign=middle sdval="255255255252" sdnum="1033;0;#,##0"><font face="Arial" size=3 color="#000000">255,255,255,252</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.27.161 - 192.217.27.162</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.27.163</font></td>
	</tr>
	<tr>
		<td   height="120" align="center" valign=middle><b><font face="Arial" size=3 color="#000000">A9</font></b></td>
		<td   align="center" valign=middle sdval="2" sdnum="1033;"><font face="Arial" size=3 color="#000000">2</font></td>
		<td   align="center" valign=middle sdval="2" sdnum="1033;"><font face="Arial" size=3 color="#000000">2</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.27.164</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">/30</font></td>
		<td   align="center" valign=middle sdval="255255255252" sdnum="1033;0;#,##0"><font face="Arial" size=3 color="#000000">255,255,255,252</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.27.165 - 192.217.27.166</font></td>
		<td   align="center" valign=middle><font face="Arial" size=3 color="#000000">192.217.27.167</font></td>
	</tr>
</table>
### Metode Subnetting dan Routing CIDR

### Kendala