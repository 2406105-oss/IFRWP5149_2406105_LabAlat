<!-- DESKRIPSI SKENARIO -->

Mahasiswa mengajukan peminjaman peralatan dengan memilih alat, 
jumlah, dan rentang waktu. Sistem memeriksa ketersediaan. Jika 
tersedia dan data lengkap, sistem menyimpan pengajuan berstatus 
menunggu keputusan. Pada tampilan konfirmasi, mahasiswa dapat 
memilih mencetak bukti pengajuan. Petugas mengelola data peralatan 
serta menyetujui atau menolak pengajuan. Kepala laboratorium melihat 
laporan peminjaman. 

<!-- TABEL KEBTUHAN -->

| ID | Kebutuhan |
| LAB-R01 | Mahasiswa dapat melihat ketersediaan peralatan. |
| LAB-R02 | Petugas dapat mengelola data peralatan. |
| LAB-R03 | Mahasiswa dapat mengajukan peminjaman; sistem memeriksa ketersediaan sebelum menyimpan pengajuan. |
| LAB-R04 | Mahasiswa dapat mencetak bukti pada konfirmasi pengajuan jika memilihnya. |
| LAB-R05 | Petugas dapat menetapkan persetujuan atau penolakan pengajuan. |
| LAB-R06 | Kepala laboratorium dapat melihat laporan peminjaman. |

<!-- Batas sistem dan aturan -->

• Sistem mencatat dan menyediakan informasi; perpindahan fisik alat tidak 
terjadi di dalam perangkat lunak. 
• Pengguna telah terautentikasi dan memiliki hak akses sesuai peran. 
• Pengajuan yang diterima sistem berstatus Menunggu keputusan, bukan 
otomatis Disetujui.
• Pengajuan dengan peralatan tidak tersedia tidak disimpan sebagai 
pengajuan berhasil. 
• Pencetakan bukti tidak menjadi syarat keberhasilan pengajuan. 
• Persetujuan petugas belum dimodelkan sebagai reservasi teknis stok. 
• Pengambilan, pengembalian, kondisi alat, dan denda belum dianalisis 
pada potongan model ini.

<!-- Tabel identifikasi aktor -->

| Aktor | Tujuan terhadap Sistem |
| Mahasiswa | Melihat ketersediaan peralatan, mengajukan peminjaman, dan mencetak bukti peminjaman. |
| Petugas Laboratorium | Mengelola data peralatan dan memproses keputusan persetujuan atau penolakan pengajuan peminjaman. |
| Kepala Laboratorium | Melihat laporan peminjaman peralatan laboratorium. |

<!-- Tabel katalog use case -->

Berikut tabel use case sistem peminjaman peralatan laboratorium yang sudah dirapikan:

| ID | Nama Use Case | Peran dalam Model |
| --- | --- | --- |
| LAB-UC01 | Lihat Ketersediaan Peralatan | Fungsi utama mahasiswa |
| LAB-UC02 | Kelola Data Peralatan | Fungsi utama petugas laboratorium |
| LAB-UC03 | Ajukan Peminjaman | Fungsi utama mahasiswa |
| LAB-UC04 | Periksa Ketersediaan | Perilaku yang disertakan (include) pada UC03 |
| LAB-UC05 | Cetak Bukti Pengajuan | Tambahan bersyarat (extend) pada UC03 |
| LAB-UC06 | Proses Keputusan Peminjaman | Fungsi utama petugas laboratorium |
| LAB-UC07 | Lihat Laporan Peminjaman | Fungsi utama kepala laboratorium |

<!-- Includ -->
Alasan: pemeriksaan menjadi bagian validasi pengajuan. 

<!-- extend -->
Extension point: Bukti pengajuan tersedia. 
Kondisi: [mahasiswa memilih cetak]. 
Alasan: pengajuan tetap berhasil tanpa pencetakan.
