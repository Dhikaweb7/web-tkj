# Ulangan Harian Pemrograman Dasar Berbasis Android
> SMK RADEN PAKU
---

## Soal

1. Tuliskan sebuah program untuk menghitung dan menentukan Bilangan Ganjil dan Genap, untuk nilai dimasukkan melalui keyboard sedangkan besar nilai, muncul secara otomatis dihp kalian serta bangun ruang apa yang anda kerjakan yaitu ... (**Tidak Boleh Sama Dengan Temannya**)
2. Buatlah diagram alur (Flowchart) sesuai dengan soal diatas (no. 1)
3. Tuliskan dan jelaskan bagian bagian coding sesuai dengan soal diatas (no.1)
4. Tuliskan hasil keluarannya sesuai soal diatas (no. 1) jika coding bahasa C yang telah dicompile di Run (**Dijalankan**)
5. Jelaskan masing-masing fungsi operasi pemrograman yang sering digunakan yaitu :
        - Variabel  : ...
        - Tipe data : ...
        - Konstanta : ...
        - Operator  : ...
        - Ekspresi  : ...
6. Tentukan variabel-variabel yang dibutuhkan dalam pembuatan KTP (Kartu Tanda Penduduk)!
7. Tuliskan dan buatkan program C++ untuk memeriksa 3 bilangan yang diinput. output harus memunculkan bilangan yang paling besar dan bilangan kecil, lalu apakah bilangan itu positif atau negatif!
8. Tuliskan dan buatkan program mencetak yang mencetak bilangan bulat antara 10 sampai dengan 50 dan berapa jumlah bilangan yang ada ?.
9. Tuliskan dan Buatkan program untuk memasukan bilangan yang diinput, bila di input angka nol maka proses penginputan selesai, lalu bilangan yang di input dijumlahkan dan dicari nilai rata ratanya. Berikut asalah tampilan yang di inginkan

```c++

#include <stdio.h>

int main(void)
{
  printf("## Program Bahasa C Menghitung Gaji Karyawan ## \n");
  printf("================================================ \n\n");

  char nama[50];
  char golongan;
  int jam_kerja, upah_per_jam, total_upah;

  // proses input
  printf("Nama Karyawan :  ");
  gets(nama);

  printff("Golongan:  ")
  scanf("%c", &golongan);

  printff("Jumlah Jam Kerja:  ")
  scanf("%d", &jam_kerja);

  // tentukan jumlah upah per jam berdasarkan golongan
  switch (golongan){
    case 'A' :
        upah_per_jam = 5000;
        break;
    case 'B' :
        upah_per_jam = 7000;
        break;
    case 'C' :
        upah_per_jam = 8000;
        break;
    case 'D' :
        upah_per_jam = 10000;
        break;

 }
 total_upah = jam_kerja = upah_per_jam;

 // cek apakah jam kerja lebih dari 48 jam
 if ( (jam_kerja - 48) > 0 ) {
    total_upah = total_upah + ((jam_kerja - 48)*4000);
 }

 // proses output
 printf("\n");
 printf("%s menerima upah Rp. %d per minggu \n", nama, total_upah);

 return 0;
}

```

10. Tuliskan Hasil Outputnya sesuai kode program diatas!

11. Buatlah dan tuliskan kode program yang meminta data input berupa sebuah tahun (4 digit angka). Program kemudian memeriksa apakah tahun tersebut merupakan tahun kabisat atau tidak.
> Tahun Kabisat adalah tahun yang bulan februari nya berjumlah 29 hari. Biasanya tahun kabisat datang setiap 4 tahun sekali, tapi ada ketentuan yang lebih khusus yaitu :
- jika angka tahun itu habis dibagi 400, maka tahun itu **tahun kabisat**
- jika angka tahun itu tidak habis dibagi 400 tetapi dibagi 100, maka itu **bukan tahun kabisat**
- jika angka tahun itu tidak habis dibagi 400, akan tetapi habis dibagi 4 maka tahun itu tahun kabisat.
- jika angka tahun tidak habis dibagi 400, tidak habis dibagi 100, dan tidak habis dibagi 4, maka **bukan tahun kabisat**.
12. Jelaskan yang anda ketahui mengenai Aritmatika sesuai dengan Bahasa pemrograman C.
13. Jelaskan perbedaan Float dan Double menurut bahasa pemrogramam C.
14. Tuliskan sebuah program untuk menghitung luas bangun datar/luas bangun ruang, untuk nilai dimasukann melalui keyboard dan nilai luas muncul secara otomatis.
15. Sebutkan dan jelaskan Tipe data bahasa C.

