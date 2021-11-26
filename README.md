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

### Metode Subnetting dan Routing CIDR

### Kendala