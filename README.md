# Laporan Praktikum

## 1. Membuat Aplikasi Flutter Pemula
- Pembuatan project baru bernama **startup_namer** di vscode
![Screenshot](images/newproject_startup_namer.png)

- Mengedit isi _lib/main.dart_
![Screenshot](images/editisi_main.dart.png)

- Menjalankan aplikasi
![Screenshot](images/runproject_startup_namer.png)

## 2. Menggunakan _External Package_
- Penambahan _package_ **english_words** sebagai **dependency** aplikasi
![Screenshot](images/english_word_packages.png)
![Screenshot](images/perubahan_pubspec.lock.png)
![Screenshot](images/perubahan_pubspec.yaml.png)
> Pada saat _package_ **english_words** ditambahkan ke _project_, file **pubspec.lock** dan **pubspec.yaml juga berubah, seperti pada gambar diatas**.

- Import _package_ baru ke file **main.dart**
![Screenshot](images/import_english_words_ke_main.dart.png)

- Perubahan pada file **main.dart**
![Screenshot](images/edit_main.dart.png)

- *Running* aplikasi
![Screenshot](images/running_aplikasi.png)
![Screenshot](images/running_aplikasi_hotreload.png)
> Ketika aplikasi di jalankan, aplikasi akan menampilkan tulisan dari package **english_words**. Kemudian tiap kalo aplikasi dijalankan ulang / _hot reload_, tulisan akan selalu berubah. Hal ini terjadi karena pasangan kata dihasilkan di dalam metode **build**, yang berjalan setiap kali **MaterialApp** memerlukan _rendering_, atau saat mengaktifkan _Platform_ di _Flutter Inspector_.



