### Nama: Muhammad Ikhsan Revaldi
### NIM: 09011282328060
### Kelas: SK3C

Praktikum 3 (Sistem File)
1. Lihat peralatan I/O, character device, yang ada pada system komputer.
   ### Jawab:
   Menggunakan command line **iostat** maka kita dapat melihatnya sebagai berikut ![step 1](https://github.com/Hiratsuu/Tugas-Praktikum-3-Sistem-Operasi_Muhammad-Ikhsan-Revaldi_09011282328060_SK3C/blob/main/Tugas%20praktikum%203/Step%201.png?raw=true)
   
2. Buatlah sub direktori januari, februari dan maret sekaligus pada direktori latihan5.
   ### Jawab:
   dengan menggunakan command **mkdir (nama direktori)** ![step 2](https://github.com/Hiratsuu/Tugas-Praktikum-3-Sistem-Operasi_Muhammad-Ikhsan-Revaldi_09011282328060_SK3C/blob/main/Tugas%20praktikum%203/step%202.png?raw=true)
   
3. Buatlah file dataku yang berisi nama, nim dan alamat anda pada sub direktori januari 
   dan copy-kan file tersebut ke sub direktori februari dan maret.
   ### Jawab:
   dengan menggunakan Command **touch (nama file)** kita bisa membuat file bernama dataku.txt dan dengan menggunakan Command **nano (nama file** kita bisa membuat nama,nim dan alamat nya. untuk menyalin file tersebut ke sub driektori februari dan maret maka kita perlu menggunakan Command **"cp dataku.txt /home/ikhsan/latihan_5/februari"** begitu juga dengan maret. ![step 3](https://github.com/Hiratsuu/Tugas-Praktikum-3-Sistem-Operasi_Muhammad-Ikhsan-Revaldi_09011282328060_SK3C/blob/main/Tugas%20praktikum%203/step%203.png?raw=true)

4. Ubahlah ijin akses file dataku pada sub direktori januari sehingga group dan others 
dapat melakukan write.
### Jawab:
dengan menggunakan command **"sudo chmodd go+w"** yang mana **g** merupakan group, **o** merupakan others dan **+w** menambahkan akses write. jadi artinua group dan other dapat melakukan write pada file dataku. ![step 4](https://github.com/Hiratsuu/Tugas-Praktikum-3-Sistem-Operasi_Muhammad-Ikhsan-Revaldi_09011282328060_SK3C/blob/main/Tugas%20praktikum%203/step%204.png?raw=true)

5. Ubahlah ijin akses file dataku pada sub direktori pebruari sehingga user dapat 
melakukan baik write, read maupun execute, tetapi group dan others hanya bisa read 
dan execute.
### Jawab: 
dengan menggunakan command **"sudo chmod u+rwx"** yang mana **u** merupakan user **+rwx** untuk memberikan akses pada user agar dapat melakukan write, read dan execute. sedangkan pada **sudo chmod go-w** berfungsi untuk menghilangkan akses wrtie pada group dan others. ![step 5](https://github.com/Hiratsuu/Tugas-Praktikum-3-Sistem-Operasi_Muhammad-Ikhsan-Revaldi_09011282328060_SK3C/blob/main/Tugas%20praktikum%203/step%205.png?raw=true)

6. Ubahlah ijin akses file dataku pada sub direktori maret sehingga semua dapat 
melakukan write, read dan execute.
### Jawab: 
dengan menggunakan command **"sudo chmod ugo+rwx"** user, group dan other dapat melakukan write, read dan execute. ![step 6](https://github.com/Hiratsuu/Tugas-Praktikum-3-Sistem-Operasi_Muhammad-Ikhsan-Revaldi_09011282328060_SK3C/blob/main/Tugas%20praktikum%203/step%206.png?raw=true)

7. Hapuslah direktori maret.
   ### Jawab:
   dengan command **"rm -r maret"** kita bisa menghapus direktori maret beserta isi yang ada di dalam direktori tersebut. ![step 7](https://github.com/Hiratsuu/Tugas-Praktikum-3-Sistem-Operasi_Muhammad-Ikhsan-Revaldi_09011282328060_SK3C/blob/main/Tugas%20praktikum%203/step%207.png?raw=true)

8. Ubahkan kepemilikan sub direktori februari sehingga user dan group hanya dapat 
melakukan read, dan cobalah untuk membuat direktori baru haha pada sub direktori 
februari.
### Jawab:
dengan menggunakan command **"chown -v root februari"** kita dapat mengubah kepemilikan file tersebut ke root yang mana membuat user dan group hanya dapat melakukan read saja. sebagai contoh jika kita membuat file haha di dalam direktori tersebut maka akan muncul permission denied. ![step 8](https://github.com/Hiratsuu/Tugas-Praktikum-3-Sistem-Operasi_Muhammad-Ikhsan-Revaldi_09011282328060_SK3C/blob/main/Tugas%20praktikum%203/step%208.png?raw=true)

9. Modifikasi umask dari file dataku pada sub direktori januari menjadi 027 dan berapakan 
nilai default-nya ?
### Jawab: 
dengan menggunakan command line **"umask** untuk menampilkan nilai deafult dari umask tersebut. lalu, untuk mengubah nilai umask maka kita bisa menggunakan **"umask 027"**. ![step 9[(https://github.com/Hiratsuu/Tugas-Praktikum-3-Sistem-Operasi_Muhammad-Ikhsan-Revaldi_09011282328060_SK3C/blob/main/Tugas%20praktikum%203/step%209.png?raw=true)

10.  Buatlah link dari file dataku ke file dataku.ini dan file dataku.juga dan dengan perintah 
list perhatikan berapa link yang terjadi ?
### Jawab:
untuk membuat link nya kita bisa menggunakan command **"ln -s (nama file yang akan di jadikan link) (nama link tersebut)"** seperti berikut. ![step 10](https://github.com/Hiratsuu/Tugas-Praktikum-3-Sistem-Operasi_Muhammad-Ikhsan-Revaldi_09011282328060_SK3C/blob/main/Tugas%20praktikum%203/step%2010.png?raw=true)
