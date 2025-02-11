# Week 7 Flutter
## Brilyan Satria Wahyuda
## TI-3H 2241720019

### Praktikum Langkah 2
Pada langkah 2 dilakukan ```flutter pub add auto_size_text```
langkah ini dilakukan untuk menambahkan plugin ```auto_size_text``` pada ```pubspec.yaml``` di project kita agar bisa digunakan.

### Praktikum langkah 5
pada langkah 5 dibuat ```final String text;``` untuk digunakan pada widget ```RedTextWidget``` Selain itu ditambahkan ```required this.text``` karena menandakan parameter text harus diisi saat memanggil function. Hal ini memastikan tidak ada null value yang akan dimasukkan saat function dipanggil.

### Praktikum langkah 6
Terdapat dua container, yang awal menggunakan widget dan yang kedua tidak. Bisa dilihat perbedaannya saat app di jalankan, column pertama memiliki text berwarna merah, memiliki 2 baris, font nya berukuran 14 dan memiliki ```TextOverflowElipsis``` dikarenakan menggunakan ```RedTextWidget``` dimana didalamnya juga terdapat ```AutoSizeText``` sehingga tidak perlu mengatur lagi style dari text nya. Karena pada widget ```RedTextWidget``` Sudah diatur style nya.

### Soal nomor 5
#### Berikut adalah penjelasan setiap parameter plugin auto_size_text
- key * = Mengontrol bagaimana sebuah widget menggantikan widget lain dalam widget tree
- textKey = Set key untuk hasil Text widget
- style * = jika tidak null akan digunakan style ini
- minFontSize = set font size minimum saat auto-sizing
- maxFontSize - set font size maksimum saat auto-sizing
- stepGranularity = ukuran langkah atau interval penyesuaian font
- presetFontSizes = daftar ukuran font yang sudah ditetapkan sebelumnya
- group = Menghubungkan beberapa text yang memakai AutoSizeText
- textAlign = Menentukan teks harus disejajarkan secara horizontal
- textDirection = menentukan arah penulisan teks
- locale = Digunakan untuk memilih font yang tepat ketika karakter Unicode yang sama dapat dirender berbeda berdasarkan lokal bahasa atau wilayah.
- softWrap: menentkan apaka teks harus menggunakan softwrap (dipisah atau dipotong saat soft break)
- wrapWords: Menentukan apakah kata-kata yang tidak sesuai dalam satu baris harus dipisah dan dipindahkan ke baris berikutnya. 
- overflow: Menentukan bagaimana visual overflow (teks yang meluap dari batas) akan ditangani, apakah akan dipotong, disembunyikan, atau ditampilkan dengan cara lain
- overflowReplacement: Widget pengganti yang akan ditampilkan jika teks meluap dan tidak bisa dimuat dalam batas yang ditentukan.
- textScaleFactor: Faktor skala yang mempengaruhi ukuran font berdasarkan piksel logis. Ini juga berdampak pada minFontSize, maxFontSize, dan presetFontSizes.
- maxLines: Batas maksimal jumlah baris yang dapat digunakan oleh teks. Jika teks melebihi jumlah baris ini, teks akan dipotong.
- semanticsLabel: Label alternatif yang dapat diberikan untuk teks ini, biasanya digunakan untuk tujuan aksesibilitas, seperti pembaca layar.