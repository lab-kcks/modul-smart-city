# MODUL 3.1 PERANCANGAN PROOF OF CONCEPT (PoC)
**Mata Kuliah:** Teknologi Smart City (ET234504)  
**Program Studi:** Teknologi Informasi  
**Departemen:** Teknologi Informasi, ITS  
**Bobot Praktikum:** 1 SKS

---

## 1. Tujuan Pembelajaran

Setelah mempelajari materi ini, mahasiswa diharapkan mampu:

1. Memahami konsep aliran data dan menyusun Data Flow Diagram (DFD) untuk menggambarkan aliran data dalam sistem Smart City.
2. Mengidentifikasi dan mengklasifikasikan jenis data yang digunakan dalam sistem.
3. Memahami prinsip tata kelola data dan tahapan siklus hidup data.
4. Mengidentifikasi risiko keamanan data serta menentukan kebutuhan kontrol teknis.
5. Memahami prinsip privasi, ketentuan UU Pelindungan Data Pribadi, dan etika pemanfaatan data warga.

## 2. Perancangan Alur Data (Data Flow Diagram)

### 2.1 Konsep Aliran Data dalam Sistem Smart City

Sistem Smart City menggunakan data sebagai dasar untuk menjalankan layanan, memantau kondisi perkotaan, dan mendukung pengambilan keputusan. Data dapat berasal dari berbagai sumber, seperti sensor, perangkat Internet of Things (IoT), aplikasi, sistem informasi pemerintah, dan masukan masyarakat.

Dalam sebuah sistem, data melewati beberapa proses sebelum menghasilkan informasi yang digunakan oleh pengguna atau instansi terkait.

Secara umum, aliran data melibatkan:

1. **Sumber Data:** Pihak, perangkat, atau sistem yang menghasilkan dan menyediakan data.
2. **Proses Pengolahan:** Aktivitas untuk menerima, memvalidasi, mengolah, atau menganalisis data.
3. **Penyimpanan Data:** Media atau sistem yang digunakan untuk menyimpan data.
4. **Penggunaan Data:** Pemanfaatan data oleh pengguna, aplikasi, atau instansi untuk menghasilkan informasi atau mendukung suatu layanan.

Pemahaman terhadap aliran data diperlukan untuk mengetahui asal data, proses yang dilalui, lokasi penyimpanan, serta pihak yang menerima atau menggunakan data.

### 2.2 Data Flow Diagram (DFD)

<img width="715" height="655" alt="image" src="https://github.com/user-attachments/assets/2142988a-649d-42a9-bbee-521c0d0123fd" />


**Data Flow Diagram (DFD)** merupakan diagram yang digunakan untuk menggambarkan pergerakan data dalam suatu sistem, termasuk sumber data, proses pengolahan, penyimpanan, dan tujuan data.

DFD membantu menjelaskan bagaimana data masuk ke dalam sistem, diproses, disimpan, dan menghasilkan keluaran. DFD berfokus pada aliran dan transformasi data, bukan pada urutan instruksi program atau detail algoritma.

Terdapat empat komponen utama dalam DFD.

#### A. External Entity

External Entity merupakan pihak atau sistem di luar batas sistem yang dimodelkan dan berinteraksi dengan sistem melalui pertukaran data.

Contoh:
- Masyarakat.
- Petugas operasional.
- Instansi pemerintah.
- Perangkat atau sistem eksternal.

#### B. Process

Process merupakan aktivitas yang mengolah atau mentransformasikan data dari satu bentuk menjadi bentuk lain.

Contoh:
- Memvalidasi data.
- Menghitung jumlah kendaraan.
- Menganalisis kondisi lingkungan.
- Menghasilkan laporan.

Setiap proses harus memiliki masukan dan menghasilkan keluaran yang relevan dengan fungsi proses tersebut.

#### C. Data Store

Data Store merupakan tempat penyimpanan data yang digunakan oleh sistem. Data Store dapat berupa basis data, berkas, atau media penyimpanan lainnya.

Contoh:
- Database pengguna.
- Database sensor.
- Penyimpanan riwayat transaksi.
- Penyimpanan hasil pengukuran.

#### D. Data Flow

Data Flow merupakan aliran data yang berpindah dari satu komponen ke komponen lainnya. Arah perpindahan ditunjukkan menggunakan garis berpanah.

Setiap aliran data harus memiliki nama yang menjelaskan informasi yang dipindahkan.

Contoh:
- Data suhu.
- Data lokasi.
- Data kendaraan.
- Data laporan masyarakat.
- Hasil analisis.

