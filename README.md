# README - Perhitungan Hari

## Deskripsi Aplikasi
Aplikasi **Perhitungan Hari** adalah sebuah aplikasi desktop berbasis Java yang digunakan untuk menghitung jumlah hari dalam suatu bulan pada tahun tertentu dan menghitung selisih antara dua tanggal. Aplikasi ini memanfaatkan komponen-komponen Java Swing untuk antarmuka grafis (GUI) yang mudah digunakan.

## Fitur Aplikasi
- **Pemilihan Bulan dan Tahun**: Pengguna dapat memilih bulan dan tahun untuk menghitung jumlah hari dalam bulan tersebut.
- **Penghitungan Jumlah Hari**: Aplikasi menghitung jumlah hari dalam bulan yang dipilih, termasuk informasi apakah tahun tersebut adalah tahun kabisat.
- **Pilih Tanggal Awal dan Akhir**: Pengguna dapat memilih tanggal awal dan tanggal akhir menggunakan dua kalender.
- **Hitung Selisih Hari**: Setelah memilih dua tanggal, aplikasi akan menghitung dan menampilkan selisih hari antara tanggal yang dipilih.
- **Tahun Kabisat**: Aplikasi dapat mendeteksi dan menampilkan apakah tahun yang dipilih adalah tahun kabisat atau bukan.

## Komponen Utama dalam Aplikasi
Aplikasi ini menggunakan komponen-komponen **Java Swing** untuk antarmuka pengguna yang interaktif dan mudah digunakan:

### 1. **JComboBox** (Pilih Bulan)
`JComboBox` adalah komponen grafis yang memungkinkan pengguna untuk memilih satu nilai dari daftar pilihan yang telah disediakan. Pada aplikasi ini, `JComboBox` digunakan untuk memilih bulan dalam satu tahun. Pilihan yang ada adalah nama bulan dari Januari hingga Desember.

- **Fungsi**: Pengguna memilih bulan dari daftar yang disediakan untuk menentukan bulan yang ingin dihitung jumlah harinya.
- **Terkait dengan**: Tahun yang dimasukkan melalui `JSpinner` dan tanggal yang ditampilkan pada kalender.
- **Cara Kerja**: Ketika pengguna memilih bulan, aplikasi akan menyesuaikan tanggal pada kedua kalender (`JCalendar`) dan mengupdate informasi hari pertama, hari terakhir, serta jumlah hari dalam bulan yang dipilih.

### 2. **JSpinner** (Masukkan Tahun)
`JSpinner` adalah komponen grafis yang memungkinkan pengguna untuk memilih nilai numerik melalui tombol naik (↑) dan turun (↓) atau dengan memasukkan nilai secara manual. Pada aplikasi ini, `JSpinner` digunakan untuk memasukkan tahun yang ingin dihitung.

- **Fungsi**: Pengguna memilih atau memasukkan tahun yang akan digunakan untuk perhitungan jumlah hari dalam bulan yang dipilih.
- **Terkait dengan**: Bulan yang dipilih melalui `JComboBox` dan tanggal pada `JCalendar`.
- **Cara Kerja**: Ketika tahun diubah, tanggal yang ditampilkan pada kedua kalender (`JCalendar`) akan diperbarui agar sesuai dengan tahun yang dimasukkan.

### 3. **JCalendar** (Pilih Tanggal Awal dan Akhir)
`JCalendar` adalah komponen kalender yang memungkinkan pengguna untuk memilih tanggal. Pada aplikasi ini, terdapat dua `JCalendar`:
- **jCalendar1**: Digunakan untuk memilih tanggal awal.
- **jCalendar2**: Digunakan untuk memilih tanggal akhir.

- **Fungsi**: Pengguna memilih tanggal mulai dan tanggal akhir yang akan dihitung selisihnya.
- **Terkait dengan**: Bulan yang dipilih melalui `JComboBox` dan tahun yang dimasukkan melalui `JSpinner`.
- **Cara Kerja**: Ketika pengguna memilih tanggal, informasi hari pertama dan hari terakhir akan diperbarui sesuai dengan tanggal yang dipilih.

## Cara Penggunaan
1. **Pilih Bulan**: Pilih bulan yang diinginkan dari dropdown `JComboBox`.
2. **Masukkan Tahun**: Masukkan tahun yang akan digunakan dalam `JSpinner`.
3. **Pilih Tanggal Awal dan Akhir**: Pilih tanggal awal dan tanggal akhir melalui dua `JCalendar` yang disediakan.
4. **Hitung Hari**: Tekan tombol **Hitung Hari** untuk menghitung jumlah hari dalam bulan yang dipilih dan selisih antara tanggal yang dipilih.
5. **Tampilkan Hasil**: Hasil perhitungan jumlah hari dalam bulan, hari pertama, hari terakhir, dan selisih hari akan ditampilkan pada label.

## Contoh Hasil
- Jika memilih **Bulan Maret 2024**, aplikasi akan menampilkan bahwa Maret memiliki **31 hari** dan hari pertama bulan Maret 2024 adalah **Minggu** dan hari terakhir adalah **Minggu**.
- Jika memilih dua tanggal untuk dihitung selisihnya, misalnya **1 Januari 2024** dan **10 Januari 2024**, aplikasi akan menghitung dan menampilkan **9 hari**.

## Keunggulan Aplikasi
1. **Antarmuka Pengguna yang Sederhana**: Aplikasi ini menggunakan antarmuka grafis yang mudah digunakan, dengan komponen seperti `JComboBox`, `JSpinner`, dan `JCalendar` yang memungkinkan pengguna berinteraksi dengan mudah.
2. **Dukungan Tahun Kabisat**: Aplikasi ini otomatis mengidentifikasi tahun kabisat dan menampilkan informasi tersebut kepada pengguna.
3. **Perhitungan Selisih Hari**: Aplikasi ini memungkinkan pengguna untuk menghitung selisih hari antara dua tanggal dengan akurat.
4. **Penggunaan Kalender**: Dengan menggunakan `JCalendar`, aplikasi memungkinkan pengguna untuk memilih tanggal secara visual, yang meningkatkan pengalaman pengguna.
5. **Validasi Input**: Aplikasi ini memvalidasi input pengguna, memastikan tahun yang dimasukkan memiliki format yang benar (empat digit).

## Pembuat Aplikasi
  Muhammad Ikhya - 2210010405

## Demo
![Demo GIF](/img/PerhitunganHari.gif)
  

