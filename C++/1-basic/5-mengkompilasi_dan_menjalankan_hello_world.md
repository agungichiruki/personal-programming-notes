# Mengkompilasi Dan Menjalankan Hello World
Kode sumber dari aplikasi "Hello World" yang sudah dibuat pada catatan sebelumnya belum bisa kita jalankan. Butuh proses kompilasi dengan compiler untuk mengkonversinya menjadi binary file atau aplikasi agar dapat dijalankan.

## 5.1 Kompilasi
Buka terminal kemudian arahkan path-nya ke folder tempat file kode sumber tersimpan. Kemudian, untuk mengcompile kode sumber C++ dengan GCC, gunakan format perintah :

```
g++ nama_file_kode_sumber.cpp -o nama_file_aplikasi_hasil_compile
```

Contoh pada kode sumber "Hello World".

```
g++ hello_world.cpp -o hello_world
```

![Compile Hello World Dengan GCC](./gambar/5.1-compile_hello_world.png)

Setelah proses kompilasi berhasil dengan ditandai tidak adanya pesan error, maka akan muncul file aplikasi atau binary file hasil dari proses kompilasi tadi yang dapat dijalankan langsung.

![Hasil Kompilasi Kode Sumber Hello World](./gambar/5.2-hasil_kompilasi_hello_world.png)

## 5.2 Menjalankan Aplikasi Hello World
Masih pada terminal yang sama, untuk menjalankan aplikasi hello_world ini gunakan perintah :

```
./hello_world
```

![Menjalankan Aplikasi hello_world](./gambar/5.3-eksekusi_hello_world.png)

Terlihat pada terminal tercetak teks "Hello World!" ketika kita menjalankan aplikasi hello_world. Ini menandakan bahwa aplikasi ini berhasil dijalankan tanpa adanya error.