**Ringkasan komponen DFD:**

| Komponen | Fungsi | Contoh |
|---|---|---|
| External Entity | Sumber atau penerima data di luar sistem | Masyarakat |
| Process | Mengolah atau mentransformasikan data | Validasi data |
| Data Store | Menyimpan data | Database sensor |
| Data Flow | Menunjukkan perpindahan data | Data pengukuran |

#### Notasi DFD

Notasi DFD dapat berbeda antarreferensi atau metode pemodelan. Oleh karena itu, satu konvensi notasi harus digunakan secara konsisten dalam satu diagram.

Empat komponen tersebut dapat direpresentasikan menggunakan notasi berikut.

| Komponen | Representasi umum |
|---|---|
| External Entity | Persegi panjang |
| Process | Lingkaran atau persegi panjang bersudut tumpul |
| Data Store | Dua garis sejajar atau simbol penyimpanan terbuka |
| Data Flow | Garis berpanah |

**Catatan:** Bentuk simbol dapat berbeda sesuai notasi yang digunakan. Fungsi setiap komponen harus tetap dapat dibedakan dengan jelas.

#### Prinsip Penyusunan DFD

Dalam menyusun DFD, beberapa prinsip berikut perlu diperhatikan:

1. Setiap komponen harus memiliki nama yang jelas dan menggambarkan fungsinya.
2. Setiap Data Flow harus menunjukkan arah perpindahan data.
3. Nama Data Flow harus menjelaskan data yang dipindahkan, bukan aktivitas atau proses.
4. Proses harus menggambarkan aktivitas pengolahan data.
5. Data Store harus menunjukkan tempat penyimpanan data yang digunakan oleh sistem.
6. External Entity harus berada di luar batas sistem yang sedang dimodelkan.
7. Diagram harus menggambarkan aliran data sesuai fungsi dan batas sistem yang ditentukan.

DFD yang baik harus dapat menjelaskan hubungan antara sumber data, proses pengolahan, penyimpanan, dan pihak yang menggunakan hasil pengolahan data.

### 2.3 Klasifikasi dan Pelabelan Jenis Data

Klasifikasi data merupakan pengelompokan data berdasarkan karakteristik dan kebutuhan pengelolaannya. Klasifikasi membantu menentukan bagaimana data dapat digunakan, disimpan, dan dibagikan.

Dalam perancangan PoC, jenis data perlu diidentifikasi agar pengelolaan dan perlindungannya dapat dirancang sesuai karakteristik data tersebut.

Untuk kebutuhan identifikasi awal, data dapat diberi label berdasarkan kategori berikut.

| Kategori | Pengertian | Contoh |
|---|---|---|
| Data Publik | Data yang dapat diakses atau dipublikasikan kepada masyarakat sesuai ketentuan yang berlaku | Statistik jumlah kendaraan, data kualitas udara agregat |
| Data Internal | Data yang digunakan untuk kebutuhan operasional atau administrasi organisasi dan tidak ditujukan untuk publikasi umum | Konfigurasi operasional sistem, laporan internal |
| Data Pribadi | Data tentang orang perseorangan yang teridentifikasi atau dapat diidentifikasi secara langsung maupun tidak langsung | Nama, nomor telepon, data kesehatan |

Ketiga kategori tersebut merupakan label operasional untuk membantu pengelolaan data dalam rancangan sistem. Kategori publik dan internal bukan klasifikasi hukum Data Pribadi dalam UU PDP.

Menurut Pasal 4 UU Nomor 27 Tahun 2022, Data Pribadi dibedakan menjadi dua jenis:

**A. Data Pribadi yang Bersifat Spesifik**

Meliputi:
- Data dan informasi kesehatan.
- Data biometrik.
- Data genetika.
- Catatan kejahatan.
- Data anak.
- Data keuangan pribadi.
- Data lainnya sesuai ketentuan peraturan perundang-undangan.

**B. Data Pribadi yang Bersifat Umum**

Meliputi:
- Nama lengkap.
- Jenis kelamin.
- Kewarganegaraan.
- Agama.
- Status perkawinan.
- Data Pribadi yang dikombinasikan untuk mengidentifikasi seseorang.

Klasifikasi berdasarkan UU PDP harus dibedakan dari label publik dan internal yang digunakan untuk kebutuhan pengelolaan informasi organisasi.

