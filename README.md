# sr-programming-test-2
## Deskripsi
Repositori ini digunakan sebagai rujukan untuk test pemrograman senior.

# Spesifikasi Program
Pemohon diharapkan dapat menunjukkan pemahaman dan kemampuannya membuat program dengan membuat aplikasi sederhana yang:
* dibuat dalam bahasa yang dikuasai (java, scala, python, php, nodejs atau lainnya)
* mendapatkan DETAIL_ARTIKEL berita dengan dua cara:
  * membuka rss links: http://www.tribunnews.com/rss
  * halaman indeks berita: https://www.antaranews.com/indeks
* Untuk pengambilan DETAIL_ARTIKEL dari halaman indeks berita, haruslah menggunakan XPATH
  * Silakan mengakses URL berikut ini untuk keterangan lebih lanjut: [XPATH w3schools](https://www.w3schools.com/xml/xpath_intro.asp)
* menyimpan DETAIL_ARTIKEL ke dalam database dan solr
  * Untuk database, silahkan melihat [skema ini](https://github.com/sonarid/sr-programming-test-2/blob/master/schema/sql/news_article.sql)
  * Untuk solr, silahkan melihat [skema ini](https://github.com/sonarid/sr-programming-test-2/blob/master/schema/news_solr.txt)
* DETAIL_ARTIKEL terdiri dari:
  * URL
  * Judul
  * Waktu Tayang (berupa unix timestamp)
  * Konten Lengkap (bukan summary)
Catatan Tambahan:
* Aplikasi dibuat dengan konsep MVC yang baik
* Diharapkan dapat menggunakan framework bagi bahasa pemrograman yang dipilih, jika tidak bisa pastikan kodenya terstruktur dengan baik
* Code Readability sangat penting
* Dilengkapi dengan dokumentasi yang memadai, minimal di setiap kelas ataupun fungsi yang penting
* Aplikasi yang dibuat harus disertakan dengan langkah instalasi dan pengetesan
* Aplikasi bisa dijalankan dengan docker menjadi nilai tambah
* Aplikasi yang dibuat harus dizip dan dikirimkan ke alamat email yang ditentukan

# Contoh DETAIL_ARTIKEL:
  * URL: **https://bisnis.tempo.co/read/1381362/dikabarkan-utang-untuk-put-bukopin-dari-mana-dana-bosowa-sebenarnya**
  * Judul: **Dikabarkan Utang untuk PUT Bukopin, dari Mana Dana Bosowa Sebenarnya?**
  * Waktu Tayang: **1598952660**
  * Konten Lengkap: 
> TEMPO.CO, Jakarta -  Saat mengikuti Penawaran Umum Terbatas (PUT) V Bank Bukopin, PT Bosowa Corporindo menempatkan dana di escrow account senilai Rp 243 miliar. Bosowa pun melaksanakan pembelian 1,09 miliar lembar saham melalui skema Hak Memesan Efek Terlebih Dahulu (HMETD) pada PUT V tersebut.
Dengan harga Rp180 per lembar saham, dana yang dikeluarkan Bosowa untuk mengikuti PUT V adalah senilai R p196 miliar, sehingga porsi kepemilikan sahamnya menjadi 23,40 persen.
Direktur Keuangan Bosowa Corporindo, Evyana Mukti mengatakan pihaknya telah menerima undangan klarifikasi dari Otoritas Jasa Keuangan (OJK),  untuk menjelaskan sumber dana perseroan dalam mengikuti PUT V Bukopin. Namun, undangan tersebut berdekatan dengan jadwal pertemuan Bosowa dengan KB Kookmin sehingga pihaknya baru bisa membalas surat tersebut dengan meminta kelonggaran waktu.
Hanya saja dengan balasan tersebut, Evyana menyebutkan, OJK merespons dengan berasumsi bahwa sumber dana Bosowa berasal dari utang. Padahal, Bosowa sudah menjelaskan bahwa sumber dana perseroan dalam mengikuti PUT adalah berasal dari penjualan saham di perusahaan lain, penjualan aset, dana operasional, dan dari anak usaha.
"Kami jelaskan lagi sumber dana dari penjualan saham, dana operasional, dan anak usaha yang mampu. Ini kami jawab tertulis ke OJK," katanya saat berkunjung ke kantor Bisnis, Senin 31 Agustus 2020.
Penawaran Umum Terbatas (PUT) V merupakan aksi korporasi yang dilakukan Bank Bukopin untuk meningkatkan rasio kecukupan modal (capital adequacy ratio/CAR) ke level 14 persen. Bank Bukopin mendapat tambahan modal baru senilai Rp 838 miliar. Dana yang diperoleh rencananya digunakan 40 persen untuk pengembangan bisnis segmen konsumer, dan 60 persen untuk pengembangan bisnis 
Usai proses PUT V melalui skema Hak Memesan Efek Terlebih Dahulu (HMETD), KB Kookmin Bank resmi menjadi pemegang saham terbesar Bank Bukopin. KB Kookmin Bank menyerap sekitar 2,97 miliar lembar saham baru selama masa perdagangan dan pemesanan tambahan HMETD. Sementara itu, Bosowa Corporindo, yang juga melaksanakan porsi HMETD-nya, menyerap 1,09 miliar lembar saham.
Setelah PUT V, komposisi urutan Pemegang Saham di Bank Bukopin menjadi KB Kookmin Bank dengan porsi kepemilikan 33,90 persen disusul Bosowa sebesar 23,40 persen, Negara Republik Indonesia pada 6,37 persen, dan pemegang saham publik dengan kepemilikan di bawah 5 persen mencapai 36,33 persen.