## Jawaban

### 1.

```c++

#include <iostream>
using namespace std;

int main() {
   int namakalian;
   cout << "===[ X TKJ 1 ]===\n";
   cout << "Masukkan bilangan: ";
   cin >> namakalian;
        // X TKJ 1 SMK RADEN PAKU
   if (namakalian % 2 == 0) {
      cout << namakalian << " adalah bilangan genap." << endl;
   } else {
      cout << namakalian << " adalah bilangan ganjil." << endl;
   }

   return 0;
}

```

### 2.

```bash

            ( Start )
   Ya                    Tidak

    -    /Jika Bilangan \  -
    |     dibagi dua dan   |
           apakah sisa
/ output / \         /  / output ganjil /
  genap
    |                      |
    - -     ( end )     -  -

```

### 3.

Penjelasan bagian bagian koding "Program Ganjil Genap C++"

> #include <iostream> : memanggil file standar c++ bernama iostream

> using namespace std : mmenyatakan perintah bahwa kita menggunakan seluruh berkas, class atau fungsi.

> int main(){ } : menjadi badan program

> int namakalian : menyatakan tipe data pada variabel namakalian berupa data integer / bilangan bulat.

> cout << "Masukan bilangan: "; : membuat teks dilayar dan sebagai input an user / pengguna bila ditambah

```c++
cin >> namakalian ;

```
selain itu kode cin >> namakalian juga berfungsi untuk memasukan data input kedalam variable namakalian

```c++

if(namakalian % 2 == 0)

```
berfungsi sebagao acuan bahwa jika nilainya dalam angka yang di input user bisa dibagi 2 yang mana mempengaruhi hasil ganjil/genap.

```c++
cout << namakalian << " adalah bilangan genap atau ganjil ";
```

berfungsi sebagai output entah itu genap atau ganjil.

> if jika iya maka genap

> else jika tidak maka ganjil

> return 0; : program selesai.

### 4.

```bash

root@localhost# /ulangan-pemrograman> ./ganjil-genap
===[ XTKJ1 ]===| andhika pratama putra |
Masukan bilangan : 1
1 adalah bilangan ganjil

atau jika :

root@localhost# /ulangan-pemrograman> ./ganjil-ge>
===[ XTKJ1 ]===| andhika pratama putra |
Masukan bilangan : 2
2 adalah bilangan genap

```

### 5

- Variabel : untuk menyimpan data / nilai yang berubah ubah
- Tipe data : klasifikasi data pada bahasa pemrograman
- Konstanta : nilai tetap atau tifsk berubah rubah.
- operator : simbol simbol untuk melakukan operasi tertentu misalnya operator matematika.
- ekspresi : kombinasi dari variabel, konstanta, tipe data dan operator.

### 6

- nama
- nik
- tempat tanggal lahir
- alamat
- agama
- pekerjaan
- status perkawinan

### 7

```c++

#include <iostream>
using namespace std;
// SMK RADEN PAKU
int main() {
    int a, b, c;
    cout << "===[ XTKJ 1 ]===\n";
    //  nama kalian
    cout << "Masukkan tiga bilangan: ";
    cin >> a >> b >> c;

    // cari bilangan terbesar
    int max = a;
    if (b > max) {
        max = b;
    }
    if (c > max) {
        max = c;
    }

    // cari bilangan terkecil
    int min = a;
    if (b < min) {
        min = b;
    }
    if (c < min) {
        min = c;
    }

    // cek apakah bilangan positif atau negatif
    if (a > 0) {
        cout << a << " adalah bilangan positif" << endl;
    } else if (a < 0) {
        cout << a << " adalah bilangan negatif" << endl;
    } else {
        cout << a << " adalah nol" << endl;
    }

    if (b > 0) {
        cout << b << " adalah bilangan positif" << endl;
    } else if (b < 0) {
        cout << b << " adalah bilangan negatif" << endl;
    } else {
        cout << b << " adalah nol" << endl;
    }

    if (c > 0) {
        cout << c << " adalah bilangan positif" << endl;
    } else if (c < 0) {
        cout << c << " adalah bilangan negatif" << endl;
    } else {
        cout << c << " adalah nol" << endl;
    }

    cout << "Bilangan terbesar adalah " << max << endl;
    cout << "Bilangan terkecil adalah " << min << endl;

    return 0;
}

```