Dalam DFD, label jenis data perlu dicantumkan pada setiap aliran data yang relevan. Apabila satu aliran membawa beberapa jenis data, setiap jenis data perlu diidentifikasi secara jelas.

**Contoh:**

Sebuah sistem pemantauan transportasi dapat menggunakan:
- Data jumlah kendaraan sebagai data non-pribadi.
- Data lokasi kendaraan yang terhubung dengan identitas pemilik atau pengemudi sebagai data yang dapat termasuk Data Pribadi.
- Data operasional petugas sebagai data internal organisasi, bergantung pada isi dan kebijakan aksesnya.

Status Data Pribadi ditentukan berdasarkan apakah seseorang dapat diidentifikasi dari data tersebut, baik secara langsung maupun melalui kombinasi dengan informasi lain.

---

## 3. Tata Kelola dan Siklus Hidup Data

### 3.1 Data Governance

**Data Governance** merupakan pengaturan mengenai kebijakan, tanggung jawab, kewenangan, dan pengambilan keputusan dalam pengelolaan data organisasi.

Menurut DAMA International melalui DAMA-DMBOK, tata kelola data merupakan salah satu area utama dalam manajemen data yang mengatur kebijakan, peran, standar, dan akuntabilitas agar data dikelola secara konsisten.

Dalam konteks Smart City, data dapat dikelola dan digunakan oleh beberapa instansi atau pihak yang berbeda. Tanpa pengaturan yang jelas, dapat terjadi ketidakkonsistenan data, ketidakjelasan tanggung jawab, dan penggunaan data yang tidak sesuai tujuan.

Prinsip pengelolaan data mencakup beberapa aspek berikut.

**A. Kepemilikan dan Tanggung Jawab Data**

Organisasi perlu menentukan pihak yang bertanggung jawab atas data yang dikelola, termasuk pihak yang berwenang menetapkan aturan penggunaannya.

**B. Kualitas Data**

Data yang digunakan harus memiliki kualitas yang sesuai dengan kebutuhan sistem. Kualitas data dapat diperhatikan melalui:
- Akurasi: data sesuai dengan kondisi yang direpresentasikan.
- Kelengkapan: data memiliki informasi yang dibutuhkan.
- Konsistensi: data tidak saling bertentangan dalam penggunaan yang relevan.
- Kemutakhiran: data diperbarui sesuai kebutuhan penggunaan.

**C. Akses dan Penggunaan Data**

Penggunaan data harus mengikuti kewenangan dan tujuan yang telah ditentukan. Tidak seluruh pihak yang terlibat dalam sistem harus memiliki akses terhadap seluruh data.

**D. Kepatuhan dan Akuntabilitas**

Pengelolaan data harus mengikuti ketentuan yang berlaku. Pihak yang bertanggung jawab perlu dapat menjelaskan dasar, tujuan, dan mekanisme penggunaan data.

Dalam perancangan PoC, tata kelola data digunakan untuk menentukan:
1. Pihak yang bertanggung jawab atas data.
2. Pihak yang mengelola dan menggunakan data.
3. Tujuan penggunaan data.
4. Ketentuan akses dan pembagian data.
5. Mekanisme pengelolaan dan perlindungan data.

### 3.2 Siklus Hidup Data (Data Lifecycle)

Siklus hidup data merupakan rangkaian tahapan yang dilalui data sejak diperoleh atau dibuat hingga tidak lagi digunakan dan dimusnahkan atau dihapus.

NIST mendefinisikan siklus hidup informasi sebagai tahapan yang mencakup pembuatan atau pengumpulan, pemrosesan, penyebarluasan, penggunaan, penyimpanan, serta disposisi termasuk pemusnahan dan penghapusan.

Dalam konteks praktikum ini, pengelolaan siklus hidup data difokuskan pada tahapan berikut.

#### A. Pengumpulan Data (Data Collection)

Pengumpulan data merupakan tahap memperoleh data dari sumber yang telah ditentukan.

Sumber data dapat berupa:
- Sensor dan perangkat IoT.
- Aplikasi pengguna.
- Sistem informasi instansi.
- Data administrasi.
- Data hasil survei atau pelaporan masyarakat.

Pada tahap ini, perlu ditentukan jenis data yang dikumpulkan, sumber data, tujuan pengumpulan, serta dasar pemrosesan apabila melibatkan Data Pribadi.

#### B. Penyimpanan Data (Data Storage)

Penyimpanan data merupakan tahap menempatkan data pada media atau sistem penyimpanan agar dapat digunakan sesuai kebutuhan.

