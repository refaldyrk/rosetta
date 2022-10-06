---
title: Variabel dan Tipe Data
created: 03-10-2022
update: -
---
# 2. Variabel dan Tipe Data
Pada bab ini akan membahas mengenai Variabel dan Tipe Data pada bahasa C.

## Variabel
- Variabel

Variabel adalah wadah yang digunakan untuk menampung data/value. Jika dianalogikan, variabel adalah wadah semacam gelas yang didalamnya terdapat air. Atau bisa juga, variabel adalah piring yang didalamnya merupakan makanan.

Variabel adalah identitas, untuk menampung sebuah data/value yang diinginkan.

Deklarasi variabel adalah sebuah perintah agar program menyediakan variabel yang akan kita pakai. 

Berikut adalah aturan dalam penulisan variabel : **(Perlu Diingat)**

a)     Pendeklarasian variabel harus diawali dengan tipe data variabel (pembahasan tipe data akan dibahas pada bagian selanjutnya)

b)	Boleh terdiri dari gabungan huruf dan angka dengan karakter pertama harus huruf.

c)	Bahasa C bersifat case sensitive, artinya huruf besar dan kecil dianggap berbeda. Jadi, antara NAMA, nama dan Nama itu dianggap berbeda.

d)	Tidak boleh mengandung spasi. Tidak Boleh mengandung simbol-simbol khusus, kecuali garis bawah (underscore).

e)	Yang termasuk simbol khusus yang tidak diperbolehan antara lain : !,@,#,$,%,^,&,*,(,),-,+,=.


| Benar                    | Salah                  |
| ------------------------ | ---------------------- |
| Nama_Mahasiswa           | %nama-mahasiswa        |
| Kelas2                   | 2Kelas                 |
| _HaSiLaKhIr_             | Hasil Akhir            |
| TotalBelanja             | Total-belanja          |


- Jenis Variabel

Jenis variabel dibedakan berdasarkan letak pendeklaran variabel, perhatikan gambar dibawah ini :
![image](https://user-images.githubusercontent.com/66554199/193556169-f26528ca-ee61-4853-a756-6c0e7a22e592.png)


Jadi apa perbedaannya?

a)	Variabel lokal

Variabel lokal adalah variabel yang deklarasinya berada di dalam fungsi, misalnya fungsi main. Sehingga variabel tersebut hanya bisa diakses oleh anggota main 
itu sendiri.

b)	Variabel global

Variabel global adalah variabel yang deklarasinya berada di luar fungsi main atau fungsi manapun sehingga  variabel itu bisa di akses oleh fungsi manapun dan 
dikenal oleh siapapun.


- Konstanta

Konstanta adalah variabel yang isinya tetap/tidak dapat berubah-ubah. Konstanta tidak dapat dikenai assignment (datanya diisi lagi/diubah) dan saat pembuatan 
variabel konstanta harus langsung diinisialisasi/diisi data sesuai dengan tipe data. 

## Tipe Data
- Numerik dan Karakter

Tipe data adalah suatu pengenal yang merupakan bagian program yang paling penting karena tipe data mempengaruhi setiap intruksi yang akan dilaksanakan oleh komputer. 
Misalnya 5 dibagi 2 saja bisa menghasilkan hasil yang berbeda tergantung tipe datanya, mari kita coba cermati kode berikut:

 ```C
  int $count = 5 / 2;
  printf("%i  ", $count);
  //Output: 2
    
  float $count2 = 5 / 2;
  printf("%f  ", $count2);
  //Output: 2.000000
  ```


Kita juga harus mengetahui format specifier, apa itu format specifier? 

Format specifier adalah sebuah kode yang digunakan untuk membaca variabel ketika akan dicetak. Format specifier biasanya diawali dengan menuliskan 
karakter %(persen) untuk kemudian diikuti huruf sesuai tipe datanya. Tipe data dasar dalam bahasa C:


| Type            | Penulisan              | Format Specifier     | Digunakan untuk                                                      |
| --------------- | ---------------------- | -------------------- | -------------------------------------------------------------------- |
| Integer         | int                    | %d atau %i           | Bilangan bulat yang hanya memuat 8 angka                             |
| Long            | long                   | %ld atau %li         | Bilangan bulat yang memuat lebih dari 8 angka                        |
| Float           | float                  | %f                   | Bilangan desimal yang memuat 8 angka di belakang koma                |
| Double          | double                 | %lf                  | Bilangan desimal yang memuat lebih dari 8 angka dibelakang koma      |
| Character       | char                   | %c                   | Satu karakter                                                        |
| String          | char* atau char[]      | %s                   | Kumpulan karakter                                                    |



- Boolean

Boolean merupakan tipe data dasar dalam bahasa C, hanya saja tidak ada penulisan atau pendeklaran secara jelas. Hanya kondisi True atau False yang biasa digunakan 
dalam operator logika. Boolean juga bisa dikondisikan sebagai angka misalnya 1 sebagai kondisi True dan 0 sebagai kondisi False.
