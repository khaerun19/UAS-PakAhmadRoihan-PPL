# UAS-PakAhmadRoihan-PPL

AHMAD KHAERUN MAKNUN (2211310004)

#no1

Skema Hardware

- Laptop anggota kelompok
  
Skema Software

-MySQL

-PHP

-Visual Studio Code

-Visual paradigm

Skema Database

![image](https://github.com/user-attachments/assets/98d8b6a0-3507-4480-a846-e8016ee855fe)


Hubungan Antar Tabel

a. Tabel Utama:
Tabel utama adalah barang, kategori, dan member, karena data ini menjadi pusat untuk mencatat transaksi dan informasi lain.

b. Relasi Penting:
Barang ke Kategori: Setiap barang memiliki kategori (id_kategori).

Penjualan dan Nota ke Barang: Transaksi terkait barang yang dijual.

Penjualan dan Nota ke Member: Transaksi juga mencatat pelanggan yang melakukan pembelian.

Login ke Member: Setiap login hanya berlaku untuk member tertentu.

Skema Actor

- Use Case diagram

![image](https://github.com/user-attachments/assets/8f22118c-8b71-4b38-bd1f-aa091552ca10)


Penjelasan Diagram
Login: Admin harus login sebelum menggunakan sistem.

Mengelola Data Barang: Admin dapat menambah, mengedit, atau menghapus barang yang ada di sistem.

Mengelola Stok Barang: Admin menambah atau mengurangi stok barang yang tersedia.

Melakukan Penjualan: Admin memilih barang yang dijual, memproses checkout, dan mencetak invoice.

Melihat Laporan Penjualan: Admin dapat melihat laporan penjualan secara berkala.

Melihat Riwayat Transaksi: Admin dapat melihat transaksi yang sudah terjadi untuk keperluan pencatatan.

- Sequence Diagram

  ![image](https://github.com/user-attachments/assets/f1227281-4160-45bc-871d-9a27558597a6)


Deskripsi Sequence Diagram:
Aktor:

Admin
Entitas website Sistem Penjualan:

Database

Modul Login

Modul Barang

Modul Penjualan

Modul Laporan

Skema Interaksi:

Admin Login:

Admin memasukkan username dan password.

Sistem memverifikasi kredensial di database.

Sistem memberikan akses jika berhasil.

Mengelola Barang:

Admin menambah/mengedit/menghapus data barang.

Sistem menyimpan perubahan di database.

Melakukan Penjualan:

Admin memilih barang untuk dijual.

Admin memasukkan jumlah barang yang dijual.

Sistem menghitung total harga dan menyimpan data transaksi.

Melihat Laporan:

Admin meminta laporan penjualan.

Sistem mengambil data dari database dan menampilkan laporan.

- Activity Diagram

  ![image](https://github.com/user-attachments/assets/dec42d86-228f-45db-9ecb-52d3ec8a1b62)

#NO2

Untuk proyek ini, bahasa pemrograman yang akan digunakan adalah PHP dengan tambahan JavaScript untuk pengembangan sisi klien, serta MySQL untuk basis data

1. Bahasa Pemrograman yang Digunakan
   
PHP:

PHP dipilih karena ini adalah bahasa pemrograman server-side yang sangat populer untuk pengembangan aplikasi web dinamis. Beberapa alasan memilih PHP:

Mudah dipelajari: PHP relatif mudah dipelajari bagi pemula dan memiliki dokumentasi yang luas.

Ketersediaan hosting: PHP didukung oleh hampir semua penyedia layanan hosting, sehingga lebih mudah untuk deploy aplikasi web.

Keamanan: PHP memiliki banyak fitur keamanan yang sudah ada, seperti proteksi terhadap SQL injection dan Cross-Site Scripting (XSS).

Kompatibilitas Database: PHP terintegrasi dengan MySQL secara alami dan memiliki banyak library untuk mempermudah pengelolaan database.

JavaScript:

JavaScript digunakan di sisi klien (frontend) untuk membuat antarmuka pengguna (UI) yang interaktif dan dinamis. JavaScript memungkinkan manipulasi DOM secara langsung, serta pengiriman dan pengambilan data melalui AJAX, yang meningkatkan pengalaman pengguna.

MySQL:

MySQL dipilih sebagai sistem manajemen basis data (DBMS) karena kehandalan dan kemudahan integrasi dengan PHP. MySQL adalah salah satu database yang paling banyak digunakan dalam pengembangan aplikasi web dan memiliki fitur yang kuat serta kinerja yang tinggi untuk menangani data dalam jumlah besar.

2. Platform Pengembangan
   
Aplikasi berbasis Web:

Platform yang dipilih untuk pengembangan adalah aplikasi berbasis web. Hal ini memungkinkan pengguna untuk mengakses aplikasi dari perangkat apapun yang terhubung ke internet tanpa perlu menginstal perangkat lunak tambahan. Dengan menggunakan PHP di sisi server dan JavaScript di sisi klien, aplikasi dapat memberikan antarmuka yang dinamis dan dapat diakses di berbagai perangkat.

4. Perangkat Lunak Pendukung
   
IDE (Integrated Development Environment):

Visual Studio Code (VSCode): VSCode dipilih karena ringan, mudah digunakan, dan memiliki banyak ekstensi yang mendukung PHP, JavaScript, dan MySQL.

XAMPP atau MAMP:

XAMPP (atau MAMP untuk macOS) digunakan untuk menyediakan server lokal dengan Apache, PHP, dan MySQL, yang memungkinkan pengembangan dan pengujian aplikasi secara offline.

Git:

Digunakan untuk version control. Proyek ini akan menggunakan Git sebagai alat untuk mengelola dan melacak perubahan kode yang dilakukan oleh tim pengembangan, serta untuk kolaborasi melalui GitHub.

MySQL Workbench:

Untuk memudahkan desain dan manajemen database MySQL, MySQL Workbench digunakan. Dengan Workbench, proses pembuatan dan pengelolaan database menjadi lebih intuitif.

![image](https://github.com/user-attachments/assets/f46ab90f-fd68-4a68-80f5-d6e0bb2c6042)


#no3

Gambaran proses implementasi sistem dari persiapan lingkungan kerja hingga penerapan komponen-komponen perangkat lunak. Langkah-langkah ini mencakup integrasi hardware, software, database, dan antarmuka pengguna untuk memastikan sistem berjalan sesuai desain.

1. Persiapan Lingkungan Kerja
   
- Instalasi Perangkat Lunak dan Alat Pengembangan:

-Instalasi IDE: Pertama, install IDE seperti Visual Studio Code (VSCode) yang akan digunakan untuk menulis kode PHP dan JavaScript. Pastikan VSCode terkonfigurasi dengan ekstensi untuk PHP, JavaScript, dan MySQL.

-Instalasi XAMPP/MAMP: Install XAMPP (atau MAMP untuk macOS) untuk menyediakan server lokal yang mencakup Apache, PHP, dan MySQL. Ini akan menjadi platform pengujian untuk aplikasi berbasis web yang sedang dikembangkan.

-Instalasi Git: Instal Git untuk kontrol versi, sehingga dapat melacak perubahan kode dan kolaborasi dengan tim pengembang.

-MySQL Workbench: Instal MySQL Workbench untuk desain dan manajemen basis data.

-Konfigurasi Database:

Buat database baru di MySQL dengan nama tb_anugrah (sesuai dengan struktur yang sudah direncanakan).
Buat tabel yang diperlukan dalam database sesuai dengan desain yang telah dibuat, seperti detail, pesanan, masuk, pesanan_produk, dan user.
Siapkan hubungan antar tabel (relasi) menggunakan foreign keys jika diperlukan untuk memastikan integritas data.

-Pengaturan Server Lokal:

Pastikan XAMPP/MAMP berjalan dengan baik dan Apache serta MySQL dapat diakses melalui localhost.
Uji apakah PHP dapat dijalankan dengan membuat file PHP sederhana dan mengaksesnya melalui browser.

2. Pengembangan Aplikasi
   
-Desain dan Pengembangan Antarmuka Pengguna (Frontend):

HTML, CSS, dan JavaScript digunakan untuk membuat tampilan antarmuka pengguna. Halaman seperti login.php, dashboard.php, produk.php, dan pesanan.php dikembangkan dengan elemen-elemen HTML dan CSS yang bersih dan responsif.
Gunakan JavaScript untuk menambah interaktivitas, seperti pengambilan data secara dinamis melalui AJAX, validasi formulir di sisi klien, dan manipulasi DOM untuk memberikan pengalaman pengguna yang lebih baik.

-Pengembangan Backend:

PHP digunakan untuk menangani logika aplikasi di sisi server. Ini termasuk:
Koneksi ke database menggunakan db.php.
Menangani proses autentikasi dan manajemen sesi pada login.php.
Memproses data yang dikirimkan dari formulir dan melakukan operasi CRUD pada pesanan.php, produk.php, dan detail_pesanan.php.
Mengubah status pesanan melalui ubah_status.php dan mengelola laporan pada laporan.php.
Kode PHP akan mengakses dan memodifikasi data di database tb_anugrah sesuai dengan permintaan pengguna.

-Integrasi Sistem Keamanan:

Terapkan prosedur keamanan standar seperti hashing password menggunakan fungsi PHP password_hash() untuk melindungi data pengguna.
Gunakan prepared statements di PHP untuk mencegah SQL Injection saat berinteraksi dengan database.
Terapkan pengamanan untuk melindungi aplikasi dari Cross-Site Scripting (XSS) dan Cross-Site Request Forgery (CSRF).

3. Pengujian Sistem
   
-Pengujian Fungsional:

Uji setiap fitur aplikasi untuk memastikan bahwa semua fungsionalitas berfungsi seperti yang diinginkan, mulai dari login, manajemen produk, hingga pengelolaan pesanan.
Lakukan pengujian terhadap form input untuk memastikan data yang dimasukkan ke dalam database akurat dan tidak ada kesalahan logika dalam aplikasi.

-Pengujian Keamanan:

Lakukan uji keamanan seperti penetration testing untuk mencari potensi celah di aplikasi.
Pastikan bahwa session hijacking dan SQL injection tidak bisa dilakukan oleh pihak yang tidak berwenang.

-Pengujian Performa:

Uji performa aplikasi di server lokal dengan beberapa beban pengguna untuk memastikan aplikasi dapat menangani permintaan dengan cepat dan tanpa masalah.

4. Integrasi dan Penyebaran
   
-Integrasi Sistem:

Setelah semua komponen diuji secara terpisah, integrasikan frontend dan backend secara penuh.
Pastikan komunikasi antara frontend (JavaScript) dan backend (PHP) berjalan lancar. Penggunaan AJAX untuk pengiriman data secara dinamis dan pemrosesan di PHP harus berfungsi tanpa hambatan.

-Penyebaran ke Server Produksi:

Setelah aplikasi siap untuk digunakan, deploy aplikasi ke server produksi.
Pastikan konfigurasi server di hosting sudah sesuai, seperti pengaturan domain, basis data, dan keamanan server.
Terapkan SSL untuk enkripsi data yang dikirimkan antara klien dan server.

5. Pemeliharaan dan Pembaruan
   
-Pemantauan dan Logging:

Pasang alat pemantauan untuk memantau performa server dan aplikasi. Gunakan log error untuk melacak masalah yang muncul selama penggunaan.

-Pembaruan Sistem:

Secara rutin lakukan pembaruan terhadap aplikasi, memperbaiki bug yang ditemukan, serta meningkatkan fitur dan keamanan sistem.

#4 

- Metode Pengujian: Black-Box Testing
  
Black-box testing berfokus pada pengujian fungsionalitas aplikasi tanpa melihat implementasi internal dari kode sumber. Pengujian ini berfokus pada input dan output aplikasi untuk memastikan aplikasi bekerja sesuai dengan persyaratan pengguna dan spesifikasi sistem. Pengujian ini akan mencakup jenis-jenis pengujian berikut:

Jenis Pengujian Black-Box:

Unit Testing:

Unit testing akan menguji bagian-bagian terkecil dari aplikasi seperti fungsi atau metode individual untuk memastikan bahwa setiap unit kode berfungsi dengan benar. Misalnya, pengujian validasi form login untuk memastikan hanya pengguna yang valid yang dapat masuk.

Hasil Pengujian:

Jika fungsi login menerima input yang benar (username dan password yang valid), maka pengguna dapat diarahkan ke dashboard. Sebaliknya, input yang salah akan menghasilkan pesan error.

#5

1. Identifikasi Masalah
Kesalahan pencatatan transaksi secara manual, seperti total pembayaran atau stok barang.

Kesulitan dalam mengetahui stok barang secara real-time.

Proses pembuatan laporan yang memakan waktu karena dilakukan secara manual.

Risiko kehilangan data akibat tidak adanya sistem terpusat.

Kurangnya efisiensi dalam pengelolaan data barang dan transaksi.

2.  Rumusan Masalah
Bagaimana merancang sistem penjualan berbasis website untuk mempermudah pencatatan transaksi di toko bangunan?

Bagaimana sistem ini dapat membantu memantau stok barang secara real-time?

Bagaimana cara mengintegrasikan pembuatan laporan otomatis ke dalam sistem?

Bagaimana memastikan keamanan dan akurasi data dalam sistem penjualan berbasis website?

3. Solusi
   
- Sistem Penjualan Berbasis Website

Mengembangkan sistem penjualan berbasis web yang memungkinkan pencatatan transaksi secara otomatis dan tersimpan dalam database.
Setiap transaksi yang dilakukan akan langsung terintegrasi ke sistem tanpa perlu pencatatan manual.

- Pemantauan Stok Barang Real-Time

Menyediakan fitur manajemen stok yang otomatis memperbarui jumlah barang setelah transaksi.
Menggunakan database MySQL untuk menyimpan data stok barang dan AJAX untuk menampilkan data stok secara real-time di dashboard admin.

- Pembuatan Laporan Otomatis

Mengembangkan modul laporan otomatis yang menghasilkan laporan penjualan dan stok barang berdasarkan data transaksi.
Laporan dapat diekspor dalam format PDF/Excel dan ditampilkan dalam bentuk grafik untuk analisis lebih mudah.

- Keamanan dan Akurasi Data

Mengimplementasikan validasi input dan enkripsi data sensitif (seperti hash password dengan password_hash()).
Menggunakan backup database otomatis untuk mencegah kehilangan data.
Menerapkan role-based access control (RBAC) untuk membatasi akses pengguna berdasarkan hak tertentu.