Hal yang perlu diperhatikan:
- Lokasi penyimpanan.
- Jenis media penyimpanan.
- Pihak yang bertanggung jawab.
- Ketentuan akses.
- Perlindungan data yang disimpan.
- Jangka waktu penyimpanan.

#### C. Pemrosesan Data (Data Processing)

Pemrosesan data merupakan aktivitas mengolah data untuk menghasilkan informasi yang dibutuhkan sistem.

Contohnya:
- Validasi dan pembersihan data.
- Penggabungan data dari beberapa sumber.
- Perhitungan atau agregasi.
- Analisis data.
- Penyajian informasi dalam dashboard.

Pemrosesan harus sesuai dengan tujuan yang telah ditetapkan dan memperhatikan karakteristik data yang digunakan.

#### D. Pembagian dan Penggunaan Data (Data Sharing and Usage)

Data dapat digunakan oleh sistem atau dibagikan kepada pihak lain untuk mendukung layanan dan pengambilan keputusan.

Pada tahap ini perlu ditentukan:
- Tujuan penggunaan data.
- Pihak penerima data.
- Jenis data yang dibagikan.
- Dasar dan kewenangan pembagian data.
- Ketentuan perlindungan data selama proses pertukaran.

Pembagian Data Pribadi harus mengikuti ketentuan pelindungan data yang berlaku.

#### E. Retensi Data (Data Retention)

Retensi merupakan penetapan jangka waktu penyimpanan data sebelum data dihapus atau dimusnahkan.

Jangka waktu penyimpanan perlu mempertimbangkan tujuan pemrosesan dan ketentuan peraturan perundang-undangan.

Data Pribadi tidak boleh disimpan tanpa batas waktu. UU PDP mengatur penghapusan atau pemusnahan Data Pribadi setelah masa retensi berakhir, kecuali ditentukan lain oleh peraturan perundang-undangan.

#### F. Pemusnahan Data (Data Destruction)

Pemusnahan data merupakan tahap menghapus atau memusnahkan data yang tidak lagi diperlukan sesuai ketentuan yang berlaku.

Pemusnahan dilakukan dengan mempertimbangkan:
- Berakhirnya masa retensi.
- Tidak adanya kebutuhan pemrosesan lanjutan.
- Ketentuan hukum yang mengatur penyimpanan data.
- Permintaan Subjek Data Pribadi sesuai hak dan ketentuan yang berlaku.

Pemusnahan harus dilakukan dengan cara yang mencegah data digunakan atau diakses kembali secara tidak sah.

**Ringkasan siklus hidup data:**

| Tahap | Aktivitas utama |
|---|---|
| Pengumpulan | Memperoleh data dari sumber |
| Penyimpanan | Menempatkan data pada media penyimpanan |
| Pemrosesan | Mengolah data menjadi informasi |
| Pembagian dan penggunaan | Menggunakan atau memberikan data kepada pihak yang berwenang |
| Retensi | Menentukan jangka waktu penyimpanan |
| Pemusnahan | Menghapus atau memusnahkan data |

Tahapan tersebut merupakan model konseptual pengelolaan data. Urutan dan aktivitasnya dapat menyesuaikan karakteristik sistem. Dalam satu sistem, data juga dapat melalui proses pemrosesan dan penyimpanan berulang.

---

## 4. Keamanan Siber dan Perlindungan Data

### 4.1 Konsep Keamanan Informasi
<img width="416" height="350" alt="image" src="https://github.com/user-attachments/assets/280ce56c-3557-4d7e-b431-9e6684790a1e" />


Keamanan informasi merupakan upaya melindungi informasi dan sistem informasi dari akses, penggunaan, pengungkapan, gangguan, perubahan, atau penghancuran yang tidak sah.

Menurut National Institute of Standards and Technology (NIST), keamanan informasi bertujuan menjaga tiga aspek utama yang dikenal sebagai **Confidentiality, Integrity, dan Availability (CIA Triad)**.

#### A. Confidentiality (Kerahasiaan)

Confidentiality merupakan prinsip untuk memastikan informasi hanya dapat diakses atau diungkapkan kepada pihak yang berwenang.

Tujuannya adalah mencegah pihak yang tidak berwenang memperoleh informasi yang bersifat terbatas atau sensitif.

Contoh risiko:
Data identitas masyarakat dapat diakses oleh pihak yang tidak memiliki kewenangan.

#### B. Integrity (Integritas)

Integrity merupakan prinsip untuk menjaga keakuratan dan keutuhan informasi agar tidak mengalami perubahan atau kerusakan yang tidak sah.

