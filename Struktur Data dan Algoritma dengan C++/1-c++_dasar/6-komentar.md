# Komentar
Komentar umumnya digunakan oleh para programmer untuk memberikan keterangan atau catatan tentang fungsi suatu kode program yang dibuat. Ini dilakukan agar kode yang dikembangkan mudah untuk dibaca, dipahami, dan dimengerti oleh programmer lain atau programmer yang membuat kode itu sendiri kita ia lupa.

Pada C++ terdapat dua jenis komentar yaitu, komentar single-line dan komentar multi-line. Saat compiler mengkompilasi kode sumber C++, compiler akan mengabaikan semua komentar. Jadi, komentar tidak akan berdampak pada fungsi dari suatu kode program yang kita tulis. Karena komentar tidak termaksud statment atau expression, maka komentar tidak perlu ditutup dengan karakter `;`.

## 6.1 Komentar Single-Line
Komentar single-line umumnya digunakan untuk membuat catatan pendek yang tidak lebih dari sebaris. Di C++, komentar singel-line ditandai dengan karakter `//`. Berikut adalah contoh penggunannya :

```
#include <iostream>

// ini adalah contoh komentar sebaris

int main() {
	
	// kode ini berfungsi untuk mencetak teks
	std::cout << "Halo C++";

	return 0;

}
```


## 6.2 Komentar Multi-Line
Komentar multi-line umumnya digunakan untuk membuat catatn panjang dengan banyak baris. Biasanya programmer menggunakan jenis komentar ini untuk menuliskan detail dari programmnya atau mendeskripsikan fungsi programmnya secara keseluruhan. Di C++, komentar multi-line diawali dengan karakter `/*` dan diakhiri dengan karakter `*/`. berikut adalah contoh penggunaannya :

```
/* 
	Author	: Mohammad Agung (agungichiruki)
	Date	: 23 June 2023
	Version	: hello_world 1.2
*/

#include <iostream>

int main() {
	/*
		std::endl adalah fungsi dari library standar
		iostream yang berguna untuk menambahkan karakater
		enter (Carriage Return).
	*/
	std::cout << "Hello World!" << std::endl;

	return 0;
}
```