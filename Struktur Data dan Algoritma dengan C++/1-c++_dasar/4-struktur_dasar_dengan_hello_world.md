# Struktur Dasar & Hello World Di C++
Struktur dasar dan aturan penulisan bahasa pemrograman C++ penting untuk dipahami. Tujuannya adalah, agar kita mengenal karakteristik dari C++ dan bagaimana cara menuliskan kode program yang benar dengan C++.

## 4.1 Struktur Dasar C++
Struktur dasar adalah blok kode program minimal yang harus ada saat kita menulis kode program dengan C++. Perhatikan kode program dibawah ini.

```
int main() {
	return 0;
}
```

Kode diatas adalah struktur dasar dari C++ yang terdiri dari sebuah fungsi utama bernama main dan bertipe data integer. Fungsi utama atau main function ini wajib ada pada sebuah kode program yang dibuat dengan C++, karena fungsi ini adalah entry point yang akan dicari dan dieksekusi pertama kali ketika program dijalankan.

Di fungsi utama inilah diantara karakter `{` dan `}` kita menuliskan kode program kita. Ruang diantara karakter `{` dan `}` pada sebuah fungsi dinamakan juga badan fungsi. Saat sebuah fungsi dijalankan, semua kode program yang kita tulisankan pada badan fungsi akan dieksekusi baris per baris dari atas kebawah.

Adapun `return 0;` ini berfungsi untuk mengembalikan nilai integer 0 yang berfungsi untuk memberitahukan sistem operasi bahwa program berhasil dijalankan tanpa error. nilai yang dikembalikan haruslah bertipe integer karena fungsi utama yang kita buat bertipe integer.

Pada `return 0;` terdapat karakter `;`. `return 0;` adalah sebuah statment dan di C++, Statment dan expression wajib diakhiri atau ditutup dengan karakter `;` yang berfungsi sebagai penanda akhir dari sebuah statment atau expression. Jika terdapat statment atau expression yang tidak ditutup dengan karakter ini, maka akan terjadi error saat proses kompilasi.

Yang harus diperhatikan adalah, fungsi utama atau main function pada C++ haruslah bertipe data int (integer). Jika diberikan tipe data lain misalnya void, maka akan terjadi error saat proses kompilasi. Begitu juga dengan penamaan fungsi utama atau main function, kita tidak boleh kreatif. fungsi utama harus bernama `main` dengan huruf kecil. Penamaan selain itu, maka tidak akan dianggap sebagai fungsi utama dan akan terjadi error saat proses kompilasi, karena compiler akan menganggap kode program kita tidak memiliki fungsi utama atau main function.

Dengan struktur dasar yang hanya memiliki fungsi utama saja seperti kode program diatas, kita bisa mengkompilasi source code kita menjadi sebuah aplikasi. Tetapi saat dijalankan, tidak akan terjadi apa-apa karena memang kita tidak menuliskan perintah apapun.

## 4.2 Hello World :smiley:
Hello World adalah aplikasi sederhana yang hanya menampilkan teks `Hello World!` di terminal. Membuat aplikasi Hello World ini sudah seperti tradisi bagi programmer yang baru belajar atau yang sedang mempelajari bahasa pemrograman baru. Ketikkan kode program dibawah ini pada teks editor atau IDE.

```
#include <iostream>

int main() {
	std::cout << "Hello World!";

	return 0;
}
```

Kemudian simpan dengan nama `hello_world.cpp`. Pastikan bahwa ekstensi dari file kode sumber kita adalah `.cpp`, karena selain itu maka tidak akan dianggap kode sumber C++.

Pada kode program diatas, selain kode program struktrur dasar, ada beberapa kode program baru seperti :

`#include <iostream>`, ini berfungsi untuk menginclude-kan library lain kedalam kode sumber kita. Format penggunaan-nya adalah `#include <nama_library>`. Secara singkat, library atau pustaka di C++ adalah kumpulan fungsi-fungsi yang berguna untuk mempermudah kita ketika memprogram dengan C++. Pada kode sumber diatas, library yang diinclude-kan adalah library **iostream**. Library ini adalah standart library yang memiliki berbagai fungsi untuk menangani aliran (stream) input dan output seperti menerima inputan dari keyboard atau mencetak teks di layar (output).

```
std::cout << "Hello World!";
```

Ini adalah baris perintah yang berfungsi untuk mencetak teks "Hello World!" pada terminal. Perintah ini agak panjang jadi kita bahas satu persatu.

Yang pertama adalah `std::cout`. cout adalah fungsi di library iostream yang berguna untuk mencetak atau menampilkan data ke layar. Kata kunci `std` yang diikuti dengan scope operator `::` dibutuhkan untuk memanggil fungsi ini karena cout adalah anggota dari namespace std yang merupakan namespace standard di C++.

Kemudian ada `<<` yang merupakan operator "stream insertion". Operator ini berfungsi untuk memasukkan nilai atau variable ke dalam fungsi cout, yang pada kode program diatas nilai yang dimasukkan adalah "Hello World!".