Data yang digunakan oleh sistem harus tetap akurat dan dapat dipercaya.

Contoh risiko:
Data hasil pengukuran sensor diubah tanpa kewenangan sehingga menghasilkan informasi yang tidak sesuai kondisi sebenarnya.

#### C. Availability (Ketersediaan)

Availability merupakan prinsip untuk memastikan informasi dan sistem tersedia ketika dibutuhkan oleh pihak yang berwenang.

Contoh risiko:
Gangguan pada server menyebabkan dashboard pemantauan tidak dapat digunakan oleh petugas operasional.

**Ringkasan CIA Triad:**

| Prinsip | Tujuan | Risiko yang dicegah |
|---|---|---|
| Confidentiality | Menjaga kerahasiaan informasi | Pengungkapan data tanpa izin |
| Integrity | Menjaga keakuratan dan keutuhan data | Perubahan data tanpa kewenangan |
| Availability | Menjamin ketersediaan informasi | Gangguan akses terhadap sistem |

Ketiga prinsip tersebut digunakan sebagai dasar untuk menentukan kebutuhan perlindungan informasi dalam sistem.

### 4.2 Ancaman dan Risiko Keamanan Data

Sistem Smart City dapat menghadapi berbagai ancaman keamanan karena melibatkan perangkat, jaringan, aplikasi, penyimpanan data, dan pihak yang menggunakan sistem.

**Ancaman keamanan** merupakan potensi kejadian atau tindakan yang dapat mengganggu keamanan informasi maupun sistem.

Contoh ancaman:
- Akses tidak sah terhadap sistem.
- Pencurian atau kebocoran data.
- Perubahan data tanpa kewenangan.
- Serangan terhadap jaringan atau server.
- Gangguan terhadap layanan sistem.
- Penyalahgunaan data oleh pihak yang memiliki akses.

Dalam mengidentifikasi risiko, beberapa aspek perlu diperhatikan:

1. **Aset:** Data, perangkat, aplikasi, atau infrastruktur yang perlu dilindungi.
2. **Ancaman:** Potensi kejadian yang dapat menimbulkan gangguan.
3. **Kerentanan:** Kelemahan pada sistem atau proses yang dapat dimanfaatkan oleh ancaman.
4. **Dampak:** Konsekuensi yang muncul apabila risiko terjadi.
5. **Mitigasi:** Tindakan untuk mengurangi kemungkinan atau dampak risiko.

Identifikasi risiko harus didasarkan pada karakteristik sistem dan data yang digunakan, bukan hanya daftar ancaman umum.

### 4.3 Kontrol Teknis Keamanan

Kontrol keamanan merupakan tindakan perlindungan yang diterapkan untuk mengurangi risiko terhadap informasi dan sistem.

Kontrol teknis merupakan perlindungan yang diterapkan melalui perangkat keras, perangkat lunak, jaringan, dan konfigurasi sistem.

Pemilihan kontrol teknis harus mempertimbangkan:
- Jenis data yang dikelola.
- Tingkat sensitivitas data.
- Ancaman yang mungkin terjadi.
- Kerentanan sistem.
- Dampak apabila keamanan terganggu.
- Kebutuhan operasional sistem.

Tidak semua sistem membutuhkan kontrol yang sama. Kontrol keamanan harus disesuaikan dengan risiko dan kebutuhan perlindungan masing-masing sistem.

NIST Cybersecurity Framework 2.0 dapat digunakan sebagai referensi untuk memahami pengelolaan risiko keamanan siber. Kerangka ini mencakup enam fungsi utama:

1. Govern: Menetapkan dan mengawasi strategi serta kebijakan pengelolaan risiko keamanan siber.
2. Identify: Mengidentifikasi aset, kondisi, dan risiko keamanan.
3. Protect: Menerapkan perlindungan untuk mengurangi risiko.
4. Detect: Mendeteksi potensi kejadian keamanan.
5. Respond: Menangani insiden keamanan yang terdeteksi.
6. Recover: Memulihkan kemampuan dan layanan setelah terjadi insiden.

Keenam fungsi tersebut merupakan bagian dari kerangka pengelolaan risiko keamanan siber NIST CSF 2.0. Kerangka ini memberikan hasil yang perlu dicapai, bukan mewajibkan satu teknologi atau kontrol tertentu untuk seluruh sistem.

Dalam praktikum, mahasiswa perlu menghubungkan setiap risiko yang ditemukan dengan kontrol teknis yang sesuai.