### 8

```c++

#include <iostream>
using namespace std;
// X TKJ 1
int main() {
    int namamu = 0; // inisialisasi hitungan bilangan
    for (int i = 10; i <= 50; i++) {
        cout << i << " "; // cetak bilangan
        namamu++; // tambahkan hitungan
    }
    cout << endl;
    cout << "Jumlah bilangan: " << namamu << endl;

    return 0;
}

```

### 9

```c++

No 9.

#include <iostream>
using namespace std;

int main() {
    int bilangan, jumlah = 0, count = 0;
    float rata_rata;

    do {
        cout << "Masukkan bilangan: ";
        cin >> bilangan;

        if (bilangan != 0) {
            jumlah += bilangan;
            count++;
        }
    } while (bilangan != 0);

    rata_rata = static_cast<float>(jumlah) / count;

    cout << "Jumlah bilangan: " << jumlah << endl;
    cout << "Rata-rata bilangan: " << rata_rata << endl;
    cout << "=================\n";
    cout << "ganti namamu \n";
    return 0;
}

```

### 10

```c++

## Program Bahasa C Menghitung Gaji Karyawan ##
===============================================
Nama Karyawan    : Erwin S.kom
Golongan         : A
Jumlah Jam Kerja : 6 Jam

menerima upah Rp. 198.000 per minggu
Erwin 198.000

```

### 11

```c++


#include <iostream>
using namespace std;

int main() {
    int tahun;
    cout << "==[ Program Cek Tahun Kabisat]==\n";
    // ganti en namakalian
    cout << "Masukkan tahun: ";
    cin >> tahun;

    if (tahun % 4 == 0) {
        if (tahun % 100 == 0) {
            if (tahun % 400 == 0)
                cout << tahun << " adalah tahun kabisat.";
            else
                cout << tahun << " bukan tahun kabisat.";
        }
        else
            cout << tahun << " adalah tahun kabisat.";
    }
    else
        cout << tahun << " bukan tahun kabisat.";

    return 0;
}


```

### 12

Aritmatika pada bahasa C merujuk pada kumpulan operasi aritmatika seperti +,-,x(kali), pembagian (/), modulus (%) yaitu sisa dari pembagian.

### 13

Float dan double adalah tipe data numerik (angka) perbedaannya hanya pada ukuran memori.
Float menyimpan nolai desimal dengan 4 byte memori.
sedangkan double menggunakan 8 byte memori.

sebagai contoh float menyimpan data `3.14`
sedangkan double seperti angka `3.141592653589793`

### 14

```c++

Menghitung Luas dan Keliling Bangun Persegi Panjang

#include <iostream>
using namespace std;
// Awang X TKJ 1
int main() {
   float panjang, lebar;

   cout << "Masukkan panjang: ";
   cin >> panjang;
   cout << "Masukkan lebar: ";
   cin >> lebar;

   float luas = panjang * lebar;
   float keliling = 2 * (panjang + lebar);

   cout << "Luas persegi panjang: " << luas << endl;
   cout << "Keliling persegi panjang: " << keliling << endl;

   return 0;
}

```

### 15

 | tipe data | Keterangan |
 | --- | --- |
 | int | menyimpan bilangan bulat (bilangan bulat), tanpa desimal, seperti 123 atau -123 |
 | double | menyimpan angka floating point, dengan desimal, seperti 19,99 atau -19,99 |
 | char  |  menyimpan karakter tunggal, seperti 'a' atau 'B'. Nilai karakter dikelilingi oleh tanda kutip tunggal |
 | string |  menyimpan teks, seperti "Hello World". Nilai string dikelilingi oleh tanda kutip ganda |
 | boolean | menyimpan nilai dengan dua status: benar atau salah ( true / false , high / low ) |
 | void | merupakan tipe data yang tidak bernilai dan tidak bertipe biasanya digunakan untuk data kosong |
 | Wchar_t | adalah tipe data yang digunakan sama seperti char yang menyimpan karakter besar, biasanya digunakan untuk menyimpan karakter yang tidak ada di huruf abjad misalnya huruf japan, china, korea, dll. |
