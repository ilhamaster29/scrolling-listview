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
> Ketika aplikasi di jalankan, aplikasi akan menampilkan tulisan dari package **english_words**. Kemudian tiap kali aplikasi dijalankan ulang / _hot reload_, tulisan akan selalu berubah. Hal ini terjadi karena pasangan kata dihasilkan di dalam metode **build**, yang berjalan setiap kali **MaterialApp** memerlukan _rendering_, atau saat mengaktifkan _Platform_ di _Flutter Inspector_.

## 3. Menambahkan _Stateful Widget_
- Membuat kode _boilerplate_ untuk _stateful widget_
![Screenshot](images/buat_stateful_widget.png)
> Ketika **stful** diketikkan pada baris baru file **main.dart**, maka akan muncul popup untuk memmbuat _stateful widget_.

- Menamakan widget sebagai **RandomWords**
![Screenshot](images/namawidget_randomwords.png)
> Ketika salah satu tulisan **MyWidget** diganti dengan tulisan **RandomWords**, maka semua kata **MyWidget** akan berubah secara otomatis menjadi **MyWidget**.

- Memperbarui metode **build()** pada **_RandomWordsState**
![Screenshot](images/update_build__RandomWordsState.png)

- Menghilangkan _word-generation_ dari **MyApp**
![Screenshot](images/menghilangkan_word-generation.png)

- _Hot reload_ aplikasi
![Screenshot](images/statefulwidget_running.png)
![Screenshot](images/statefulwidget_running_hotreload.png)

## 4. Membuat _Infinite Scrolling ListView_

- Menambahkan _state variable_ ke kelas **_RandomWordsState**
![Screenshot](images/suggestion_biggerfont.png)
> Menambahkan sebuah daftar **_suggestion** untuk menyimpan gabungan kata yang disarankan. Juga, menambahkan variabel **_biggerFont** untuk membuat *font* lebih besar. 

- Memperbarui metode **build** pada **_RandomWordsState**
![Screenshot](images/panggil_word-generation.png)

- Memperbarui metode **build** pada **MyApp**
![Screenshot](images/update_build__MyApp.png)

- _Running final app_
![Screenshot](images/final_running.png)