---

## 5. Privasi dan Pelindungan Data Pribadi

### 5.1 Konsep Privasi Data

Privasi data berkaitan dengan hak dan kepentingan individu atas pengumpulan, penggunaan, penyimpanan, serta pembagian data yang berkaitan dengan dirinya.

Dalam sistem Smart City, data warga dapat digunakan untuk mendukung pelayanan publik, pemantauan kondisi perkotaan, dan pengambilan keputusan.

Namun, penggunaan data harus memperhatikan tujuan, kebutuhan, kewenangan, dan hak individu yang datanya diproses.

Pengumpulan data yang tidak diperlukan, penggunaan data di luar tujuan awal, serta pembagian data tanpa dasar yang sah dapat menimbulkan risiko terhadap privasi masyarakat.

OECD Privacy Guidelines menetapkan prinsip-prinsip perlindungan privasi dan aliran data pribadi lintas negara yang dapat digunakan sebagai referensi internasional.

Prinsip tersebut meliputi:

1. **Collection Limitation:** Pengumpulan data pribadi perlu dibatasi dan dilakukan melalui cara yang sah dan wajar.
2. **Data Quality:** Data harus relevan dengan tujuan penggunaannya, akurat, lengkap, dan mutakhir sesuai kebutuhan.
3. **Purpose Specification:** Tujuan pengumpulan data harus ditentukan paling lambat pada saat pengumpulan.
4. **Use Limitation:** Data tidak boleh digunakan atau diungkapkan untuk tujuan yang tidak sesuai dengan tujuan yang telah ditetapkan, kecuali terdapat persetujuan atau dasar hukum.
5. **Security Safeguards:** Data harus dilindungi dari risiko kehilangan, akses tidak sah, perubahan, penggunaan, atau pengungkapan tanpa kewenangan.
6. **Openness:** Kebijakan dan praktik pengelolaan data perlu disampaikan secara terbuka.
7. **Individual Participation:** Individu memiliki hak untuk memperoleh informasi mengenai data dirinya dan mengajukan koreksi sesuai ketentuan.
8. **Accountability:** Pihak yang mengelola data bertanggung jawab atas penerapan prinsip pelindungan data.

Prinsip OECD tersebut merupakan pedoman internasional, bukan pengganti ketentuan hukum Indonesia.

### 5.2 Undang-Undang Nomor 27 Tahun 2022 tentang Pelindungan Data Pribadi

Indonesia memiliki landasan hukum pelindungan data pribadi melalui **Undang-Undang Nomor 27 Tahun 2022 tentang Pelindungan Data Pribadi (UU PDP)**.

UU PDP mengatur hak Subjek Data Pribadi, jenis Data Pribadi, pemrosesan Data Pribadi, kewajiban pengendali dan prosesor, serta ketentuan lain terkait pelindungan data pribadi.

Beberapa ketentuan yang relevan dengan perancangan PoC adalah sebagai berikut.

#### A. Asas Pelindungan Data Pribadi

Pasal 3 UU PDP menetapkan delapan asas:

1. Pelindungan.
2. Kepastian hukum.
3. Kepentingan umum.
4. Kemanfaatan.
5. Kehati-hatian.
6. Keseimbangan.
7. Pertanggungjawaban.
8. Kerahasiaan.

Asas tersebut menjadi dasar dalam pelaksanaan pemrosesan Data Pribadi.

#### B. Jenis Data Pribadi

Pasal 4 membagi Data Pribadi menjadi dua kategori:

- Data Pribadi yang bersifat spesifik.
- Data Pribadi yang bersifat umum.

Pembagian dan contoh kedua kategori telah dijelaskan pada bagian klasifikasi data.

#### C. Hak Subjek Data Pribadi

Subjek Data Pribadi merupakan orang perseorangan yang pada dirinya melekat Data Pribadi.

UU PDP memberikan hak kepada Subjek Data Pribadi, antara lain:

| Pasal | Hak Subjek Data Pribadi |
|---|---|
| 5 | Mendapatkan informasi mengenai identitas, dasar kepentingan hukum, tujuan penggunaan data, dan akuntabilitas pihak yang meminta data |
| 6 | Melengkapi, memperbarui, dan memperbaiki data |
| 7 | Mendapatkan akses dan salinan data |
| 8 | Mengakhiri pemrosesan, menghapus, dan/atau memusnahkan data sesuai ketentuan |
| 9 | Menarik kembali persetujuan pemrosesan data |
| 10 | Mengajukan keberatan terhadap keputusan otomatis tertentu |
| 11 | Menunda atau membatasi pemrosesan data secara proporsional |
| 12 | Menggugat dan menerima ganti rugi atas pelanggaran pemrosesan data sesuai ketentuan |

