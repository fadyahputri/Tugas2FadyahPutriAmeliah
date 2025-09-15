Tugas 2: Crawling Data Twitter dengan Tweet-Harvest
Latar Belakang

Twitter merupakan salah satu media sosial yang sangat dinamis dan sering digunakan untuk menyampaikan opini publik. Dengan jutaan pengguna aktif, Twitter menyimpan banyak data yang relevan untuk penelitian, analisis tren, maupun pemetaan sentimen. Untuk keperluan tersebut, digunakan tweet-harvest, yaitu sebuah tool berbasis Node.js yang dapat mengambil tweet sesuai kata kunci, rentang waktu, bahasa, dan jumlah data tertentu.

Dalam tugas ini, proses crawling difokuskan pada kata kunci tertentu, misalnya “gibran”, dengan periode waktu yang sudah ditentukan. Data yang berhasil dikumpulkan kemudian disimpan dalam format CSV agar bisa dianalisis lebih lanjut menggunakan Python dan library pandas.

Alur Pengerjaan
1. Autentikasi

Proses pengambilan data Twitter memerlukan auth token sebagai kunci akses. Token ini memastikan bahwa tool yang digunakan memiliki izin untuk mengakses tweet dari platform Twitter.

2. Persiapan Lingkungan

Sebelum proses crawling, perlu dipasang library Python (seperti pandas untuk analisis data) dan Node.js (karena tweet-harvest dibangun di atas Node.js). Tahap ini memastikan bahwa semua dependensi yang dibutuhkan tersedia di Google Colab.

3. Menentukan Parameter Crawling

Beberapa parameter penting ditetapkan sebelum crawling dilakukan, antara lain:

Nama file output → tempat penyimpanan hasil crawling dalam format CSV.

Kata kunci pencarian → misalnya “gibran”, dilengkapi filter waktu dan bahasa.

Batas jumlah tweet → misalnya 100 tweet, agar hasil sesuai kebutuhan.

4. Proses Crawling

Tweet-harvest dijalankan dengan parameter yang telah ditentukan. Proses ini secara otomatis mengambil tweet dari Twitter sesuai kriteria (kata kunci, waktu, bahasa, dan jumlah tweet). Hasilnya langsung tersimpan dalam file CSV.

5. Membaca dan Mengecek Data

File CSV hasil crawling kemudian dibaca menggunakan pandas. Data yang sudah masuk ditampilkan dalam bentuk tabel untuk mempermudah pengecekan. Selain itu, jumlah tweet yang berhasil dikumpulkan dihitung untuk memastikan sesuai dengan batas (limit) yang ditentukan sebelumnya.

Kesimpulan

Proses crawling data Twitter dengan tweet-harvest memungkinkan pengumpulan tweet secara cepat, otomatis, dan terstruktur. Hasil akhirnya berupa file CSV yang dapat langsung dianalisis lebih lanjut, misalnya untuk:

melihat tren percakapan,

menganalisis sentimen,

atau memetakan opini publik terhadap tokoh/isu tertentu.

Dengan alur ini, peneliti atau praktisi dapat dengan mudah mengakses data Twitter dalam jumlah besar tanpa perlu mengambil tweet secara manual.# Tugas2FadyahPutriAmeliah