Hak tersebut dilaksanakan sesuai persyaratan dan ketentuan yang diatur dalam undang-undang.

#### D. Pemrosesan Data Pribadi

Pasal 16 UU PDP mengatur bahwa pemrosesan Data Pribadi meliputi:

1. Pemerolehan dan pengumpulan.
2. Pengolahan dan penganalisisan.
3. Penyimpanan.
4. Perbaikan dan pembaruan.
5. Penampilan, pengumuman, transfer, penyebarluasan, atau pengungkapan.
6. Penghapusan atau pemusnahan.

Pemrosesan Data Pribadi harus memenuhi prinsip pelindungan, antara lain:

- Pengumpulan dilakukan secara terbatas dan spesifik, sah secara hukum, serta transparan.
- Pemrosesan dilakukan sesuai tujuan.
- Hak Subjek Data Pribadi dijamin.
- Data diproses secara akurat, lengkap, tidak menyesatkan, mutakhir, dan dapat dipertanggungjawabkan.
- Keamanan Data Pribadi dilindungi dari akses, pengungkapan, perubahan, penyalahgunaan, perusakan, dan penghilangan yang tidak sah.
- Tujuan dan aktivitas pemrosesan diberitahukan.
- Data dihapus atau dimusnahkan setelah masa retensi berakhir, kecuali ditentukan lain oleh peraturan perundang-undangan.
- Pemrosesan dilakukan secara bertanggung jawab dan dapat dibuktikan.

#### E. Dasar Pemrosesan Data Pribadi

Pasal 20 UU PDP mengatur bahwa Pengendali Data Pribadi wajib memiliki dasar pemrosesan Data Pribadi.

Dasar pemrosesan tersebut meliputi:

1. Persetujuan yang sah secara eksplisit dari Subjek Data Pribadi untuk tujuan tertentu.
2. Pemenuhan kewajiban perjanjian.
3. Pemenuhan kewajiban hukum.
4. Pemenuhan pelindungan kepentingan vital Subjek Data Pribadi.
5. Pelaksanaan tugas dalam rangka kepentingan umum, pelayanan publik, atau pelaksanaan kewenangan berdasarkan peraturan perundang-undangan.
6. Pemenuhan kepentingan sah lainnya dengan memperhatikan tujuan, kebutuhan, dan keseimbangan kepentingan Pengendali Data Pribadi serta hak Subjek Data Pribadi.

Dengan demikian, persetujuan bukan satu-satunya dasar hukum pemrosesan Data Pribadi. Dasar yang digunakan harus sesuai dengan kondisi dan tujuan pemrosesan.

#### F. Kewajiban Pengendali Data Pribadi

Pengendali Data Pribadi merupakan pihak yang menentukan tujuan dan melakukan kendali atas pemrosesan Data Pribadi.

Beberapa kewajiban yang relevan berdasarkan UU PDP meliputi:

- Memiliki dasar pemrosesan Data Pribadi (Pasal 20).
- Melakukan penilaian dampak Pelindungan Data Pribadi apabila pemrosesan memiliki potensi risiko tinggi terhadap Subjek Data Pribadi (Pasal 34).
- Melindungi dan memastikan keamanan Data Pribadi yang diproses (Pasal 35).
- Menjaga kerahasiaan Data Pribadi (Pasal 36).
- Mengawasi pihak yang terlibat dalam pemrosesan di bawah kendalinya (Pasal 37).
- Melindungi Data Pribadi dari pemrosesan yang tidak sah (Pasal 38).
- Mencegah akses tidak sah terhadap Data Pribadi (Pasal 39).

Ketentuan tersebut perlu diperhatikan ketika suatu PoC melibatkan pengumpulan atau pemrosesan Data Pribadi warga.

### 5.3 Etika Pemanfaatan Data Warga

Selain memenuhi ketentuan hukum, pemanfaatan data warga perlu mempertimbangkan aspek etika.

Kepatuhan terhadap hukum merupakan persyaratan dasar, tetapi tidak secara otomatis menjawab seluruh pertimbangan etis dalam penggunaan data.

Beberapa prinsip yang perlu diperhatikan:

**A. Transparansi**

Masyarakat perlu memperoleh informasi yang jelas mengenai data yang dikumpulkan, tujuan penggunaannya, dan pihak yang bertanggung jawab.

**B. Pembatasan Pengumpulan Data**

Sistem sebaiknya hanya mengumpulkan data yang relevan dan diperlukan untuk mencapai tujuan layanan.

**C. Pembatasan Penggunaan**

Data tidak seharusnya digunakan untuk tujuan lain yang tidak sesuai dengan tujuan awal tanpa dasar yang sah.

**D. Perlindungan terhadap Individu**

Penggunaan data harus memperhatikan risiko terhadap privasi, keamanan, dan hak individu.

**E. Akuntabilitas**

Pihak yang mengelola data harus bertanggung jawab atas keputusan dan aktivitas pemrosesan data.

Prinsip tersebut relevan dalam perancangan sistem Smart City karena data yang digunakan dapat berkaitan langsung dengan identitas, aktivitas, lokasi, dan kondisi masyarakat.

---

## 6. Rangkuman Materi

Pertemuan pertama membahas dua aspek utama dalam perancangan PoC, yaitu alur data dan tata kelola data.

**Perancangan Alur Data**

DFD digunakan untuk menggambarkan sumber data, proses pengolahan, penyimpanan, dan tujuan data. Setiap aliran data perlu diidentifikasi dan diberi label sesuai jenis data yang dipindahkan.

**Tata Kelola dan Siklus Hidup Data**

Data Governance mengatur kebijakan, tanggung jawab, dan penggunaan data. Pengelolaan data perlu memperhatikan seluruh siklus hidupnya, mulai dari pengumpulan hingga pemusnahan.

**Keamanan Siber**

Keamanan informasi berfokus pada kerahasiaan, integritas, dan ketersediaan data. Risiko keamanan perlu diidentifikasi berdasarkan aset, ancaman, kerentanan, dan dampaknya. Kontrol teknis ditentukan berdasarkan kebutuhan perlindungan sistem.

**Privasi dan Pelindungan Data Pribadi**

Pemrosesan Data Pribadi harus memiliki dasar yang sah, sesuai tujuan, memperhatikan hak Subjek Data Pribadi, dan memenuhi kewajiban pelindungan berdasarkan UU PDP. Penggunaan data warga juga perlu memperhatikan prinsip transparansi, pembatasan pengumpulan, perlindungan individu, dan akuntabilitas.

Keempat aspek tersebut menjadi dasar untuk merancang pengelolaan data yang aman dan sesuai ketentuan pada PoC Smart City.

---

## 7. Referensi

### Referensi Utama

1. Indonesia. (2022). **Undang-Undang Republik Indonesia Nomor 27 Tahun 2022 tentang Pelindungan Data Pribadi.** Lembaran Negara Republik Indonesia Tahun 2022 Nomor 196.  
   https://jdih.komdigi.go.id/produk_hukum/view/id/832

2. National Institute of Standards and Technology. (2024). **The NIST Cybersecurity Framework (CSF) 2.0.** NIST Cybersecurity White Paper 29.  
   https://doi.org/10.6028/NIST.CSWP.29

3. DAMA International. (2017). **DAMA-DMBOK: Data Management Body of Knowledge (2nd Edition).** Technics Publications.

4. Organisation for Economic Co-operation and Development. (2013). **The OECD Privacy Framework.** OECD Publishing.  
   https://www.oecd.org/sti/ieconomy/oecd_privacy_framework.pdf

### Referensi Pendukung

5. Internal Revenue Service. (2023). **Internal Revenue Manual 2.5.11: Analysis Techniques and Deliverables.** Bagian Data Flow Diagrams.  
   https://www.irs.gov/irm/part2/irm_02-005-011

6. National Institute of Standards and Technology. **Information Life Cycle. NIST Computer Security Resource Center Glossary.**  
   https://csrc.nist.gov/glossary/term/information_life_cycle

7. National Institute of Standards and Technology. **Information Security. NIST Computer Security Resource Center Glossary.**  
   https://csrc.nist.gov/glossary/term/information_security

8. IBM. **Apa Itu Diagram Aliran Data (DFD)?** IBM Think.  
   https://www.ibm.com/id-id/think/topics/data-flow-diagram

---

**Catatan sumber:** UU PDP merupakan landasan hukum Indonesia. NIST, DAMA-DMBOK, OECD, IRS, dan IBM digunakan sebagai referensi konseptual atau teknis sesuai bidangnya. Referensi internasional tersebut tidak menggantikan ketentuan hukum Indonesia.
